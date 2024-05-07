# Comparing `tmp/cvprocessor-0.0.15.tar.gz` & `tmp/cvprocessor-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.0.15.tar", last modified: Tue May  7 21:25:44 2024, max compression
+gzip compressed data, was "cvprocessor-0.0.16.tar", last modified: Tue May  7 21:57:10 2024, max compression
```

## Comparing `cvprocessor-0.0.15.tar` & `cvprocessor-0.0.16.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 21:25:44.061297 cvprocessor-0.0.15/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.15/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1635 2024-05-07 21:25:44.060578 cvprocessor-0.0.15/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      987 2024-05-07 21:25:18.000000 cvprocessor-0.0.15/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-07 21:22:03.000000 cvprocessor-0.0.15/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-07 21:25:44.061473 cvprocessor-0.0.15/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 21:25:44.048781 cvprocessor-0.0.15/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 21:25:44.056627 cvprocessor-0.0.15/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.15/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     5851 2024-05-04 22:18:45.000000 cvprocessor-0.0.15/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.15/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     2439 2024-05-07 21:20:32.000000 cvprocessor-0.0.15/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     3514 2024-05-04 09:03:16.000000 cvprocessor-0.0.15/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.15/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.15/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.15/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.15/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.15/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     1050 2024-05-05 10:18:42.000000 cvprocessor-0.0.15/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.15/src/cvprocessor/software.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 21:25:44.059958 cvprocessor-0.0.15/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1635 2024-05-07 21:25:44.000000 cvprocessor-0.0.15/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      565 2024-05-07 21:25:44.000000 cvprocessor-0.0.15/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-07 21:25:44.000000 cvprocessor-0.0.15/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-07 21:25:44.000000 cvprocessor-0.0.15/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-07 21:25:44.000000 cvprocessor-0.0.15/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 21:57:10.582995 cvprocessor-0.0.16/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.16/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 21:57:10.582521 cvprocessor-0.0.16/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      990 2024-05-07 21:56:16.000000 cvprocessor-0.0.16/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-07 21:56:19.000000 cvprocessor-0.0.16/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-07 21:57:10.583138 cvprocessor-0.0.16/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 21:57:10.568756 cvprocessor-0.0.16/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 21:57:10.579139 cvprocessor-0.0.16/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.16/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5851 2024-05-04 22:18:45.000000 cvprocessor-0.0.16/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.16/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2439 2024-05-07 21:20:32.000000 cvprocessor-0.0.16/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3514 2024-05-04 09:03:16.000000 cvprocessor-0.0.16/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.16/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.16/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.16/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.16/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.16/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1050 2024-05-05 10:18:42.000000 cvprocessor-0.0.16/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.16/src/cvprocessor/software.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 21:57:10.582065 cvprocessor-0.0.16/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 21:57:10.000000 cvprocessor-0.0.16/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      565 2024-05-07 21:57:10.000000 cvprocessor-0.0.16/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-07 21:57:10.000000 cvprocessor-0.0.16/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-07 21:57:10.000000 cvprocessor-0.0.16/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-07 21:57:10.000000 cvprocessor-0.0.16/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.0.15/LICENSE` & `cvprocessor-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.15/PKG-INFO` & `cvprocessor-0.0.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.15
+Version: 0.0.16
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -37,15 +37,15 @@
 ```
 
 ## Usage
 
 Here's a simple example of how to use CVProcessor to extract personal details from a CV:
 
 ```python
-from cvprocessor import CV
+from cvprocessor.cv import CV
 
 # Load a CV file
 cv_file = "cv.xlsx"
 cv = CV(cv_file)
 
 # print CV details
 cv.print()
```

### Comparing `cvprocessor-0.0.15/README.md` & `cvprocessor-0.0.16/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ```
 
 ## Usage
 
 Here's a simple example of how to use CVProcessor to extract personal details from a CV:
 
 ```python
-from cvprocessor import CV
+from cvprocessor.cv import CV
 
 # Load a CV file
 cv_file = "cv.xlsx"
 cv = CV(cv_file)
 
 # print CV details
 cv.print()
```

### Comparing `cvprocessor-0.0.15/pyproject.toml` & `cvprocessor-0.0.16/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.0.15"
+version = "0.0.16"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.0.15/src/cvprocessor/authors.py` & `cvprocessor-0.0.16/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.15/src/cvprocessor/cv.py` & `cvprocessor-0.0.16/src/cvprocessor/cv.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.15/src/cvprocessor/education.py` & `cvprocessor-0.0.16/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.15/src/cvprocessor/institutes.py` & `cvprocessor-0.0.16/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.15/src/cvprocessor/intro.py` & `cvprocessor-0.0.16/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.15/src/cvprocessor/news.py` & `cvprocessor-0.0.16/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.15/src/cvprocessor/publications.py` & `cvprocessor-0.0.16/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.15/src/cvprocessor/research_interests.py` & `cvprocessor-0.0.16/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.15/src/cvprocessor/software.py` & `cvprocessor-0.0.16/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.15/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.0.16/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.15
+Version: 0.0.16
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -37,15 +37,15 @@
 ```
 
 ## Usage
 
 Here's a simple example of how to use CVProcessor to extract personal details from a CV:
 
 ```python
-from cvprocessor import CV
+from cvprocessor.cv import CV
 
 # Load a CV file
 cv_file = "cv.xlsx"
 cv = CV(cv_file)
 
 # print CV details
 cv.print()
```

### Comparing `cvprocessor-0.0.15/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.0.16/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

