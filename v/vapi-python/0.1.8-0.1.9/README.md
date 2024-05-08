# Comparing `tmp/vapi_python-0.1.8.tar.gz` & `tmp/vapi_python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vapi_python-0.1.8.tar", last modified: Sat Dec  2 19:31:44 2023, max compression
+gzip compressed data, was "vapi_python-0.1.9.tar", last modified: Wed May  8 07:02:45 2024, max compression
```

## Comparing `vapi_python-0.1.8.tar` & `vapi_python-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jordandearsley   (501) staff       (20)        0 2023-12-02 19:31:44.615412 vapi_python-0.1.8/
--rw-r--r--   0 jordandearsley   (501) staff       (20)       89 2023-11-22 03:53:10.000000 vapi_python-0.1.8/HISTORY.rst
--rw-r--r--   0 jordandearsley   (501) staff       (20)     1066 2023-11-20 23:03:05.000000 vapi_python-0.1.8/LICENSE
--rw-r--r--   0 jordandearsley   (501) staff       (20)      262 2023-11-20 23:03:05.000000 vapi_python-0.1.8/MANIFEST.in
--rw-r--r--   0 jordandearsley   (501) staff       (20)     4276 2023-12-02 19:31:44.615330 vapi_python-0.1.8/PKG-INFO
--rw-r--r--   0 jordandearsley   (501) staff       (20)     3443 2023-11-23 02:16:55.000000 vapi_python-0.1.8/README.rst
--rw-r--r--   0 jordandearsley   (501) staff       (20)      383 2023-12-02 19:31:44.615686 vapi_python-0.1.8/setup.cfg
--rw-r--r--   0 jordandearsley   (501) staff       (20)     1553 2023-12-02 19:31:10.000000 vapi_python-0.1.8/setup.py
-drwxr-xr-x   0 jordandearsley   (501) staff       (20)        0 2023-12-02 19:31:44.613704 vapi_python-0.1.8/vapi_python/
--rw-r--r--   0 jordandearsley   (501) staff       (20)      153 2023-11-23 02:16:55.000000 vapi_python-0.1.8/vapi_python/__init__.py
--rw-r--r--   0 jordandearsley   (501) staff       (20)     4993 2023-12-01 02:19:55.000000 vapi_python-0.1.8/vapi_python/daily_call.py
--rw-r--r--   0 jordandearsley   (501) staff       (20)     1385 2023-12-02 19:30:03.000000 vapi_python-0.1.8/vapi_python/vapi_python.py
-drwxr-xr-x   0 jordandearsley   (501) staff       (20)        0 2023-12-02 19:31:44.615003 vapi_python-0.1.8/vapi_python.egg-info/
--rw-r--r--   0 jordandearsley   (501) staff       (20)     4276 2023-12-02 19:31:44.000000 vapi_python-0.1.8/vapi_python.egg-info/PKG-INFO
--rw-r--r--   0 jordandearsley   (501) staff       (20)      384 2023-12-02 19:31:44.000000 vapi_python-0.1.8/vapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 jordandearsley   (501) staff       (20)        1 2023-12-02 19:31:44.000000 vapi_python-0.1.8/vapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 jordandearsley   (501) staff       (20)       53 2023-12-02 19:31:44.000000 vapi_python-0.1.8/vapi_python.egg-info/entry_points.txt
--rw-r--r--   0 jordandearsley   (501) staff       (20)        1 2023-11-22 03:53:21.000000 vapi_python-0.1.8/vapi_python.egg-info/not-zip-safe
--rw-r--r--   0 jordandearsley   (501) staff       (20)       21 2023-12-02 19:31:44.000000 vapi_python-0.1.8/vapi_python.egg-info/requires.txt
--rw-r--r--   0 jordandearsley   (501) staff       (20)       12 2023-12-02 19:31:44.000000 vapi_python-0.1.8/vapi_python.egg-info/top_level.txt
+drwxr-xr-x   0 jordandearsley   (501) staff       (20)        0 2024-05-08 07:02:45.453899 vapi_python-0.1.9/
+-rw-r--r--   0 jordandearsley   (501) staff       (20)       89 2024-05-08 06:59:31.000000 vapi_python-0.1.9/HISTORY.rst
+-rw-r--r--   0 jordandearsley   (501) staff       (20)     1066 2024-05-08 06:59:31.000000 vapi_python-0.1.9/LICENSE
+-rw-r--r--   0 jordandearsley   (501) staff       (20)      262 2024-05-08 06:59:31.000000 vapi_python-0.1.9/MANIFEST.in
+-rw-r--r--   0 jordandearsley   (501) staff       (20)     4752 2024-05-08 07:02:45.453832 vapi_python-0.1.9/PKG-INFO
+-rw-r--r--   0 jordandearsley   (501) staff       (20)     3895 2024-05-08 06:59:31.000000 vapi_python-0.1.9/README.rst
+-rw-r--r--   0 jordandearsley   (501) staff       (20)      383 2024-05-08 07:02:45.454169 vapi_python-0.1.9/setup.cfg
+-rw-r--r--   0 jordandearsley   (501) staff       (20)     1553 2024-05-08 06:59:31.000000 vapi_python-0.1.9/setup.py
+drwxr-xr-x   0 jordandearsley   (501) staff       (20)        0 2024-05-08 07:02:45.452545 vapi_python-0.1.9/vapi_python/
+-rw-r--r--   0 jordandearsley   (501) staff       (20)      153 2024-05-08 06:59:31.000000 vapi_python-0.1.9/vapi_python/__init__.py
+-rw-r--r--   0 jordandearsley   (501) staff       (20)     4993 2024-05-08 06:59:31.000000 vapi_python-0.1.9/vapi_python/daily_call.py
+-rw-r--r--   0 jordandearsley   (501) staff       (20)     1497 2024-05-08 06:59:31.000000 vapi_python-0.1.9/vapi_python/vapi_python.py
+drwxr-xr-x   0 jordandearsley   (501) staff       (20)        0 2024-05-08 07:02:45.453589 vapi_python-0.1.9/vapi_python.egg-info/
+-rw-r--r--   0 jordandearsley   (501) staff       (20)     4752 2024-05-08 07:02:45.000000 vapi_python-0.1.9/vapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 jordandearsley   (501) staff       (20)      384 2024-05-08 07:02:45.000000 vapi_python-0.1.9/vapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jordandearsley   (501) staff       (20)        1 2024-05-08 07:02:45.000000 vapi_python-0.1.9/vapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jordandearsley   (501) staff       (20)       53 2024-05-08 07:02:45.000000 vapi_python-0.1.9/vapi_python.egg-info/entry_points.txt
+-rw-r--r--   0 jordandearsley   (501) staff       (20)        1 2024-05-08 07:02:45.000000 vapi_python-0.1.9/vapi_python.egg-info/not-zip-safe
+-rw-r--r--   0 jordandearsley   (501) staff       (20)       30 2024-05-08 07:02:45.000000 vapi_python-0.1.9/vapi_python.egg-info/requires.txt
+-rw-r--r--   0 jordandearsley   (501) staff       (20)       12 2024-05-08 07:02:45.000000 vapi_python-0.1.9/vapi_python.egg-info/top_level.txt
```

### Comparing `vapi_python-0.1.8/LICENSE` & `vapi_python-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vapi_python-0.1.8/PKG-INFO` & `vapi_python-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vapi_python
-Version: 0.1.8
+Version: 0.1.9
 Summary: This package lets you start Vapi calls directly from Python.
 Home-page: https://github.com/jordan.cde/vapi_python
 Author: Vapi AI
 Author-email: team@vapi.ai
 License: MIT license
 Keywords: vapi_python
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: daily-python
 Requires-Dist: pyaudio
+Requires-Dist: requests
 
 ===============
 Vapi Python SDK
 ===============
 
 
 .. image:: https://img.shields.io/pypi/v/vapi_python.svg
@@ -93,15 +94,29 @@
          }
        }
      ]
    }
 
    vapi.start(assistant=assistant)
 
-The `start` method will initiate a new call. 
+The `start` method will initiate a new call.
+
+You can override existing assistant parameters or set variables with the `assistant_overrides` parameter.
+Assume the first message is `Hey, {{name}} how are you?` and you want to set the value of `name` to `John`:
+
+.. code-block:: python
+
+   assistant_overrides = {
+      "recordingEnabled": False,
+      "variableValues": {
+         "name": "John"
+      }
+   }
+
+   vapi.start(assistant_id='your-assistant-id', assistant_overrides=assistant_overrides)
 
 You can stop the session by calling the `stop` method:
 
 .. code-block:: python
 
    vapi.stop()
```

### Comparing `vapi_python-0.1.8/README.rst` & `vapi_python-0.1.9/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -71,15 +71,29 @@
          }
        }
      ]
    }
 
    vapi.start(assistant=assistant)
 
-The `start` method will initiate a new call. 
+The `start` method will initiate a new call.
+
+You can override existing assistant parameters or set variables with the `assistant_overrides` parameter.
+Assume the first message is `Hey, {{name}} how are you?` and you want to set the value of `name` to `John`:
+
+.. code-block:: python
+
+   assistant_overrides = {
+      "recordingEnabled": False,
+      "variableValues": {
+         "name": "John"
+      }
+   }
+
+   vapi.start(assistant_id='your-assistant-id', assistant_overrides=assistant_overrides)
 
 You can stop the session by calling the `stop` method:
 
 .. code-block:: python
 
    vapi.stop()
```

### Comparing `vapi_python-0.1.8/setup.py` & `vapi_python-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,10 +45,10 @@
     include_package_data=True,
     keywords='vapi_python',
     name='vapi_python',
     packages=find_packages(include=['vapi_python', 'vapi_python.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/jordan.cde/vapi_python',
-    version='0.1.8',
+    version='0.1.9',
     zip_safe=False,
 )
```

### Comparing `vapi_python-0.1.8/vapi_python/daily_call.py` & `vapi_python-0.1.9/vapi_python/daily_call.py`

 * *Files identical despite different names*

### Comparing `vapi_python-0.1.8/vapi_python/vapi_python.py` & `vapi_python-0.1.9/vapi_python/vapi_python.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 
 
 class Vapi:
     def __init__(self, *, api_key, api_url="https://api.vapi.ai"):
         self.api_key = api_key
         self.api_url = api_url
 
-    def start(self, *, assistant_id=None, assistant=None):
+    def start(self, *, assistant_id=None, assistant=None, assistant_overrides=None):
         # Start a new call
         if assistant_id:
-            assistant = {'assistantId': assistant_id}
+            assistant = {'assistantId': assistant_id, 'assistantOverrides': assistant_overrides}
         elif assistant:
-            assistant = {'assistant': assistant}
+            assistant = {'assistant': assistant, 'assistantOverrides': assistant_overrides}
 
         call_id, web_call_url = create_web_call(
             self.api_url, self.api_key, assistant)
 
         if not web_call_url:
             raise Exception("Error: Unable to create call.")
```

### Comparing `vapi_python-0.1.8/vapi_python.egg-info/PKG-INFO` & `vapi_python-0.1.9/vapi_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vapi-python
-Version: 0.1.8
+Name: vapi_python
+Version: 0.1.9
 Summary: This package lets you start Vapi calls directly from Python.
 Home-page: https://github.com/jordan.cde/vapi_python
 Author: Vapi AI
 Author-email: team@vapi.ai
 License: MIT license
 Keywords: vapi_python
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: daily-python
 Requires-Dist: pyaudio
+Requires-Dist: requests
 
 ===============
 Vapi Python SDK
 ===============
 
 
 .. image:: https://img.shields.io/pypi/v/vapi_python.svg
@@ -93,15 +94,29 @@
          }
        }
      ]
    }
 
    vapi.start(assistant=assistant)
 
-The `start` method will initiate a new call. 
+The `start` method will initiate a new call.
+
+You can override existing assistant parameters or set variables with the `assistant_overrides` parameter.
+Assume the first message is `Hey, {{name}} how are you?` and you want to set the value of `name` to `John`:
+
+.. code-block:: python
+
+   assistant_overrides = {
+      "recordingEnabled": False,
+      "variableValues": {
+         "name": "John"
+      }
+   }
+
+   vapi.start(assistant_id='your-assistant-id', assistant_overrides=assistant_overrides)
 
 You can stop the session by calling the `stop` method:
 
 .. code-block:: python
 
    vapi.stop()
```

