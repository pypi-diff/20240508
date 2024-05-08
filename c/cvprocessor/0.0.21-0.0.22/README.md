# Comparing `tmp/cvprocessor-0.0.21.tar.gz` & `tmp/cvprocessor-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.0.21.tar", last modified: Wed May  8 02:09:42 2024, max compression
+gzip compressed data, was "cvprocessor-0.0.22.tar", last modified: Wed May  8 02:21:25 2024, max compression
```

## Comparing `cvprocessor-0.0.21.tar` & `cvprocessor-0.0.22.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:09:42.754163 cvprocessor-0.0.21/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.21/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-08 02:09:42.753442 cvprocessor-0.0.21/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      990 2024-05-07 21:56:16.000000 cvprocessor-0.0.21/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-08 02:09:01.000000 cvprocessor-0.0.21/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-08 02:09:42.754311 cvprocessor-0.0.21/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:09:42.736279 cvprocessor-0.0.21/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:09:42.748596 cvprocessor-0.0.21/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.21/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     5846 2024-05-07 21:58:53.000000 cvprocessor-0.0.21/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.21/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     2666 2024-05-08 00:27:54.000000 cvprocessor-0.0.21/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     3629 2024-05-07 22:13:41.000000 cvprocessor-0.0.21/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.21/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     2153 2024-05-07 23:24:10.000000 cvprocessor-0.0.21/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.21/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.21/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.21/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.21/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)      918 2024-05-07 23:06:14.000000 cvprocessor-0.0.21/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.21/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     4517 2024-05-08 02:07:59.000000 cvprocessor-0.0.21/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:09:42.752833 cvprocessor-0.0.21/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-08 02:09:42.000000 cvprocessor-0.0.21/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      626 2024-05-08 02:09:42.000000 cvprocessor-0.0.21/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-08 02:09:42.000000 cvprocessor-0.0.21/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-08 02:09:42.000000 cvprocessor-0.0.21/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-08 02:09:42.000000 cvprocessor-0.0.21/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:21:25.837308 cvprocessor-0.0.22/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.22/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-08 02:21:25.836273 cvprocessor-0.0.22/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      990 2024-05-07 21:56:16.000000 cvprocessor-0.0.22/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-08 02:13:50.000000 cvprocessor-0.0.22/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-08 02:21:25.837486 cvprocessor-0.0.22/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:21:25.816517 cvprocessor-0.0.22/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:21:25.831267 cvprocessor-0.0.22/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.22/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5846 2024-05-07 21:58:53.000000 cvprocessor-0.0.22/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.22/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2666 2024-05-08 00:27:54.000000 cvprocessor-0.0.22/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3629 2024-05-07 22:13:41.000000 cvprocessor-0.0.22/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.22/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2153 2024-05-07 23:24:10.000000 cvprocessor-0.0.22/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.22/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.22/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.22/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.22/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)      918 2024-05-07 23:06:14.000000 cvprocessor-0.0.22/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.22/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4974 2024-05-08 02:16:16.000000 cvprocessor-0.0.22/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 02:21:25.835280 cvprocessor-0.0.22/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-08 02:21:25.000000 cvprocessor-0.0.22/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      626 2024-05-08 02:21:25.000000 cvprocessor-0.0.22/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-08 02:21:25.000000 cvprocessor-0.0.22/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-08 02:21:25.000000 cvprocessor-0.0.22/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-08 02:21:25.000000 cvprocessor-0.0.22/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.0.21/LICENSE` & `cvprocessor-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.21/PKG-INFO` & `cvprocessor-0.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.21
+Version: 0.0.22
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.21/README.md` & `cvprocessor-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.21/pyproject.toml` & `cvprocessor-0.0.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.0.21"
+version = "0.0.22"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.0.21/src/cvprocessor/authors.py` & `cvprocessor-0.0.22/src/cvprocessor/authors.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.21/src/cvprocessor/cv.py` & `cvprocessor-0.0.22/src/cvprocessor/cv.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.21/src/cvprocessor/education.py` & `cvprocessor-0.0.22/src/cvprocessor/education.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.21/src/cvprocessor/grants_awards.py` & `cvprocessor-0.0.22/src/cvprocessor/grants_awards.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.21/src/cvprocessor/institutes.py` & `cvprocessor-0.0.22/src/cvprocessor/institutes.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.21/src/cvprocessor/intro.py` & `cvprocessor-0.0.22/src/cvprocessor/intro.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.21/src/cvprocessor/news.py` & `cvprocessor-0.0.22/src/cvprocessor/news.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.21/src/cvprocessor/publications.py` & `cvprocessor-0.0.22/src/cvprocessor/publications.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.21/src/cvprocessor/research_interests.py` & `cvprocessor-0.0.22/src/cvprocessor/research_interests.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.21/src/cvprocessor/software.py` & `cvprocessor-0.0.22/src/cvprocessor/software.py`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.21/src/cvprocessor/teaching.py` & `cvprocessor-0.0.22/src/cvprocessor/teaching.py`

 * *Files 7% similar despite different names*

```diff
@@ -150,14 +150,28 @@
     def filename(self):
         return self._filename
 
     @property
     def teaching(self):
         return self._teaching
 
+    def get_teaching_type_ordered(self):
+        teaching_type = []
+        for teaching in self.teaching:
+            if teaching.type not in teaching_type:
+                teaching_type.append(teaching.type)
+        return teaching_type
+
+    def get_num_teaching_by_document_type(self, teaching_type):
+        count = 0
+        for teaching in self.teaching:
+            if teaching.type == teaching_type:
+                count += 1
+        return count
+
     def _load_teaching(self):
         teaching_df = pd.read_excel(self.filename, sheet_name="Teaching")
         return [TeachingData(teaching) for _, teaching in teaching_df.iterrows()]
 
     def print(self):
         for teaching in self.teaching:
             teaching.print()
```

### Comparing `cvprocessor-0.0.21/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.0.22/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.21
+Version: 0.0.22
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cvprocessor-0.0.21/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.0.22/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

