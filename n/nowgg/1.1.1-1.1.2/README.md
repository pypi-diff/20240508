# Comparing `tmp/nowgg-1.1.1.tar.gz` & `tmp/nowgg-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowgg-1.1.1.tar", last modified: Tue May  7 06:40:08 2024, max compression
+gzip compressed data, was "nowgg-1.1.2.tar", last modified: Wed May  8 13:08:39 2024, max compression
```

## Comparing `nowgg-1.1.1.tar` & `nowgg-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 06:40:08.092449 nowgg-1.1.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2236 2024-05-07 06:40:08.092449 nowgg-1.1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2040 2024-05-07 06:40:07.000000 nowgg-1.1.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 06:40:08.092449 nowgg-1.1.1/nowgg.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2236 2024-05-07 06:40:08.000000 nowgg-1.1.1/nowgg.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      203 2024-05-07 06:40:08.000000 nowgg-1.1.1/nowgg.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-07 06:40:08.000000 nowgg-1.1.1/nowgg.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-07 06:40:08.000000 nowgg-1.1.1/nowgg.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-05-07 06:40:08.000000 nowgg-1.1.1/nowgg.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-07 06:40:08.000000 nowgg-1.1.1/nowgg.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12438 2024-05-07 06:40:07.000000 nowgg-1.1.1/nowgg.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-07 06:40:08.092449 nowgg-1.1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      516 2024-05-07 06:40:07.000000 nowgg-1.1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-08 13:08:39.670557 nowgg-1.1.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2438 2024-05-08 13:08:39.670557 nowgg-1.1.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2242 2024-05-08 13:08:38.000000 nowgg-1.1.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-08 13:08:39.670557 nowgg-1.1.2/nowgg.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2438 2024-05-08 13:08:39.000000 nowgg-1.1.2/nowgg.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      203 2024-05-08 13:08:39.000000 nowgg-1.1.2/nowgg.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-08 13:08:39.000000 nowgg-1.1.2/nowgg.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-08 13:08:39.000000 nowgg-1.1.2/nowgg.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-05-08 13:08:39.000000 nowgg-1.1.2/nowgg.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-08 13:08:39.000000 nowgg-1.1.2/nowgg.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12438 2024-05-08 13:08:38.000000 nowgg-1.1.2/nowgg.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-08 13:08:39.670557 nowgg-1.1.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      516 2024-05-08 13:08:39.000000 nowgg-1.1.2/setup.py
```

### Comparing `nowgg-1.1.1/PKG-INFO` & `nowgg-1.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowgg
-Version: 1.1.1
+Version: 1.1.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author-email: cloudmaster@now.gg
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -23,30 +23,35 @@
     * Used to identify the publisher company.
     * Your Publisher token is available under the [Account Information](https://docs.now.gg/nowstudio/start-using-nowstudio#ac-info) section of nowStudio.
 
 ## Using nowgg CLI
 
 Open any terminal on macOS or Windows.
 
-### Install nowgg CLI tool
+#### Install nowgg CLI tool
 ```bash
   pip install nowgg
 ```
-### Initialize nowgg CLI
+#### Initialize nowgg CLI
 ```bash
   nowgg init --token "<your_publisherToken_from_nowStudio>"
 ```
 
-## Upload app using nowgg CLI to NowStudio
+#### Upload App to App Library
 
 ```bash
   nowgg upload --app_id <your_app_id> --file_path "/directory/sample.apk" --apk_version <apk_version> --version_code <app_version_code>
 ```
 
-#### Note
+#### Upload App to Test Track and Trigger Deployment
+```bash
+  nowgg upload --app_id <your_app_id> --file_path "/directory/sample.apk" --apk_version <apk_version> --version_code <app_version_code> --deploy
+```
+
+##### Note
 - Each test track has a unique `app_id`, that you can use to create a draft release on that test track. For example, if your `app_id` is `1234`, the `app_id` for test track 1 would be `1234_t1`, 
 
 - If you provide `1234` instead of `1234_t1` the app will be uploaded to the App library only.
 
 - Adding `--deploy` triggers the deployment process on the specified test track, this will only work if you've given the `app_id` for a test track as per the above format.
 
 Example for `--deploy`
```

### Comparing `nowgg-1.1.1/README.md` & `nowgg-1.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -13,30 +13,35 @@
     * Used to identify the publisher company.
     * Your Publisher token is available under the [Account Information](https://docs.now.gg/nowstudio/start-using-nowstudio#ac-info) section of nowStudio.
 
 ## Using nowgg CLI
 
 Open any terminal on macOS or Windows.
 
-### Install nowgg CLI tool
+#### Install nowgg CLI tool
 ```bash
   pip install nowgg
 ```
-### Initialize nowgg CLI
+#### Initialize nowgg CLI
 ```bash
   nowgg init --token "<your_publisherToken_from_nowStudio>"
 ```
 
-## Upload app using nowgg CLI to NowStudio
+#### Upload App to App Library
 
 ```bash
   nowgg upload --app_id <your_app_id> --file_path "/directory/sample.apk" --apk_version <apk_version> --version_code <app_version_code>
 ```
 
-#### Note
+#### Upload App to Test Track and Trigger Deployment
+```bash
+  nowgg upload --app_id <your_app_id> --file_path "/directory/sample.apk" --apk_version <apk_version> --version_code <app_version_code> --deploy
+```
+
+##### Note
 - Each test track has a unique `app_id`, that you can use to create a draft release on that test track. For example, if your `app_id` is `1234`, the `app_id` for test track 1 would be `1234_t1`, 
 
 - If you provide `1234` instead of `1234_t1` the app will be uploaded to the App library only.
 
 - Adding `--deploy` triggers the deployment process on the specified test track, this will only work if you've given the `app_id` for a test track as per the above format.
 
 Example for `--deploy`
```

### Comparing `nowgg-1.1.1/nowgg.egg-info/PKG-INFO` & `nowgg-1.1.2/nowgg.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowgg
-Version: 1.1.1
+Version: 1.1.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author-email: cloudmaster@now.gg
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -23,30 +23,35 @@
     * Used to identify the publisher company.
     * Your Publisher token is available under the [Account Information](https://docs.now.gg/nowstudio/start-using-nowstudio#ac-info) section of nowStudio.
 
 ## Using nowgg CLI
 
 Open any terminal on macOS or Windows.
 
-### Install nowgg CLI tool
+#### Install nowgg CLI tool
 ```bash
   pip install nowgg
 ```
-### Initialize nowgg CLI
+#### Initialize nowgg CLI
 ```bash
   nowgg init --token "<your_publisherToken_from_nowStudio>"
 ```
 
-## Upload app using nowgg CLI to NowStudio
+#### Upload App to App Library
 
 ```bash
   nowgg upload --app_id <your_app_id> --file_path "/directory/sample.apk" --apk_version <apk_version> --version_code <app_version_code>
 ```
 
-#### Note
+#### Upload App to Test Track and Trigger Deployment
+```bash
+  nowgg upload --app_id <your_app_id> --file_path "/directory/sample.apk" --apk_version <apk_version> --version_code <app_version_code> --deploy
+```
+
+##### Note
 - Each test track has a unique `app_id`, that you can use to create a draft release on that test track. For example, if your `app_id` is `1234`, the `app_id` for test track 1 would be `1234_t1`, 
 
 - If you provide `1234` instead of `1234_t1` the app will be uploaded to the App library only.
 
 - Adding `--deploy` triggers the deployment process on the specified test track, this will only work if you've given the `app_id` for a test track as per the above format.
 
 Example for `--deploy`
```

### Comparing `nowgg-1.1.1/nowgg.py` & `nowgg-1.1.2/nowgg.py`

 * *Files identical despite different names*

### Comparing `nowgg-1.1.1/setup.py` & `nowgg-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 import os
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
     name='nowgg',
-    version='1.1.1',
+    version='1.1.2',
     scripts=['nowgg.py'],
     author_email='cloudmaster@now.gg',
     install_requires=[
         'requests'
     ],
     long_description=long_description,
     long_description_content_type='text/markdown',
```

