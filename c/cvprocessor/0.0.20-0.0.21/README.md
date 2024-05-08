# Comparing `tmp/cvprocessor-0.0.20.tar.gz` & `tmp/cvprocessor-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.0.20.tar", last modified: Tue May  7 23:22:53 2024, max compression
+gzip compressed data, was "cvprocessor-0.0.21.tar", last modified: Wed May  8 02:09:42 2024, max compression
```

## Comparing `cvprocessor-0.0.20.tar` & `cvprocessor-0.0.21.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:22:53.372902 cvprocessor-0.0.20/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.20/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 23:22:53.372472 cvprocessor-0.0.20/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      990 2024-05-07 21:56:16.000000 cvprocessor-0.0.20/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-07 23:22:20.000000 cvprocessor-0.0.20/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-07 23:22:53.373088 cvprocessor-0.0.20/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:22:53.357017 cvprocessor-0.0.20/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:22:53.367738 cvprocessor-0.0.20/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.20/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     5846 2024-05-07 21:58:53.000000 cvprocessor-0.0.20/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.20/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     2476 2024-05-07 23:19:37.000000 cvprocessor-0.0.20/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     3629 2024-05-07 22:13:41.000000 cvprocessor-0.0.20/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.20/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     2078 2024-05-07 23:22:00.000000 cvprocessor-0.0.20/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.20/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.20/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.20/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.20/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)      918 2024-05-07 23:06:14.000000 cvprocessor-0.0.20/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.20/src/cvprocessor/software.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:22:53.372001 cvprocessor-0.0.20/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 23:22:53.000000 cvprocessor-0.0.20/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      598 2024-05-07 23:22:53.000000 cvprocessor-0.0.20/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-07 23:22:53.000000 cvprocessor-0.0.20/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-07 23:22:53.000000 cvprocessor-0.0.20/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-07 23:22:53.000000 cvprocessor-0.0.20/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:09:42.754163 cvprocessor-0.0.21/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.21/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-08 02:09:42.753442 cvprocessor-0.0.21/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      990 2024-05-07 21:56:16.000000 cvprocessor-0.0.21/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-08 02:09:01.000000 cvprocessor-0.0.21/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-08 02:09:42.754311 cvprocessor-0.0.21/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:09:42.736279 cvprocessor-0.0.21/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:09:42.748596 cvprocessor-0.0.21/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.21/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5846 2024-05-07 21:58:53.000000 cvprocessor-0.0.21/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.21/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2666 2024-05-08 00:27:54.000000 cvprocessor-0.0.21/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3629 2024-05-07 22:13:41.000000 cvprocessor-0.0.21/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.21/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2153 2024-05-07 23:24:10.000000 cvprocessor-0.0.21/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.21/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.21/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.21/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.21/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)      918 2024-05-07 23:06:14.000000 cvprocessor-0.0.21/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.21/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4517 2024-05-08 02:07:59.000000 cvprocessor-0.0.21/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:09:42.752833 cvprocessor-0.0.21/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-08 02:09:42.000000 cvprocessor-0.0.21/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      626 2024-05-08 02:09:42.000000 cvprocessor-0.0.21/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-08 02:09:42.000000 cvprocessor-0.0.21/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-08 02:09:42.000000 cvprocessor-0.0.21/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-08 02:09:42.000000 cvprocessor-0.0.21/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.0.20/LICENSE` & `cvprocessor-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.20/PKG-INFO` & `cvprocessor-0.0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.20
+Version: 0.0.21
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.20/README.md` & `cvprocessor-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.20/pyproject.toml` & `cvprocessor-0.0.21/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.0.20"
+version = "0.0.21"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.0.20/src/cvprocessor/authors.py` & `cvprocessor-0.0.21/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.20/src/cvprocessor/cv.py` & `cvprocessor-0.0.21/src/cvprocessor/cv.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 from cvprocessor.publications import Publications
 from cvprocessor.authors import Authors
 from cvprocessor.software import Software
 from cvprocessor.institutes import Institutes
 from cvprocessor.news import News
 from cvprocessor.research_interests import ResearchInterests
 from cvprocessor.grants_awards import GrantsAwards
+from cvprocessor.teaching import Teaching
 
 
 class CV:
     def __init__(self, filename):
         self._filename = filename
         self._education = Education(self.filename)
         self._institutes = Institutes(self.filename)
         self._software = Software(self.filename)
         self._intro = Intro(self.filename)
         self._authors = Authors(self.filename, self)
         self._news = News(self.filename)
         self._publications = Publications(self.filename, self)
         self._research_interests = ResearchInterests(self.filename)
         self._grants_awards = GrantsAwards(self.filename)
+        self._teaching = Teaching(self.filename)
 
     @property
     def filename(self):
         return self._filename
 
     @property
     def intro(self):
@@ -67,25 +69,30 @@
     def research_interests(self):
         return self._research_interests
 
     @property
     def grants_awards(self):
         return self._grants_awards
 
+    @property
+    def teaching(self):
+        return self._teaching
+
     def print(self):
         print("CV")
         print("Filename:", self.filename)
         self.intro.print()
         self.education.print()
         self.institutes.print()
         self.authors.print()
         self.software.print()
         self.publications.print()
         self.news.print()
         self.research_interests.print()
         self.grants_awards.print()
+        self.teaching.print()
 
 
 if __name__ == "__main__":
     cv = CV("cv.xlsx")
     cv.print()
     sys.exit(0)
```

### Comparing `cvprocessor-0.0.20/src/cvprocessor/education.py` & `cvprocessor-0.0.21/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.20/src/cvprocessor/grants_awards.py` & `cvprocessor-0.0.21/src/cvprocessor/grants_awards.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,17 @@
     def filename(self):
         return self._filename
 
     @property
     def grants_awards(self):
         return self._grants_awards
 
+    def get_oldest_year(self):
+        return self.grants_awards[-1].year
+
     def _load_grants_awards(self):
         self._filename = pd.read_excel(
             self.filename, sheet_name="Grants_awards")
         return [GrantsAwardsData(row) for index, row in self.filename.iterrows()]
 
     def print(self):
         for grant_award in self.grants_awards:
```

### Comparing `cvprocessor-0.0.20/src/cvprocessor/institutes.py` & `cvprocessor-0.0.21/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.20/src/cvprocessor/intro.py` & `cvprocessor-0.0.21/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.20/src/cvprocessor/news.py` & `cvprocessor-0.0.21/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.20/src/cvprocessor/publications.py` & `cvprocessor-0.0.21/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.20/src/cvprocessor/research_interests.py` & `cvprocessor-0.0.21/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.20/src/cvprocessor/software.py` & `cvprocessor-0.0.21/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.20/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.0.21/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.20
+Version: 0.0.21
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.20/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.0.21/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,12 +10,13 @@
 src/cvprocessor/grants_awards.py
 src/cvprocessor/institutes.py
 src/cvprocessor/intro.py
 src/cvprocessor/news.py
 src/cvprocessor/publications.py
 src/cvprocessor/research_interests.py
 src/cvprocessor/software.py
+src/cvprocessor/teaching.py
 src/cvprocessor.egg-info/PKG-INFO
 src/cvprocessor.egg-info/SOURCES.txt
 src/cvprocessor.egg-info/dependency_links.txt
 src/cvprocessor.egg-info/requires.txt
 src/cvprocessor.egg-info/top_level.txt
```

