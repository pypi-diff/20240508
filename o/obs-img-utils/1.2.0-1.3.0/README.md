# Comparing `tmp/obs-img-utils-1.2.0.tar.gz` & `tmp/obs_img_utils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obs-img-utils-1.2.0.tar", last modified: Mon Mar  6 15:35:56 2023, max compression
+gzip compressed data, was "obs_img_utils-1.3.0.tar", last modified: Wed May  8 15:34:33 2024, max compression
```

## Comparing `obs-img-utils-1.2.0.tar` & `obs_img_utils-1.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:35:56.841220 obs-img-utils-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    32402 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-03-06 15:35:56.841220 obs-img-utils-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:35:56.841220 obs-img-utils-1.2.0/obs_img_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/obs_img_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20785 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/obs_img_utils/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/obs_img_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/obs_img_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/obs_img_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/obs_img_utils/web_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:35:56.841220 obs-img-utils-1.2.0/obs_img_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-03-06 15:35:56.000000 obs-img-utils-1.2.0/obs_img_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-06 15:35:56.000000 obs-img-utils-1.2.0/obs_img_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 15:35:56.000000 obs-img-utils-1.2.0/obs_img_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-06 15:35:56.000000 obs-img-utils-1.2.0/obs_img_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 15:35:56.000000 obs-img-utils-1.2.0/obs_img_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-06 15:35:56.000000 obs-img-utils-1.2.0/obs_img_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-06 15:35:56.000000 obs-img-utils-1.2.0/obs_img_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:35:56.841220 obs-img-utils-1.2.0/package/
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/package/python3-obs-img-utils.spec
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-06 15:35:56.841220 obs-img-utils-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:35:56.841220 obs-img-utils-1.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:35:56.841220 obs-img-utils-1.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/tests/data/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/tests/data/index.json
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/tests/data/index_name_picker.html
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/tests/data/index_new.html
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/tests/data/openSUSE-Leap-15.0-Azure.x86_64-1.0.0-Build1.133.packages
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/tests/data/report
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/tests/test_obs_img_utils_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/tests/test_obs_img_utils_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/tests/test_obs_img_utils_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-03-06 15:35:46.000000 obs-img-utils-1.2.0/tests/test_web_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:33.575693 obs_img_utils-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32402 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-08 15:34:33.575693 obs_img_utils-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:33.571694 obs_img_utils-1.3.0/obs_img_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/obs_img_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21144 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/obs_img_utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/obs_img_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/obs_img_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/obs_img_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/obs_img_utils/web_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:33.575693 obs_img_utils-1.3.0/obs_img_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-08 15:34:33.000000 obs_img_utils-1.3.0/obs_img_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-08 15:34:33.000000 obs_img_utils-1.3.0/obs_img_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:34:33.000000 obs_img_utils-1.3.0/obs_img_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 15:34:33.000000 obs_img_utils-1.3.0/obs_img_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:34:33.000000 obs_img_utils-1.3.0/obs_img_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-08 15:34:33.000000 obs_img_utils-1.3.0/obs_img_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 15:34:33.000000 obs_img_utils-1.3.0/obs_img_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:33.571694 obs_img_utils-1.3.0/package/
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/package/python3-obs-img-utils.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-08 15:34:33.575693 obs_img_utils-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:33.571694 obs_img_utils-1.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:34:33.575693 obs_img_utils-1.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/data/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/data/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/data/index_name_picker.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/data/index_new.html
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/data/openSUSE-Leap-15.0-Azure.x86_64-1.0.0-Build1.133.packages
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/data/report
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/test_obs_img_utils_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/test_obs_img_utils_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/test_obs_img_utils_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-08 15:34:25.000000 obs_img_utils-1.3.0/tests/test_web_content.py
```

### Comparing `obs-img-utils-1.2.0/CHANGES.md` & `obs_img_utils-1.3.0/CHANGES.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+v1.3.0 (2024-05-08)
+===================
+
+- Do not raise if image metadata not found unless conditions are provided
+- Cleanup tests and rename setup method
+- Update readthedocs config file
+
 v1.2.0 (2023-03-06)
 ===================
 - Adds new required extension (vmdk.xz) for images
 - In case base_name variable is not set, the highest version-release combination of matching images in OBS is chosen.
 
 v1.1.0 (2023-01-26)
 ===================
```

### Comparing `obs-img-utils-1.2.0/CONTRIBUTING.md` & `obs_img_utils-1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `obs-img-utils-1.2.0/LICENSE` & `obs_img_utils-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `obs-img-utils-1.2.0/PKG-INFO` & `obs_img_utils-1.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-img-utils
-Version: 1.2.0
+Version: 1.3.0
 Summary: Package provides utils for images in Open Build Service.
 Home-page: https://github.com/SUSE-Enceladus/obs-img-utils
 Author: SUSE
 Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
 Keywords: obs-img-utils obs_img_utils
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,17 +15,32 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: lxml
+Requires-Dist: pyyaml
+Requires-Dist: xmltodict
 Provides-Extra: dev
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: sphinx-click; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 
 ![Continuous testing & Linting](https://github.com/SUSE-Enceladus/obs-img-utils/workflows/Continuous%20testing%20&%20Linting/badge.svg?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/obs-img-utils/badge/?version=latest)](https://obs-img-utils.readthedocs.io/en/latest/?badge=latest)
 [![Py Versions](https://img.shields.io/pypi/pyversions/obs-img-utils.svg)](https://pypi.org/project/obs-img-utils/)
 [![License](https://img.shields.io/pypi/l/obs-img-utils.svg)](https://pypi.org/project/obs-img-utils/)
 
 # [obs-img-utils](https://github.com/SUSE-Enceladus/obs-img-utils)
```

### Comparing `obs-img-utils-1.2.0/README.md` & `obs_img_utils-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `obs-img-utils-1.2.0/obs_img_utils/__init__.py` & `obs_img_utils-1.3.0/obs_img_utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __author__ = """SUSE"""
 __email__ = 'public-cloud-dev@susecloud.net'
-__version__ = '1.2.0'
+__version__ = '1.3.0'
```

### Comparing `obs-img-utils-1.2.0/obs_img_utils/api.py` & `obs_img_utils-1.3.0/obs_img_utils/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import os
 import re
 import time
 import xmltodict
 
 from collections import namedtuple
 from distutils.dir_util import mkpath
-from pkg_resources import parse_version
+import packaging.version as pv
 from urllib.error import ContentTooShortError, URLError
 
 from obs_img_utils.exceptions import (
     OBSImageDownloadException,
     DownloadMetadataFileExceptionOBS,
     OBSImageConditionsException,
     PackageVersionExceptionOBS,
@@ -403,19 +403,30 @@
             )
         )
 
         self._image_version = version.kiwi_version
         self._image_release = version.obs_build
 
     @retry(DownloadMetadataFileExceptionOBS)
-    def get_image_packages_metadata(self):
+    def get_image_packages_metadata(self) -> dict:
+        has_error = None
+        result_packages = {}
         try:
             result_packages = self.parse_report_file()
         except DownloadMetadataFileExceptionOBS:
-            result_packages = self.parse_packages_file()
+            try:
+                result_packages = self.parse_packages_file()
+            except DownloadMetadataFileExceptionOBS as issue:
+                has_error = issue
+
+        if self.conditions and has_error:
+            self.log_callback.error(
+                f'Cannot verify {self.conditions} without metadata'
+            )
+            raise OBSImageConditionsException(has_error)
 
         return result_packages
 
     def parse_report_file(self):
         result_packages = {}
         self.download_metadata_file('report')
 
@@ -475,23 +486,23 @@
         return result_packages
 
     def _version_compare(self, current, expected, condition):
         if not current:
             current = 'unknown'
 
         if condition == '>=':
-            return parse_version(current) >= parse_version(expected)
+            return pv.Version(current) >= pv.Version(expected)
         elif condition == '<=':
-            return parse_version(current) <= parse_version(expected)
+            return pv.Version(current) <= pv.Version(expected)
         elif condition == '==':
-            return parse_version(current) == parse_version(expected)
+            return pv.Version(current) == pv.Version(expected)
         elif condition == '>':
-            return parse_version(current) > parse_version(expected)
+            return pv.Version(current) > pv.Version(expected)
         elif condition == '<':
-            return parse_version(current) < parse_version(expected)
+            return pv.Version(current) < pv.Version(expected)
         else:
             raise PackageVersionExceptionOBS(
                 'Invalid version compare expression: "{0}"'.format(condition)
             )
 
     def _lookup_package(self, packages, condition):
         package_name = condition['package_name']
```

### Comparing `obs-img-utils-1.2.0/obs_img_utils/cli.py` & `obs_img_utils-1.3.0/obs_img_utils/cli.py`

 * *Files identical despite different names*

### Comparing `obs-img-utils-1.2.0/obs_img_utils/exceptions.py` & `obs_img_utils-1.3.0/obs_img_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `obs-img-utils-1.2.0/obs_img_utils/utils.py` & `obs_img_utils-1.3.0/obs_img_utils/utils.py`

 * *Files identical despite different names*

### Comparing `obs-img-utils-1.2.0/obs_img_utils/web_content.py` & `obs_img_utils-1.3.0/obs_img_utils/web_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from lxml import html
 
 from urllib.request import (
     urlretrieve,
     urlopen,
     Request
 )
-from pkg_resources import parse_version
+import packaging.version as pv
 
 
 class WebContent(object):
     """
     Web Content Scanner and Download interface
     """
     def __init__(self, uri):
@@ -170,11 +170,11 @@
                     new_version = new_version[:-1]
 
                 if highest_version is None:
                     highest_version = new_version
                     chosen_tuple = (filename, extension)
                     continue
 
-                if parse_version(new_version) > parse_version(highest_version):
+                if pv.Version(new_version) > pv.Version(highest_version):
                     highest_version = new_version
                     chosen_tuple = (filename, extension)
         return chosen_tuple
```

### Comparing `obs-img-utils-1.2.0/obs_img_utils.egg-info/PKG-INFO` & `obs_img_utils-1.3.0/obs_img_utils.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obs-img-utils
-Version: 1.2.0
+Version: 1.3.0
 Summary: Package provides utils for images in Open Build Service.
 Home-page: https://github.com/SUSE-Enceladus/obs-img-utils
 Author: SUSE
 Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
 Keywords: obs-img-utils obs_img_utils
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,17 +15,32 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: lxml
+Requires-Dist: pyyaml
+Requires-Dist: xmltodict
 Provides-Extra: dev
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: sphinx-click; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 
 ![Continuous testing & Linting](https://github.com/SUSE-Enceladus/obs-img-utils/workflows/Continuous%20testing%20&%20Linting/badge.svg?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/obs-img-utils/badge/?version=latest)](https://obs-img-utils.readthedocs.io/en/latest/?badge=latest)
 [![Py Versions](https://img.shields.io/pypi/pyversions/obs-img-utils.svg)](https://pypi.org/project/obs-img-utils/)
 [![License](https://img.shields.io/pypi/l/obs-img-utils.svg)](https://pypi.org/project/obs-img-utils/)
 
 # [obs-img-utils](https://github.com/SUSE-Enceladus/obs-img-utils)
```

### Comparing `obs-img-utils-1.2.0/obs_img_utils.egg-info/SOURCES.txt` & `obs_img_utils-1.3.0/obs_img_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obs-img-utils-1.2.0/package/python3-obs-img-utils.spec` & `obs_img_utils-1.3.0/package/python3-obs-img-utils.spec`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Please submit bugfixes or comments via http://bugs.opensuse.org/
 #
 
 
 %bcond_without test
 Name:           python3-obs-img-utils
-Version:        1.2.0
+Version:        1.3.0
 Release:        0
 Summary:        API and CLI utilities for images in OBS
 License:        GPL-3.0-or-later
 Group:          Development/Languages/Python
 Url:            https://github.com/SUSE-Enceladus/obs-img-utils
 Source:         https://files.pythonhosted.org/packages/source/o/obs-img-utils/obs-img-utils-%{version}.tar.gz
 BuildRequires:  python-rpm-macros
```

### Comparing `obs-img-utils-1.2.0/setup.py` & `obs_img_utils-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 with open('requirements-dev.txt') as req_file:
     dev_requirements = test_requirements + req_file.read().splitlines()[2:]
 
 
 setup(
     name='obs-img-utils',
-    version='1.2.0',
+    version='1.3.0',
     description="Package provides utils for images in Open Build Service.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="SUSE",
     author_email='public-cloud-dev@susecloud.net',
     url='https://github.com/SUSE-Enceladus/obs-img-utils',
     packages=find_packages(),
```

### Comparing `obs-img-utils-1.2.0/tests/data/index.html` & `obs_img_utils-1.3.0/tests/data/index.html`

 * *Files identical despite different names*

### Comparing `obs-img-utils-1.2.0/tests/data/index_name_picker.html` & `obs_img_utils-1.3.0/tests/data/index_name_picker.html`

 * *Files identical despite different names*

### Comparing `obs-img-utils-1.2.0/tests/data/index_new.html` & `obs_img_utils-1.3.0/tests/data/index_new.html`

 * *Files identical despite different names*

### Comparing `obs-img-utils-1.2.0/tests/test_obs_img_utils_api.py` & `obs_img_utils-1.3.0/tests/test_obs_img_utils_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 from unittest.mock import patch
 
 from obs_img_utils.api import OBSImageUtil, package_type
 from obs_img_utils.exceptions import PackageVersionExceptionOBS
 
 
-class TestAPI(object):
-    def setup(self):
+class TestAPI:
+    def setup_method(self, cls):
         self.downloader = OBSImageUtil(
             'https://provo-mirror.opensuse.org/repositories/',
             'openSUSE-Leap-15.0-Azure',
             arch='x86_64',
             target_directory='tests/data'
         )
```

### Comparing `obs-img-utils-1.2.0/tests/test_obs_img_utils_cli.py` & `obs_img_utils-1.3.0/tests/test_obs_img_utils_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,15 @@
               '==\n'
               '1.0.0\n'
               '\n'
               'y\n'
               'apparmor-parser\n'
               '\n'
               '2.12.2\n'
-              'lp150.6.14.1\n'
+              '\n'
               'n\n'
               'y\n'
               'GPL\n'
               'n\n'
               'y\n'
               '*-mini\n'
               'n\n'
```

### Comparing `obs-img-utils-1.2.0/tests/test_obs_img_utils_utils.py` & `obs_img_utils-1.3.0/tests/test_obs_img_utils_utils.py`

 * *Files identical despite different names*

### Comparing `obs-img-utils-1.2.0/tests/test_web_content.py` & `obs_img_utils-1.3.0/tests/test_web_content.py`

 * *Files identical despite different names*

