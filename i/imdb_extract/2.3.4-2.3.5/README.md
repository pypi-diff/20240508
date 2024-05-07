# Comparing `tmp/imdb_extract-2.3.4.tar.gz` & `tmp/imdb_extract-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imdb_extract-2.3.4.tar", max compression
+gzip compressed data, was "imdb_extract-2.3.5.tar", max compression
```

## Comparing `imdb_extract-2.3.4.tar` & `imdb_extract-2.3.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1500 2022-07-10 12:24:59.642328 imdb_extract-2.3.4/LICENSE
--rw-r--r--   0        0        0      488 2022-08-15 15:28:59.772433 imdb_extract-2.3.4/README.rst
--rw-r--r--   0        0        0      581 2023-06-10 19:24:04.137055 imdb_extract-2.3.4/berhoel/__init__.py
--rw-r--r--   0        0        0     8763 2024-01-25 17:10:11.540243 imdb_extract-2.3.4/berhoel/imdb_extract/__init__.py
--rw-r--r--   0        0        0     1079 2022-08-15 14:56:19.709348 imdb_extract-2.3.4/berhoel/imdb_extract/tests/conftest.py
--rw-r--r--   0        0        0      715 2022-08-15 14:57:52.361288 imdb_extract-2.3.4/berhoel/imdb_extract/tests/test_base.py
--rw-r--r--   0        0        0      981 2022-08-15 15:06:24.665011 imdb_extract-2.3.4/berhoel/imdb_extract/tests/test_unicodewriter.py
--rw-r--r--   0        0        0      556 2022-08-15 15:04:54.689051 imdb_extract-2.3.4/berhoel/imdb_extract/unicodewriter.py
--rw-r--r--   0        0        0     2771 2024-01-25 17:07:12.790368 imdb_extract-2.3.4/pyproject.toml
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 imdb_extract-2.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1500 2022-07-10 12:24:59.642328 imdb_extract-2.3.5/LICENSE
+-rw-r--r--   0        0        0      488 2022-08-15 15:28:59.772433 imdb_extract-2.3.5/README.rst
+-rw-r--r--   0        0        0      581 2023-06-10 19:24:04.137055 imdb_extract-2.3.5/berhoel/__init__.py
+-rw-r--r--   0        0        0     8801 2024-05-07 23:03:55.466068 imdb_extract-2.3.5/berhoel/imdb_extract/__init__.py
+-rw-r--r--   0        0        0     1079 2022-08-15 14:56:19.709348 imdb_extract-2.3.5/berhoel/imdb_extract/tests/conftest.py
+-rw-r--r--   0        0        0      715 2022-08-15 14:57:52.361288 imdb_extract-2.3.5/berhoel/imdb_extract/tests/test_base.py
+-rw-r--r--   0        0        0      981 2022-08-15 15:06:24.665011 imdb_extract-2.3.5/berhoel/imdb_extract/tests/test_unicodewriter.py
+-rw-r--r--   0        0        0      556 2022-08-15 15:04:54.689051 imdb_extract-2.3.5/berhoel/imdb_extract/unicodewriter.py
+-rw-r--r--   0        0        0     2771 2024-05-07 21:49:34.219613 imdb_extract-2.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 imdb_extract-2.3.5/PKG-INFO
```

### Comparing `imdb_extract-2.3.4/LICENSE` & `imdb_extract-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `imdb_extract-2.3.4/berhoel/__init__.py` & `imdb_extract-2.3.5/berhoel/__init__.py`

 * *Files identical despite different names*

### Comparing `imdb_extract-2.3.4/berhoel/imdb_extract/__init__.py` & `imdb_extract-2.3.5/berhoel/imdb_extract/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.firefox.options import Options
 from selenium.webdriver.firefox.firefox_profile import FirefoxProfile
 
 # Local library imports.
 from .unicodewriter import UnicodeWriter
 
-__date__ = "2024/01/25 18:10:11 hoel"
+__date__ = "2024/05/08 01:03:55 hoel"
 __author__ = "Berthold Höllmann"
 __copyright__ = "Copyright © 2011,2013,2023 by Berthold Höllmann"
 __credits__ = ["Berthold Höllmann"]
 __maintainer__ = "Berthold Höllmann"
 __email__ = "berhoel@gmail.com"
 __version__ = __import__("importlib.metadata", fromlist=["version"]).version(
     "imdb_extract"
@@ -178,33 +178,32 @@
                     EC.element_to_be_clickable(
                         (
                             By.XPATH,
                             '//article[contains(@class,"episode-item-wrapper")]',
                         )
                     )
                 )
-                descriptions = [
-                    i.text
-                    for i in elem.find_elements(
-                        By.XPATH, '//div[@class="ipc-html-content-inner-div"]'
-                    )
-                ]
-                links = [
-                    i
-                    for i in elem.find_elements(
-                        By.XPATH,
-                        "/html/body/div[2]/main/div/section/div/section/div/div[1]/"
-                        "section[2]/section[2]/article//a",
-                    )
-                    if i.text
-                ]
+                articles = elem.find_elements(
+                    By.XPATH,
+                    '//article[contains(@class,"episode-item-wrapper")]',
+                )
 
                 episodes = []
 
-                for description, link in zip(descriptions, links):
+                for article in articles:
+                    description = article.find_elements(
+                        By.XPATH, './/div[@class="ipc-html-content-inner-div"]'
+                    )
+                    if not description:
+                        description = ""
+                    else:
+                        description = description[0].text
+                    link = article.find_element(
+                        By.XPATH, './/a[@class="ipc-title-link-wrapper"]'
+                    )
                     episodes.append(
                         IMDBEntry(
                             season, link.text, link.get_attribute("href"), description
                         )
                     )
 
                 episodes.sort()
```

### Comparing `imdb_extract-2.3.4/berhoel/imdb_extract/tests/conftest.py` & `imdb_extract-2.3.5/berhoel/imdb_extract/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `imdb_extract-2.3.4/berhoel/imdb_extract/tests/test_base.py` & `imdb_extract-2.3.5/berhoel/imdb_extract/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `imdb_extract-2.3.4/berhoel/imdb_extract/tests/test_unicodewriter.py` & `imdb_extract-2.3.5/berhoel/imdb_extract/tests/test_unicodewriter.py`

 * *Files identical despite different names*

### Comparing `imdb_extract-2.3.4/berhoel/imdb_extract/unicodewriter.py` & `imdb_extract-2.3.5/berhoel/imdb_extract/unicodewriter.py`

 * *Files identical despite different names*

### Comparing `imdb_extract-2.3.4/pyproject.toml` & `imdb_extract-2.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imdb_extract"
-version = "2.3.4"
+version = "2.3.5"
 description = "Download IMDB series information."
 authors = ["Berthold Höllmann <berthold@xn--hllmanns-n4a.de>"]
 readme = 'README.rst'
 license = "BSD"
 repository = "https://gitlab.com/berhoel/python/IMDBExtract"
 homepage = "https://python.xn--hllmanns-n4a.de/IMDBExtract/"
 documentation = "https://python.xn--hllmanns-n4a.de/IMDBExtract/"
```

### Comparing `imdb_extract-2.3.4/PKG-INFO` & `imdb_extract-2.3.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imdb_extract
-Version: 2.3.4
+Version: 2.3.5
 Summary: Download IMDB series information.
 Home-page: https://python.xn--hllmanns-n4a.de/IMDBExtract/
 License: BSD
 Author: Berthold Höllmann
 Author-email: berthold@xn--hllmanns-n4a.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

