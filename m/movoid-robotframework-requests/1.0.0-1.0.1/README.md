# Comparing `tmp/movoid_robotframework_requests-1.0.0.tar.gz` & `tmp/movoid_robotframework_requests-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_robotframework_requests-1.0.0.tar", last modified: Wed Feb 21 12:35:16 2024, max compression
+gzip compressed data, was "movoid_robotframework_requests-1.0.1.tar", last modified: Wed May  8 15:55:48 2024, max compression
```

## Comparing `movoid_robotframework_requests-1.0.0.tar` & `movoid_robotframework_requests-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-02-21 12:35:16.444757 movoid_robotframework_requests-1.0.0/
--rw-rw-rw-   0        0        0      363 2024-02-21 12:35:16.442756 movoid_robotframework_requests-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework_requests-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-21 12:35:16.431350 movoid_robotframework_requests-1.0.0/RobotFrameworkRequests/
--rw-rw-rw-   0        0        0      391 2024-02-21 12:31:34.000000 movoid_robotframework_requests-1.0.0/RobotFrameworkRequests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-21 12:35:16.433350 movoid_robotframework_requests-1.0.0/RobotFrameworkRequests/lib/
--rw-rw-rw-   0        0        0      267 2024-02-21 12:27:00.000000 movoid_robotframework_requests-1.0.0/RobotFrameworkRequests/lib/__init__.py
--rw-rw-rw-   0        0        0     2802 2024-02-21 12:31:34.000000 movoid_robotframework_requests-1.0.0/RobotFrameworkRequests/lib/requests.py
--rw-rw-rw-   0        0        0     1705 2024-02-13 09:37:13.000000 movoid_robotframework_requests-1.0.0/RobotFrameworkRequests/lib/type.py
-drwxrwxrwx   0        0        0        0 2024-02-21 12:35:16.436350 movoid_robotframework_requests-1.0.0/RobotFrameworkRequests/main/
--rw-rw-rw-   0        0        0      275 2024-02-21 12:15:19.000000 movoid_robotframework_requests-1.0.0/RobotFrameworkRequests/main/__init__.py
--rw-rw-rw-   0        0        0      262 2024-02-21 12:15:19.000000 movoid_robotframework_requests-1.0.0/RobotFrameworkRequests/main/action.py
--rw-rw-rw-   0        0        0      269 2024-02-21 11:27:41.000000 movoid_robotframework_requests-1.0.0/RobotFrameworkRequests/main/common.py
-drwxrwxrwx   0        0        0        0 2024-02-21 12:35:16.442756 movoid_robotframework_requests-1.0.0/movoid_robotframework_requests.egg-info/
--rw-rw-rw-   0        0        0      363 2024-02-21 12:35:16.000000 movoid_robotframework_requests-1.0.0/movoid_robotframework_requests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2024-02-21 12:35:16.000000 movoid_robotframework_requests-1.0.0/movoid_robotframework_requests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-21 12:35:16.000000 movoid_robotframework_requests-1.0.0/movoid_robotframework_requests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-02-21 12:35:16.000000 movoid_robotframework_requests-1.0.0/movoid_robotframework_requests.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-02-21 12:35:16.000000 movoid_robotframework_requests-1.0.0/movoid_robotframework_requests.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-21 12:35:16.444757 movoid_robotframework_requests-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      652 2024-02-21 11:24:50.000000 movoid_robotframework_requests-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:55:48.133720 movoid_robotframework_requests-1.0.1/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework_requests-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      394 2024-05-08 15:55:48.131670 movoid_robotframework_requests-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework_requests-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 15:55:48.106142 movoid_robotframework_requests-1.0.1/RobotFrameworkRequests/
+-rw-rw-rw-   0        0        0      391 2024-02-21 12:31:34.000000 movoid_robotframework_requests-1.0.1/RobotFrameworkRequests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:55:48.111264 movoid_robotframework_requests-1.0.1/RobotFrameworkRequests/lib/
+-rw-rw-rw-   0        0        0      267 2024-02-21 12:27:00.000000 movoid_robotframework_requests-1.0.1/RobotFrameworkRequests/lib/__init__.py
+-rw-rw-rw-   0        0        0     2757 2024-05-08 15:36:43.000000 movoid_robotframework_requests-1.0.1/RobotFrameworkRequests/lib/requests.py
+-rw-rw-rw-   0        0        0      405 2024-05-08 15:36:43.000000 movoid_robotframework_requests-1.0.1/RobotFrameworkRequests/lib/type.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:55:48.117417 movoid_robotframework_requests-1.0.1/RobotFrameworkRequests/main/
+-rw-rw-rw-   0        0        0      275 2024-02-21 12:15:19.000000 movoid_robotframework_requests-1.0.1/RobotFrameworkRequests/main/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-05-08 15:53:44.000000 movoid_robotframework_requests-1.0.1/RobotFrameworkRequests/main/action.py
+-rw-rw-rw-   0        0        0     1848 2024-05-08 15:53:44.000000 movoid_robotframework_requests-1.0.1/RobotFrameworkRequests/main/common.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:55:48.125867 movoid_robotframework_requests-1.0.1/movoid_robotframework_requests.egg-info/
+-rw-rw-rw-   0        0        0      394 2024-05-08 15:55:48.000000 movoid_robotframework_requests-1.0.1/movoid_robotframework_requests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      563 2024-05-08 15:55:48.000000 movoid_robotframework_requests-1.0.1/movoid_robotframework_requests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 15:55:48.000000 movoid_robotframework_requests-1.0.1/movoid_robotframework_requests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-05-08 15:55:48.000000 movoid_robotframework_requests-1.0.1/movoid_robotframework_requests.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-08 15:55:48.000000 movoid_robotframework_requests-1.0.1/movoid_robotframework_requests.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 15:55:48.133720 movoid_robotframework_requests-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      693 2024-05-08 15:54:51.000000 movoid_robotframework_requests-1.0.1/setup.py
```

### Comparing `movoid_robotframework_requests-1.0.0/RobotFrameworkRequests/lib/requests.py` & `movoid_robotframework_requests-1.0.1/RobotFrameworkRequests/lib/requests.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 # File          : requests
 # Author        : Sun YiFan-Movoid
 # Time          : 2024/1/31 0:07
 # Description   : 
 """
 from requests import Response
 
-from .type import TypeRequest, TypeResponse
-
 from typing import Dict
 
-import requests
 from movoid_function import wraps_func
 from movoid_function.type import Type
 from RobotFrameworkBasic import RfError
 
+import requests
+
 
 def simple_check_response_status(response_status: int = 200):
     _response_status = 200 if response_status is None else int(response_status)
 
     def dec(func):
         @wraps_func(func)
         def wrapper(kwargs, check_response_status=_response_status):
```

### Comparing `movoid_robotframework_requests-1.0.0/movoid_robotframework_requests.egg-info/SOURCES.txt` & `movoid_robotframework_requests-1.0.1/movoid_robotframework_requests.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+MANIFEST.in
 README.md
 setup.py
 RobotFrameworkRequests/__init__.py
 RobotFrameworkRequests/lib/__init__.py
 RobotFrameworkRequests/lib/requests.py
 RobotFrameworkRequests/lib/type.py
 RobotFrameworkRequests/main/__init__.py
```

### Comparing `movoid_robotframework_requests-1.0.0/setup.py` & `movoid_robotframework_requests-1.0.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='movoid_robotframework_requests',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     url='',
     license='',
     author='movoid',
     author_email='bobrobotsun@163.com',
     description='',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['requests',
                       'movoid_function',
+                      'movoid_package',
                       'movoid_robotframework',
                       'robotframework-requests',
                       ],
 )
```

