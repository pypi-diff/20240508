# Comparing `tmp/pychute-0.0.4.tar.gz` & `tmp/pychute-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychute-0.0.4.tar", last modified: Tue May  7 17:44:35 2024, max compression
+gzip compressed data, was "pychute-0.0.5.tar", last modified: Tue May  7 17:49:40 2024, max compression
```

## Comparing `pychute-0.0.4.tar` & `pychute-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 17:44:35.162683 pychute-0.0.4/
--rw-rw-rw-   0        0        0     1090 2024-05-07 10:43:46.000000 pychute-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3914 2024-05-07 17:44:35.160034 pychute-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1968 2024-05-07 17:37:40.000000 pychute-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 17:44:35.141552 pychute-0.0.4/pychute/
--rw-rw-rw-   0        0        0      196 2024-05-07 16:42:55.000000 pychute-0.0.4/pychute/__init__.py
--rw-rw-rw-   0        0        0      110 2024-05-07 16:37:24.000000 pychute-0.0.4/pychute/config.py
--rw-rw-rw-   0        0        0      669 2024-05-07 10:59:12.000000 pychute-0.0.4/pychute/helpers.py
--rw-rw-rw-   0        0        0     3759 2024-05-07 16:42:55.000000 pychute-0.0.4/pychute/main.py
-drwxrwxrwx   0        0        0        0 2024-05-07 17:44:35.157989 pychute-0.0.4/pychute.egg-info/
--rw-rw-rw-   0        0        0     3914 2024-05-07 17:44:35.000000 pychute-0.0.4/pychute.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-05-07 17:44:35.000000 pychute-0.0.4/pychute.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 17:44:35.000000 pychute-0.0.4/pychute.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-07 17:44:35.000000 pychute-0.0.4/pychute.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-07 17:44:35.000000 pychute-0.0.4/pychute.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      786 2024-05-07 17:39:19.000000 pychute-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 17:44:35.163732 pychute-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      643 2024-05-07 17:39:19.000000 pychute-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 17:44:35.155305 pychute-0.0.4/tests/
--rw-rw-rw-   0        0        0      937 2024-05-07 16:42:56.000000 pychute-0.0.4/tests/test_functionality.py
--rw-rw-rw-   0        0        0      915 2024-05-07 16:44:38.000000 pychute-0.0.4/tests/test_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:49:40.530773 pychute-0.0.5/
+-rw-rw-rw-   0        0        0     1090 2024-05-07 10:43:46.000000 pychute-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3914 2024-05-07 17:49:40.528085 pychute-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1968 2024-05-07 17:37:40.000000 pychute-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 17:49:40.505893 pychute-0.0.5/pychute/
+-rw-rw-rw-   0        0        0      196 2024-05-07 16:42:55.000000 pychute-0.0.5/pychute/__init__.py
+-rw-rw-rw-   0        0        0      110 2024-05-07 16:37:24.000000 pychute-0.0.5/pychute/config.py
+-rw-rw-rw-   0        0        0      669 2024-05-07 10:59:12.000000 pychute-0.0.5/pychute/helpers.py
+-rw-rw-rw-   0        0        0     3732 2024-05-07 17:48:46.000000 pychute-0.0.5/pychute/main.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:49:40.525066 pychute-0.0.5/pychute.egg-info/
+-rw-rw-rw-   0        0        0     3914 2024-05-07 17:49:40.000000 pychute-0.0.5/pychute.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-07 17:49:40.000000 pychute-0.0.5/pychute.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 17:49:40.000000 pychute-0.0.5/pychute.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-07 17:49:40.000000 pychute-0.0.5/pychute.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 17:49:40.000000 pychute-0.0.5/pychute.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      786 2024-05-07 17:49:13.000000 pychute-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 17:49:40.530773 pychute-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      643 2024-05-07 17:49:13.000000 pychute-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 17:49:40.522066 pychute-0.0.5/tests/
+-rw-rw-rw-   0        0        0      937 2024-05-07 16:42:56.000000 pychute-0.0.5/tests/test_functionality.py
+-rw-rw-rw-   0        0        0      915 2024-05-07 16:44:38.000000 pychute-0.0.5/tests/test_helpers.py
```

### Comparing `pychute-0.0.4/LICENSE` & `pychute-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pychute-0.0.4/PKG-INFO` & `pychute-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychute
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library that helps downloading videos from bitchute.com
 Home-page: http://github.com/paichiwo/pychute
 Author: Lukasz Zerucha
 Author-email: Lukasz Zerucha <lzerucha@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Lukasz Zerucha
```

### Comparing `pychute-0.0.4/README.md` & `pychute-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pychute-0.0.4/pychute/helpers.py` & `pychute-0.0.5/pychute/helpers.py`

 * *Files identical despite different names*

### Comparing `pychute-0.0.4/pychute/main.py` & `pychute-0.0.5/pychute/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
             return result
         else:
             raise Exception('Video title could not be fetched')
 
     def publish_date(self) -> str:
         result = self.__soup.find('div', class_='video-publish-date').text
         if result:
-            print(result)
             return format_date_string(result)
         else:
             raise Exception('Publish date could not be fetched')
 
     def channel(self) -> str:
         result = [div.find('a').text for div in self.__soup.findAll('div', attrs={'class': 'details'})]
         if result:
```

### Comparing `pychute-0.0.4/pychute.egg-info/PKG-INFO` & `pychute-0.0.5/pychute.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychute
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library that helps downloading videos from bitchute.com
 Home-page: http://github.com/paichiwo/pychute
 Author: Lukasz Zerucha
 Author-email: Lukasz Zerucha <lzerucha@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Lukasz Zerucha
```

### Comparing `pychute-0.0.4/pyproject.toml` & `pychute-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pychute"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Lukasz Zerucha", email="lzerucha@gmail.com" },
 ]
 description = "A library that helps downloading videos from bitchute.com"
 readme = "README.md"
 requires-python = ">=3.8"
 license={file="LICENSE"}
```

### Comparing `pychute-0.0.4/setup.py` & `pychute-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_desc = f.read()
 
 setup(
     name='pychute',
-    version='0.0.4',
+    version='0.0.5',
     packages=setuptools.find_packages(),
     url='http://github.com/paichiwo/pychute',
     author='Lukasz Zerucha',
     author_email='lzerucha@gmail.com',
     description='A library that helps downloading videos from bitchute.com',
     long_description=long_desc,
     long_description_content_type='text/markdown',
```

### Comparing `pychute-0.0.4/tests/test_functionality.py` & `pychute-0.0.5/tests/test_functionality.py`

 * *Files identical despite different names*

### Comparing `pychute-0.0.4/tests/test_helpers.py` & `pychute-0.0.5/tests/test_helpers.py`

 * *Files identical despite different names*

