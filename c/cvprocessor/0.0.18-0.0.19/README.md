# Comparing `tmp/cvprocessor-0.0.18.tar.gz` & `tmp/cvprocessor-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.0.18.tar", last modified: Tue May  7 23:01:51 2024, max compression
+gzip compressed data, was "cvprocessor-0.0.19.tar", last modified: Tue May  7 23:06:53 2024, max compression
```

## Comparing `cvprocessor-0.0.18.tar` & `cvprocessor-0.0.19.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:01:51.077465 cvprocessor-0.0.18/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.18/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 23:01:51.076734 cvprocessor-0.0.18/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      990 2024-05-07 21:56:16.000000 cvprocessor-0.0.18/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-07 23:01:04.000000 cvprocessor-0.0.18/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-07 23:01:51.077588 cvprocessor-0.0.18/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:01:51.065033 cvprocessor-0.0.18/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:01:51.072779 cvprocessor-0.0.18/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.18/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     5846 2024-05-07 21:58:53.000000 cvprocessor-0.0.18/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.18/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     2439 2024-05-07 22:14:10.000000 cvprocessor-0.0.18/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     3629 2024-05-07 22:13:41.000000 cvprocessor-0.0.18/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.18/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.18/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.18/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.18/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.18/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)      947 2024-05-07 23:00:55.000000 cvprocessor-0.0.18/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.18/src/cvprocessor/software.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:01:51.076150 cvprocessor-0.0.18/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 23:01:51.000000 cvprocessor-0.0.18/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      565 2024-05-07 23:01:51.000000 cvprocessor-0.0.18/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-07 23:01:51.000000 cvprocessor-0.0.18/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-07 23:01:51.000000 cvprocessor-0.0.18/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-07 23:01:51.000000 cvprocessor-0.0.18/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:06:53.778015 cvprocessor-0.0.19/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.19/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 23:06:53.777595 cvprocessor-0.0.19/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      990 2024-05-07 21:56:16.000000 cvprocessor-0.0.19/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-07 23:06:39.000000 cvprocessor-0.0.19/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-07 23:06:53.778093 cvprocessor-0.0.19/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:06:53.767356 cvprocessor-0.0.19/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:06:53.775039 cvprocessor-0.0.19/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.19/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5846 2024-05-07 21:58:53.000000 cvprocessor-0.0.19/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.19/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2439 2024-05-07 22:14:10.000000 cvprocessor-0.0.19/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3629 2024-05-07 22:13:41.000000 cvprocessor-0.0.19/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.19/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.19/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.19/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.19/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.19/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)      918 2024-05-07 23:06:14.000000 cvprocessor-0.0.19/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.19/src/cvprocessor/software.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:06:53.777143 cvprocessor-0.0.19/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 23:06:53.000000 cvprocessor-0.0.19/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      565 2024-05-07 23:06:53.000000 cvprocessor-0.0.19/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-07 23:06:53.000000 cvprocessor-0.0.19/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-07 23:06:53.000000 cvprocessor-0.0.19/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-07 23:06:53.000000 cvprocessor-0.0.19/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.0.18/LICENSE` & `cvprocessor-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.18/PKG-INFO` & `cvprocessor-0.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.18
+Version: 0.0.19
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.18/README.md` & `cvprocessor-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.18/pyproject.toml` & `cvprocessor-0.0.19/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.0.18"
+version = "0.0.19"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.0.18/src/cvprocessor/authors.py` & `cvprocessor-0.0.19/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.18/src/cvprocessor/cv.py` & `cvprocessor-0.0.19/src/cvprocessor/cv.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.18/src/cvprocessor/education.py` & `cvprocessor-0.0.19/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.18/src/cvprocessor/institutes.py` & `cvprocessor-0.0.19/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.18/src/cvprocessor/intro.py` & `cvprocessor-0.0.19/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.18/src/cvprocessor/news.py` & `cvprocessor-0.0.19/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.18/src/cvprocessor/publications.py` & `cvprocessor-0.0.19/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.18/src/cvprocessor/research_interests.py` & `cvprocessor-0.0.19/src/cvprocessor/research_interests.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 import pandas as pd
 
 
 class ResearchInterests:
     def __init__(self, filename):
         self._filename = filename
-        self._interest = None
+        self._research_interests = None
         self._keywords = []
         self._load_interests()
 
     @property
     def filename(self):
         return self._filename
 
     @property
-    def interest(self):
-        return self._interest
-
-    @property
     def keywords(self):
         return self._keywords
 
     @property
     def research_interests(self):
         return self._research_interests
 
     def _load_interests(self):
         self._filename = pd.read_excel(
             self.filename, sheet_name="Research_Interests")
-        self._interest = self.filename["Interests"].values[0]
+        self._research_interests = self.filename["Interests"].values[0]
         keywords = self.filename["Keywords"]
         for keyword in keywords:
             self._keywords.append(keyword)
 
     def print(self):
-        print(f"Interest: {self._interest}")
+        print(f"Research Interests: {self._research_interests}")
         print(f"Keywords: {self._keywords}")
         print("\n")
```

### Comparing `cvprocessor-0.0.18/src/cvprocessor/software.py` & `cvprocessor-0.0.19/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.18/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.0.19/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.18
+Version: 0.0.19
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.18/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.0.19/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

