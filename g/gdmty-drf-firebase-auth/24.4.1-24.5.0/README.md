# Comparing `tmp/gdmty_drf_firebase_auth-24.4.1.tar.gz` & `tmp/gdmty_drf_firebase_auth-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdmty_drf_firebase_auth-24.4.1.tar", last modified: Wed May  8 20:04:34 2024, max compression
+gzip compressed data, was "gdmty_drf_firebase_auth-24.5.0.tar", last modified: Wed May  8 20:05:16 2024, max compression
```

## Comparing `gdmty_drf_firebase_auth-24.4.1.tar` & `gdmty_drf_firebase_auth-24.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 20:04:34.048817 gdmty_drf_firebase_auth-24.4.1/
--rw-rw-rw-   0        0        0    11552 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.4.1/LICENSE
--rw-rw-rw-   0        0        0       51 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0    20224 2024-05-08 20:04:34.048817 gdmty_drf_firebase_auth-24.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     5806 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.4.1/README.md
--rw-rw-rw-   0        0        0     1645 2024-05-08 20:02:47.000000 gdmty_drf_firebase_auth-24.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 20:04:34.054039 gdmty_drf_firebase_auth-24.4.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 20:04:34.022452 gdmty_drf_firebase_auth-24.4.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 20:04:34.040312 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/
--rw-rw-rw-   0        0        0     1653 2024-05-08 20:02:47.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/__init__.py
--rw-rw-rw-   0        0        0      877 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/admin.py
--rw-rw-rw-   0        0        0      888 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/apps.py
--rw-rw-rw-   0        0        0     8657 2024-05-08 20:00:33.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/authentication.py
-drwxrwxrwx   0        0        0        0 2024-05-08 20:04:34.048817 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/migrations/
--rw-rw-rw-   0        0        0     1119 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      698 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/migrations/0002_initial.py
--rw-rw-rw-   0        0        0        0 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/migrations/__init__.py
--rw-rw-rw-   0        0        0     1759 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/models.py
--rw-rw-rw-   0        0        0     2494 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/settings.py
--rw-rw-rw-   0        0        0      743 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/tests.py
--rw-rw-rw-   0        0        0     2184 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/utils.py
--rw-rw-rw-   0        0        0      705 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/views.py
-drwxrwxrwx   0        0        0        0 2024-05-08 20:04:34.048817 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth.egg-info/
--rw-rw-rw-   0        0        0    20224 2024-05-08 20:04:34.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      807 2024-05-08 20:04:34.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 20:04:34.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2024-05-08 20:04:34.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-08 20:04:34.000000 gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 20:05:16.999149 gdmty_drf_firebase_auth-24.5.0/
+-rw-rw-rw-   0        0        0    11552 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.0/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    20224 2024-05-08 20:05:16.999149 gdmty_drf_firebase_auth-24.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5806 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.0/README.md
+-rw-rw-rw-   0        0        0     1645 2024-05-08 20:05:05.000000 gdmty_drf_firebase_auth-24.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 20:05:16.999149 gdmty_drf_firebase_auth-24.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 20:05:16.978944 gdmty_drf_firebase_auth-24.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 20:05:16.992643 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/
+-rw-rw-rw-   0        0        0     1653 2024-05-08 20:05:05.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/__init__.py
+-rw-rw-rw-   0        0        0      877 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/admin.py
+-rw-rw-rw-   0        0        0      888 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/apps.py
+-rw-rw-rw-   0        0        0     8657 2024-05-08 20:00:33.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/authentication.py
+drwxrwxrwx   0        0        0        0 2024-05-08 20:05:16.999149 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/migrations/
+-rw-rw-rw-   0        0        0     1119 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      698 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/migrations/0002_initial.py
+-rw-rw-rw-   0        0        0        0 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1759 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/models.py
+-rw-rw-rw-   0        0        0     2494 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/settings.py
+-rw-rw-rw-   0        0        0      743 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/tests.py
+-rw-rw-rw-   0        0        0     2184 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/utils.py
+-rw-rw-rw-   0        0        0      705 2024-04-03 19:57:48.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/views.py
+drwxrwxrwx   0        0        0        0 2024-05-08 20:05:16.999149 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth.egg-info/
+-rw-rw-rw-   0        0        0    20224 2024-05-08 20:05:16.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      807 2024-05-08 20:05:16.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 20:05:16.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2024-05-08 20:05:16.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-08 20:05:16.000000 gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth.egg-info/top_level.txt
```

### Comparing `gdmty_drf_firebase_auth-24.4.1/LICENSE` & `gdmty_drf_firebase_auth-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.4.1/PKG-INFO` & `gdmty_drf_firebase_auth-24.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-drf-firebase-auth
-Version: 24.4.1
+Version: 24.5.0
 Summary: Custom Django Rest Framework authentication backend than can be used with many firebase projects at same time, and storing as local users.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `gdmty_drf_firebase_auth-24.4.1/README.md` & `gdmty_drf_firebase_auth-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.4.1/pyproject.toml` & `gdmty_drf_firebase_auth-24.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gdmty-drf-firebase-auth"
-version = "24.4.1"
+version = "24.5.0"
 description = "Custom Django Rest Framework authentication backend than can be used with many firebase projects at same time, and storing as local users."
 readme = "README.md"
 authors = [{ name="Gobierno de Monterrey", email="cesar.benjamin@monterrey.gob.mx" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -32,15 +32,15 @@
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 "Homepage" = "https://github.com/SIGAMty/gdmty-drf-firebase-auth"
 "Bug Tracker" = "https://github.com/SIGAMty/gdmty-drf-firebase-auth/issues"
 
 [tool.bumpver]
-current_version = "24.4.1"
+current_version = "24.5.0"
 version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/__init__.py` & `gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 This package also adds support for login
 with email and password, and also adds support for
 custom user models. And is fully integrated with gdmty-id.
 
 """
 
 __title__ = 'gdmty_drf_firebase_auth'
-__version__ = '24.4.1'
+__version__ = '24.5.0'
 __description__ = (
     'Custom Django Rest Framework authentication backend for '
     'parsing Firebase uid tokens and storing as local users.'
     'This package is a fork of django-firebase-auth '
     'with some fixes and improvements. '
     'This package also adds support for login '
     'with email and password, and also adds support for '
```

### Comparing `gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/admin.py` & `gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/admin.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/apps.py` & `gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/apps.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/authentication.py` & `gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/migrations/0001_initial.py` & `gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/migrations/0002_initial.py` & `gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/models.py` & `gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/models.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/settings.py` & `gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/settings.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/tests.py` & `gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/tests.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/utils.py` & `gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/utils.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth/views.py` & `gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth/views.py`

 * *Files identical despite different names*

### Comparing `gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth.egg-info/PKG-INFO` & `gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-drf-firebase-auth
-Version: 24.4.1
+Version: 24.5.0
 Summary: Custom Django Rest Framework authentication backend than can be used with many firebase projects at same time, and storing as local users.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `gdmty_drf_firebase_auth-24.4.1/src/gdmty_drf_firebase_auth.egg-info/SOURCES.txt` & `gdmty_drf_firebase_auth-24.5.0/src/gdmty_drf_firebase_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

