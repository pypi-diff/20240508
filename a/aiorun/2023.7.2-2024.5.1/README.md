# Comparing `tmp/aiorun-2023.7.2.tar.gz` & `tmp/aiorun-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorun-2023.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiorun-2024.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiorun-2023.7.2.tar` & `aiorun-2024.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      176 2022-10-24 05:13:26.729633 aiorun-2023.7.2/.coveragerc
--rw-r--r--   0        0        0      214 2022-10-24 05:13:26.729633 aiorun-2023.7.2/.dockerignore
--rw-r--r--   0        0        0       32 2022-10-24 05:13:26.729633 aiorun-2023.7.2/.flake8
--rw-r--r--   0        0        0       62 2022-10-24 05:13:26.729633 aiorun-2023.7.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      143 2022-10-24 05:13:26.729633 aiorun-2023.7.2/.github/dependabot.yml
--rw-r--r--   0        0        0     2045 2023-07-05 11:37:00.734767 aiorun-2023.7.2/.github/workflows/pythonapp.yml
--rw-r--r--   0        0        0     1157 2022-10-24 05:13:26.729633 aiorun-2023.7.2/.gitignore
--rw-r--r--   0        0        0      751 2022-10-24 05:13:26.729633 aiorun-2023.7.2/CHANGES
--rw-r--r--   0        0        0      213 2023-07-05 11:37:29.070554 aiorun-2023.7.2/CONTRIBUTORS
--rw-r--r--   0        0        0    11357 2022-10-24 05:13:26.729633 aiorun-2023.7.2/LICENSE
--rw-r--r--   0        0        0    18697 2022-10-24 05:13:26.729633 aiorun-2023.7.2/README.rst
--rw-r--r--   0        0        0      193 2022-10-24 05:13:26.729633 aiorun-2023.7.2/TODO
--rw-r--r--   0        0        0    17429 2023-07-05 12:04:00.838936 aiorun-2023.7.2/aiorun.py
--rw-r--r--   0        0        0      171 2022-10-24 05:13:26.729633 aiorun-2023.7.2/docker-compose.yml
--rw-r--r--   0        0        0      442 2022-10-24 05:13:26.729633 aiorun-2023.7.2/examples/echo_client.py
--rw-r--r--   0        0        0      705 2022-10-24 05:13:26.729633 aiorun-2023.7.2/examples/echo_server.py
--rw-r--r--   0        0        0      147 2022-10-24 05:13:26.729633 aiorun-2023.7.2/examples/stop_unhandled.py
--rw-r--r--   0        0        0      683 2022-10-24 05:13:26.729633 aiorun-2023.7.2/examples/stop_unhandled_custom.py
--rw-r--r--   0        0        0      324 2022-10-24 05:13:26.729633 aiorun-2023.7.2/examples/stop_unhandled_illegal.py
--rw-r--r--   0        0        0      262 2022-10-24 05:13:26.729633 aiorun-2023.7.2/examples/stop_unhandled_task.py
--rw-r--r--   0        0        0      794 2023-03-18 17:49:30.751617 aiorun-2023.7.2/pyproject.toml
--rw-r--r--   0        0        0      311 2022-10-24 05:13:26.729633 aiorun-2023.7.2/pytest.ini
--rw-r--r--   0        0        0       96 2022-10-24 05:13:26.729633 aiorun-2023.7.2/requirements-test.txt
--rw-r--r--   0        0        0      331 2022-10-24 05:13:26.729633 aiorun-2023.7.2/test.dockerfile
--rw-r--r--   0        0        0      330 2022-10-24 05:13:26.729633 aiorun-2023.7.2/test38.dockerfile
--rw-r--r--   0        0        0      359 2022-10-24 05:13:26.729633 aiorun-2023.7.2/tests/conftest.py
--rw-r--r--   0        0        0      290 2022-10-24 05:13:26.729633 aiorun-2023.7.2/tests/fake_main.py
--rw-r--r--   0        0        0    12135 2022-10-24 05:13:26.729633 aiorun-2023.7.2/tests/test_posix.py
--rw-r--r--   0        0        0     2625 2023-03-18 17:43:59.033791 aiorun-2023.7.2/tests/test_stop_on_errors.py
--rw-r--r--   0        0        0      947 2022-10-24 05:13:26.729633 aiorun-2023.7.2/tests/test_win.py
--rw-r--r--   0        0        0      315 2022-10-24 05:13:26.729633 aiorun-2023.7.2/testshield.py
--rw-r--r--   0        0        0       84 2022-10-24 05:13:26.729633 aiorun-2023.7.2/watchtest.sh
--rw-r--r--   0        0        0    19509 1970-01-01 00:00:00.000000 aiorun-2023.7.2/PKG-INFO
+-rw-r--r--   0        0        0      176 2022-10-24 05:13:26.729633 aiorun-2024.5.1/.coveragerc
+-rw-r--r--   0        0        0      214 2022-10-24 05:13:26.729633 aiorun-2024.5.1/.dockerignore
+-rw-r--r--   0        0        0       32 2022-10-24 05:13:26.729633 aiorun-2024.5.1/.flake8
+-rw-r--r--   0        0        0       62 2022-10-24 05:13:26.729633 aiorun-2024.5.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      143 2022-10-24 05:13:26.729633 aiorun-2024.5.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2020 2024-05-08 21:40:29.561044 aiorun-2024.5.1/.github/workflows/pythonapp.yml
+-rw-r--r--   0        0        0     1157 2022-10-24 05:13:26.729633 aiorun-2024.5.1/.gitignore
+-rw-r--r--   0        0        0      751 2022-10-24 05:13:26.729633 aiorun-2024.5.1/CHANGES
+-rw-r--r--   0        0        0      213 2023-07-05 11:37:29.070554 aiorun-2024.5.1/CONTRIBUTORS
+-rw-r--r--   0        0        0    11357 2022-10-24 05:13:26.729633 aiorun-2024.5.1/LICENSE
+-rw-r--r--   0        0        0    18697 2022-10-24 05:13:26.729633 aiorun-2024.5.1/README.rst
+-rw-r--r--   0        0        0      193 2022-10-24 05:13:26.729633 aiorun-2024.5.1/TODO
+-rw-r--r--   0        0        0    17374 2024-05-08 21:41:10.396832 aiorun-2024.5.1/aiorun.py
+-rw-r--r--   0        0        0      171 2022-10-24 05:13:26.729633 aiorun-2024.5.1/docker-compose.yml
+-rw-r--r--   0        0        0      442 2022-10-24 05:13:26.729633 aiorun-2024.5.1/examples/echo_client.py
+-rw-r--r--   0        0        0      705 2022-10-24 05:13:26.729633 aiorun-2024.5.1/examples/echo_server.py
+-rw-r--r--   0        0        0      147 2022-10-24 05:13:26.729633 aiorun-2024.5.1/examples/stop_unhandled.py
+-rw-r--r--   0        0        0      683 2022-10-24 05:13:26.729633 aiorun-2024.5.1/examples/stop_unhandled_custom.py
+-rw-r--r--   0        0        0      324 2022-10-24 05:13:26.729633 aiorun-2024.5.1/examples/stop_unhandled_illegal.py
+-rw-r--r--   0        0        0      262 2022-10-24 05:13:26.729633 aiorun-2024.5.1/examples/stop_unhandled_task.py
+-rw-r--r--   0        0        0      795 2024-05-08 21:40:29.561044 aiorun-2024.5.1/pyproject.toml
+-rw-r--r--   0        0        0      311 2022-10-24 05:13:26.729633 aiorun-2024.5.1/pytest.ini
+-rw-r--r--   0        0        0       96 2022-10-24 05:13:26.729633 aiorun-2024.5.1/requirements-test.txt
+-rw-r--r--   0        0        0      331 2022-10-24 05:13:26.729633 aiorun-2024.5.1/test.dockerfile
+-rw-r--r--   0        0        0      330 2022-10-24 05:13:26.729633 aiorun-2024.5.1/test38.dockerfile
+-rw-r--r--   0        0        0      359 2022-10-24 05:13:26.729633 aiorun-2024.5.1/tests/conftest.py
+-rw-r--r--   0        0        0      290 2022-10-24 05:13:26.729633 aiorun-2024.5.1/tests/fake_main.py
+-rw-r--r--   0        0        0    12135 2022-10-24 05:13:26.729633 aiorun-2024.5.1/tests/test_posix.py
+-rw-r--r--   0        0        0     2625 2023-03-18 17:43:59.033791 aiorun-2024.5.1/tests/test_stop_on_errors.py
+-rw-r--r--   0        0        0      947 2022-10-24 05:13:26.729633 aiorun-2024.5.1/tests/test_win.py
+-rw-r--r--   0        0        0      315 2022-10-24 05:13:26.729633 aiorun-2024.5.1/testshield.py
+-rw-r--r--   0        0        0       84 2022-10-24 05:13:26.729633 aiorun-2024.5.1/watchtest.sh
+-rw-r--r--   0        0        0    19510 1970-01-01 00:00:00.000000 aiorun-2024.5.1/PKG-INFO
```

### Comparing `aiorun-2023.7.2/.github/workflows/pythonapp.yml` & `aiorun-2024.5.1/.github/workflows/pythonapp.yml`

 * *Files 14% similar despite different names*

```diff
@@ -10,25 +10,24 @@
 
 jobs:
   build:
     name: Test on Python ${{ matrix.python-version }} and ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
-        os: [ubuntu-latest, windows-latest, macOS-latest]
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
+        os: [ubuntu-latest, windows-latest, macos-latest]
       fail-fast: false
     timeout-minutes: 15
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
-        architecture: x64
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -r requirements-test.txt flit pygments
     - name: Lint with flake8
       run: |
         pip install flake8
```

### Comparing `aiorun-2023.7.2/.gitignore` & `aiorun-2024.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aiorun-2023.7.2/CHANGES` & `aiorun-2024.5.1/CHANGES`

 * *Files identical despite different names*

### Comparing `aiorun-2023.7.2/LICENSE` & `aiorun-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorun-2023.7.2/README.rst` & `aiorun-2024.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `aiorun-2023.7.2/aiorun.py` & `aiorun-2024.5.1/aiorun.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         Callable[[AbstractEventLoop], Awaitable],
         Callable[[AbstractEventLoop], None],
     ]
 ]
 
 
 __all__ = ["run", "shutdown_waits_for"]
-__version__ = "2023.7.2"
+__version__ = "2024.5.1"
 logger = logging.getLogger("aiorun")
 WINDOWS = sys.platform == "win32"
 
 
 _DO_NOT_CANCEL_COROS = WeakSet()
 
 
@@ -290,15 +290,14 @@
 
     if tasks:
         logger.info("Cancelling pending tasks.")
         for t in tasks:
             # TODO: we don't need access to the coro. We could simply
             # TODO: store the task itself in the weakset.
             if t._coro not in _DO_NOT_CANCEL_COROS:
-                logger.debug("Cancelling task: %s", t)
                 t.cancel()
 
     async def wait_for_cancelled_tasks(timeout):
         """ Wait for the cancelled tasks to finish up. They have received
         CancelledError and must exit. However, it is possible that some
         badly-behaved tasks catch CancelledError (or BaseException) and
         then do not exit as they're supposed to. Thus, we only wait for
```

### Comparing `aiorun-2023.7.2/examples/echo_server.py` & `aiorun-2024.5.1/examples/echo_server.py`

 * *Files identical despite different names*

### Comparing `aiorun-2023.7.2/examples/stop_unhandled_custom.py` & `aiorun-2024.5.1/examples/stop_unhandled_custom.py`

 * *Files identical despite different names*

### Comparing `aiorun-2023.7.2/pyproject.toml` & `aiorun-2024.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
-requires = ["flit_core >=2,<3"]
+requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.flit.metadata]
 module = "aiorun"
 author = "Caleb Hattingh"
 author-email = "caleb.hattingh@gmail.com"
 home-page = "https://github.com/cjrh/aiorun"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent"
     ]
 description-file = "README.rst"
 requires-python = ">=3.7"
 
 [tool.flit.metadata.requires-extra]
 dev = [
```

### Comparing `aiorun-2023.7.2/tests/test_posix.py` & `aiorun-2024.5.1/tests/test_posix.py`

 * *Files identical despite different names*

### Comparing `aiorun-2023.7.2/tests/test_stop_on_errors.py` & `aiorun-2024.5.1/tests/test_stop_on_errors.py`

 * *Files identical despite different names*

### Comparing `aiorun-2023.7.2/tests/test_win.py` & `aiorun-2024.5.1/tests/test_win.py`

 * *Files identical despite different names*

### Comparing `aiorun-2023.7.2/PKG-INFO` & `aiorun-2024.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aiorun
-Version: 2023.7.2
+Version: 2024.5.1
 Summary: Boilerplate for asyncio applications
 Home-page: https://github.com/cjrh/aiorun
 Author: Caleb Hattingh
 Author-email: caleb.hattingh@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Provides-Extra: dev
 
 .. image:: https://github.com/cjrh/aiorun/workflows/Python%20application/badge.svg
     :target: https://github.com/cjrh/aiorun/actions
```

