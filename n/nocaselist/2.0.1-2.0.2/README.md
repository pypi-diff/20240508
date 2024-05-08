# Comparing `tmp/nocaselist-2.0.1.tar.gz` & `tmp/nocaselist-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nocaselist-2.0.1.tar", last modified: Sun May  5 08:13:14 2024, max compression
+gzip compressed data, was "nocaselist-2.0.2.tar", last modified: Wed May  8 15:43:20 2024, max compression
```

## Comparing `nocaselist-2.0.1.tar` & `nocaselist-2.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 08:13:14.020842 nocaselist-2.0.1/
--rw-r--r--   0 maiera     (501) staff       (20)      182 2024-05-04 16:41:38.000000 nocaselist-2.0.1/AUTHORS.md
--rw-r--r--   0 maiera     (501) staff       (20)      424 2022-08-04 11:04:17.000000 nocaselist-2.0.1/INSTALL.md
--rw-r--r--   0 maiera     (501) staff       (20)    11357 2022-08-04 11:04:17.000000 nocaselist-2.0.1/LICENSE
--rw-r--r--   0 maiera     (501) staff       (20)      262 2024-05-05 08:11:33.000000 nocaselist-2.0.1/MANIFEST.in
--rw-r--r--   0 maiera     (501) staff       (20)     4404 2024-05-05 08:13:14.020323 nocaselist-2.0.1/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)     2736 2024-05-05 08:11:22.000000 nocaselist-2.0.1/README.md
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 08:13:14.008436 nocaselist-2.0.1/nocaselist/
--rw-r--r--   0 maiera     (501) staff       (20)      226 2024-05-04 16:11:26.000000 nocaselist-2.0.1/nocaselist/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)    21739 2024-05-04 16:11:26.000000 nocaselist-2.0.1/nocaselist/_nocaselist.py
--rw-r--r--   0 maiera     (501) staff       (20)      361 2024-05-04 17:01:48.000000 nocaselist-2.0.1/nocaselist/_version.py
--rw-r--r--   0 maiera     (501) staff       (20)        0 2023-08-22 06:44:32.000000 nocaselist-2.0.1/nocaselist/py.typed
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 08:13:14.018389 nocaselist-2.0.1/nocaselist.egg-info/
--rw-r--r--   0 maiera     (501) staff       (20)     4404 2024-05-05 08:13:13.000000 nocaselist-2.0.1/nocaselist.egg-info/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)      629 2024-05-05 08:13:13.000000 nocaselist-2.0.1/nocaselist.egg-info/SOURCES.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2024-05-05 08:13:13.000000 nocaselist-2.0.1/nocaselist.egg-info/dependency_links.txt
--rw-r--r--   0 maiera     (501) staff       (20)      201 2024-05-05 08:13:13.000000 nocaselist-2.0.1/nocaselist.egg-info/requires.txt
--rw-r--r--   0 maiera     (501) staff       (20)       11 2024-05-05 08:13:13.000000 nocaselist-2.0.1/nocaselist.egg-info/top_level.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2024-05-05 08:13:13.000000 nocaselist-2.0.1/nocaselist.egg-info/zip-safe
--rw-r--r--   0 maiera     (501) staff       (20)      750 2023-08-22 06:44:32.000000 nocaselist-2.0.1/requirements.txt
--rw-r--r--   0 maiera     (501) staff       (20)       38 2024-05-05 08:13:14.020978 nocaselist-2.0.1/setup.cfg
--rwxr-xr-x   0 maiera     (501) staff       (20)     6681 2024-05-04 16:29:08.000000 nocaselist-2.0.1/setup.py
--rw-r--r--   0 maiera     (501) staff       (20)     1231 2023-08-22 06:48:32.000000 nocaselist-2.0.1/test-requirements.txt
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 08:13:14.012699 nocaselist-2.0.1/tests/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-19 13:03:24.000000 nocaselist-2.0.1/tests/__init__.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 08:13:14.013127 nocaselist-2.0.1/tests/installtest/
--rwxr-xr-x   0 maiera     (501) staff       (20)    11906 2024-05-04 16:11:26.000000 nocaselist-2.0.1/tests/installtest/test_install.sh
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 08:13:14.015957 nocaselist-2.0.1/tests/unittest/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-19 13:03:24.000000 nocaselist-2.0.1/tests/unittest/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)    85076 2024-05-04 16:11:26.000000 nocaselist-2.0.1/tests/unittest/test_nocaselist.py
--rw-r--r--   0 maiera     (501) staff       (20)      436 2024-05-04 16:11:26.000000 nocaselist-2.0.1/tests/unittest/test_package.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-05 08:13:14.017591 nocaselist-2.0.1/tests/utils/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 04:12:03.000000 nocaselist-2.0.1/tests/utils/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     3479 2024-05-04 16:11:26.000000 nocaselist-2.0.1/tests/utils/import_installed.py
--rw-r--r--   0 maiera     (501) staff       (20)     7202 2024-05-04 16:11:26.000000 nocaselist-2.0.1/tests/utils/simplified_test_function.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-08 15:43:20.981529 nocaselist-2.0.2/
+-rw-r--r--   0 maiera     (501) staff       (20)      182 2024-05-04 16:41:38.000000 nocaselist-2.0.2/AUTHORS.md
+-rw-r--r--   0 maiera     (501) staff       (20)      424 2022-08-04 11:04:17.000000 nocaselist-2.0.2/INSTALL.md
+-rw-r--r--   0 maiera     (501) staff       (20)    11357 2022-08-04 11:04:17.000000 nocaselist-2.0.2/LICENSE
+-rw-r--r--   0 maiera     (501) staff       (20)      262 2024-05-08 15:43:20.000000 nocaselist-2.0.2/MANIFEST.in
+-rw-r--r--   0 maiera     (501) staff       (20)     4619 2024-05-08 15:43:20.980917 nocaselist-2.0.2/PKG-INFO
+-rw-r--r--   0 maiera     (501) staff       (20)     2736 2024-05-05 08:11:22.000000 nocaselist-2.0.2/README.md
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-08 15:43:20.966885 nocaselist-2.0.2/nocaselist/
+-rw-r--r--   0 maiera     (501) staff       (20)      226 2024-05-04 16:11:26.000000 nocaselist-2.0.2/nocaselist/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)    21739 2024-05-04 16:11:26.000000 nocaselist-2.0.2/nocaselist/_nocaselist.py
+-rw-r--r--   0 maiera     (501) staff       (20)      361 2024-05-08 15:33:09.000000 nocaselist-2.0.2/nocaselist/_version.py
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2023-08-22 06:44:32.000000 nocaselist-2.0.2/nocaselist/py.typed
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-08 15:43:20.977905 nocaselist-2.0.2/nocaselist.egg-info/
+-rw-r--r--   0 maiera     (501) staff       (20)     4619 2024-05-08 15:43:20.000000 nocaselist-2.0.2/nocaselist.egg-info/PKG-INFO
+-rw-r--r--   0 maiera     (501) staff       (20)      629 2024-05-08 15:43:20.000000 nocaselist-2.0.2/nocaselist.egg-info/SOURCES.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        1 2024-05-08 15:43:20.000000 nocaselist-2.0.2/nocaselist.egg-info/dependency_links.txt
+-rw-r--r--   0 maiera     (501) staff       (20)      365 2024-05-08 15:43:20.000000 nocaselist-2.0.2/nocaselist.egg-info/requires.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       11 2024-05-08 15:43:20.000000 nocaselist-2.0.2/nocaselist.egg-info/top_level.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        1 2024-05-08 15:43:20.000000 nocaselist-2.0.2/nocaselist.egg-info/zip-safe
+-rw-r--r--   0 maiera     (501) staff       (20)      750 2023-08-22 06:44:32.000000 nocaselist-2.0.2/requirements.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       38 2024-05-08 15:43:20.981710 nocaselist-2.0.2/setup.cfg
+-rwxr-xr-x   0 maiera     (501) staff       (20)     6684 2024-05-06 07:20:33.000000 nocaselist-2.0.2/setup.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1652 2024-05-08 15:19:34.000000 nocaselist-2.0.2/test-requirements.txt
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-08 15:43:20.970820 nocaselist-2.0.2/tests/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-19 13:03:24.000000 nocaselist-2.0.2/tests/__init__.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-08 15:43:20.971251 nocaselist-2.0.2/tests/installtest/
+-rwxr-xr-x   0 maiera     (501) staff       (20)    11906 2024-05-04 16:11:26.000000 nocaselist-2.0.2/tests/installtest/test_install.sh
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-08 15:43:20.973465 nocaselist-2.0.2/tests/unittest/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-19 13:03:24.000000 nocaselist-2.0.2/tests/unittest/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)    85042 2024-05-06 07:10:18.000000 nocaselist-2.0.2/tests/unittest/test_nocaselist.py
+-rw-r--r--   0 maiera     (501) staff       (20)      436 2024-05-04 16:11:26.000000 nocaselist-2.0.2/tests/unittest/test_package.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2024-05-08 15:43:20.977104 nocaselist-2.0.2/tests/utils/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 04:12:03.000000 nocaselist-2.0.2/tests/utils/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     3446 2024-05-06 07:10:18.000000 nocaselist-2.0.2/tests/utils/import_installed.py
+-rw-r--r--   0 maiera     (501) staff       (20)     7202 2024-05-04 16:11:26.000000 nocaselist-2.0.2/tests/utils/simplified_test_function.py
```

### Comparing `nocaselist-2.0.1/LICENSE` & `nocaselist-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nocaselist-2.0.1/PKG-INFO` & `nocaselist-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nocaselist
-Version: 2.0.1
+Version: 2.0.2
 Summary: A case-insensitive list for Python
 Home-page: https://github.com/pywbem/nocaselist
 Author: Andreas Maier
 Author-email: andreas.r.maier@gmx.de
 Maintainer: Andreas Maier
 Maintainer-email: andreas.r.maier@gmx.de
 License: Apache Software License 2.0
@@ -21,24 +21,26 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: typing-extensions<4.2.0,>=3.10; python_version == "3.6"
 Requires-Dist: typing-extensions>=3.10; python_version >= "3.7"
 Provides-Extra: test
 Requires-Dist: pytest>=7.0.0; extra == "test"
-Requires-Dist: virtualenv>=20.1.0; extra == "test"
-Requires-Dist: six>=1.14.0; extra == "test"
-Requires-Dist: packaging<22.0,>=21.0; extra == "test"
+Requires-Dist: virtualenv<20.16.3,>=20.2.1; python_version <= "3.7" and extra == "test"
+Requires-Dist: virtualenv>=20.2.1; python_version >= "3.8" and extra == "test"
+Requires-Dist: six>=1.14.0; python_version <= "3.11" and extra == "test"
+Requires-Dist: six>=1.16.0; python_version >= "3.12" and extra == "test"
+Requires-Dist: packaging>=21.3; extra == "test"
 Requires-Dist: pluggy>=0.13.1; extra == "test"
 
 # nocaselist - A case-insensitive list for Python
 
 [![Version on Pypi](https://img.shields.io/pypi/v/nocaselist.svg)](https://pypi.python.org/pypi/nocaselist/)
 [![Test status (master)](https://github.com/pywbem/nocaselist/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/pywbem/nocaselist/actions/workflows/test.yml?query=branch%3Amaster)
 [![Docs status (master)](https://readthedocs.org/projects/nocaselist/badge/?version=latest)](https://readthedocs.org/projects/nocaselist/builds/)
```

### Comparing `nocaselist-2.0.1/README.md` & `nocaselist-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nocaselist-2.0.1/nocaselist/_nocaselist.py` & `nocaselist-2.0.2/nocaselist/_nocaselist.py`

 * *Files identical despite different names*

### Comparing `nocaselist-2.0.1/nocaselist.egg-info/PKG-INFO` & `nocaselist-2.0.2/nocaselist.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nocaselist
-Version: 2.0.1
+Version: 2.0.2
 Summary: A case-insensitive list for Python
 Home-page: https://github.com/pywbem/nocaselist
 Author: Andreas Maier
 Author-email: andreas.r.maier@gmx.de
 Maintainer: Andreas Maier
 Maintainer-email: andreas.r.maier@gmx.de
 License: Apache Software License 2.0
@@ -21,24 +21,26 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: typing-extensions<4.2.0,>=3.10; python_version == "3.6"
 Requires-Dist: typing-extensions>=3.10; python_version >= "3.7"
 Provides-Extra: test
 Requires-Dist: pytest>=7.0.0; extra == "test"
-Requires-Dist: virtualenv>=20.1.0; extra == "test"
-Requires-Dist: six>=1.14.0; extra == "test"
-Requires-Dist: packaging<22.0,>=21.0; extra == "test"
+Requires-Dist: virtualenv<20.16.3,>=20.2.1; python_version <= "3.7" and extra == "test"
+Requires-Dist: virtualenv>=20.2.1; python_version >= "3.8" and extra == "test"
+Requires-Dist: six>=1.14.0; python_version <= "3.11" and extra == "test"
+Requires-Dist: six>=1.16.0; python_version >= "3.12" and extra == "test"
+Requires-Dist: packaging>=21.3; extra == "test"
 Requires-Dist: pluggy>=0.13.1; extra == "test"
 
 # nocaselist - A case-insensitive list for Python
 
 [![Version on Pypi](https://img.shields.io/pypi/v/nocaselist.svg)](https://pypi.python.org/pypi/nocaselist/)
 [![Test status (master)](https://github.com/pywbem/nocaselist/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/pywbem/nocaselist/actions/workflows/test.yml?query=branch%3Amaster)
 [![Docs status (master)](https://readthedocs.org/projects/nocaselist/badge/?version=latest)](https://readthedocs.org/projects/nocaselist/builds/)
```

### Comparing `nocaselist-2.0.1/nocaselist.egg-info/SOURCES.txt` & `nocaselist-2.0.2/nocaselist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nocaselist-2.0.1/requirements.txt` & `nocaselist-2.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `nocaselist-2.0.1/setup.py` & `nocaselist-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         "test": test_requirements,
     },
     cmdclass={
         'test': test,
     },
     description="A case-insensitive list for Python",
     long_description=read_file('README.md'),
-    long_description_content_type='text/x-rst',
+    long_description_content_type='text/markdown',
     license="Apache Software License 2.0",
     author="Andreas Maier",
     author_email='andreas.r.maier@gmx.de',
     maintainer="Andreas Maier",
     maintainer_email='andreas.r.maier@gmx.de',
     url='https://github.com/pywbem/nocaselist',
     project_urls={
```

### Comparing `nocaselist-2.0.1/test-requirements.txt` & `nocaselist-2.0.2/test-requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -13,28 +13,34 @@
 # pytest 7.0.0 started using type hints
 pytest>=7.0.0
 
 
 # Install test direct dependencies:
 
 # virtualenv
-# tox 3.21.0 requires virtualenv!=20.0.[0-7],>=16.0.0 and requires py>=3.5
-virtualenv>=20.1.0
+# virtualenv 20.18.0 dropped support for Python 3.6
+# virtualenv 20.16.3 started requiring importlib-metadata>=4.8.3, but
+#   flake8 4.0/5.0 requires importlib-metadata>=1.1.0,<4.3 on Python<=3.7
+# virtualenv 20.2.1 started removing the prior pinning of importlib-metadata to <3
+# tox 3.21.0 requires virtualenv!=20.0.[0-7],>=16.0.0 and requires Python >=3.5
+virtualenv>=20.2.1,<20.16.3; python_version <= '3.7'
+virtualenv>=20.2.1; python_version >= '3.8'
 
 # six (also used by virtualenv, tox, probably others)
 # virtualenv 20.0 requires six>=1.12.0 on py>=3.8
 # tox 3.17 requires six>=1.14.0
-six>=1.14.0
+# six 1.16.0 fixes issue with 'six.moves' not available on Python 3.12
+six>=1.14.0; python_version <= '3.11'
+six>=1.16.0; python_version >= '3.12'
 
 
 # Indirect dependencies with special constraints:
 
 # packaging (used by pytest)
-# safety 2.3.5 started pinning packaging to <22.0 and requires >=21.0
-packaging>=21.0,<22.0
+packaging>=21.3
 
 # pluggy (used by pytest, tox)
 # Pluggy 0.12.0 has a bug causing pytest plugins to fail loading on py38
 # pytest 4.3.1 depends on pluggy>=0.7
 # tox 3.21.0 depends on pluggy>=0.12.0
 pluggy>=0.13.1
```

### Comparing `nocaselist-2.0.1/tests/installtest/test_install.sh` & `nocaselist-2.0.2/tests/installtest/test_install.sh`

 * *Files identical despite different names*

### Comparing `nocaselist-2.0.1/tests/unittest/test_nocaselist.py` & `nocaselist-2.0.2/tests/unittest/test_nocaselist.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,15 +429,15 @@
     # The code to be tested
     act_value = nclist[index]
 
     # Ensure that exceptions raised in the remainder of this function
     # are not mistaken as expected exceptions
     assert testcase.exp_exc_types is None
 
-    assert act_value == exp_value, "Unexpected value at index {}".format(index)
+    assert act_value == exp_value, f"Unexpected value at index {index}"
 
 
 TESTCASES_NOCASELIST_SETITEM = [
 
     # Testcases for NocaseList.__setitem__() / ncl[idx] = value
 
     # Each list item is a testcase tuple with these items:
@@ -584,15 +584,15 @@
     assert testcase.exp_exc_types is None
 
     # The verification below also uses some NocaseList features, but that is
     # unavoidable if we want to work through the public interface:
 
     act_value = nclist[index]  # Uses NocaseList.__getitem__()
 
-    assert act_value == value, "Unexpected value at index {}".format(index)
+    assert act_value == value, f"Unexpected value at index {index}"
 
     assert_equal(nclist, exp_nclist)  # Uses NocaseList.__iter__()
 
 
 TESTCASES_NOCASELIST_DELITEM = [
 
     # Testcases for NocaseList.__delitem__() / del ncl[idx]
@@ -1010,16 +1010,15 @@
     # The code to be tested
     act_result = value in nclist
 
     # Ensure that exceptions raised in the remainder of this function
     # are not mistaken as expected exceptions
     assert testcase.exp_exc_types is None
 
-    assert act_result == exp_result, \
-        "Unexpected result for value {!r}".format(value)
+    assert act_result == exp_result, f"Unexpected result for value {value!r}"
 
 
 TESTCASES_NOCASELIST_SIZEOF = [
 
     # Testcases for NocaseList.__sizeof__() / len(ncl)
 
     # Each list item is a testcase tuple with these items:
```

### Comparing `nocaselist-2.0.1/tests/utils/import_installed.py` & `nocaselist-2.0.2/tests/utils/import_installed.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,39 +46,39 @@
         dirpath = ''
         try:
             ix = sys.path.index(dirpath)
         except ValueError:
             ix = None
         if ix is not None:
             if test_installed == 'DEBUG':
-                print("Debug: Removing {0} at index {1} from module search "
-                      "path".format(dirpath, ix))
+                print(f"Debug: Removing {dirpath} at index {ix} from module "
+                      "search path")
             del sys.path[ix]
 
         # Move CWD to end. Reason is that when testing with an editable
         # installation, the CWD is needed, but when testing with a non-editable
         # installation, the package should not be found inthe CWD.
         # Note that somehow the CWD gets inserted at the begin of the search
         # path every time, so we need a loop.
         dirpath = os.getcwd()
         while True:
             try:
                 ix = sys.path.index(dirpath)
             except ValueError:
                 if test_installed == 'DEBUG':
-                    print("Debug: Appending {0} to end of module search "
-                          "path".format(dirpath))
+                    print(f"Debug: Appending {dirpath} to end of module "
+                          "search path")
                 sys.path.append(dirpath)
                 break
             if ix == len(sys.path) - 1:
                 # it exists once at the end
                 break
             if test_installed == 'DEBUG':
-                print("Debug: Removing {0} at index {1} from module search "
-                      "path".format(dirpath, ix))
+                print(f"Debug: Removing {dirpath} at index {ix} from module "
+                      "search path")
             del sys.path[ix]
 
     if module_name not in sys.modules:
         module = __import__(module_name, level=0)  # only absolute imports
         if test_installed == 'DEBUG':
             print("Debug: {0} module newly loaded from: {1}".
                   format(module_name, module.__file__))
```

### Comparing `nocaselist-2.0.1/tests/utils/simplified_test_function.py` & `nocaselist-2.0.2/tests/utils/simplified_test_function.py`

 * *Files identical despite different names*

