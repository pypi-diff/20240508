# Comparing `tmp/rqrisk-1.0.8.tar.gz` & `tmp/rqrisk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rqrisk/rqrisk/dist/.tmp-z5lfbk7u/rqrisk-1.0.8.tar", last modified: Tue Jan 30 06:49:05 2024, max compression
+gzip compressed data, was "/home/runner/work/rqrisk/rqrisk/dist/.tmp-t6f3qcob/rqrisk-1.0.9.tar", last modified: Wed May  8 06:50:37 2024, max compression
```

## Comparing `rqrisk-1.0.8.tar` & `rqrisk-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 06:49:05.000000 rqrisk-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-01-30 06:48:55.000000 rqrisk-1.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-30 06:48:55.000000 rqrisk-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-30 06:49:05.000000 rqrisk-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-30 06:48:55.000000 rqrisk-1.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 06:49:05.000000 rqrisk-1.0.8/rqrisk/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-30 06:48:55.000000 rqrisk-1.0.8/rqrisk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-30 06:49:05.000000 rqrisk-1.0.8/rqrisk/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-01-30 06:48:55.000000 rqrisk-1.0.8/rqrisk/risk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-01-30 06:48:55.000000 rqrisk-1.0.8/rqrisk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 06:49:05.000000 rqrisk-1.0.8/rqrisk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-30 06:49:05.000000 rqrisk-1.0.8/rqrisk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-01-30 06:49:05.000000 rqrisk-1.0.8/rqrisk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 06:49:05.000000 rqrisk-1.0.8/rqrisk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 06:49:05.000000 rqrisk-1.0.8/rqrisk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-30 06:49:05.000000 rqrisk-1.0.8/rqrisk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-30 06:49:05.000000 rqrisk-1.0.8/rqrisk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-01-30 06:49:05.000000 rqrisk-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-01-30 06:48:55.000000 rqrisk-1.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86835 2024-01-30 06:48:55.000000 rqrisk-1.0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:50:37.000000 rqrisk-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-08 06:50:33.000000 rqrisk-1.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 06:50:33.000000 rqrisk-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-08 06:50:37.000000 rqrisk-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 06:50:33.000000 rqrisk-1.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:50:37.000000 rqrisk-1.0.9/rqrisk/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-08 06:50:33.000000 rqrisk-1.0.9/rqrisk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-08 06:50:37.000000 rqrisk-1.0.9/rqrisk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-05-08 06:50:33.000000 rqrisk-1.0.9/rqrisk/risk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-08 06:50:33.000000 rqrisk-1.0.9/rqrisk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:50:37.000000 rqrisk-1.0.9/rqrisk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-08 06:50:37.000000 rqrisk-1.0.9/rqrisk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-08 06:50:37.000000 rqrisk-1.0.9/rqrisk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 06:50:37.000000 rqrisk-1.0.9/rqrisk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 06:50:37.000000 rqrisk-1.0.9/rqrisk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 06:50:37.000000 rqrisk-1.0.9/rqrisk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 06:50:37.000000 rqrisk-1.0.9/rqrisk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-08 06:50:37.000000 rqrisk-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-08 06:50:33.000000 rqrisk-1.0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86835 2024-05-08 06:50:33.000000 rqrisk-1.0.9/versioneer.py
```

### Comparing `rqrisk-1.0.8/LICENSE.txt` & `rqrisk-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rqrisk-1.0.8/rqrisk/risk.py` & `rqrisk-1.0.9/rqrisk/risk.py`

 * *Files identical despite different names*

### Comparing `rqrisk-1.0.8/rqrisk/utils.py` & `rqrisk-1.0.9/rqrisk/utils.py`

 * *Files identical despite different names*

### Comparing `rqrisk-1.0.8/setup.py` & `rqrisk-1.0.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     url="https://www.ricequant.com/",
     packages=find_packages(),
     author="Ricequant",
     install_requires=readfile("requirements.txt"),
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     description="risk calc"
 )
```

### Comparing `rqrisk-1.0.8/versioneer.py` & `rqrisk-1.0.9/versioneer.py`

 * *Files identical despite different names*

