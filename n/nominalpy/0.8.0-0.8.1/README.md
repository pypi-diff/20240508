# Comparing `tmp/nominalpy-0.8.0.tar.gz` & `tmp/nominalpy-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nominalpy-0.8.0.tar", last modified: Fri Feb  9 04:00:53 2024, max compression
+gzip compressed data, was "nominalpy-0.8.1.tar", last modified: Tue May  7 06:18:04 2024, max compression
```

## Comparing `nominalpy-0.8.0.tar` & `nominalpy-0.8.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 04:00:53.479873 nominalpy-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-09 04:00:43.000000 nominalpy-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-02-09 04:00:53.479873 nominalpy-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-09 04:00:43.000000 nominalpy-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 04:00:53.479873 nominalpy-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-02-09 04:00:43.000000 nominalpy-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 04:00:53.471873 nominalpy-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 04:00:53.471873 nominalpy-0.8.0/src/nominalpy/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 04:00:53.475873 nominalpy-0.8.0/src/nominalpy/connection/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/connection/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/connection/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/connection/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 04:00:53.475873 nominalpy-0.8.0/src/nominalpy/image/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/image/visualiser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 04:00:53.475873 nominalpy-0.8.0/src/nominalpy/maths/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/maths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62348 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/maths/astro.py
--rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/maths/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    30685 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/maths/constellations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/maths/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/maths/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/maths/value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 04:00:53.475873 nominalpy-0.8.0/src/nominalpy/mqtt/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/mqtt/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 04:00:53.475873 nominalpy-0.8.0/src/nominalpy/objects/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/objects/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/objects/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/objects/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/objects/object.py
--rw-r--r--   0 runner    (1001) docker     (127)    31460 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/objects/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 04:00:53.475873 nominalpy-0.8.0/src/nominalpy/sensitivity/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/sensitivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/sensitivity/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/sensitivity/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/sensitivity/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 04:00:53.479873 nominalpy-0.8.0/src/nominalpy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/utils/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-09 04:00:43.000000 nominalpy-0.8.0/src/nominalpy/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 04:00:53.479873 nominalpy-0.8.0/src/nominalpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-02-09 04:00:53.000000 nominalpy-0.8.0/src/nominalpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-02-09 04:00:53.000000 nominalpy-0.8.0/src/nominalpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 04:00:53.000000 nominalpy-0.8.0/src/nominalpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-09 04:00:53.000000 nominalpy-0.8.0/src/nominalpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-09 04:00:53.000000 nominalpy-0.8.0/src/nominalpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:18:04.165345 nominalpy-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-07 06:17:58.000000 nominalpy-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-07 06:18:04.165345 nominalpy-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-07 06:17:58.000000 nominalpy-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 06:18:04.165345 nominalpy-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-07 06:17:58.000000 nominalpy-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:18:04.157345 nominalpy-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:18:04.157345 nominalpy-0.8.1/src/nominalpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:18:04.161345 nominalpy-0.8.1/src/nominalpy/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/connection/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/connection/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/connection/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:18:04.161345 nominalpy-0.8.1/src/nominalpy/image/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/image/visualiser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:18:04.161345 nominalpy-0.8.1/src/nominalpy/maths/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/maths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62348 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/maths/astro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/maths/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30685 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/maths/constellations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/maths/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/maths/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/maths/value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:18:04.161345 nominalpy-0.8.1/src/nominalpy/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/mqtt/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:18:04.165345 nominalpy-0.8.1/src/nominalpy/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/objects/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/objects/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/objects/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/objects/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31460 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/objects/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:18:04.165345 nominalpy-0.8.1/src/nominalpy/sensitivity/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/sensitivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/sensitivity/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/sensitivity/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/sensitivity/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:18:04.165345 nominalpy-0.8.1/src/nominalpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/utils/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-07 06:17:58.000000 nominalpy-0.8.1/src/nominalpy/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 06:18:04.165345 nominalpy-0.8.1/src/nominalpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-07 06:18:04.000000 nominalpy-0.8.1/src/nominalpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-07 06:18:04.000000 nominalpy-0.8.1/src/nominalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 06:18:04.000000 nominalpy-0.8.1/src/nominalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 06:18:04.000000 nominalpy-0.8.1/src/nominalpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 06:18:04.000000 nominalpy-0.8.1/src/nominalpy.egg-info/top_level.txt
```

### Comparing `nominalpy-0.8.0/LICENSE` & `nominalpy-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/README.md` & `nominalpy-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/setup.py` & `nominalpy-0.8.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 # with the 'nominalpy' module. Copyright Nominal Systems, 2024.
 
 from setuptools import setup, find_packages
 
 # Setup the project
 setup(
     name='nominalpy',
-    version='0.8.0',
+    version='0.8.1',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=["requests", "urllib3", "paho-mqtt", "numpy", "pandas", "matplotlib"],
     author='Nominal Systems',
     author_email='support@nominalsys.com',
     description='Python Interface to the Nominal API for simulations',
     long_description="This is the Python interface library for the Nominal API. \
+        The Nominal API allows access to spacecraft and space-domain simulation functions \
+        and the framework for simulating high-fidelity satellites. \
         It enables accessing the REST API simulation functions in an easy format.\
         Examples of how to construct Nominal simulations are provided on the\
         Nominal Systems documentation found at https://docs.nominalsys.com.",
     url='https://github.com/NominalSystems/nominalpy',
 )
```

### Comparing `nominalpy-0.8.0/src/nominalpy/connection/credentials.py` & `nominalpy-0.8.1/src/nominalpy/connection/credentials.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #                     [ NOMINAL SYSTEMS ]
 # This code is developed by Nominal Systems to aid with communication 
 # to the public API. All code is under the the license provided along
 # with the 'nominalpy' module. Copyright Nominal Systems, 2024.
 
-import requests, time
-from ..utils import printer
+import requests, time, json
+from ..utils import printer, NominalException
+import pkg_resources
 
 
 class Credentials:
     '''
     The Credentials class stores the credential access to the Nominal API 
     for making API calls to the server. This can allow for both a remote 
     or a local server call.
@@ -74,63 +75,88 @@
 
         # If this is a local-host, skip
         if self.is_local:
             return
         
         # A flag for whether this is the first attempt
         first_attempt: bool = True
-        SESSION_TIMEOUT: float = 30
-        counter: float = SESSION_TIMEOUT
+        
+        # Attempt to create the session
+        # If there is no valid session, it will throw an execption at this point.
+        self.__create_session()
         
         # Loop until the health is valid
         while True:
 
-            # If the time is greater than the wait, create a session
-            if counter >= SESSION_TIMEOUT:
-                self.__create_session()
-                counter = 0.0
-
             # Fetch the health
             if self.__is_healthy():
                 return
             
             # Print some information
             if first_attempt:
-                printer.warning("New sessions may take up to 3 minutes to start up. Please wait while your session is being configured.")
+                printer.warning("New sessions may take up to 3 minutes to start up. Each session will last 2 hours once created. Please wait while your session is being configured...")
                 first_attempt = False
-            else:
-                printer.log("Unable to find session. Attempting again in 10 seconds.")
             
-            # Wait some time
-            delta: float = 10.0
-            time.sleep(delta)
-            counter += delta
+            # Wait some time before attempting again
+            time.sleep(3.0)
 
     def __create_session (self) -> None:
         '''
         Attempts to create or fetch a new session from the AWS batch system. This
         will call the API for a new session or load one that already exists.
         '''
 
         # Fetch the data
         printer.log("Attempting to find or create a new user session. This may take a few seconds.")
         response = requests.get(
             self.url + "session", 
             verify=False, 
-            params={}, 
+            params={},
             headers = {'x-api-key': self.access_key, 'Content-Type': 'application/json'}
         )
 
         # Update the data and get the data
         if response.status_code == 200:
-            self.session_id = response.text
-            printer.log("A session has been created successfully.")
+            data: dict = json.loads(response.text)
+            self.session_id = data['id']
+            printer.log("A session has been found. Continuing session...")
+
+            # Fetch the version
+            api_version: str = data['version']
+            pkg_version: str = pkg_resources.get_distribution('nominalpy').version
+
+            # If the versions do not match, print a warning
+            if api_version != pkg_version:
+                printer.warning("API Version Mismatch. You are on an older version of the API. " +
+                    f"\nPlease upgrade to version {api_version} via 'pip install nominalpy --upgrade'. Some features may not work as intended.")
+        
+        # If there is a code, check the status
         else:
-            printer.error("Failed to create an API user session or retrieve previous session.")
 
+            # In the case of 402, then the account needs to purchase more credits
+            # In this case, stop the loop.
+            if response.status_code == 402:
+                data: dict = json.loads(response.text)
+                raise NominalException(data["error"])
+            
+            # Otherwise, check if there is an error message
+            else:
+
+                # Attempt to raise an exception with the custom error
+                try:
+                    data: dict = json.loads(response.text)
+                    error: str = data["error"]
+
+                # Otherwise, just raise the error manually
+                except:
+                    raise NominalException(f"ERROR {response.status_code}: {response.text}")
+                
+                # Raise the error with the data
+                raise NominalException(error)
+                
     def __is_healthy (self) -> bool:
         '''
         Returns whether the current session with the instance that is available
         is healthy as of right now. This will return a true or false flag.
 
         :returns:   A healthy success flag
         :rtype:     bool
```

### Comparing `nominalpy-0.8.0/src/nominalpy/connection/helper.py` & `nominalpy-0.8.1/src/nominalpy/connection/helper.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/connection/http.py` & `nominalpy-0.8.1/src/nominalpy/connection/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,9 +295,13 @@
 
     if code == 200:
         return
     elif code == 403:
         raise NominalException("Invalid Credentials: Access key is unauthorised to connect to the API.")
     elif code == 404:
         raise NominalException("Invalid Connection: The URL specified does not exist.")
+    elif code == 500:
+        raise NominalException("Invalid Connection: An internal server exception was thrown. Please try again later.")
+    elif code == 402:
+        raise NominalException("Invalid Connection: Your API key is not associated with a valid account. Please create an account and try again.")
     else:
         raise NominalException("Unknown Error: A communication link with the API is broken. Status Code: %d" % code)
```

### Comparing `nominalpy-0.8.0/src/nominalpy/image/visualiser.py` & `nominalpy-0.8.1/src/nominalpy/image/visualiser.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/maths/astro.py` & `nominalpy-0.8.1/src/nominalpy/maths/astro.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/maths/constants.py` & `nominalpy-0.8.1/src/nominalpy/maths/constants.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/maths/constellations.py` & `nominalpy-0.8.1/src/nominalpy/maths/constellations.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/maths/data.py` & `nominalpy-0.8.1/src/nominalpy/maths/data.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/maths/utils.py` & `nominalpy-0.8.1/src/nominalpy/maths/utils.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/maths/value.py` & `nominalpy-0.8.1/src/nominalpy/maths/value.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/mqtt/client.py` & `nominalpy-0.8.1/src/nominalpy/mqtt/client.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/objects/component.py` & `nominalpy-0.8.1/src/nominalpy/objects/component.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/objects/entity.py` & `nominalpy-0.8.1/src/nominalpy/objects/entity.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/objects/message.py` & `nominalpy-0.8.1/src/nominalpy/objects/message.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/objects/object.py` & `nominalpy-0.8.1/src/nominalpy/objects/object.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/objects/simulation.py` & `nominalpy-0.8.1/src/nominalpy/objects/simulation.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/sensitivity/analysis.py` & `nominalpy-0.8.1/src/nominalpy/sensitivity/analysis.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/sensitivity/case.py` & `nominalpy-0.8.1/src/nominalpy/sensitivity/case.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/sensitivity/configuration.py` & `nominalpy-0.8.1/src/nominalpy/sensitivity/configuration.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/utils/exception.py` & `nominalpy-0.8.1/src/nominalpy/utils/exception.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/utils/printer.py` & `nominalpy-0.8.1/src/nominalpy/utils/printer.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy/utils/types.py` & `nominalpy-0.8.1/src/nominalpy/utils/types.py`

 * *Files identical despite different names*

### Comparing `nominalpy-0.8.0/src/nominalpy.egg-info/SOURCES.txt` & `nominalpy-0.8.1/src/nominalpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

