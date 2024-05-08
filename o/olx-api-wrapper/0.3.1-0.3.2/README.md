# Comparing `tmp/olx-api-wrapper-0.3.1.tar.gz` & `tmp/olx-api-wrapper-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olx-api-wrapper-0.3.1.tar", last modified: Wed May  8 16:24:43 2024, max compression
+gzip compressed data, was "olx-api-wrapper-0.3.2.tar", last modified: Wed May  8 16:39:24 2024, max compression
```

## Comparing `olx-api-wrapper-0.3.1.tar` & `olx-api-wrapper-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:24:43.906155 olx-api-wrapper-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 16:24:31.000000 olx-api-wrapper-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-08 16:24:43.906155 olx-api-wrapper-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-05-08 16:24:31.000000 olx-api-wrapper-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:24:43.906155 olx-api-wrapper-0.3.1/olx/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-08 16:24:31.000000 olx-api-wrapper-0.3.1/olx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:24:43.906155 olx-api-wrapper-0.3.1/olx_api_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-08 16:24:43.000000 olx-api-wrapper-0.3.1/olx_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-08 16:24:43.000000 olx-api-wrapper-0.3.1/olx_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:24:43.000000 olx-api-wrapper-0.3.1/olx_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 16:24:43.000000 olx-api-wrapper-0.3.1/olx_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 16:24:43.000000 olx-api-wrapper-0.3.1/olx_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:24:43.906155 olx-api-wrapper-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-08 16:24:31.000000 olx-api-wrapper-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:24.126045 olx-api-wrapper-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-08 16:39:24.126045 olx-api-wrapper-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:24.122044 olx-api-wrapper-0.3.2/olx/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:24.122044 olx-api-wrapper-0.3.2/olx/partner/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/advert_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/advert_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/adverts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/categories_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/cities_districts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/languages_currencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/olx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/paid_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/threads_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/user_business.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/partner/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:24.126045 olx-api-wrapper-0.3.2/olx/public/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/public/checkout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:24.126045 olx-api-wrapper-0.3.2/olx/public/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/public/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:24.126045 olx-api-wrapper-0.3.2/olx/public/models/offers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/public/models/offers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/public/models/offers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/public/models/offers/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/public/models/offers/offers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:24.126045 olx-api-wrapper-0.3.2/olx/public/models/seo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/public/models/seo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/public/models/seo/offers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/public/models/seo/popular_searches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/public/offers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/public/olx_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/olx/public/seo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:24.126045 olx-api-wrapper-0.3.2/olx_api_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-08 16:39:24.000000 olx-api-wrapper-0.3.2/olx_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-08 16:39:24.000000 olx-api-wrapper-0.3.2/olx_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:39:24.000000 olx-api-wrapper-0.3.2/olx_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 16:39:24.000000 olx-api-wrapper-0.3.2/olx_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 16:39:24.000000 olx-api-wrapper-0.3.2/olx_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:39:24.126045 olx-api-wrapper-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:24.126045 olx-api-wrapper-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/tests/test_cities_and_districts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-08 16:39:15.000000 olx-api-wrapper-0.3.2/tests/test_users.py
```

### Comparing `olx-api-wrapper-0.3.1/LICENSE` & `olx-api-wrapper-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.1/PKG-INFO` & `olx-api-wrapper-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olx-api-wrapper
-Version: 0.3.1
+Version: 0.3.2
 Summary: Unofficial Wrapper for OLX API
 Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: Paweł Stawikowski
 Author-email: pawikoski@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.1 Summary: Unofficial
+Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.2 Summary: Unofficial
 Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
```

### Comparing `olx-api-wrapper-0.3.1/README.md` & `olx-api-wrapper-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.1/olx_api_wrapper.egg-info/PKG-INFO` & `olx-api-wrapper-0.3.2/olx_api_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olx-api-wrapper
-Version: 0.3.1
+Version: 0.3.2
 Summary: Unofficial Wrapper for OLX API
 Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: Paweł Stawikowski
 Author-email: pawikoski@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.1 Summary: Unofficial
+Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.2 Summary: Unofficial
 Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
```

### Comparing `olx-api-wrapper-0.3.1/setup.py` & `olx-api-wrapper-0.3.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="olx-api-wrapper",
-    version="0.3.1",
+    version="0.3.2",
     description="Unofficial Wrapper for OLX API",
     author="Paweł Stawikowski",
     author_email="pawikoski@gmail.com",
-    packages=["olx"],
+    packages=find_packages(),
     url="https://github.com/Pawikoski/olx-api-wrapper",
     install_requires=["requests", "dacite"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
         "Development Status :: 4 - Beta",
```

