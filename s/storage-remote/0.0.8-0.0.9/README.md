# Comparing `tmp/storage-remote-0.0.8.tar.gz` & `tmp/storage_remote-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storage-remote-0.0.8.tar", last modified: Fri Sep 15 00:33:14 2023, max compression
+gzip compressed data, was "storage_remote-0.0.9.tar", last modified: Wed May  8 02:39:41 2024, max compression
```

## Comparing `storage-remote-0.0.8.tar` & `storage_remote-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 00:33:14.255298 storage-remote-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-09-15 00:33:14.255298 storage-remote-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-09-15 00:32:48.000000 storage-remote-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-09-15 00:32:48.000000 storage-remote-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-15 00:33:14.255298 storage-remote-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2023-09-15 00:32:48.000000 storage-remote-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 00:33:14.255298 storage-remote-0.0.8/storage_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 00:33:14.255298 storage-remote-0.0.8/storage_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 00:32:48.000000 storage-remote-0.0.8/storage_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2023-09-15 00:32:48.000000 storage-remote-0.0.8/storage_remote/src/remote_circles_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 00:33:14.255298 storage-remote-0.0.8/storage_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-09-15 00:33:14.000000 storage-remote-0.0.8/storage_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-09-15 00:33:14.000000 storage-remote-0.0.8/storage_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-15 00:33:14.000000 storage-remote-0.0.8/storage_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-09-15 00:33:14.000000 storage-remote-0.0.8/storage_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-09-15 00:33:14.000000 storage-remote-0.0.8/storage_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:39:41.871025 storage_remote-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-08 02:39:41.871025 storage_remote-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-08 02:39:33.000000 storage_remote-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-08 02:39:33.000000 storage_remote-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 02:39:41.871025 storage_remote-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-08 02:39:33.000000 storage_remote-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:39:41.867025 storage_remote-0.0.9/storage_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:39:41.871025 storage_remote-0.0.9/storage_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 02:39:33.000000 storage_remote-0.0.9/storage_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-08 02:39:33.000000 storage_remote-0.0.9/storage_remote/src/remote_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:39:41.871025 storage_remote-0.0.9/storage_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-08 02:39:41.000000 storage_remote-0.0.9/storage_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 02:39:41.000000 storage_remote-0.0.9/storage_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 02:39:41.000000 storage_remote-0.0.9/storage_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-08 02:39:41.000000 storage_remote-0.0.9/storage_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 02:39:41.000000 storage_remote-0.0.9/storage_remote.egg-info/top_level.txt
```

### Comparing `storage-remote-0.0.8/setup.py` & `storage_remote-0.0.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,27 @@
 import setuptools
 
-PACKAGE_NAME = "storage-remote"
+PACKAGE_NAME = "storage-remote"  # TODO: should it be called storage-remote-graphql ?
 package_dir = PACKAGE_NAME.replace("-", "_")
 
-with open('README.md') as f:
-    readme = f.read()
-
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/storage-remote
-    version='0.0.8',
+    version='0.0.9',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/storage-remote-graphql-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
-    long_description=readme,
+    long_description="This is a package for sharing common methods of storage remote used in different repositories",
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "requests>=2.31.0",
-        "python-dotenv>=1.0.0",
-        "mysql-connector>=2.2.9",
-        "pymysql>=1.1.0",
-        "pytest>=7.4.0",
-
-        "logger-local>=0.0.61",
-        "database-without-orm-local>=0.0.90",
-        "url-local>=0.0.28"
+        "python-sdk-remote>=0.0.93",
+        "url-remote>=0.0.28"
     ]
 )
```

### Comparing `storage-remote-0.0.8/storage_remote/src/remote_circles_storage.py` & `storage_remote-0.0.9/storage_remote/src/remote_storage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import requests
-import os
-from dotenv import load_dotenv
-from url_local.url_circlez import UrlCirclez
-from url_local.component_name_enum import ComponentName
-from url_local.entity_name_enum import EntityName
-
-load_dotenv()
-BRAND_NAME: str = os.getenv('BRAND_NAME')
-ENVIRONMENT_NAME: str = os.getenv('ENVIRONMENT_NAME')
+from python_sdk_remote.utilities import our_get_env
+from url_remote.component_name_enum import ComponentName
+from url_remote.entity_name_enum import EntityName
+from url_remote.url_circlez import OurUrl
+
+# TODO Please replace all strings and Magic Numbers such as "graphql" to const enum
+version = 1
+action = "graphql"
+BRAND_NAME = our_get_env('BRAND_NAME')
+ENVIRONMENT_NAME = our_get_env('ENVIRONMENT_NAME')
 
-
-class RemoteCirclesStorage:
+# TODO: use logger
+class RemoteStorage:
     def __init__(self) -> None:
-        # TODO Please replace all strings and Magic Numbers such as "graphql" to const enum
-        version = 1
-        action = "graphql"
-        self.url: str = UrlCirclez.endpoint_url(
-            BRAND_NAME, ENVIRONMENT_NAME, ComponentName.GROUP_PROFILE.value,
-            EntityName.GROUP_PROFILE.value, version, action)
+        self.url = OurUrl.endpoint_url(
+            brand_name=BRAND_NAME, environment_name=ENVIRONMENT_NAME,
+            component_name=ComponentName.GROUP_PROFILE.value,
+            entity_name=EntityName.GROUP_PROFILE.value, version=version,
+            action_name=action)
 
-    def put(self, filename: str, local_path: str, created_user_id: int, entity_type_id: int, profile_id: int) -> str:
+    def put(self, *, filename: str, local_path: str, created_user_id: int, entity_type_id: int, profile_id: int) -> str:
         """
         Uploads a file to the remote storage and returns the file's remote path.
 
         :param filename: The name of the file.
         :param local_path: The local path to the file on your system.
         :param created_user_id: The ID of the user who created the file.
         :param entity_type_id: The ID of the entity type associated with the file.
@@ -41,18 +41,20 @@
           )
         }}"""
         response = requests.post(self.url, json={"query": put_query})
 
         response_data = response.json().get("data", {})
         if "errors" in response_data:
             raise Exception(response_data["errors"][0]["message"])
+        elif "put" not in response_data:
+            raise Exception("Unknown error while uploading file", response_data)
+        else:
+            return response_data["put"]
 
-        return response_data["put"]
-
-    def download(self, filename: str, local_path: str, entity_type_id: int, profile_id: int) -> str:
+    def download(self, *, filename: str, local_path: str, entity_type_id: int, profile_id: int) -> str:
         """
         Downloads a file from the remote storage and returns the file's contents.
 
         :param filename: The name of the file to download.
         :param entity_type_id: The ID of the entity type associated with the file.
         :param profile_id: The ID of the profile associated with the file.
         :param local_path: The local path where the downloaded file should be saved.
```

