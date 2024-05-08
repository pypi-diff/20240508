# Comparing `tmp/testflows-2.3.0.tar.gz` & `tmp/testflows-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows-2.3.0.tar", last modified: Wed Mar  6 13:38:04 2024, max compression
+gzip compressed data, was "testflows-2.3.1.tar", last modified: Wed May  8 15:01:29 2024, max compression
```

## Comparing `testflows-2.3.0.tar` & `testflows-2.3.1.tar`

### file list

```diff
@@ -1,32 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:38:04.844568 testflows-2.3.0/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:38:04.840568 testflows-2.3.0/.github/
--rw-rw-r--   0 user      (1000) user      (1000)      597 2023-03-13 22:24:37.000000 testflows-2.3.0/.github/pull_request_template.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:38:04.840568 testflows-2.3.0/.github/workflows/
--rw-rw-r--   0 user      (1000) user      (1000)     1576 2023-03-13 22:24:37.000000 testflows-2.3.0/.github/workflows/cla.yml
--rw-rw-r--   0 user      (1000) user      (1000)       49 2022-12-28 17:16:30.000000 testflows-2.3.0/.gitignore
--rw-rw-r--   0 user      (1000) user      (1000)     1354 2023-03-13 22:24:37.000000 testflows-2.3.0/CONTRIBUTING.md
--rw-rw-r--   0 user      (1000) user      (1000)      630 2022-12-28 17:16:30.000000 testflows-2.3.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     3061 2024-03-06 13:38:04.844568 testflows-2.3.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2231 2023-11-30 21:26:32.000000 testflows-2.3.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:38:04.840568 testflows-2.3.0/cla/
--rw-rw-r--   0 user      (1000) user      (1000)      413 2023-03-13 21:20:58.000000 testflows-2.3.0/cla/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     7525 2023-03-13 19:25:51.000000 testflows-2.3.0/cla/corporate_v1.md
--rw-rw-r--   0 user      (1000) user      (1000)     6358 2023-03-13 22:24:37.000000 testflows-2.3.0/cla/individual_esign_v1.md
--rw-rw-r--   0 user      (1000) user      (1000)     6985 2023-03-13 19:25:51.000000 testflows-2.3.0/cla/individual_v1.md
--rwxrwxr-x   0 user      (1000) user      (1000)      814 2022-12-23 06:55:06.000000 testflows-2.3.0/install
--rwxrwxr-x   0 user      (1000) user      (1000)     1655 2022-12-23 06:55:06.000000 testflows-2.3.0/package
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-03-06 13:38:04.844568 testflows-2.3.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1758 2024-03-06 13:37:07.000000 testflows-2.3.0/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:38:04.840568 testflows-2.3.0/signatures/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:38:04.840568 testflows-2.3.0/signatures/version1/
--rw-rw-r--   0 user      (1000) user      (1000)      420 2023-04-14 21:06:49.000000 testflows-2.3.0/signatures/version1/cla.json
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:38:04.840568 testflows-2.3.0/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:38:04.840568 testflows-2.3.0/testflows/version/
--rw-rw-r--   0 user      (1000) user      (1000)      739 2022-12-28 17:16:30.000000 testflows-2.3.0/testflows/version/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-06 13:38:04.840568 testflows-2.3.0/testflows.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3061 2024-03-06 13:38:04.000000 testflows-2.3.0/testflows.egg-info/PKG-INFO
--rwxrwxr-x   0 user      (1000) user      (1000)      465 2024-03-06 13:38:04.000000 testflows-2.3.0/testflows.egg-info/SOURCES.txt
--rwxrwxr-x   0 user      (1000) user      (1000)        1 2024-03-06 13:38:04.000000 testflows-2.3.0/testflows.egg-info/dependency_links.txt
--rwxrwxr-x   0 user      (1000) user      (1000)        1 2022-12-23 06:55:06.000000 testflows-2.3.0/testflows.egg-info/not-zip-safe
--rwxrwxr-x   0 user      (1000) user      (1000)      231 2024-03-06 13:38:04.000000 testflows-2.3.0/testflows.egg-info/requires.txt
--rwxrwxr-x   0 user      (1000) user      (1000)       10 2024-03-06 13:38:04.000000 testflows-2.3.0/testflows.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:01:29.047178 testflows-2.3.1/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2024-03-14 16:48:03.000000 testflows-2.3.1/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     2767 2024-05-08 15:01:29.047178 testflows-2.3.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2231 2024-03-14 16:48:03.000000 testflows-2.3.1/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-08 15:01:29.047178 testflows-2.3.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1758 2024-05-08 15:00:51.000000 testflows-2.3.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:01:29.047178 testflows-2.3.1/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:01:29.047178 testflows-2.3.1/testflows/version/
+-rw-rw-r--   0 user      (1000) user      (1000)      739 2024-03-14 16:48:03.000000 testflows-2.3.1/testflows/version/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-08 15:01:29.047178 testflows-2.3.1/testflows.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2767 2024-05-08 15:01:29.000000 testflows-2.3.1/testflows.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      252 2024-05-08 15:01:29.000000 testflows-2.3.1/testflows.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-08 15:01:29.000000 testflows-2.3.1/testflows.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-08 15:01:29.000000 testflows-2.3.1/testflows.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)      231 2024-05-08 15:01:29.000000 testflows-2.3.1/testflows.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2024-05-08 15:01:29.000000 testflows-2.3.1/testflows.egg-info/top_level.txt
```

### Comparing `testflows-2.3.0/LICENSE` & `testflows-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows-2.3.0/PKG-INFO` & `testflows-2.3.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 Metadata-Version: 2.1
 Name: testflows
-Version: 2.3.0
+Version: 2.3.1
 Summary: TestFlows.com Open-Source Software Testing Framework
 Home-page: https://github.com/testflows/testflows
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: testflows.core==2.1.240306.1133530
-Requires-Dist: testflows.asserts==7.0.231001.1010150
-Requires-Dist: testflows.stash==1.1.230317.1211113
-Requires-Dist: testflows.uexpect==1.7.230414.1210501
-Requires-Dist: testflows.connect==1.7.230414.1210340
-Requires-Dist: testflows.database==1.6.200713.1142213
 Provides-Extra: dev
+License-File: LICENSE
 
 # TestFlows.com Open-Source Software Testing Framework
 
 ![TestFlows.com Open-Source Software Testing Framework](https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png)
 
 ## Introduction
 
@@ -101,7 +96,9 @@
 Join our channel on [Telegram].
 
 [TestFlows.com Open-Source Software Testing Framework]: https://testflows.com
 [Telegram]: https://telegram.me/testflows
 [pip3]: https://github.com/pypa/pip
 [Python 3]: https://www.python.org/
 [Ubuntu]: https://ubuntu.com/ 
+
+
```

### Comparing `testflows-2.3.0/README.md` & `testflows-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `testflows-2.3.0/install` & `testflows-2.3.1/testflows/version/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-#!/usr/bin/env python3
-# Copyright 2019 Katteli Inc.
+# Copyright 2021 Katteli Inc.
 # TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import subprocess
+import pkg_resources
 
-subprocess.run("pip3 uninstall -y testflows", shell=True)
-subprocess.run("pip3 install ./dist/*.tar.gz", shell=True)
+version = pkg_resources.get_distribution("testflows").version
```

### Comparing `testflows-2.3.0/setup.py` & `testflows-2.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setup(
     name="testflows",
-    version="2.3.0",
+    version="2.3.1",
     description="TestFlows.com Open-Source Software Testing Framework",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/testflows/testflows",
     classifiers=[
@@ -32,15 +32,15 @@
         "Operating System :: POSIX :: Linux",
     ],
     python_requires=">=3.8",
     license="Apache-2.0",
     packages=["testflows.version"],
     zip_safe=False,
     install_requires=[
-        "testflows.core==2.1.240306.1133530",
+        "testflows.core==2.0.240508.1150015",
         "testflows.asserts==7.0.231001.1010150",
         "testflows.stash==1.1.230317.1211113",
         "testflows.uexpect==1.7.230414.1210501",
         "testflows.connect==1.7.230414.1210340",
         "testflows.database==1.6.200713.1142213",
     ],
     extras_require={"dev": []},
```

### Comparing `testflows-2.3.0/testflows.egg-info/PKG-INFO` & `testflows-2.3.1/testflows.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 Metadata-Version: 2.1
 Name: testflows
-Version: 2.3.0
+Version: 2.3.1
 Summary: TestFlows.com Open-Source Software Testing Framework
 Home-page: https://github.com/testflows/testflows
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: testflows.core==2.1.240306.1133530
-Requires-Dist: testflows.asserts==7.0.231001.1010150
-Requires-Dist: testflows.stash==1.1.230317.1211113
-Requires-Dist: testflows.uexpect==1.7.230414.1210501
-Requires-Dist: testflows.connect==1.7.230414.1210340
-Requires-Dist: testflows.database==1.6.200713.1142213
 Provides-Extra: dev
+License-File: LICENSE
 
 # TestFlows.com Open-Source Software Testing Framework
 
 ![TestFlows.com Open-Source Software Testing Framework](https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png)
 
 ## Introduction
 
@@ -101,7 +96,9 @@
 Join our channel on [Telegram].
 
 [TestFlows.com Open-Source Software Testing Framework]: https://testflows.com
 [Telegram]: https://telegram.me/testflows
 [pip3]: https://github.com/pypa/pip
 [Python 3]: https://www.python.org/
 [Ubuntu]: https://ubuntu.com/ 
+
+
```

