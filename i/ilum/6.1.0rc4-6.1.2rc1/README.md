# Comparing `tmp/ilum-6.1.0rc4.tar.gz` & `tmp/ilum-6.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilum-6.1.0rc4.tar", last modified: Tue Feb 20 10:32:38 2024, max compression
+gzip compressed data, was "ilum-6.1.2rc1.tar", last modified: Wed May  8 09:33:04 2024, max compression
```

## Comparing `ilum-6.1.0rc4.tar` & `ilum-6.1.2rc1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-20 10:32:38.100829 ilum-6.1.0rc4/
--rw-r--r--   0 runner    (1001) runner    (1001)     2244 2024-02-20 10:32:38.100829 ilum-6.1.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)     1516 2024-02-20 10:05:44.000000 ilum-6.1.0rc4/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-20 10:32:38.096830 ilum-6.1.0rc4/ilum/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-02-20 10:05:44.000000 ilum-6.1.0rc4/ilum/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      642 2024-02-20 10:05:44.000000 ilum-6.1.0rc4/ilum/api.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-02-20 10:32:38.100829 ilum-6.1.0rc4/ilum.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     2244 2024-02-20 10:32:37.000000 ilum-6.1.0rc4/ilum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      159 2024-02-20 10:32:38.000000 ilum-6.1.0rc4/ilum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-02-20 10:32:37.000000 ilum-6.1.0rc4/ilum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        5 2024-02-20 10:32:37.000000 ilum-6.1.0rc4/ilum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-02-20 10:32:38.100829 ilum-6.1.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)     1076 2024-02-20 10:24:20.000000 ilum-6.1.0rc4/setup.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-08 09:33:04.191729 ilum-6.1.2rc1/
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2244 2024-05-08 09:33:04.191729 ilum-6.1.2rc1/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1516 2023-08-17 13:17:27.000000 ilum-6.1.2rc1/README.md
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-08 09:33:04.191729 ilum-6.1.2rc1/ilum/
+-rw-rw-r--   0 oem      (29999) oem      (29999)        0 2023-08-17 13:17:27.000000 ilum-6.1.2rc1/ilum/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)      642 2023-08-17 13:17:27.000000 ilum-6.1.2rc1/ilum/api.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-05-08 09:33:04.191729 ilum-6.1.2rc1/ilum.egg-info/
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2244 2024-05-08 09:33:03.000000 ilum-6.1.2rc1/ilum.egg-info/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)      159 2024-05-08 09:33:04.000000 ilum-6.1.2rc1/ilum.egg-info/SOURCES.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        1 2024-05-08 09:33:03.000000 ilum-6.1.2rc1/ilum.egg-info/dependency_links.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        5 2024-05-08 09:33:04.000000 ilum-6.1.2rc1/ilum.egg-info/top_level.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       38 2024-05-08 09:33:04.191729 ilum-6.1.2rc1/setup.cfg
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1076 2024-05-08 08:45:55.000000 ilum-6.1.2rc1/setup.py
```

### Comparing `ilum-6.1.0rc4/PKG-INFO` & `ilum-6.1.2rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilum
-Version: 6.1.0rc4
+Version: 6.1.2rc1
 Summary: Ilum job python api
 Home-page: https://ilum.cloud
 Author: Ilum Labs LLC
 Author-email: info@ilum.cloud
 License: apache-2.0
 Project-URL: Documentation, https://ilum.cloud/docs/
 Project-URL: API Ref, https://ilum.cloud/docs/api/
```

### Comparing `ilum-6.1.0rc4/README.md` & `ilum-6.1.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `ilum-6.1.0rc4/ilum/api.py` & `ilum-6.1.2rc1/ilum/api.py`

 * *Files identical despite different names*

### Comparing `ilum-6.1.0rc4/ilum.egg-info/PKG-INFO` & `ilum-6.1.2rc1/ilum.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilum
-Version: 6.1.0rc4
+Version: 6.1.2rc1
 Summary: Ilum job python api
 Home-page: https://ilum.cloud
 Author: Ilum Labs LLC
 Author-email: info@ilum.cloud
 License: apache-2.0
 Project-URL: Documentation, https://ilum.cloud/docs/
 Project-URL: API Ref, https://ilum.cloud/docs/api/
```

### Comparing `ilum-6.1.0rc4/setup.py` & `ilum-6.1.2rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ilum",
-    version="6.1.0-RC4",
+    version="6.1.2-RC1",
     packages=find_packages(),
     package_data={"": ["ilum/*"]},
     url="https://ilum.cloud",
     author="Ilum Labs LLC",
     author_email="info@ilum.cloud",
     description="Ilum job python api",
     long_description=long_description,
```

