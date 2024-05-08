# Comparing `tmp/cvprocessor-0.0.22.tar.gz` & `tmp/cvprocessor-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.0.22.tar", last modified: Wed May  8 02:21:25 2024, max compression
+gzip compressed data, was "cvprocessor-0.0.23.tar", last modified: Wed May  8 02:51:04 2024, max compression
```

## Comparing `cvprocessor-0.0.22.tar` & `cvprocessor-0.0.23.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:21:25.837308 cvprocessor-0.0.22/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.22/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-08 02:21:25.836273 cvprocessor-0.0.22/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      990 2024-05-07 21:56:16.000000 cvprocessor-0.0.22/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-08 02:13:50.000000 cvprocessor-0.0.22/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-08 02:21:25.837486 cvprocessor-0.0.22/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:21:25.816517 cvprocessor-0.0.22/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:21:25.831267 cvprocessor-0.0.22/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.22/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     5846 2024-05-07 21:58:53.000000 cvprocessor-0.0.22/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.22/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     2666 2024-05-08 00:27:54.000000 cvprocessor-0.0.22/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     3629 2024-05-07 22:13:41.000000 cvprocessor-0.0.22/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.22/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     2153 2024-05-07 23:24:10.000000 cvprocessor-0.0.22/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.22/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.22/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.22/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.22/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)      918 2024-05-07 23:06:14.000000 cvprocessor-0.0.22/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.22/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     4974 2024-05-08 02:16:16.000000 cvprocessor-0.0.22/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:21:25.835280 cvprocessor-0.0.22/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-08 02:21:25.000000 cvprocessor-0.0.22/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      626 2024-05-08 02:21:25.000000 cvprocessor-0.0.22/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-08 02:21:25.000000 cvprocessor-0.0.22/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-08 02:21:25.000000 cvprocessor-0.0.22/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-08 02:21:25.000000 cvprocessor-0.0.22/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:51:04.244921 cvprocessor-0.0.23/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.23/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-08 02:51:04.244110 cvprocessor-0.0.23/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      990 2024-05-07 21:56:16.000000 cvprocessor-0.0.23/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-08 02:48:16.000000 cvprocessor-0.0.23/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-08 02:51:04.245373 cvprocessor-0.0.23/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:51:04.225979 cvprocessor-0.0.23/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:51:04.239926 cvprocessor-0.0.23/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.23/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5846 2024-05-07 21:58:53.000000 cvprocessor-0.0.23/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.23/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2666 2024-05-08 00:27:54.000000 cvprocessor-0.0.23/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3629 2024-05-07 22:13:41.000000 cvprocessor-0.0.23/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.23/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2153 2024-05-07 23:24:10.000000 cvprocessor-0.0.23/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.23/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.23/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.23/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.23/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)      918 2024-05-07 23:06:14.000000 cvprocessor-0.0.23/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.23/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5178 2024-05-08 02:47:48.000000 cvprocessor-0.0.23/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:51:04.243424 cvprocessor-0.0.23/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-08 02:51:04.000000 cvprocessor-0.0.23/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      626 2024-05-08 02:51:04.000000 cvprocessor-0.0.23/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-08 02:51:04.000000 cvprocessor-0.0.23/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-08 02:51:04.000000 cvprocessor-0.0.23/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-08 02:51:04.000000 cvprocessor-0.0.23/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.0.22/LICENSE` & `cvprocessor-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.22/PKG-INFO` & `cvprocessor-0.0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.22
+Version: 0.0.23
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.22/README.md` & `cvprocessor-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.22/pyproject.toml` & `cvprocessor-0.0.23/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.0.22"
+version = "0.0.23"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.0.22/src/cvprocessor/authors.py` & `cvprocessor-0.0.23/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.22/src/cvprocessor/cv.py` & `cvprocessor-0.0.23/src/cvprocessor/cv.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.22/src/cvprocessor/education.py` & `cvprocessor-0.0.23/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.22/src/cvprocessor/grants_awards.py` & `cvprocessor-0.0.23/src/cvprocessor/grants_awards.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.22/src/cvprocessor/institutes.py` & `cvprocessor-0.0.23/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.22/src/cvprocessor/intro.py` & `cvprocessor-0.0.23/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.22/src/cvprocessor/news.py` & `cvprocessor-0.0.23/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.22/src/cvprocessor/publications.py` & `cvprocessor-0.0.23/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.22/src/cvprocessor/research_interests.py` & `cvprocessor-0.0.23/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.22/src/cvprocessor/software.py` & `cvprocessor-0.0.23/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.22/src/cvprocessor/teaching.py` & `cvprocessor-0.0.23/src/cvprocessor/teaching.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,48 +67,57 @@
         return self._supervisor
 
     @property
     def responsibilities(self):
         return self._responsibilities
 
     def get_start_year(self):
-        year = 0
+        year = 1e6
+        date = None
         for start, _ in self.year:
+            if not start:
+                continue
             if int(start.year) < year:
                 year = int(start.year)
-        return year
+                date = start
+        return date
 
     def get_end_year(self):
         year = 0
+        date = None
         for _, end in self.year:
+            if not end:
+                continue
             if int(end.year) > year:
                 year = int(end.year)
-        return year
+                date = end
+        return date
 
     def format_year(self, year):
         year = year.strip()
         year = pd.to_datetime(year, format="%b %Y")
         return year
 
     def process_year_data(self):
+        self.print()
         self._year = self.filename["Year"]
         self._year = self._year.split(";")
         self._year = list(filter(None, self._year))
         year_list = []
         for year in self._year:
             year_split = year.split("-")
-            if len(year_split) > 2:
+            if len(year_split) > 1:
                 start_year = year_split[0]
                 end_year = year_split[1]
             else:
                 start_year = year_split[0]
-                end_year = year_split[-1]
-            start_year = "Jul 2020"
+                end_year = None
             start_year = self.format_year(start_year)
-            end_year = self.format_year(end_year)
+            if end_year:
+                end_year = self.format_year(end_year)
             year_list.append((start_year, end_year))
         self._year = year_list
 
     def _load_teaching(self):
         self.process_year_data()
         self._start_year = self.get_start_year()
         self._end_year = self.get_end_year()
@@ -140,15 +149,15 @@
 
 class Teaching:
     def __init__(self, filename):
         self._filename = filename
         self._teaching = self._load_teaching()
         # Sort the teaching data by type then by year
         self._teaching = sorted(
-            self.teaching, key=lambda x: (x.type, x.end_year), reverse=True)
+            self.teaching, key=lambda x: (x.type, x.start_year), reverse=True)
 
     @property
     def filename(self):
         return self._filename
 
     @property
     def teaching(self):
```

### Comparing `cvprocessor-0.0.22/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.0.23/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.22
+Version: 0.0.23
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.22/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.0.23/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

