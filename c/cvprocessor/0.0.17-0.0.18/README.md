# Comparing `tmp/cvprocessor-0.0.17.tar.gz` & `tmp/cvprocessor-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.0.17.tar", last modified: Tue May  7 22:01:14 2024, max compression
+gzip compressed data, was "cvprocessor-0.0.18.tar", last modified: Tue May  7 23:01:51 2024, max compression
```

## Comparing `cvprocessor-0.0.17.tar` & `cvprocessor-0.0.18.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 22:01:14.914565 cvprocessor-0.0.17/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.17/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 22:01:14.913890 cvprocessor-0.0.17/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      990 2024-05-07 21:56:16.000000 cvprocessor-0.0.17/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-07 22:00:35.000000 cvprocessor-0.0.17/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-07 22:01:14.914711 cvprocessor-0.0.17/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 22:01:14.904312 cvprocessor-0.0.17/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 22:01:14.910354 cvprocessor-0.0.17/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.17/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     5846 2024-05-07 21:58:53.000000 cvprocessor-0.0.17/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.17/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     2439 2024-05-07 21:20:32.000000 cvprocessor-0.0.17/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     3514 2024-05-04 09:03:16.000000 cvprocessor-0.0.17/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.17/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.17/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.17/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.17/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.17/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)     1050 2024-05-05 10:18:42.000000 cvprocessor-0.0.17/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.17/src/cvprocessor/software.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 22:01:14.913250 cvprocessor-0.0.17/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 22:01:14.000000 cvprocessor-0.0.17/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      565 2024-05-07 22:01:14.000000 cvprocessor-0.0.17/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-07 22:01:14.000000 cvprocessor-0.0.17/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-07 22:01:14.000000 cvprocessor-0.0.17/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-07 22:01:14.000000 cvprocessor-0.0.17/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:01:51.077465 cvprocessor-0.0.18/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.18/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 23:01:51.076734 cvprocessor-0.0.18/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      990 2024-05-07 21:56:16.000000 cvprocessor-0.0.18/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-07 23:01:04.000000 cvprocessor-0.0.18/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-07 23:01:51.077588 cvprocessor-0.0.18/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:01:51.065033 cvprocessor-0.0.18/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:01:51.072779 cvprocessor-0.0.18/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.18/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5846 2024-05-07 21:58:53.000000 cvprocessor-0.0.18/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.18/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2439 2024-05-07 22:14:10.000000 cvprocessor-0.0.18/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3629 2024-05-07 22:13:41.000000 cvprocessor-0.0.18/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.18/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.18/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.18/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.18/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.18/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)      947 2024-05-07 23:00:55.000000 cvprocessor-0.0.18/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.18/src/cvprocessor/software.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:01:51.076150 cvprocessor-0.0.18/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 23:01:51.000000 cvprocessor-0.0.18/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      565 2024-05-07 23:01:51.000000 cvprocessor-0.0.18/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-07 23:01:51.000000 cvprocessor-0.0.18/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-07 23:01:51.000000 cvprocessor-0.0.18/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-07 23:01:51.000000 cvprocessor-0.0.18/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.0.17/LICENSE` & `cvprocessor-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.17/PKG-INFO` & `cvprocessor-0.0.18/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.17
+Version: 0.0.18
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.17/README.md` & `cvprocessor-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.17/pyproject.toml` & `cvprocessor-0.0.18/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.0.17"
+version = "0.0.18"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.0.17/src/cvprocessor/authors.py` & `cvprocessor-0.0.18/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.17/src/cvprocessor/cv.py` & `cvprocessor-0.0.18/src/cvprocessor/cv.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.17/src/cvprocessor/education.py` & `cvprocessor-0.0.18/src/cvprocessor/education.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,14 +111,18 @@
     def filename(self):
         return self._filename
 
     @property
     def educations(self):
         return self._educations
 
+    # Get the oldest end year
+    def get_oldest_end_year(self):
+        return self.educations[-1].end_year.year
+
     def _load_educations(self):
         education_df = pd.read_excel(self.filename, sheet_name="Education")
         return [EducationData(row) for _, row in education_df.iterrows()]
 
     def print(self):
         for education in self.educations:
             education.print()
```

### Comparing `cvprocessor-0.0.17/src/cvprocessor/institutes.py` & `cvprocessor-0.0.18/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.17/src/cvprocessor/intro.py` & `cvprocessor-0.0.18/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.17/src/cvprocessor/news.py` & `cvprocessor-0.0.18/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.17/src/cvprocessor/publications.py` & `cvprocessor-0.0.18/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.17/src/cvprocessor/research_interests.py` & `cvprocessor-0.0.18/src/cvprocessor/research_interests.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 
 class ResearchInterests:
     def __init__(self, filename):
         self._filename = filename
         self._interest = None
         self._keywords = []
-        self._research_interests = self._get_research_interests()
         self._load_interests()
 
     @property
     def filename(self):
         return self._filename
 
     @property
@@ -21,20 +20,19 @@
     def keywords(self):
         return self._keywords
 
     @property
     def research_interests(self):
         return self._research_interests
 
-    def _get_research_interests(self):
-        return pd.read_excel(self.filename, sheet_name="Research_Interests")
-
     def _load_interests(self):
-        self._interest = self.research_interests["Interests"].values[0]
-        keywords = self.research_interests["Keywords"]
+        self._filename = pd.read_excel(
+            self.filename, sheet_name="Research_Interests")
+        self._interest = self.filename["Interests"].values[0]
+        keywords = self.filename["Keywords"]
         for keyword in keywords:
             self._keywords.append(keyword)
 
     def print(self):
         print(f"Interest: {self._interest}")
         print(f"Keywords: {self._keywords}")
         print("\n")
```

### Comparing `cvprocessor-0.0.17/src/cvprocessor/software.py` & `cvprocessor-0.0.18/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.17/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.0.18/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.17
+Version: 0.0.18
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.17/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.0.18/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

