# Comparing `tmp/profile-profile-local-0.0.8.tar.gz` & `tmp/profile-profile-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profile-profile-local-0.0.8.tar", last modified: Mon Oct 30 12:26:05 2023, max compression
+gzip compressed data, was "profile-profile-local-0.0.9.tar", last modified: Wed Nov 15 14:49:47 2023, max compression
```

## Comparing `profile-profile-local-0.0.8.tar` & `profile-profile-local-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 12:26:05.309521 profile-profile-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-10-30 12:26:05.309521 profile-profile-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-10-30 12:25:39.000000 profile-profile-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 12:26:05.309521 profile-profile-local-0.0.8/profile_profile_local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 12:25:39.000000 profile-profile-local-0.0.8/profile_profile_local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 12:26:05.309521 profile-profile-local-0.0.8/profile_profile_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 12:25:39.000000 profile-profile-local-0.0.8/profile_profile_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2023-10-30 12:25:39.000000 profile-profile-local-0.0.8/profile_profile_local/src/profile_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 12:26:05.309521 profile-profile-local-0.0.8/profile_profile_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-10-30 12:26:05.000000 profile-profile-local-0.0.8/profile_profile_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-10-30 12:26:05.000000 profile-profile-local-0.0.8/profile_profile_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 12:26:05.000000 profile-profile-local-0.0.8/profile_profile_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-30 12:26:05.000000 profile-profile-local-0.0.8/profile_profile_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-10-30 12:25:39.000000 profile-profile-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-30 12:26:05.309521 profile-profile-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-10-30 12:25:39.000000 profile-profile-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 14:49:47.761249 profile-profile-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2023-11-15 14:49:47.761249 profile-profile-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2023-11-15 14:49:23.000000 profile-profile-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 14:49:47.761249 profile-profile-local-0.0.9/profile_profile_local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 14:49:23.000000 profile-profile-local-0.0.9/profile_profile_local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 14:49:47.761249 profile-profile-local-0.0.9/profile_profile_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 14:49:23.000000 profile-profile-local-0.0.9/profile_profile_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2023-11-15 14:49:23.000000 profile-profile-local-0.0.9/profile_profile_local/src/profile_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 14:49:47.761249 profile-profile-local-0.0.9/profile_profile_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2023-11-15 14:49:47.000000 profile-profile-local-0.0.9/profile_profile_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2023-11-15 14:49:47.000000 profile-profile-local-0.0.9/profile_profile_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 14:49:47.000000 profile-profile-local-0.0.9/profile_profile_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-15 14:49:47.000000 profile-profile-local-0.0.9/profile_profile_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2023-11-15 14:49:23.000000 profile-profile-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 14:49:47.761249 profile-profile-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2023-11-15 14:49:23.000000 profile-profile-local-0.0.9/setup.py
```

### Comparing `profile-profile-local-0.0.8/README.md` & `profile-profile-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `profile-profile-local-0.0.8/profile_profile_local/src/profile_profile.py` & `profile-profile-local-0.0.9/profile_profile_local/src/profile_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,25 @@
         data = {
             'profile_id1': profile_id1,
             'profile_id2': profile_id2,
             'relationship_type_id': relationship_type_id,
             'job_title': f"'{job_title}'"
         }
         # TODO Please use parameter by name to make the code more readable
-        profile_profile_id = self.insert(json_data=data)
+        profile_profile_id = self.insert(data_json=data)
         logger.end(object={"profile_profile_id": profile_profile_id})
         return profile_profile_id
 
     def update_profile_profile(self, profile_profile_id: int, profile_profile_json_data: object) -> None:
         json = {
             'data': profile_profile_json_data
         }
         logger.start(object=json)
         self.update_by_id(
-            json_data=profile_profile_json_data, id_column_value=profile_profile_id)
+            data_json=profile_profile_json_data, id_column_value=profile_profile_id)
         logger.end("profile_profile updated")
 
     def delete_by_profile_profile_id(self, profile_profile_id: int) -> None:
         json = {
             "profile_profile_id": profile_profile_id,
         }
         logger.start(object=json)
```

### Comparing `profile-profile-local-0.0.8/setup.py` & `profile-profile-local-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
     # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix)
     name='profile-profile-local',
-    version='0.0.8',
+    version='0.0.9',
     author="Circles",
     author_email="info@circles.life",
     # TODO: Please update the description and delete this line
     description="PyPI Package for Circles profile-profile-local Python",
     # TODO: Please update the long description and delete this line
     long_description="This is a package for sharing common profile-profile-local function used in different repositories",
     long_description_content_type="text/markdown",
```

