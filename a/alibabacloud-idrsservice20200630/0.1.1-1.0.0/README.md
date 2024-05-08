# Comparing `tmp/alibabacloud_idrsservice20200630-0.1.1.tar.gz` & `tmp/alibabacloud_idrsservice20200630-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_idrsservice20200630-0.1.1.tar", last modified: Tue May  7 17:11:44 2024, max compression
+gzip compressed data, was "dist/alibabacloud_idrsservice20200630-1.0.0.tar", last modified: Wed Aug 19 06:26:22 2020, max compression
```

## Comparing `alibabacloud_idrsservice20200630-0.1.1.tar` & `alibabacloud_idrsservice20200630-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/
--rw-r--r--   0 root         (0) root         (0)      222 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2457 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1127 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1212 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/alibabacloud_idrsservice20200630/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/alibabacloud_idrsservice20200630/__init__.py
--rw-r--r--   0 root         (0) root         (0)   215373 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/alibabacloud_idrsservice20200630/client.py
--rw-r--r--   0 root         (0) root         (0)   449624 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/alibabacloud_idrsservice20200630/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/alibabacloud_idrsservice20200630.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/alibabacloud_idrsservice20200630.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/alibabacloud_idrsservice20200630.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/alibabacloud_idrsservice20200630.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/alibabacloud_idrsservice20200630.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/alibabacloud_idrsservice20200630.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2651 2024-05-07 17:11:44.000000 alibabacloud_idrsservice20200630-0.1.1/setup.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/
+-rw-rw-r--   0 admin      (531) admin      (531)       38 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/setup.cfg
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/alibabacloud_idrsservice20200630.egg-info/
+-rw-rw-r--   0 admin      (531) admin      (531)        1 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/alibabacloud_idrsservice20200630.egg-info/dependency_links.txt
+-rw-rw-r--   0 admin      (531) admin      (531)       91 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/alibabacloud_idrsservice20200630.egg-info/requires.txt
+-rw-rw-r--   0 admin      (531) admin      (531)      428 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/alibabacloud_idrsservice20200630.egg-info/SOURCES.txt
+-rw-rw-r--   0 admin      (531) admin      (531)       33 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/alibabacloud_idrsservice20200630.egg-info/top_level.txt
+-rw-rw-r--   0 admin      (531) admin      (531)     2231 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/alibabacloud_idrsservice20200630.egg-info/PKG-INFO
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/alibabacloud_idrsservice20200630/
+-rw-rw-r--   0 admin      (531) admin      (531)       21 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/alibabacloud_idrsservice20200630/__init__.py
+-rw-rw-r--   0 admin      (531) admin      (531)    24204 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/alibabacloud_idrsservice20200630/client.py
+-rw-rw-r--   0 admin      (531) admin      (531)   149111 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/alibabacloud_idrsservice20200630/models.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2692 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/setup.py
+-rw-rw-r--   0 admin      (531) admin      (531)      972 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/README.md
+-rw-rw-r--   0 admin      (531) admin      (531)     2231 2020-08-19 06:26:22.000000 alibabacloud_idrsservice20200630-1.0.0/PKG-INFO
```

### Comparing `alibabacloud_idrsservice20200630-0.1.1/PKG-INFO` & `alibabacloud_idrsservice20200630-1.0.0/alibabacloud_idrsservice20200630.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-Metadata-Version: 2.1
-Name: alibabacloud_idrsservice20200630
-Version: 0.1.1
+Metadata-Version: 1.1
+Name: alibabacloud-idrsservice20200630
+Version: 1.0.0
 Summary: Alibaba Cloud idrsservice (20200630) SDK Library for Python
-Home-page: https://github.com/aliyun/alibabacloud-python-sdk
+Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
         
         ## Alibaba Cloud idrsservice SDK for Python
         
-        ## Requirements
-        
-        - Python >= 3.6
-        
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
@@ -26,39 +22,36 @@
         pip install alibabacloud_idrsservice20200630
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/aliyun/alibabacloud-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
-        ## Usage
-        
-        [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
-        
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/idrsservice-20200630/ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
         
         [Apache-2.0](http://www.apache.org/licenses/LICENSE-2.0)
         
         Copyright (c) 2009-present, Alibaba Cloud All rights reserved.
         
-Keywords: alibabacloud,idrsservice20200630
+Keywords: alibabacloud_idrsservice20200630
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
```

### Comparing `alibabacloud_idrsservice20200630-0.1.1/README.md` & `alibabacloud_idrsservice20200630-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 English | [简体中文](README-CN.md)
 ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
 
 ## Alibaba Cloud idrsservice SDK for Python
 
-## Requirements
-
-- Python >= 3.6
-
 ## Installation
 
 - **Install with pip**
 
 Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
 
 ```bash
@@ -18,21 +14,17 @@
 pip install alibabacloud_idrsservice20200630
 ```
 
 ## Issues
 
 [Opening an Issue](https://github.com/aliyun/alibabacloud-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
 
-## Usage
-
-[Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
-
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/idrsservice-20200630/ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_idrsservice20200630-0.1.1/alibabacloud_idrsservice20200630.egg-info/PKG-INFO` & `alibabacloud_idrsservice20200630-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-Metadata-Version: 2.1
-Name: alibabacloud-idrsservice20200630
-Version: 0.1.1
+Metadata-Version: 1.1
+Name: alibabacloud_idrsservice20200630
+Version: 1.0.0
 Summary: Alibaba Cloud idrsservice (20200630) SDK Library for Python
-Home-page: https://github.com/aliyun/alibabacloud-python-sdk
+Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
         
         ## Alibaba Cloud idrsservice SDK for Python
         
-        ## Requirements
-        
-        - Python >= 3.6
-        
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
@@ -26,39 +22,36 @@
         pip install alibabacloud_idrsservice20200630
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/aliyun/alibabacloud-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
-        ## Usage
-        
-        [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
-        
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/idrsservice-20200630/ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
         
         [Apache-2.0](http://www.apache.org/licenses/LICENSE-2.0)
         
         Copyright (c) 2009-present, Alibaba Cloud All rights reserved.
         
-Keywords: alibabacloud,idrsservice20200630
+Keywords: alibabacloud_idrsservice20200630
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
```

### Comparing `alibabacloud_idrsservice20200630-0.1.1/setup.py` & `alibabacloud_idrsservice20200630-1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,66 +14,67 @@
  software distributed under the License is distributed on an
  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  KIND, either express or implied.  See the License for the
  specific language governing permissions and limitations
  under the License.
 """
 
+import sys
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_idrsservice20200630.
 
-Created on 07/05/2024
+Created on 19/08/2020
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_idrsservice20200630"
-NAME = "alibabacloud_idrsservice20200630" or "alibabacloud-package"
+NAME = "alibabacloud_idrsservice20200630"
 DESCRIPTION = "Alibaba Cloud idrsservice (20200630) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
-URL = "https://github.com/aliyun/alibabacloud-python-sdk"
+URL = "https://github.com/aliyun/alibabacloud-sdk"
+
+TOPDIR = os.path.dirname(__file__) or "."
 VERSION = __import__(PACKAGE).__version__
-REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
-    "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
-]
+REQUIRES = ["alibabacloud_tea_util==0.1.2","alibabacloud_tea_rpc==0.0.4","alibabacloud_endpoint_util==0.0.2"]
 
-LONG_DESCRIPTION = ''
-if os.path.exists('./README.md'):
+if sys.version_info[0] == 2:
+    with open("README.md") as fp:
+        LONG_DESCRIPTION = fp.read()
+else:
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
 
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
-    long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
     license="Apache License 2.0",
     url=URL,
-    keywords=["alibabacloud","idrsservice20200630"],
+    keywords=["alibabacloud_idrsservice20200630"],
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     platforms="any",
     install_requires=REQUIRES,
-    python_requires=">=3.6",
     classifiers=(
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
+        "Programming Language :: Python :: 2",
+        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
         "Topic :: Software Development"
     )
 )
```

