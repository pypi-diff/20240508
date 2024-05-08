# Comparing `tmp/pytest-rabbitmq-3.0.2.tar.gz` & `tmp/pytest_rabbitmq-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-rabbitmq-3.0.2.tar", last modified: Wed Jul  5 07:18:49 2023, max compression
+gzip compressed data, was "pytest_rabbitmq-3.1.0.tar", last modified: Wed May  8 09:55:05 2024, max compression
```

## Comparing `pytest-rabbitmq-3.0.2.tar` & `pytest_rabbitmq-3.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:18:49.066020 pytest-rabbitmq-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-07-05 07:18:49.066020 pytest-rabbitmq-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:18:49.062020 pytest-rabbitmq-3.0.2/pytest_rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:18:49.066020 pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:18:39.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:18:49.066020 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-07-05 07:18:49.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-05 07:18:49.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:18:49.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 07:18:49.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-05 07:18:49.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 07:18:49.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:18:48.000000 pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 07:18:49.066020 pytest-rabbitmq-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:55:05.389011 pytest_rabbitmq-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35146 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14942 2024-05-08 09:55:05.389011 pytest_rabbitmq-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:55:05.385010 pytest_rabbitmq-3.1.0/pytest_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/pytest_rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:55:05.385010 pytest_rabbitmq-3.1.0/pytest_rabbitmq/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/pytest_rabbitmq/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/pytest_rabbitmq/factories/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/pytest_rabbitmq/factories/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/pytest_rabbitmq/factories/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/pytest_rabbitmq/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:54:57.000000 pytest_rabbitmq-3.1.0/pytest_rabbitmq/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:55:05.385010 pytest_rabbitmq-3.1.0/pytest_rabbitmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14942 2024-05-08 09:55:05.000000 pytest_rabbitmq-3.1.0/pytest_rabbitmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-08 09:55:05.000000 pytest_rabbitmq-3.1.0/pytest_rabbitmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:55:05.000000 pytest_rabbitmq-3.1.0/pytest_rabbitmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 09:55:05.000000 pytest_rabbitmq-3.1.0/pytest_rabbitmq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-08 09:55:05.000000 pytest_rabbitmq-3.1.0/pytest_rabbitmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 09:55:05.000000 pytest_rabbitmq-3.1.0/pytest_rabbitmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:55:05.000000 pytest_rabbitmq-3.1.0/pytest_rabbitmq.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:55:05.389011 pytest_rabbitmq-3.1.0/setup.cfg
```

### Comparing `pytest-rabbitmq-3.0.2/CHANGES.rst` & `pytest_rabbitmq-3.1.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,28 @@
 CHANGELOG
 =========
 
 .. towncrier release notes start
 
+3.1.0 (2024-05-08)
+==================
+
+Features
+--------
+
+- Support Python 3.12 (`#469 <https://github.com/ClearcodeHQ/pytest-rabbitmq/issues/469>`_)
+
+
+Miscellaneus
+------------
+
+- Update code formatting with black 24.1 (`#424 <https://github.com/ClearcodeHQ/pytest-rabbitmq/issues/424>`_)
+- Drop Pipfile.lock from repository - rely on a cached/artifacted one. (`#468 <https://github.com/ClearcodeHQ/pytest-rabbitmq/issues/468>`_)
+
+
 3.0.2 (2023-07-05)
 ==================
 
 Bugfixes
 --------
 
 - Fixes logdir config option reading. (`#354 <https://github.com/ClearcodeHQ/pytest-rabbitmq/issues/354>`_)
```

### Comparing `pytest-rabbitmq-3.0.2/CONTRIBUTING.rst` & `pytest_rabbitmq-3.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.2/COPYING` & `pytest_rabbitmq-3.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.2/COPYING.lesser` & `pytest_rabbitmq-3.1.0/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.2/PKG-INFO` & `pytest_rabbitmq-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-rabbitmq
-Version: 3.0.2
+Version: 3.1.0
 Summary: RabbitMQ process and client fixtures for pytest
 Author-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,38 +166,43 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 Project-URL: Source, https://github.com/ClearcodeHQ/pytest-rabbitmq
 Project-URL: Bug Tracker, https://github.com/ClearcodeHQ/pytest-rabbitmq/issues
-Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.2/CHANGES.rst
+Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.1.0/CHANGES.rst
 Keywords: tests,pytest,fixture,rabbitmq,messsage queue
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: AUTHORS.rst
+Requires-Dist: pytest>=6.2
+Requires-Dist: port-for>=0.6.0
+Requires-Dist: mirakuru
+Requires-Dist: pika
 
 .. image:: https://raw.githubusercontent.com/ClearcodeHQ/pytest-rabbitmq/master/logo.png
     :width: 100px
     :height: 100px
     
 pytest-rabbitmq
 ===============
```

### Comparing `pytest-rabbitmq-3.0.2/README.rst` & `pytest_rabbitmq-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.2/pyproject.toml` & `pytest_rabbitmq-3.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest-rabbitmq"
-version = "3.0.2"
+version = "3.1.0"
 description = "RabbitMQ process and client fixtures for pytest"
 readme = "README.rst"
 keywords = ["tests", "pytest", "fixture", "rabbitmq", "messsage queue"]
 license = {file = "COPYING.lesser"}
 authors = [
     {name = "Grzegorz Śliwiński", email = "fizyk+pypi@fizyk.dev"}
 ]
@@ -17,14 +17,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Testing",
     "Framework :: Pytest",
 ]
 dependencies = [
@@ -34,15 +35,15 @@
     "pika",
 ]
 requires-python = ">= 3.8"
 
 [project.urls]
 "Source" = "https://github.com/ClearcodeHQ/pytest-rabbitmq"
 "Bug Tracker" = "https://github.com/ClearcodeHQ/pytest-rabbitmq/issues"
-"Changelog" = "https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.2/CHANGES.rst"
+"Changelog" = "https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.1.0/CHANGES.rst"
 
 [project.entry-points."pytest11"]
 pytest_rabbitmq = "pytest_rabbitmq.plugin"
 
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
@@ -98,15 +99,15 @@
 showcontent = true
 
 [tool.towncrier.fragment.misc]
 name = "Miscellaneus"
 showcontent = true
 
 [tool.tbump.version]
-current = "3.0.2"
+current = "3.1.0"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `pytest-rabbitmq-3.0.2/pytest_rabbitmq/__init__.py` & `pytest_rabbitmq-3.1.0/pytest_rabbitmq/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-rabbitmq. If not, see <http://www.gnu.org/licenses/>.
 """Main pytest-rabbitmq module."""
-__version__ = "3.0.2"
+__version__ = "3.1.0"
```

### Comparing `pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/__init__.py` & `pytest_rabbitmq-3.1.0/pytest_rabbitmq/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/client.py` & `pytest_rabbitmq-3.1.0/pytest_rabbitmq/factories/client.py`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/executor.py` & `pytest_rabbitmq-3.1.0/pytest_rabbitmq/factories/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """RabbitMQ Executor."""
+
 import re
 import subprocess
 from pathlib import Path
 from typing import List, Optional
 
 from mirakuru import TCPExecutor
```

### Comparing `pytest-rabbitmq-3.0.2/pytest_rabbitmq/factories/process.py` & `pytest_rabbitmq-3.1.0/pytest_rabbitmq/factories/process.py`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.2/pytest_rabbitmq/plugin.py` & `pytest_rabbitmq-3.1.0/pytest_rabbitmq/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/PKG-INFO` & `pytest_rabbitmq-3.1.0/pytest_rabbitmq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-rabbitmq
-Version: 3.0.2
+Version: 3.1.0
 Summary: RabbitMQ process and client fixtures for pytest
 Author-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,38 +166,43 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 Project-URL: Source, https://github.com/ClearcodeHQ/pytest-rabbitmq
 Project-URL: Bug Tracker, https://github.com/ClearcodeHQ/pytest-rabbitmq/issues
-Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.0.2/CHANGES.rst
+Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-rabbitmq/blob/v3.1.0/CHANGES.rst
 Keywords: tests,pytest,fixture,rabbitmq,messsage queue
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: COPYING
 License-File: COPYING.lesser
 License-File: AUTHORS.rst
+Requires-Dist: pytest>=6.2
+Requires-Dist: port-for>=0.6.0
+Requires-Dist: mirakuru
+Requires-Dist: pika
 
 .. image:: https://raw.githubusercontent.com/ClearcodeHQ/pytest-rabbitmq/master/logo.png
     :width: 100px
     :height: 100px
     
 pytest-rabbitmq
 ===============
```

### Comparing `pytest-rabbitmq-3.0.2/pytest_rabbitmq.egg-info/SOURCES.txt` & `pytest_rabbitmq-3.1.0/pytest_rabbitmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

