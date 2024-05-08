# Comparing `tmp/defendatron-0.1.4.tar.gz` & `tmp/defendatron-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defendatron-0.1.4.tar", last modified: Thu Apr 25 17:46:26 2024, max compression
+gzip compressed data, was "defendatron-0.1.5.tar", last modified: Wed May  8 18:16:53 2024, max compression
```

## Comparing `defendatron-0.1.4.tar` & `defendatron-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:46:26.175389 defendatron-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 17:46:22.000000 defendatron-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-25 17:46:26.175389 defendatron-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-25 17:46:22.000000 defendatron-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:46:26.175389 defendatron-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-25 17:46:22.000000 defendatron-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:46:26.175389 defendatron-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:46:26.175389 defendatron-0.1.4/src/defendatron/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-25 17:46:22.000000 defendatron-0.1.4/src/defendatron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-25 17:46:22.000000 defendatron-0.1.4/src/defendatron/nullscream_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:46:26.175389 defendatron-0.1.4/src/defendatron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-25 17:46:26.000000 defendatron-0.1.4/src/defendatron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-25 17:46:26.000000 defendatron-0.1.4/src/defendatron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:46:26.000000 defendatron-0.1.4/src/defendatron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 17:46:26.000000 defendatron-0.1.4/src/defendatron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 17:46:26.000000 defendatron-0.1.4/src/defendatron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:53.598393 defendatron-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 18:16:49.000000 defendatron-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-08 18:16:53.598393 defendatron-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-08 18:16:49.000000 defendatron-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:16:53.598393 defendatron-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-08 18:16:49.000000 defendatron-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:53.598393 defendatron-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:53.598393 defendatron-0.1.5/src/defendatron/
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-08 18:16:49.000000 defendatron-0.1.5/src/defendatron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-08 18:16:49.000000 defendatron-0.1.5/src/defendatron/nullscream_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:53.598393 defendatron-0.1.5/src/defendatron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-08 18:16:53.000000 defendatron-0.1.5/src/defendatron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-08 18:16:53.000000 defendatron-0.1.5/src/defendatron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:16:53.000000 defendatron-0.1.5/src/defendatron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 18:16:53.000000 defendatron-0.1.5/src/defendatron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 18:16:53.000000 defendatron-0.1.5/src/defendatron.egg-info/top_level.txt
```

### Comparing `defendatron-0.1.4/LICENSE` & `defendatron-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `defendatron-0.1.4/PKG-INFO` & `defendatron-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defendatron
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://github.com/Capsize-Games/defendatron
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `defendatron-0.1.4/README.md` & `defendatron-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `defendatron-0.1.4/setup.py` & `defendatron-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="defendatron",
-    version="0.1.4",
+    version="0.1.5",
     author="Capsize LLC",
     description="",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="",
     license="GPL-3.0",
     author_email="contact@capsizegames.com",
```

### Comparing `defendatron-0.1.4/src/defendatron/__init__.py` & `defendatron-0.1.5/src/defendatron/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+import logging
+
 import shadowlogger
 import darklock
 import nullscream
 from defendatron.nullscream_tracker import NullscreamTracker
 
+
 nullscream_tracker = NullscreamTracker()
+logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger(__name__)
+
 
 def activate(
     # Nullscream properties
     nullscream_blacklist: list = None,
     nullscream_whitelist: list = None,
     nullscream_function_blacklist: list = None,
 
@@ -20,33 +26,33 @@
     activate_shadowlogger: bool = False,
     activate_darklock: bool = False,
     activate_nullscream: bool = False,
 
     # Shadowlogger properties
     show_stdout: bool = True
 ):
-    print("Activating defendatron")
+    logger.info("Activating defendatron")
     if activate_shadowlogger:
-        print("Activating shadowlogger")
+        logger.info("Activating shadowlogger")
         shadowlogger.manager.activate(
             show_stdout=show_stdout,
             trackers=[nullscream_tracker],
         )
 
     if activate_darklock:
-        print("Activating darklock")
+        logger.info("Activating darklock")
         darklock.activate(
             whitelisted_operations=darklock_os_whitelisted_operations,
             whitelisted_filenames=darklock_os_whitelisted_filenames,
             whitelisted_imports=darklock_os_whitelisted_imports,
             blacklisted_filenames=darklock_os_blacklisted_filenames,
         )
 
     if activate_nullscream:
-        print("Activating nullscream")
+        logger.info("Activating nullscream")
         nullscream.activate(
             blacklist=nullscream_blacklist,
             whitelist=nullscream_whitelist,
             function_blacklist=nullscream_function_blacklist,
         )
```

### Comparing `defendatron-0.1.4/src/defendatron/nullscream_tracker.py` & `defendatron-0.1.5/src/defendatron/nullscream_tracker.py`

 * *Files identical despite different names*

### Comparing `defendatron-0.1.4/src/defendatron.egg-info/PKG-INFO` & `defendatron-0.1.5/src/defendatron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defendatron
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://github.com/Capsize-Games/defendatron
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

