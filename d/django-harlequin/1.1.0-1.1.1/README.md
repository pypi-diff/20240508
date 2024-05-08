# Comparing `tmp/django_harlequin-1.1.0.tar.gz` & `tmp/django_harlequin-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_harlequin-1.1.0.tar", last modified: Mon May  6 21:53:35 2024, max compression
+gzip compressed data, was "django_harlequin-1.1.1.tar", last modified: Wed May  8 09:51:40 2024, max compression
```

## Comparing `django_harlequin-1.1.0.tar` & `django_harlequin-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-06 21:53:35.546293 django_harlequin-1.1.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      239 2024-05-06 21:53:33.000000 django_harlequin-1.1.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2024-05-05 06:27:49.000000 django_harlequin-1.1.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      115 2024-05-05 06:26:38.000000 django_harlequin-1.1.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4273 2024-05-06 21:53:35.546036 django_harlequin-1.1.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2878 2024-05-06 12:17:13.000000 django_harlequin-1.1.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     2123 2024-05-06 21:53:33.000000 django_harlequin-1.1.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)       38 2024-05-06 21:53:35.546350 django_harlequin-1.1.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-06 21:53:35.543239 django_harlequin-1.1.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-06 21:53:35.544356 django_harlequin-1.1.0/src/django_harlequin/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.0/src/django_harlequin/__init__.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-06 21:53:35.545128 django_harlequin-1.1.0/src/django_harlequin/management/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.0/src/django_harlequin/management/__init__.py
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-06 21:53:35.545447 django_harlequin-1.1.0/src/django_harlequin/management/commands/
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.0/src/django_harlequin/management/commands/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5844 2024-05-06 21:17:40.000000 django_harlequin-1.1.0/src/django_harlequin/management/commands/harlequin.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.0/src/django_harlequin/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-06 21:53:35.545754 django_harlequin-1.1.0/src/django_harlequin.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4273 2024-05-06 21:53:35.000000 django_harlequin-1.1.0/src/django_harlequin.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      492 2024-05-06 21:53:35.000000 django_harlequin-1.1.0/src/django_harlequin.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2024-05-06 21:53:35.000000 django_harlequin-1.1.0/src/django_harlequin.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2024-05-06 21:53:35.000000 django_harlequin-1.1.0/src/django_harlequin.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       17 2024-05-06 21:53:35.000000 django_harlequin-1.1.0/src/django_harlequin.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-08 09:51:40.807324 django_harlequin-1.1.1/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      359 2024-05-08 09:51:37.000000 django_harlequin-1.1.1/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2024-05-05 06:27:49.000000 django_harlequin-1.1.1/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      115 2024-05-05 06:26:38.000000 django_harlequin-1.1.1/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4333 2024-05-08 09:51:40.807122 django_harlequin-1.1.1/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2913 2024-05-08 09:47:58.000000 django_harlequin-1.1.1/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2138 2024-05-08 09:51:37.000000 django_harlequin-1.1.1/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       38 2024-05-08 09:51:40.807374 django_harlequin-1.1.1/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-08 09:51:40.804038 django_harlequin-1.1.1/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-08 09:51:40.805457 django_harlequin-1.1.1/src/django_harlequin/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.1/src/django_harlequin/__init__.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-08 09:51:40.806324 django_harlequin-1.1.1/src/django_harlequin/management/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.1/src/django_harlequin/management/__init__.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-08 09:51:40.806553 django_harlequin-1.1.1/src/django_harlequin/management/commands/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.1/src/django_harlequin/management/commands/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5844 2024-05-06 21:17:40.000000 django_harlequin-1.1.1/src/django_harlequin/management/commands/harlequin.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2024-05-05 06:26:40.000000 django_harlequin-1.1.1/src/django_harlequin/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2024-05-08 09:51:40.806886 django_harlequin-1.1.1/src/django_harlequin.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4333 2024-05-08 09:51:40.000000 django_harlequin-1.1.1/src/django_harlequin.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      492 2024-05-08 09:51:40.000000 django_harlequin-1.1.1/src/django_harlequin.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2024-05-08 09:51:40.000000 django_harlequin-1.1.1/src/django_harlequin.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       22 2024-05-08 09:51:40.000000 django_harlequin-1.1.1/src/django_harlequin.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       17 2024-05-08 09:51:40.000000 django_harlequin-1.1.1/src/django_harlequin.egg-info/top_level.txt
```

### Comparing `django_harlequin-1.1.0/LICENSE` & `django_harlequin-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_harlequin-1.1.0/PKG-INFO` & `django_harlequin-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-harlequin
-Version: 1.1.0
+Version: 1.1.1
 Summary: Launch Harlequin, the SQL IDE for your Terminal, with your Django database configuration.
 Author-email: Adam Johnson <me@adamj.eu>
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-harlequin/blob/main/CHANGELOG.rst
 Project-URL: Funding, https://adamj.eu/books/
 Project-URL: Repository, https://github.com/adamchainz/django-harlequin
 Keywords: Django
@@ -26,14 +26,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Django>=3.2
+Requires-Dist: harlequin
 
 ================
 django-harlequin
 ================
 
 .. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/django-harlequin/main.yml.svg?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/django-harlequin/actions?workflow=CI
@@ -73,15 +74,15 @@
 
 **First,** install with pip:
 
 .. code-block:: bash
 
     python -m pip install django-harlequin
 
-**Second,** install the appropriate Harlequin `adapter package <https://harlequin.sh/docs/adapters>`__ for your database backend.
+**Second,** install the appropriate Harlequin `adapter package <https://harlequin.sh/docs/adapters>`__ for your database backend, if necessary (SQLite is built-in).
 For example, for the `PostgreSQL adapter <https://harlequin.sh/docs/postgres/index>`__:
 
 .. code-block:: bash
 
     python -m pip install harlequin-postgres
 
 **Third,** add the app to your ``INSTALLED_APPS`` setting:
```

### Comparing `django_harlequin-1.1.0/README.rst` & `django_harlequin-1.1.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 **First,** install with pip:
 
 .. code-block:: bash
 
     python -m pip install django-harlequin
 
-**Second,** install the appropriate Harlequin `adapter package <https://harlequin.sh/docs/adapters>`__ for your database backend.
+**Second,** install the appropriate Harlequin `adapter package <https://harlequin.sh/docs/adapters>`__ for your database backend, if necessary (SQLite is built-in).
 For example, for the `PostgreSQL adapter <https://harlequin.sh/docs/postgres/index>`__:
 
 .. code-block:: bash
 
     python -m pip install harlequin-postgres
 
 **Third,** add the app to your ``INSTALLED_APPS`` setting:
```

### Comparing `django_harlequin-1.1.0/pyproject.toml` & `django_harlequin-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools",
 ]
 
 [project]
 name = "django-harlequin"
-version = "1.1.0"
+version = "1.1.1"
 description = "Launch Harlequin, the SQL IDE for your Terminal, with your Django database configuration."
 readme = {file = "README.rst", content-type = "text/x-rst"}
 keywords = [
   "Django",
 ]
 license = {text = "MIT"}
 authors = [{name = "Adam Johnson", email = "me@adamj.eu"}]
@@ -33,14 +33,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Typing :: Typed",
 ]
 dependencies = [
   "Django>=3.2",
+  "harlequin",
 ]
 [project.urls]
 Changelog = "https://github.com/adamchainz/django-harlequin/blob/main/CHANGELOG.rst"
 Funding = "https://adamj.eu/books/"
 Repository = "https://github.com/adamchainz/django-harlequin"
 
 [tool.isort]
```

### Comparing `django_harlequin-1.1.0/src/django_harlequin/management/commands/harlequin.py` & `django_harlequin-1.1.1/src/django_harlequin/management/commands/harlequin.py`

 * *Files identical despite different names*

### Comparing `django_harlequin-1.1.0/src/django_harlequin.egg-info/PKG-INFO` & `django_harlequin-1.1.1/src/django_harlequin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-harlequin
-Version: 1.1.0
+Version: 1.1.1
 Summary: Launch Harlequin, the SQL IDE for your Terminal, with your Django database configuration.
 Author-email: Adam Johnson <me@adamj.eu>
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-harlequin/blob/main/CHANGELOG.rst
 Project-URL: Funding, https://adamj.eu/books/
 Project-URL: Repository, https://github.com/adamchainz/django-harlequin
 Keywords: Django
@@ -26,14 +26,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Django>=3.2
+Requires-Dist: harlequin
 
 ================
 django-harlequin
 ================
 
 .. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/django-harlequin/main.yml.svg?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/django-harlequin/actions?workflow=CI
@@ -73,15 +74,15 @@
 
 **First,** install with pip:
 
 .. code-block:: bash
 
     python -m pip install django-harlequin
 
-**Second,** install the appropriate Harlequin `adapter package <https://harlequin.sh/docs/adapters>`__ for your database backend.
+**Second,** install the appropriate Harlequin `adapter package <https://harlequin.sh/docs/adapters>`__ for your database backend, if necessary (SQLite is built-in).
 For example, for the `PostgreSQL adapter <https://harlequin.sh/docs/postgres/index>`__:
 
 .. code-block:: bash
 
     python -m pip install harlequin-postgres
 
 **Third,** add the app to your ``INSTALLED_APPS`` setting:
```

