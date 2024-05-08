# Comparing `tmp/cvprocessor-0.0.19.tar.gz` & `tmp/cvprocessor-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.0.19.tar", last modified: Tue May  7 23:06:53 2024, max compression
+gzip compressed data, was "cvprocessor-0.0.20.tar", last modified: Tue May  7 23:22:53 2024, max compression
```

## Comparing `cvprocessor-0.0.19.tar` & `cvprocessor-0.0.20.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:06:53.778015 cvprocessor-0.0.19/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.19/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 23:06:53.777595 cvprocessor-0.0.19/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      990 2024-05-07 21:56:16.000000 cvprocessor-0.0.19/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-07 23:06:39.000000 cvprocessor-0.0.19/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-07 23:06:53.778093 cvprocessor-0.0.19/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:06:53.767356 cvprocessor-0.0.19/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:06:53.775039 cvprocessor-0.0.19/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.19/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     5846 2024-05-07 21:58:53.000000 cvprocessor-0.0.19/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.19/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     2439 2024-05-07 22:14:10.000000 cvprocessor-0.0.19/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     3629 2024-05-07 22:13:41.000000 cvprocessor-0.0.19/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.19/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.19/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.19/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.19/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.19/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)      918 2024-05-07 23:06:14.000000 cvprocessor-0.0.19/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.19/src/cvprocessor/software.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:06:53.777143 cvprocessor-0.0.19/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 23:06:53.000000 cvprocessor-0.0.19/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      565 2024-05-07 23:06:53.000000 cvprocessor-0.0.19/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-07 23:06:53.000000 cvprocessor-0.0.19/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-07 23:06:53.000000 cvprocessor-0.0.19/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-07 23:06:53.000000 cvprocessor-0.0.19/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:22:53.372902 cvprocessor-0.0.20/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.20/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 23:22:53.372472 cvprocessor-0.0.20/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      990 2024-05-07 21:56:16.000000 cvprocessor-0.0.20/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-07 23:22:20.000000 cvprocessor-0.0.20/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-07 23:22:53.373088 cvprocessor-0.0.20/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:22:53.357017 cvprocessor-0.0.20/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:22:53.367738 cvprocessor-0.0.20/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.20/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5846 2024-05-07 21:58:53.000000 cvprocessor-0.0.20/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.20/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2476 2024-05-07 23:19:37.000000 cvprocessor-0.0.20/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3629 2024-05-07 22:13:41.000000 cvprocessor-0.0.20/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.20/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2078 2024-05-07 23:22:00.000000 cvprocessor-0.0.20/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.20/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.20/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.20/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.20/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)      918 2024-05-07 23:06:14.000000 cvprocessor-0.0.20/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.20/src/cvprocessor/software.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-07 23:22:53.372001 cvprocessor-0.0.20/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-07 23:22:53.000000 cvprocessor-0.0.20/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      598 2024-05-07 23:22:53.000000 cvprocessor-0.0.20/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-07 23:22:53.000000 cvprocessor-0.0.20/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-07 23:22:53.000000 cvprocessor-0.0.20/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-07 23:22:53.000000 cvprocessor-0.0.20/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.0.19/LICENSE` & `cvprocessor-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.19/PKG-INFO` & `cvprocessor-0.0.20/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.19
+Version: 0.0.20
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.19/README.md` & `cvprocessor-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.19/pyproject.toml` & `cvprocessor-0.0.20/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.0.19"
+version = "0.0.20"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.0.19/src/cvprocessor/authors.py` & `cvprocessor-0.0.20/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.19/src/cvprocessor/cv.py` & `cvprocessor-0.0.20/src/cvprocessor/cv.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 from cvprocessor.education import Education
 from cvprocessor.publications import Publications
 from cvprocessor.authors import Authors
 from cvprocessor.software import Software
 from cvprocessor.institutes import Institutes
 from cvprocessor.news import News
 from cvprocessor.research_interests import ResearchInterests
+from cvprocessor.grants_awards import GrantsAwards
 
 
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
+        self._grants_awards = GrantsAwards(self.filename)
 
     @property
     def filename(self):
         return self._filename
 
     @property
     def intro(self):
@@ -61,31 +63,29 @@
     def publications(self):
         return self._publications
 
     @property
     def research_interests(self):
         return self._research_interests
 
+    @property
+    def grants_awards(self):
+        return self._grants_awards
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
+        self.grants_awards.print()
 
 
 if __name__ == "__main__":
     cv = CV("cv.xlsx")
-    cv.intro.print()
-    cv.education.print()
-    cv.institutes.print()
-    cv.authors.print()
-    cv.software.print()
-    cv.publications.print()
-    cv.news.print()
-    cv.research_interests.print()
+    cv.print()
     sys.exit(0)
```

### Comparing `cvprocessor-0.0.19/src/cvprocessor/education.py` & `cvprocessor-0.0.20/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.19/src/cvprocessor/institutes.py` & `cvprocessor-0.0.20/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.19/src/cvprocessor/intro.py` & `cvprocessor-0.0.20/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.19/src/cvprocessor/news.py` & `cvprocessor-0.0.20/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.19/src/cvprocessor/publications.py` & `cvprocessor-0.0.20/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.19/src/cvprocessor/research_interests.py` & `cvprocessor-0.0.20/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.19/src/cvprocessor/software.py` & `cvprocessor-0.0.20/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.19/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.0.20/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.19
+Version: 0.0.20
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.19/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.0.20/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 src/cvprocessor/__init__.py
 src/cvprocessor/authors.py
 src/cvprocessor/common.py
 src/cvprocessor/cv.py
 src/cvprocessor/education.py
 src/cvprocessor/experience.py
+src/cvprocessor/grants_awards.py
 src/cvprocessor/institutes.py
 src/cvprocessor/intro.py
 src/cvprocessor/news.py
 src/cvprocessor/publications.py
 src/cvprocessor/research_interests.py
 src/cvprocessor/software.py
 src/cvprocessor.egg-info/PKG-INFO
```

