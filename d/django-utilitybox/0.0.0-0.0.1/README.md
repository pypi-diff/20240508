# Comparing `tmp/django_utilitybox-0.0.0.tar.gz` & `tmp/django_utilitybox-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_utilitybox-0.0.0.tar", last modified: Sat Apr 27 01:42:56 2024, max compression
+gzip compressed data, was "django_utilitybox-0.0.1.tar", last modified: Wed May  8 21:37:25 2024, max compression
```

## Comparing `django_utilitybox-0.0.0.tar` & `django_utilitybox-0.0.1.tar`

### file list

```diff
@@ -1,18 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 01:42:56.979702 django_utilitybox-0.0.0/
--rw-rw-rw-   0        0        0     1080 2024-04-24 18:36:00.000000 django_utilitybox-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      561 2024-04-27 01:42:56.978186 django_utilitybox-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-27 01:30:52.000000 django_utilitybox-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 01:42:56.971191 django_utilitybox-0.0.0/django_utilitybox/
--rw-rw-rw-   0        0        0       21 2024-04-24 18:36:00.000000 django_utilitybox-0.0.0/django_utilitybox/__init__.py
--rw-rw-rw-   0        0        0      173 2024-04-24 18:36:00.000000 django_utilitybox-0.0.0/django_utilitybox/__main__.py
--rw-rw-rw-   0        0        0        0 2024-04-24 18:36:00.000000 django_utilitybox-0.0.0/django_utilitybox/app.py
-drwxrwxrwx   0        0        0        0 2024-04-27 01:42:56.978186 django_utilitybox-0.0.0/django_utilitybox.egg-info/
--rw-rw-rw-   0        0        0      561 2024-04-27 01:42:56.000000 django_utilitybox-0.0.0/django_utilitybox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-04-27 01:42:56.000000 django_utilitybox-0.0.0/django_utilitybox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 01:42:56.000000 django_utilitybox-0.0.0/django_utilitybox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-27 01:42:56.000000 django_utilitybox-0.0.0/django_utilitybox.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-04-27 01:42:56.000000 django_utilitybox-0.0.0/django_utilitybox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 01:42:56.979702 django_utilitybox-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1091 2024-04-27 01:42:53.000000 django_utilitybox-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 01:42:56.976188 django_utilitybox-0.0.0/test/
--rw-rw-rw-   0        0        0        0 2024-04-24 18:36:00.000000 django_utilitybox-0.0.0/test/test.py
+drwxrwxrwx   0        0        0        0 2024-05-08 21:37:25.658645 django_utilitybox-0.0.1/
+-rw-rw-rw-   0        0        0     1080 2024-04-24 18:36:00.000000 django_utilitybox-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2385 2024-05-08 21:37:25.657500 django_utilitybox-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1790 2024-05-08 21:29:07.000000 django_utilitybox-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 21:37:25.644300 django_utilitybox-0.0.1/dj_utilitybox/
+-rw-rw-rw-   0        0        0        0 2024-05-01 21:11:39.000000 django_utilitybox-0.0.1/dj_utilitybox/__init__.py
+-rw-rw-rw-   0        0        0      173 2024-04-24 18:36:00.000000 django_utilitybox-0.0.1/dj_utilitybox/__main__.py
+-rw-rw-rw-   0        0        0        0 2024-04-24 18:36:00.000000 django_utilitybox-0.0.1/dj_utilitybox/app.py
+drwxrwxrwx   0        0        0        0 2024-05-08 21:37:25.645301 django_utilitybox-0.0.1/dj_utilitybox/get/
+-rw-rw-rw-   0        0        0        0 2024-04-27 01:09:15.000000 django_utilitybox-0.0.1/dj_utilitybox/get/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 21:37:25.646301 django_utilitybox-0.0.1/dj_utilitybox/post/
+-rw-rw-rw-   0        0        0        0 2024-04-27 01:09:15.000000 django_utilitybox-0.0.1/dj_utilitybox/post/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 21:37:25.649502 django_utilitybox-0.0.1/dj_utilitybox/response/
+-rw-rw-rw-   0        0        0        0 2024-05-01 21:11:39.000000 django_utilitybox-0.0.1/dj_utilitybox/response/__init__.py
+-rw-rw-rw-   0        0        0     1357 2024-05-01 21:05:52.000000 django_utilitybox-0.0.1/dj_utilitybox/response/base.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 01:52:02.000000 django_utilitybox-0.0.1/dj_utilitybox/response/good.py
+-rw-rw-rw-   0        0        0     2405 2024-05-08 20:57:49.000000 django_utilitybox-0.0.1/dj_utilitybox/response/raise_response.py
+drwxrwxrwx   0        0        0        0 2024-05-08 21:37:25.650503 django_utilitybox-0.0.1/dj_utilitybox/update/
+-rw-rw-rw-   0        0        0        0 2024-04-27 01:09:15.000000 django_utilitybox-0.0.1/dj_utilitybox/update/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 21:37:25.656503 django_utilitybox-0.0.1/django_utilitybox.egg-info/
+-rw-rw-rw-   0        0        0     2385 2024-05-08 21:37:25.000000 django_utilitybox-0.0.1/django_utilitybox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-05-08 21:37:25.000000 django_utilitybox-0.0.1/django_utilitybox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 21:37:25.000000 django_utilitybox-0.0.1/django_utilitybox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-08 21:37:25.000000 django_utilitybox-0.0.1/django_utilitybox.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-08 21:37:25.000000 django_utilitybox-0.0.1/django_utilitybox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 21:37:25.658645 django_utilitybox-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1103 2024-05-08 21:37:06.000000 django_utilitybox-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 21:37:25.657500 django_utilitybox-0.0.1/test/
+-rw-rw-rw-   0        0        0        0 2024-04-24 18:36:00.000000 django_utilitybox-0.0.1/test/test.py
```

### Comparing `django_utilitybox-0.0.0/LICENSE` & `django_utilitybox-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_utilitybox-0.0.0/setup.py` & `django_utilitybox-0.0.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from pathlib import Path
-from setuptools import setup
+from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.0'
+VERSION = '0.0.1'
 DESCRIPTION = '...'
 PACKAGE_NAME = 'django_utilitybox'
 AUTHOR = 'Jose Angel Colin Najera'
 EMAIL = 'josecolin99@gmail.com'
 GITHUB_URL = 'https://github.com/Josecolin99/...'
 
 setup(
     name = PACKAGE_NAME,
-    packages = [PACKAGE_NAME],
+    packages = find_packages(),
     entry_points={
         "console_scripts": [
-            "djangoutilitycmd=django_utilitybox.__main__:main"
+            "djangoutilitycmd=dj_utilitybox.__main__:main"
         ]
     },
     version = VERSION,
     license='MIT',
     description = DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
```

