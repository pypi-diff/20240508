# Comparing `tmp/gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0.tar.gz` & `tmp/gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0.tar", last modified: Tue Apr 30 02:39:32 2024, max compression
+gzip compressed data, was "gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1.tar", last modified: Wed May  8 19:13:17 2024, max compression
```

## Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0.tar` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:39:32.657812 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-30 02:39:21.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-30 02:39:21.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-30 02:39:32.653812 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-30 02:39:21.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-30 02:39:21.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 02:39:32.657812 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-30 02:39:21.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:39:32.653812 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:39:32.653812 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:39:32.653812 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/
--rw-r--r--   0 runner    (1001) docker     (127)    27881 2024-04-30 02:39:21.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:39:32.653812 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-30 02:39:21.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45059 2024-04-30 02:39:21.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/aws-daily-cloud-watch-logs-archive-stack@2.7.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 02:39:21.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:39:32.653812 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-30 02:39:32.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-30 02:39:32.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 02:39:32.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-30 02:39:32.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 02:39:32.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:13:17.986949 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-08 19:13:02.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 19:13:02.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-08 19:13:17.986949 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-08 19:13:02.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 19:13:02.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:13:17.986949 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-08 19:13:02.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:13:17.982949 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:13:17.982949 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:13:17.986949 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/
+-rw-r--r--   0 runner    (1001) docker     (127)    27881 2024-05-08 19:13:02.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:13:17.986949 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-08 19:13:02.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45062 2024-05-08 19:13:02.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/aws-daily-cloud-watch-logs-archive-stack@2.7.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:13:02.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:13:17.982949 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-08 19:13:17.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-08 19:13:17.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:13:17.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-08 19:13:17.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 19:13:17.000000 gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/top_level.txt
```

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/LICENSE` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/PKG-INFO` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-daily-cloud-watch-logs-archive-stack
-Version: 2.7.0
+Version: 2.7.1
 Summary: AWS CloudWatch Logs daily archive to s3 bucket
 Home-page: https://github.com/gammarers/aws-daily-cloud-watch-logs-archive-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-daily-cloud-watch-logs-archive-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/README.md` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/setup.py` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-daily-cloud-watch-logs-archive-stack",
-    "version": "2.7.0",
+    "version": "2.7.1",
     "description": "AWS CloudWatch Logs daily archive to s3 bucket",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-daily-cloud-watch-logs-archive-stack.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,27 +22,27 @@
     },
     "packages": [
         "gammarers.aws_daily_cloud_watch_logs_archive_stack",
         "gammarers.aws_daily_cloud_watch_logs_archive_stack._jsii"
     ],
     "package_data": {
         "gammarers.aws_daily_cloud_watch_logs_archive_stack._jsii": [
-            "aws-daily-cloud-watch-logs-archive-stack@2.7.0.jsii.tgz"
+            "aws-daily-cloud-watch-logs-archive-stack@2.7.1.jsii.tgz"
         ],
         "gammarers.aws_daily_cloud_watch_logs_archive_stack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "gammarers.aws-secure-bucket>=1.3.3, <1.4.0",
         "gammarers.aws-secure-log-bucket>=1.6.2, <1.7.0",
-        "jsii>=1.97.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/__init__.py` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/__init__.py` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import aws_cdk._jsii
 import constructs._jsii
 import gammarers.aws_secure_bucket._jsii
 import gammarers.aws_secure_log_bucket._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-daily-cloud-watch-logs-archive-stack",
-    "2.7.0",
+    "2.7.1",
     __name__[0:-6],
-    "aws-daily-cloud-watch-logs-archive-stack@2.7.0.jsii.tgz",
+    "aws-daily-cloud-watch-logs-archive-stack@2.7.1.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/PKG-INFO` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-daily-cloud-watch-logs-archive-stack
-Version: 2.7.0
+Version: 2.7.1
 Summary: AWS CloudWatch Logs daily archive to s3 bucket
 Home-page: https://github.com/gammarers/aws-daily-cloud-watch-logs-archive-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-daily-cloud-watch-logs-archive-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.0/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt` & `gammarers.aws-daily-cloud-watch-logs-archive-stack-2.7.1/src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt
 src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/dependency_links.txt
 src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/requires.txt
 src/gammarers.aws_daily_cloud_watch_logs_archive_stack.egg-info/top_level.txt
 src/gammarers/aws_daily_cloud_watch_logs_archive_stack/__init__.py
 src/gammarers/aws_daily_cloud_watch_logs_archive_stack/py.typed
 src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/__init__.py
-src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/aws-daily-cloud-watch-logs-archive-stack@2.7.0.jsii.tgz
+src/gammarers/aws_daily_cloud_watch_logs_archive_stack/_jsii/aws-daily-cloud-watch-logs-archive-stack@2.7.1.jsii.tgz
```

