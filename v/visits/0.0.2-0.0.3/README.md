# Comparing `tmp/visits-0.0.2.tar.gz` & `tmp/visits-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/visits-0.0.2.tar", last modified: Sun Apr 28 09:58:32 2024, max compression
+gzip compressed data, was "dist/visits-0.0.3.tar", last modified: Wed May  8 02:38:06 2024, max compression
```

## Comparing `visits-0.0.2.tar` & `visits-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-28 09:58:32.000000 visits-0.0.2/
--rw-r--r--   0 tux       (1000) users      (100)     1063 2024-04-27 23:43:36.000000 visits-0.0.2/LICENSE.txt
--rw-r--r--   0 tux       (1000) users      (100)      700 2024-04-28 09:58:32.000000 visits-0.0.2/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      133 2024-04-28 09:57:29.000000 visits-0.0.2/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2024-04-28 09:58:32.000000 visits-0.0.2/setup.cfg
--rw-r--r--   0 tux       (1000) users      (100)      860 2024-04-28 09:58:00.000000 visits-0.0.2/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-28 09:58:32.000000 visits-0.0.2/visits/
--rw-r--r--   0 tux       (1000) users      (100)       50 2024-04-28 09:58:15.000000 visits-0.0.2/visits/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      901 2024-04-28 09:38:21.000000 visits-0.0.2/visits/__main__.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-04-28 09:58:32.000000 visits-0.0.2/visits.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)      700 2024-04-28 09:58:32.000000 visits-0.0.2/visits.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      217 2024-04-28 09:58:32.000000 visits-0.0.2/visits.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2024-04-28 09:58:32.000000 visits-0.0.2/visits.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)       34 2024-04-28 09:58:32.000000 visits-0.0.2/visits.egg-info/requires.txt
--rw-r--r--   0 tux       (1000) users      (100)        7 2024-04-28 09:58:32.000000 visits-0.0.2/visits.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-05-08 02:38:06.000000 visits-0.0.3/
+-rw-r--r--   0 tux       (1000) users      (100)     1063 2024-04-27 23:43:36.000000 visits-0.0.3/LICENSE.txt
+-rw-r--r--   0 tux       (1000) users      (100)      699 2024-05-08 02:38:06.000000 visits-0.0.3/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      133 2024-04-28 09:57:29.000000 visits-0.0.3/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2024-05-08 02:38:06.000000 visits-0.0.3/setup.cfg
+-rw-r--r--   0 tux       (1000) users      (100)      859 2024-05-08 02:36:41.000000 visits-0.0.3/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-05-08 02:38:06.000000 visits-0.0.3/visits/
+-rw-r--r--   0 tux       (1000) users      (100)       50 2024-05-08 02:29:05.000000 visits-0.0.3/visits/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      901 2024-04-28 09:38:21.000000 visits-0.0.3/visits/__main__.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2024-05-08 02:38:06.000000 visits-0.0.3/visits.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)      699 2024-05-08 02:38:06.000000 visits-0.0.3/visits.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      217 2024-05-08 02:38:06.000000 visits-0.0.3/visits.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2024-05-08 02:38:06.000000 visits-0.0.3/visits.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)       34 2024-05-08 02:38:06.000000 visits-0.0.3/visits.egg-info/requires.txt
+-rw-r--r--   0 tux       (1000) users      (100)        7 2024-05-08 02:38:06.000000 visits-0.0.3/visits.egg-info/top_level.txt
```

### Comparing `visits-0.0.2/LICENSE.txt` & `visits-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `visits-0.0.2/PKG-INFO` & `visits-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: visits
-Version: 0.0.2
+Version: 0.0.3
 Summary: visits is just an example of a web page to display hits.
-Home-page: https://pypi.org/project/visits/
+Home-page: https://gitlab.com/nggit/visits
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
```

### Comparing `visits-0.0.2/setup.py` & `visits-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='visits',
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description=(
         'visits is just an example of a web page to display hits.'),
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://pypi.org/project/visits/',
+    url='https://gitlab.com/nggit/visits',
     packages=['visits'],
     install_requires=['terbilang', 'tremolo', 'tremolo_session'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Topic :: Internet :: WWW/HTTP :: HTTP Servers',
```

### Comparing `visits-0.0.2/visits/__main__.py` & `visits-0.0.3/visits/__main__.py`

 * *Files identical despite different names*

### Comparing `visits-0.0.2/visits.egg-info/PKG-INFO` & `visits-0.0.3/visits.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: visits
-Version: 0.0.2
+Version: 0.0.3
 Summary: visits is just an example of a web page to display hits.
-Home-page: https://pypi.org/project/visits/
+Home-page: https://gitlab.com/nggit/visits
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
```

