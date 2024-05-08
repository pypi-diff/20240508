# Comparing `tmp/django-camunda-0.9.5.tar.gz` & `tmp/django-camunda-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-camunda-0.9.5.tar", last modified: Tue Nov 17 16:18:05 2020, max compression
+gzip compressed data, was "dist/django-camunda-0.9.6.tar", last modified: Tue Nov 17 16:28:59 2020, max compression
```

## Comparing `django-camunda-0.9.5.tar` & `django-camunda-0.9.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 bbt       (1001) users      (985)        0 2020-11-17 16:18:05.891809 django-camunda-0.9.5/
--rw-r--r--   0 bbt       (1001) users      (985)     1061 2019-09-20 08:08:08.000000 django-camunda-0.9.5/LICENSE
--rw-r--r--   0 bbt       (1001) users      (985)      199 2019-09-20 08:08:08.000000 django-camunda-0.9.5/MANIFEST.in
--rw-r--r--   0 bbt       (1001) users      (985)     3678 2020-11-17 16:18:05.891809 django-camunda-0.9.5/PKG-INFO
--rw-r--r--   0 bbt       (1001) users      (985)     2094 2020-11-17 16:17:31.000000 django-camunda-0.9.5/README.rst
-drwxr-xr-x   0 bbt       (1001) users      (985)        0 2020-11-17 16:18:05.885142 django-camunda-0.9.5/django_camunda/
--rw-r--r--   0 bbt       (1001) users      (985)       63 2019-09-20 08:10:06.000000 django-camunda-0.9.5/django_camunda/__init__.py
--rw-r--r--   0 bbt       (1001) users      (985)     1431 2020-06-03 09:07:57.000000 django-camunda-0.9.5/django_camunda/admin.py
--rw-r--r--   0 bbt       (1001) users      (985)     3966 2020-08-25 10:20:40.000000 django-camunda-0.9.5/django_camunda/api.py
--rw-r--r--   0 bbt       (1001) users      (985)      102 2019-09-20 08:10:06.000000 django-camunda-0.9.5/django_camunda/apps.py
--rw-r--r--   0 bbt       (1001) users      (985)      563 2020-06-10 14:14:06.000000 django-camunda-0.9.5/django_camunda/bpmn.py
--rw-r--r--   0 bbt       (1001) users      (985)     3301 2020-11-17 16:17:24.000000 django-camunda-0.9.5/django_camunda/camunda_models.py
--rw-r--r--   0 bbt       (1001) users      (985)     3963 2020-03-20 15:10:34.000000 django-camunda-0.9.5/django_camunda/client.py
--rw-r--r--   0 bbt       (1001) users      (985)      115 2020-06-03 08:59:00.000000 django-camunda-0.9.5/django_camunda/constants.py
--rw-r--r--   0 bbt       (1001) users      (985)      797 2020-02-27 16:02:55.000000 django-camunda-0.9.5/django_camunda/fields.py
--rw-r--r--   0 bbt       (1001) users      (985)     4037 2020-07-29 13:02:35.000000 django-camunda-0.9.5/django_camunda/forms.py
--rw-r--r--   0 bbt       (1001) users      (985)      610 2019-09-20 09:23:39.000000 django-camunda-0.9.5/django_camunda/interface.py
-drwxr-xr-x   0 bbt       (1001) users      (985)        0 2020-11-17 16:18:05.888476 django-camunda-0.9.5/django_camunda/management/
--rw-r--r--   0 bbt       (1001) users      (985)        0 2020-03-20 14:56:54.000000 django-camunda-0.9.5/django_camunda/management/__init__.py
-drwxr-xr-x   0 bbt       (1001) users      (985)        0 2020-11-17 16:18:05.888476 django-camunda-0.9.5/django_camunda/management/commands/
--rw-r--r--   0 bbt       (1001) users      (985)        0 2020-03-20 14:56:54.000000 django-camunda-0.9.5/django_camunda/management/commands/__init__.py
--rw-r--r--   0 bbt       (1001) users      (985)      477 2020-03-20 14:56:54.000000 django-camunda-0.9.5/django_camunda/management/commands/delete_process_instance.py
-drwxr-xr-x   0 bbt       (1001) users      (985)        0 2020-11-17 16:18:05.891809 django-camunda-0.9.5/django_camunda/migrations/
--rw-r--r--   0 bbt       (1001) users      (985)     1323 2019-09-20 10:31:46.000000 django-camunda-0.9.5/django_camunda/migrations/0001_initial.py
--rw-r--r--   0 bbt       (1001) users      (985)      552 2020-02-27 16:02:55.000000 django-camunda-0.9.5/django_camunda/migrations/0002_camundaconfig_auth_header.py
--rw-r--r--   0 bbt       (1001) users      (985)      597 2020-02-27 16:02:55.000000 django-camunda-0.9.5/django_camunda/migrations/0003_auto_20200227_1552.py
--rw-r--r--   0 bbt       (1001) users      (985)      535 2020-05-25 09:35:13.000000 django-camunda-0.9.5/django_camunda/migrations/0004_camundaconfig_enabled.py
--rw-r--r--   0 bbt       (1001) users      (985)        0 2019-09-20 10:31:15.000000 django-camunda-0.9.5/django_camunda/migrations/__init__.py
--rw-r--r--   0 bbt       (1001) users      (985)     2613 2020-05-25 09:35:05.000000 django-camunda-0.9.5/django_camunda/models.py
--rw-r--r--   0 bbt       (1001) users      (985)     2361 2020-03-20 15:25:55.000000 django-camunda-0.9.5/django_camunda/tasks.py
--rw-r--r--   0 bbt       (1001) users      (985)      356 2020-06-10 14:14:06.000000 django-camunda-0.9.5/django_camunda/types.py
--rw-r--r--   0 bbt       (1001) users      (985)     2311 2020-06-03 09:07:53.000000 django-camunda-0.9.5/django_camunda/utils.py
-drwxr-xr-x   0 bbt       (1001) users      (985)        0 2020-11-17 16:18:05.888476 django-camunda-0.9.5/django_camunda.egg-info/
--rw-r--r--   0 bbt       (1001) users      (985)     3678 2020-11-17 16:18:05.000000 django-camunda-0.9.5/django_camunda.egg-info/PKG-INFO
--rw-r--r--   0 bbt       (1001) users      (985)     1050 2020-11-17 16:18:05.000000 django-camunda-0.9.5/django_camunda.egg-info/SOURCES.txt
--rw-r--r--   0 bbt       (1001) users      (985)        1 2020-11-17 16:18:05.000000 django-camunda-0.9.5/django_camunda.egg-info/dependency_links.txt
--rw-r--r--   0 bbt       (1001) users      (985)        1 2019-09-20 08:14:25.000000 django-camunda-0.9.5/django_camunda.egg-info/not-zip-safe
--rw-r--r--   0 bbt       (1001) users      (985)      232 2020-11-17 16:18:05.000000 django-camunda-0.9.5/django_camunda.egg-info/requires.txt
--rw-r--r--   0 bbt       (1001) users      (985)       15 2020-11-17 16:18:05.000000 django-camunda-0.9.5/django_camunda.egg-info/top_level.txt
--rw-r--r--   0 bbt       (1001) users      (985)     1901 2020-11-17 16:18:05.891809 django-camunda-0.9.5/setup.cfg
--rw-r--r--   0 bbt       (1001) users      (985)       38 2019-09-20 08:08:08.000000 django-camunda-0.9.5/setup.py
+drwxr-xr-x   0 bbt       (1001) users      (985)        0 2020-11-17 16:28:59.285155 django-camunda-0.9.6/
+-rw-r--r--   0 bbt       (1001) users      (985)     1061 2019-09-20 08:08:08.000000 django-camunda-0.9.6/LICENSE
+-rw-r--r--   0 bbt       (1001) users      (985)      199 2019-09-20 08:08:08.000000 django-camunda-0.9.6/MANIFEST.in
+-rw-r--r--   0 bbt       (1001) users      (985)     3678 2020-11-17 16:28:59.285155 django-camunda-0.9.6/PKG-INFO
+-rw-r--r--   0 bbt       (1001) users      (985)     2094 2020-11-17 16:28:31.000000 django-camunda-0.9.6/README.rst
+drwxr-xr-x   0 bbt       (1001) users      (985)        0 2020-11-17 16:28:59.281822 django-camunda-0.9.6/django_camunda/
+-rw-r--r--   0 bbt       (1001) users      (985)       63 2019-09-20 08:10:06.000000 django-camunda-0.9.6/django_camunda/__init__.py
+-rw-r--r--   0 bbt       (1001) users      (985)     1431 2020-06-03 09:07:57.000000 django-camunda-0.9.6/django_camunda/admin.py
+-rw-r--r--   0 bbt       (1001) users      (985)     3966 2020-08-25 10:20:40.000000 django-camunda-0.9.6/django_camunda/api.py
+-rw-r--r--   0 bbt       (1001) users      (985)      102 2019-09-20 08:10:06.000000 django-camunda-0.9.6/django_camunda/apps.py
+-rw-r--r--   0 bbt       (1001) users      (985)      563 2020-06-10 14:14:06.000000 django-camunda-0.9.6/django_camunda/bpmn.py
+-rw-r--r--   0 bbt       (1001) users      (985)     3350 2020-11-17 16:28:06.000000 django-camunda-0.9.6/django_camunda/camunda_models.py
+-rw-r--r--   0 bbt       (1001) users      (985)     3963 2020-03-20 15:10:34.000000 django-camunda-0.9.6/django_camunda/client.py
+-rw-r--r--   0 bbt       (1001) users      (985)      115 2020-06-03 08:59:00.000000 django-camunda-0.9.6/django_camunda/constants.py
+-rw-r--r--   0 bbt       (1001) users      (985)      797 2020-02-27 16:02:55.000000 django-camunda-0.9.6/django_camunda/fields.py
+-rw-r--r--   0 bbt       (1001) users      (985)     4037 2020-07-29 13:02:35.000000 django-camunda-0.9.6/django_camunda/forms.py
+-rw-r--r--   0 bbt       (1001) users      (985)      610 2019-09-20 09:23:39.000000 django-camunda-0.9.6/django_camunda/interface.py
+drwxr-xr-x   0 bbt       (1001) users      (985)        0 2020-11-17 16:28:59.281822 django-camunda-0.9.6/django_camunda/management/
+-rw-r--r--   0 bbt       (1001) users      (985)        0 2020-03-20 14:56:54.000000 django-camunda-0.9.6/django_camunda/management/__init__.py
+drwxr-xr-x   0 bbt       (1001) users      (985)        0 2020-11-17 16:28:59.281822 django-camunda-0.9.6/django_camunda/management/commands/
+-rw-r--r--   0 bbt       (1001) users      (985)        0 2020-03-20 14:56:54.000000 django-camunda-0.9.6/django_camunda/management/commands/__init__.py
+-rw-r--r--   0 bbt       (1001) users      (985)      477 2020-03-20 14:56:54.000000 django-camunda-0.9.6/django_camunda/management/commands/delete_process_instance.py
+drwxr-xr-x   0 bbt       (1001) users      (985)        0 2020-11-17 16:28:59.285155 django-camunda-0.9.6/django_camunda/migrations/
+-rw-r--r--   0 bbt       (1001) users      (985)     1323 2019-09-20 10:31:46.000000 django-camunda-0.9.6/django_camunda/migrations/0001_initial.py
+-rw-r--r--   0 bbt       (1001) users      (985)      552 2020-02-27 16:02:55.000000 django-camunda-0.9.6/django_camunda/migrations/0002_camundaconfig_auth_header.py
+-rw-r--r--   0 bbt       (1001) users      (985)      597 2020-02-27 16:02:55.000000 django-camunda-0.9.6/django_camunda/migrations/0003_auto_20200227_1552.py
+-rw-r--r--   0 bbt       (1001) users      (985)      535 2020-05-25 09:35:13.000000 django-camunda-0.9.6/django_camunda/migrations/0004_camundaconfig_enabled.py
+-rw-r--r--   0 bbt       (1001) users      (985)        0 2019-09-20 10:31:15.000000 django-camunda-0.9.6/django_camunda/migrations/__init__.py
+-rw-r--r--   0 bbt       (1001) users      (985)     2613 2020-05-25 09:35:05.000000 django-camunda-0.9.6/django_camunda/models.py
+-rw-r--r--   0 bbt       (1001) users      (985)     2361 2020-03-20 15:25:55.000000 django-camunda-0.9.6/django_camunda/tasks.py
+-rw-r--r--   0 bbt       (1001) users      (985)      356 2020-06-10 14:14:06.000000 django-camunda-0.9.6/django_camunda/types.py
+-rw-r--r--   0 bbt       (1001) users      (985)     2311 2020-06-03 09:07:53.000000 django-camunda-0.9.6/django_camunda/utils.py
+drwxr-xr-x   0 bbt       (1001) users      (985)        0 2020-11-17 16:28:59.281822 django-camunda-0.9.6/django_camunda.egg-info/
+-rw-r--r--   0 bbt       (1001) users      (985)     3678 2020-11-17 16:28:59.000000 django-camunda-0.9.6/django_camunda.egg-info/PKG-INFO
+-rw-r--r--   0 bbt       (1001) users      (985)     1050 2020-11-17 16:28:59.000000 django-camunda-0.9.6/django_camunda.egg-info/SOURCES.txt
+-rw-r--r--   0 bbt       (1001) users      (985)        1 2020-11-17 16:28:59.000000 django-camunda-0.9.6/django_camunda.egg-info/dependency_links.txt
+-rw-r--r--   0 bbt       (1001) users      (985)        1 2019-09-20 08:14:25.000000 django-camunda-0.9.6/django_camunda.egg-info/not-zip-safe
+-rw-r--r--   0 bbt       (1001) users      (985)      232 2020-11-17 16:28:59.000000 django-camunda-0.9.6/django_camunda.egg-info/requires.txt
+-rw-r--r--   0 bbt       (1001) users      (985)       15 2020-11-17 16:28:59.000000 django-camunda-0.9.6/django_camunda.egg-info/top_level.txt
+-rw-r--r--   0 bbt       (1001) users      (985)     1901 2020-11-17 16:28:59.285155 django-camunda-0.9.6/setup.cfg
+-rw-r--r--   0 bbt       (1001) users      (985)       38 2019-09-20 08:08:08.000000 django-camunda-0.9.6/setup.py
```

### Comparing `django-camunda-0.9.5/LICENSE` & `django-camunda-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/PKG-INFO` & `django-camunda-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: django-camunda
-Version: 0.9.5
+Version: 0.9.6
 Summary: Interact with Camunda from Django
 Home-page: https://github.com/maykinmedia/django-camunda
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Description: 
         
         .. django-camunda documentation master file, created by startproject.
            You can adapt this file completely to your liking, but it should at least
            contain the root `toctree` directive.
         
         Welcome to django-camunda's documentation!
         =================================================
         
-        :Version: 0.9.5
+        :Version: 0.9.6
         :Source: https://github.com/maykinmedia/django-camunda
         :Keywords: camunda, process engine, bpmn
         :PythonVersion: 3.7
         
         |build-status| |requirements| |coverage|
         
         |python-versions| |django-versions| |pypi-version|
```

### Comparing `django-camunda-0.9.5/README.rst` & `django-camunda-0.9.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 .. django-camunda documentation master file, created by startproject.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to django-camunda's documentation!
 =================================================
 
-:Version: 0.9.5
+:Version: 0.9.6
 :Source: https://github.com/maykinmedia/django-camunda
 :Keywords: camunda, process engine, bpmn
 :PythonVersion: 3.7
 
 |build-status| |requirements| |coverage|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `django-camunda-0.9.5/django_camunda/admin.py` & `django-camunda-0.9.6/django_camunda/admin.py`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/django_camunda/api.py` & `django-camunda-0.9.6/django_camunda/api.py`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/django_camunda/bpmn.py` & `django-camunda-0.9.6/django_camunda/bpmn.py`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/django_camunda/camunda_models.py` & `django-camunda-0.9.6/django_camunda/camunda_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 
 class Model:
     def __post_init__(self):
         self._type_cast()
 
     def _type_cast(self):
-        for attr, typehint in self.__annotations__.items():
+        annotations = get_all_annotations(self.__class__)
+        for attr, typehint in annotations.items():
             value = getattr(self, attr)
 
             if typehint is None:
                 typehint = type(None)
 
             # support for Optional
             if hasattr(typehint, "__origin__") and typehint.__origin__ is Union:
```

### Comparing `django-camunda-0.9.5/django_camunda/client.py` & `django-camunda-0.9.6/django_camunda/client.py`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/django_camunda/fields.py` & `django-camunda-0.9.6/django_camunda/fields.py`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/django_camunda/forms.py` & `django-camunda-0.9.6/django_camunda/forms.py`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/django_camunda/interface.py` & `django-camunda-0.9.6/django_camunda/interface.py`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/django_camunda/migrations/0001_initial.py` & `django-camunda-0.9.6/django_camunda/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/django_camunda/migrations/0002_camundaconfig_auth_header.py` & `django-camunda-0.9.6/django_camunda/migrations/0002_camundaconfig_auth_header.py`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/django_camunda/migrations/0003_auto_20200227_1552.py` & `django-camunda-0.9.6/django_camunda/migrations/0003_auto_20200227_1552.py`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/django_camunda/migrations/0004_camundaconfig_enabled.py` & `django-camunda-0.9.6/django_camunda/migrations/0004_camundaconfig_enabled.py`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/django_camunda/models.py` & `django-camunda-0.9.6/django_camunda/models.py`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/django_camunda/tasks.py` & `django-camunda-0.9.6/django_camunda/tasks.py`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/django_camunda/utils.py` & `django-camunda-0.9.6/django_camunda/utils.py`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/django_camunda.egg-info/PKG-INFO` & `django-camunda-0.9.6/django_camunda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: django-camunda
-Version: 0.9.5
+Version: 0.9.6
 Summary: Interact with Camunda from Django
 Home-page: https://github.com/maykinmedia/django-camunda
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Description: 
         
         .. django-camunda documentation master file, created by startproject.
            You can adapt this file completely to your liking, but it should at least
            contain the root `toctree` directive.
         
         Welcome to django-camunda's documentation!
         =================================================
         
-        :Version: 0.9.5
+        :Version: 0.9.6
         :Source: https://github.com/maykinmedia/django-camunda
         :Keywords: camunda, process engine, bpmn
         :PythonVersion: 3.7
         
         |build-status| |requirements| |coverage|
         
         |python-versions| |django-versions| |pypi-version|
```

### Comparing `django-camunda-0.9.5/django_camunda.egg-info/SOURCES.txt` & `django-camunda-0.9.6/django_camunda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-camunda-0.9.5/setup.cfg` & `django-camunda-0.9.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-camunda
-version = 0.9.5
+version = 0.9.6
 description = Interact with Camunda from Django
 long_description = file: README.rst
 url = https://github.com/maykinmedia/django-camunda
 license = MIT
 author = Maykin Media
 author_email = support@maykinmedia.nl
 keywords = camunda, process engine, bpmn, common ground
```

