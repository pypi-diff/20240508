# Comparing `tmp/packaged-0.0.0.tar.gz` & `tmp/packaged-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaged-0.0.0.tar", last modified: Sat May  4 21:40:36 2024, max compression
+gzip compressed data, was "packaged-0.0.1.tar", last modified: Wed May  8 21:45:39 2024, max compression
```

## Comparing `packaged-0.0.0.tar` & `packaged-0.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-04 21:40:36.409532 packaged-0.0.0/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2024-05-04 21:39:47.000000 packaged-0.0.0/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1732 2024-05-04 21:40:36.409463 packaged-0.0.0/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      643 2024-05-04 21:39:47.000000 packaged-0.0.0/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1180 2024-05-04 21:40:36.410199 packaged-0.0.0/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-04 21:39:47.000000 packaged-0.0.0/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-04 21:40:36.406429 packaged-0.0.0/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-04 21:40:36.408024 packaged-0.0.0/src/packaged/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      186 2024-05-04 21:39:47.000000 packaged-0.0.0/src/packaged/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.0.0/src/packaged/__main__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      386 2024-05-04 21:39:47.000000 packaged-0.0.0/src/packaged/cli.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.0.0/src/packaged/py.typed
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-04 21:40:36.408963 packaged-0.0.0/src/packaged.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1732 2024-05-04 21:40:36.000000 packaged-0.0.0/src/packaged.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      346 2024-05-04 21:40:36.000000 packaged-0.0.0/src/packaged.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-04 21:40:36.000000 packaged-0.0.0/src/packaged.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-04 21:40:36.000000 packaged-0.0.0/src/packaged.egg-info/entry_points.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       40 2024-05-04 21:40:36.000000 packaged-0.0.0/src/packaged.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-04 21:40:36.000000 packaged-0.0.0/src/packaged.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:45:39.772330 packaged-0.0.1/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2024-05-04 21:39:47.000000 packaged-0.0.1/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1923 2024-05-08 21:45:39.772188 packaged-0.0.1/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      808 2024-05-08 21:44:21.000000 packaged-0.0.1/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1233 2024-05-08 21:45:39.772669 packaged-0.0.1/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-04 21:39:47.000000 packaged-0.0.1/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:45:39.769325 packaged-0.0.1/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:45:39.770512 packaged-0.0.1/src/packaged/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3445 2024-05-08 21:37:01.000000 packaged-0.0.1/src/packaged/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.0.1/src/packaged/__main__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1149 2024-05-08 20:28:55.000000 packaged-0.0.1/src/packaged/cli.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.0.1/src/packaged/py.typed
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:00:51.000000 packaged-0.0.1/src/packaged/startup.template.sh
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-08 21:45:39.771588 packaged-0.0.1/src/packaged.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1923 2024-05-08 21:45:39.000000 packaged-0.0.1/src/packaged.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      379 2024-05-08 21:45:39.000000 packaged-0.0.1/src/packaged.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-08 21:45:39.000000 packaged-0.0.1/src/packaged.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-08 21:45:39.000000 packaged-0.0.1/src/packaged.egg-info/entry_points.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       51 2024-05-08 21:45:39.000000 packaged-0.0.1/src/packaged.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-08 21:45:39.000000 packaged-0.0.1/src/packaged.egg-info/top_level.txt
```

### Comparing `packaged-0.0.0/LICENSE` & `packaged-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `packaged-0.0.0/PKG-INFO` & `packaged-0.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.0.0
+Version: 0.0.1
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: yen>=0.4.2
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 
@@ -35,15 +36,23 @@
 
 ```bash
 pip install packaged
 ```
 
 ## Usage
 
-TODO
+```bash
+packaged <source_directory> <build_command> <startup_command>
+```
+
+For example:
+
+```bash
+packaged path/to/project.py 'pip install .' 'python -m your_package'
+```
 
 ## Local Development / Testing
 
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
 - Run `pytest` to run tests
```

### Comparing `packaged-0.0.0/README.md` & `packaged-0.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,23 @@
 
 ```bash
 pip install packaged
 ```
 
 ## Usage
 
-TODO
+```bash
+packaged <source_directory> <build_command> <startup_command>
+```
+
+For example:
+
+```bash
+packaged path/to/project.py 'pip install .' 'python -m your_package'
+```
 
 ## Local Development / Testing
 
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
 - Run `pytest` to run tests
```

### Comparing `packaged-0.0.0/setup.cfg` & `packaged-0.0.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = packaged
-version = 0.0.0
+version = 0.0.1
 description = The easiest way to ship python applications.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/packaged
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = MIT
@@ -20,14 +20,16 @@
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Typing :: Typed
 
 [options]
 packages = find:
+install_requires = 
+	yen>=0.4.2
 python_requires = >=3.8
 package_dir = =src
 
 [options.packages.find]
 where = ./src
 
 [options.entry_points]
@@ -41,14 +43,15 @@
 	pytest
 	pytest-cov
 	tox
 
 [options.package_data]
 packaged = 
 	py.typed
+	startup.template.sh
 
 [tool:pytest]
 addopts = --cov --cov-report=term-missing
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `packaged-0.0.0/src/packaged.egg-info/PKG-INFO` & `packaged-0.0.1/src/packaged.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.0.0
+Version: 0.0.1
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: yen>=0.4.2
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 
@@ -35,15 +36,23 @@
 
 ```bash
 pip install packaged
 ```
 
 ## Usage
 
-TODO
+```bash
+packaged <source_directory> <build_command> <startup_command>
+```
+
+For example:
+
+```bash
+packaged path/to/project.py 'pip install .' 'python -m your_package'
+```
 
 ## Local Development / Testing
 
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
 - Run `pytest` to run tests
```

