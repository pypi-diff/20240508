# Comparing `tmp/cabinet-2024.4.29.3.tar.gz` & `tmp/cabinet-2024.5.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2024.4.29.3.tar", last modified: Tue Apr 30 05:33:15 2024, max compression
+gzip compressed data, was "cabinet-2024.5.7.1.tar", last modified: Wed May  8 04:43:54 2024, max compression
```

## Comparing `cabinet-2024.4.29.3.tar` & `cabinet-2024.5.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-30 05:33:15.370165 cabinet-2024.4.29.3/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.4.29.3/LICENSE
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-30 05:33:15.370165 cabinet-2024.4.29.3/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7589 2024-04-16 03:19:05.000000 cabinet-2024.4.29.3/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.4.29.3/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-04-30 05:33:15.370165 cabinet-2024.4.29.3/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-30 05:33:15.370165 cabinet-2024.4.29.3/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-30 05:33:15.370165 cabinet-2024.4.29.3/src/cabinet/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.4.29.3/src/cabinet/__init__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.4.29.3/src/cabinet/__main__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    38261 2024-04-30 05:32:50.000000 cabinet-2024.4.29.3/src/cabinet/cabinet.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.4.29.3/src/cabinet/constants.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-28 06:57:49.000000 cabinet-2024.4.29.3/src/cabinet/helpers.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6496 2024-04-28 18:04:20.000000 cabinet-2024.4.29.3/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-30 05:33:15.370165 cabinet-2024.4.29.3/src/cabinet.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)     7941 2024-04-30 05:33:15.000000 cabinet-2024.4.29.3/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-04-30 05:33:15.000000 cabinet-2024.4.29.3/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-30 05:33:15.000000 cabinet-2024.4.29.3/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-04-30 05:33:15.000000 cabinet-2024.4.29.3/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-04-30 05:33:15.000000 cabinet-2024.4.29.3/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-08 04:43:54.702364 cabinet-2024.5.7.1/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1090 2024-01-29 08:09:41.000000 cabinet-2024.5.7.1/LICENSE
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7940 2024-05-08 04:43:54.702364 cabinet-2024.5.7.1/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7589 2024-04-16 03:19:05.000000 cabinet-2024.5.7.1/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2024-01-29 08:09:41.000000 cabinet-2024.5.7.1/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      750 2024-05-08 04:43:54.702364 cabinet-2024.5.7.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-08 04:43:54.698364 cabinet-2024.5.7.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-08 04:43:54.698364 cabinet-2024.5.7.1/src/cabinet/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       80 2024-01-29 08:09:41.000000 cabinet-2024.5.7.1/src/cabinet/__init__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       69 2024-01-29 08:09:41.000000 cabinet-2024.5.7.1/src/cabinet/__main__.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)    38351 2024-05-08 04:41:54.000000 cabinet-2024.5.7.1/src/cabinet/cabinet.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2596 2024-03-25 04:02:52.000000 cabinet-2024.5.7.1/src/cabinet/constants.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      307 2024-04-28 06:57:49.000000 cabinet-2024.5.7.1/src/cabinet/helpers.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6496 2024-04-28 18:04:20.000000 cabinet-2024.5.7.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-05-08 04:43:54.702364 cabinet-2024.5.7.1/src/cabinet.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     7940 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      359 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2024-05-08 04:43:54.000000 cabinet-2024.5.7.1/src/cabinet.egg-info/top_level.txt
```

### Comparing `cabinet-2024.4.29.3/LICENSE` & `cabinet-2024.5.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.29.3/PKG-INFO` & `cabinet-2024.5.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.4.29.3
+Version: 2024.5.7.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cabinet-2024.4.29.3/README.md` & `cabinet-2024.5.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.29.3/setup.cfg` & `cabinet-2024.5.7.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2024.04.29.3
+version = 2024.05.07.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2024.4.29.3/src/cabinet/cabinet.py` & `cabinet-2024.5.7.1/src/cabinet/cabinet.py`

 * *Files 0% similar despite different names*

```diff
@@ -747,14 +747,17 @@
 
         # Configure logger
         today = str(date.today())
         log_folder_path = log_folder_path or \
             f"{self.path_log or self.path_cabinet + '/log/'}{today}"
         log_folder_path = os.path.expanduser(log_folder_path)
 
+        if not os.path.exists(log_folder_path):
+            os.makedirs(log_folder_path)
+
         if log_name is None:
             log_name = f"LOG_DAILY_{today}"
 
         # Get or create logger
         logger = logging.getLogger(log_name)
         logger.setLevel(getattr(logging, level.upper()))
```

### Comparing `cabinet-2024.4.29.3/src/cabinet/constants.py` & `cabinet-2024.5.7.1/src/cabinet/constants.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.29.3/src/cabinet/mail.py` & `cabinet-2024.5.7.1/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2024.4.29.3/src/cabinet.egg-info/PKG-INFO` & `cabinet-2024.5.7.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2024.4.29.3
+Version: 2024.5.7.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

