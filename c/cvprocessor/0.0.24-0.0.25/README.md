# Comparing `tmp/cvprocessor-0.0.24.tar.gz` & `tmp/cvprocessor-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvprocessor-0.0.24.tar", last modified: Wed May  8 03:12:04 2024, max compression
+gzip compressed data, was "cvprocessor-0.0.25.tar", last modified: Wed May  8 07:29:14 2024, max compression
```

## Comparing `cvprocessor-0.0.24.tar` & `cvprocessor-0.0.25.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 03:12:04.216870 cvprocessor-0.0.24/
--rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.24/LICENSE
--rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-08 03:12:04.216164 cvprocessor-0.0.24/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      990 2024-05-07 21:56:16.000000 cvprocessor-0.0.24/README.md
--rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-08 03:11:23.000000 cvprocessor-0.0.24/pyproject.toml
--rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-08 03:12:04.217035 cvprocessor-0.0.24/setup.cfg
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 03:12:04.198897 cvprocessor-0.0.24/src/
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 03:12:04.211079 cvprocessor-0.0.24/src/cvprocessor/
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.24/src/cvprocessor/__init__.py
--rw-r--r--   0 fernando   (501) staff       (20)     5846 2024-05-07 21:58:53.000000 cvprocessor-0.0.24/src/cvprocessor/authors.py
--rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.24/src/cvprocessor/common.py
--rw-r--r--   0 fernando   (501) staff       (20)     2666 2024-05-08 00:27:54.000000 cvprocessor-0.0.24/src/cvprocessor/cv.py
--rw-r--r--   0 fernando   (501) staff       (20)     3629 2024-05-07 22:13:41.000000 cvprocessor-0.0.24/src/cvprocessor/education.py
--rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.24/src/cvprocessor/experience.py
--rw-r--r--   0 fernando   (501) staff       (20)     2153 2024-05-07 23:24:10.000000 cvprocessor-0.0.24/src/cvprocessor/grants_awards.py
--rw-r--r--   0 fernando   (501) staff       (20)     3340 2024-05-06 10:02:34.000000 cvprocessor-0.0.24/src/cvprocessor/institutes.py
--rw-r--r--   0 fernando   (501) staff       (20)     1396 2024-05-04 09:02:35.000000 cvprocessor-0.0.24/src/cvprocessor/intro.py
--rw-r--r--   0 fernando   (501) staff       (20)     2088 2024-05-05 08:39:17.000000 cvprocessor-0.0.24/src/cvprocessor/news.py
--rw-r--r--   0 fernando   (501) staff       (20)     9450 2024-05-07 00:03:04.000000 cvprocessor-0.0.24/src/cvprocessor/publications.py
--rw-r--r--   0 fernando   (501) staff       (20)      918 2024-05-07 23:06:14.000000 cvprocessor-0.0.24/src/cvprocessor/research_interests.py
--rw-r--r--   0 fernando   (501) staff       (20)     2967 2024-05-06 05:39:04.000000 cvprocessor-0.0.24/src/cvprocessor/software.py
--rw-r--r--   0 fernando   (501) staff       (20)     5157 2024-05-08 03:11:21.000000 cvprocessor-0.0.24/src/cvprocessor/teaching.py
-drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 03:12:04.215314 cvprocessor-0.0.24/src/cvprocessor.egg-info/
--rw-r--r--   0 fernando   (501) staff       (20)     1638 2024-05-08 03:12:04.000000 cvprocessor-0.0.24/src/cvprocessor.egg-info/PKG-INFO
--rw-r--r--   0 fernando   (501) staff       (20)      626 2024-05-08 03:12:04.000000 cvprocessor-0.0.24/src/cvprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-08 03:12:04.000000 cvprocessor-0.0.24/src/cvprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-08 03:12:04.000000 cvprocessor-0.0.24/src/cvprocessor.egg-info/requires.txt
--rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-08 03:12:04.000000 cvprocessor-0.0.24/src/cvprocessor.egg-info/top_level.txt
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 07:29:14.928408 cvprocessor-0.0.25/
+-rw-r--r--   0 fernando   (501) staff       (20)     1081 2024-05-04 07:19:07.000000 cvprocessor-0.0.25/LICENSE
+-rw-r--r--   0 fernando   (501) staff       (20)     1701 2024-05-08 07:29:14.927945 cvprocessor-0.0.25/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)     1053 2024-05-08 07:27:08.000000 cvprocessor-0.0.25/README.md
+-rw-r--r--   0 fernando   (501) staff       (20)      770 2024-05-08 07:28:02.000000 cvprocessor-0.0.25/pyproject.toml
+-rw-r--r--   0 fernando   (501) staff       (20)       38 2024-05-08 07:29:14.928492 cvprocessor-0.0.25/setup.cfg
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 07:29:14.913416 cvprocessor-0.0.25/src/
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 07:29:14.924464 cvprocessor-0.0.25/src/cvprocessor/
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-05 07:11:37.000000 cvprocessor-0.0.25/src/cvprocessor/__init__.py
+-rw-r--r--   0 fernando   (501) staff       (20)     6651 2024-05-08 07:01:09.000000 cvprocessor-0.0.25/src/cvprocessor/authors.py
+-rw-r--r--   0 fernando   (501) staff       (20)      148 2024-05-04 10:32:46.000000 cvprocessor-0.0.25/src/cvprocessor/common.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3220 2024-05-08 07:27:29.000000 cvprocessor-0.0.25/src/cvprocessor/cv.py
+-rw-r--r--   0 fernando   (501) staff       (20)     4218 2024-05-08 07:28:24.000000 cvprocessor-0.0.25/src/cvprocessor/education.py
+-rw-r--r--   0 fernando   (501) staff       (20)        0 2024-05-04 07:19:43.000000 cvprocessor-0.0.25/src/cvprocessor/experience.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2619 2024-05-08 07:09:50.000000 cvprocessor-0.0.25/src/cvprocessor/grants_awards.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3795 2024-05-08 07:11:28.000000 cvprocessor-0.0.25/src/cvprocessor/institutes.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1652 2024-05-08 07:13:23.000000 cvprocessor-0.0.25/src/cvprocessor/intro.py
+-rw-r--r--   0 fernando   (501) staff       (20)     2466 2024-05-08 07:13:59.000000 cvprocessor-0.0.25/src/cvprocessor/news.py
+-rw-r--r--   0 fernando   (501) staff       (20)     9925 2024-05-08 07:18:36.000000 cvprocessor-0.0.25/src/cvprocessor/publications.py
+-rw-r--r--   0 fernando   (501) staff       (20)     1133 2024-05-08 07:20:47.000000 cvprocessor-0.0.25/src/cvprocessor/research_interests.py
+-rw-r--r--   0 fernando   (501) staff       (20)     3509 2024-05-08 07:21:45.000000 cvprocessor-0.0.25/src/cvprocessor/software.py
+-rw-r--r--   0 fernando   (501) staff       (20)     5799 2024-05-08 07:22:45.000000 cvprocessor-0.0.25/src/cvprocessor/teaching.py
+drwxr-xr-x   0 fernando   (501) staff       (20)        0 2024-05-08 07:29:14.927337 cvprocessor-0.0.25/src/cvprocessor.egg-info/
+-rw-r--r--   0 fernando   (501) staff       (20)     1701 2024-05-08 07:29:14.000000 cvprocessor-0.0.25/src/cvprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 fernando   (501) staff       (20)      626 2024-05-08 07:29:14.000000 cvprocessor-0.0.25/src/cvprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        1 2024-05-08 07:29:14.000000 cvprocessor-0.0.25/src/cvprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 fernando   (501) staff       (20)        7 2024-05-08 07:29:14.000000 cvprocessor-0.0.25/src/cvprocessor.egg-info/requires.txt
+-rw-r--r--   0 fernando   (501) staff       (20)       12 2024-05-08 07:29:14.000000 cvprocessor-0.0.25/src/cvprocessor.egg-info/top_level.txt
```

### Comparing `cvprocessor-0.0.24/LICENSE` & `cvprocessor-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `cvprocessor-0.0.24/PKG-INFO` & `cvprocessor-0.0.25/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.24
+Version: 0.0.25
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -43,10 +43,12 @@
 ```python
 from cvprocessor.cv import CV
 
 # Load a CV file
 cv_file = "cv.xlsx"
 cv = CV(cv_file)
 
-# print CV details
-cv.print()
+# print education details
+print(cv.education)
+# Print teaching experience
+print(cv.teaching)
 ```
```

### Comparing `cvprocessor-0.0.24/README.md` & `cvprocessor-0.0.25/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -27,10 +27,12 @@
 ```python
 from cvprocessor.cv import CV
 
 # Load a CV file
 cv_file = "cv.xlsx"
 cv = CV(cv_file)
 
-# print CV details
-cv.print()
+# print education details
+print(cv.education)
+# Print teaching experience
+print(cv.teaching)
 ```
```

### Comparing `cvprocessor-0.0.24/pyproject.toml` & `cvprocessor-0.0.25/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvprocessor"
-version = "0.0.24"
+version = "0.0.25"
 authors = [
     { name = "F. Fernando Jurado-Lasso", email = "fdo.jurado@gmail.com" },
 ]
 description = "CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cvprocessor-0.0.24/src/cvprocessor/authors.py` & `cvprocessor-0.0.25/src/cvprocessor/authors.py`

 * *Files 16% similar despite different names*

```diff
@@ -121,35 +121,39 @@
         self._google_scholar = self.filename["Google Scholar"]
         self._orcid = self.filename["ORCID"]
         self._researchgate = self.filename["ResearchGate"]
         self._address = self.filename["Address"]
         self._location = self.filename["Location"]
         self._telephone = self.filename["Telephone"]
 
-    def print(self):
-        print(f"id: {self.id}")
-        print(f"Name: {self.name}")
-        print(f"Lastname: {self.lastname}")
-        print(f"Alias Long: {self.alias_long}")
-        print(f"Alias Short: {self.alias_short}")
-        print(f"Job Title: {self.job_title}")
-        print(f"Website: {self.website}")
-        print(f"Fingerprint: {self.fingerprint}")
-        print(f"Public Key: {self.public_key}")
-        print(f"Email: {self.email}")
-        print(f"LinkedIn: {self.linkedin}")
-        print(f"GitHub: {self.github}")
-        print(f"Google Scholar: {self.google_scholar}")
-        print(f"ORCID: {self.orcid}")
-        print(f"ResearchGate: {self.researchgate}")
-        print(f"Address: {self.address}")
-        print(f"Location: {self.location}")
-        print(f"Telephone: {self.telephone}")
-        print(f"Affiliation: {self.affiliation.name}")
-        print("\n")
+    def __str__(self):
+        string = f"id: {self.id}\n"
+        string += f"Name: {self.name}\n"
+        string += f"Lastname: {self.lastname}\n"
+        string += f"Alias Long: {self.alias_long}\n"
+        string += f"Alias Short: {self.alias_short}\n"
+        string += f"Job Title: {self.job_title}\n"
+        string += f"Website: {self.website}\n"
+        string += f"Fingerprint: {self.fingerprint}\n"
+        string += f"Public Key: {self.public_key}\n"
+        string += f"Email: {self.email}\n"
+        string += f"LinkedIn: {self.linkedin}\n"
+        string += f"GitHub: {self.github}\n"
+        string += f"Google Scholar: {self.google_scholar}\n"
+        string += f"ORCID: {self.orcid}\n"
+        string += f"ResearchGate: {self.researchgate}\n"
+        string += f"Address: {self.address}\n"
+        string += f"Location: {self.location}\n"
+        string += f"Telephone: {self.telephone}\n"
+        string += f"Affiliation: {self.affiliation.name}\n\n"
+        return string
+
+    def __repr__(self):
+        repr = f"Author(id={self.id}, name={self.name}, lastname={self.lastname}, alias_long={self.alias_long}, alias_short={self.alias_short}, job_title={self.job_title}, website={self.website}, fingerprint={self.fingerprint}, public_key={self.public_key}, email={self.email}, linkedin={self.linkedin}, github={self.github}, google_scholar={self.google_scholar}, orcid={self.orcid}, researchgate={self.researchgate}, address={self.address}, location={self.location}, telephone={self.telephone}, affiliation={self.affiliation})\n"
+        return repr
 
 
 class Authors:
     def __init__(self, filename, cv):
         self._filename = filename
         self._cv = cv
         self._authors = self._load_authors()
@@ -193,11 +197,16 @@
             else:
                 affiliation = self.cv.institutes.get_institute(
                     int(row["Affiliations"]))
                 author = AuthorsData(row, affiliation)
                 authors.append(author)
         return authors
 
-    def print(self):
-        print(f"Printing authors from {self.filename}...")
+    def __str__(self):
+        string = ""
         for author in self.authors:
-            author.print()
+            string += str(author)
+        return string
+
+    def __repr__(self):
+        repr = f"Authors(filename={self.filename}, cv={self.cv}, authors={self.authors})\n"
+        return repr
```

### Comparing `cvprocessor-0.0.24/src/cvprocessor/cv.py` & `cvprocessor-0.0.25/src/cvprocessor/cv.py`

 * *Files 22% similar despite different names*

```diff
@@ -73,26 +73,29 @@
     def grants_awards(self):
         return self._grants_awards
 
     @property
     def teaching(self):
         return self._teaching
 
-    def print(self):
-        print("CV")
-        print("Filename:", self.filename)
-        self.intro.print()
-        self.education.print()
-        self.institutes.print()
-        self.authors.print()
-        self.software.print()
-        self.publications.print()
-        self.news.print()
-        self.research_interests.print()
-        self.grants_awards.print()
-        self.teaching.print()
+    def __str__(self):
+        string = f"Education: {self.education}\n"
+        string += f"Institutes: {self.institutes}\n"
+        string += f"Software: {self.software}\n"
+        string += f"Intro: {self.intro}\n"
+        string += f"Authors: {self.authors}\n"
+        string += f"News: {self.news}\n"
+        string += f"Publications: {self.publications}\n"
+        string += f"Research Interests: {self.research_interests}\n"
+        string += f"Grants and Awards: {self.grants_awards}\n"
+        string += f"Teaching: {self.teaching}\n"
+        return string
+
+    def __repr__(self):
+        repr = f"CV(filename={self.filename}, education={self.education}, institutes={self.institutes}, software={self.software}, intro={self.intro}, authors={self.authors}, news={self.news}, publications={self.publications}, research_interests={self.research_interests}, grants_awards={self.grants_awards}, teaching={self.teaching})"
+        return repr
 
 
 if __name__ == "__main__":
     cv = CV("cv.xlsx")
-    cv.print()
+    print(repr(cv))
     sys.exit(0)
```

### Comparing `cvprocessor-0.0.24/src/cvprocessor/education.py` & `cvprocessor-0.0.25/src/cvprocessor/education.py`

 * *Files 17% similar despite different names*

```diff
@@ -81,26 +81,30 @@
         self._advisor = self.filename["Advisor"]
         self._thesis = self.filename["Thesis"]
         self._thesis_link = self.filename["Thesis link"]
         self._award = self.filename["Award"]
         self._institution = self.filename["Institution"]
         self._country = self.filename["Country"]
 
-    def print(self):
-        print(f"Year: {self.year}")
-        print(f"Start year: {self.start_year}")
-        print(f"End year: {self.end_year}")
-        print(f"Degree: {self.degree}")
-        print(f"Advisor: {self.advisor}")
-        print(f"Thesis: {self.thesis}")
-        print(f"Thesis link: {self.thesis_link}")
-        print(f"Award: {self.award}")
-        print(f"Institution: {self.institution}")
-        print(f"Country: {self.country}")
-        print("\n")
+    def __str__(self):
+        string = f"Year: {self.year}\n"
+        string += f"Start year: {self.start_year}\n"
+        string += f"End year: {self.end_year}\n"
+        string += f"Degree: {self.degree}\n"
+        string += f"Advisor: {self.advisor}\n"
+        string += f"Thesis: {self.thesis}\n"
+        string += f"Thesis link: {self.thesis_link}\n"
+        string += f"Award: {self.award}\n"
+        string += f"Institution: {self.institution}\n"
+        string += f"Country: {self.country}\n\n"
+        return string
+
+    def __repr__(self) -> str:
+        string = f"EducationData(year={self.year}, start_year={self.start_year}, end_year={self.end_year}, degree={self.degree}, advisor={self.advisor}, thesis={self.thesis}, thesis_link={self.thesis_link}, award={self.award}, institution={self.institution}, country={self.country})"
+        return string
 
 
 class Education:
     def __init__(self, filename):
         self._filename = filename
         self._educations = self._load_educations()
         # sort the education data by end year
@@ -119,10 +123,16 @@
     def get_oldest_end_year(self):
         return self.educations[-1].end_year.year
 
     def _load_educations(self):
         education_df = pd.read_excel(self.filename, sheet_name="Education")
         return [EducationData(row) for _, row in education_df.iterrows()]
 
-    def print(self):
+    def __str__(self) -> str:
+        string = ""
         for education in self.educations:
-            education.print()
+            string += str(education)
+        return string
+
+    def __repr__(self) -> str:
+        repr = f"Education(filename={self.filename}, educations={self.educations})\n"
+        return repr
```

### Comparing `cvprocessor-0.0.24/src/cvprocessor/institutes.py` & `cvprocessor-0.0.25/src/cvprocessor/institutes.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,23 +70,27 @@
         self._address = self._pd_dataframe["Address"]
         self._city = self._pd_dataframe["City"]
         self._country = self._pd_dataframe["Country"]
         self._url = self._pd_dataframe["URL"]
         self._coordinates = self._pd_dataframe["Coordinates"]
         self.process_coordinates()
 
-    def print(self):
-        print(f"Institute ID: {self._id}")
-        print(f"Institute Name: {self._name}")
-        print(f"Institute Address: {self._address}")
-        print(f"Institute City: {self._city}")
-        print(f"Institute Country: {self._country}")
-        print(f"Institute URL: {self._url}")
-        print(f"Institute Coordinates: {self._coordinates}")
-        print("\n")
+    def __str__(self):
+        string = f"Institute ID: {self._id}\n"
+        string += f"Institute Name: {self._name}\n"
+        string += f"Institute Address: {self._address}\n"
+        string += f"Institute City: {self._city}\n"
+        string += f"Institute Country: {self._country}\n"
+        string += f"Institute URL: {self._url}\n"
+        string += f"Institute Coordinates: {self._coordinates}\n\n"
+        return string
+
+    def __repr__(self):
+        string = f"InstituteData(id={self._id}, name={self._name}, address={self._address}, city={self._city}, country={self._country}, coordinates={self._coordinates}, url={self._url})"
+        return string
 
 
 class Institutes:
     def __init__(self, filename):
         self._filename = filename
         self._institute = self._load_institutes()
 
@@ -106,10 +110,16 @@
                 return institute
         return None
 
     def _load_institutes(self):
         institutes_df = pd.read_excel(self.filename, sheet_name="Institutes")
         return [InstituteData(institute) for index, institute in institutes_df.iterrows()]
 
-    def print(self):
+    def __str__(self):
+        string = ""
         for institute in self.institute:
-            institute.print()
+            string += str(institute)
+        return string
+
+    def __repr__(self):
+        repr = f"Institutes(filename={self.filename}, institute={self.institute})\n"
+        return repr
```

### Comparing `cvprocessor-0.0.24/src/cvprocessor/publications.py` & `cvprocessor-0.0.25/src/cvprocessor/publications.py`

 * *Files 26% similar despite different names*

```diff
@@ -196,36 +196,39 @@
         if not common.check_nan(self.page_end):
             citation += f"-{int(self.page_end)}"
         if not common.check_nan(self.doi):
             citation += f", doi: {self.doi}"
         citation += "."
         return citation
 
-    def print(self):
-        print(f"Authors: {self.authors}")
-        print(f"Title: {self.title}")
-        print(f"Year: {self.year}")
-        print(f"Source: {self.source}")
-        print(f"Volume: {self.volume}")
-        print(f"Issue: {self.issue}")
-        print(f"Art. No.: {self.artno}")
-        print(f"Page start: {self.page_start}")
-        print(f"Page end: {self.page_end}")
-        print(f"DOI: {self.doi}")
-        print(f"Preprint DOI: {self.preprint_doi}")
-        print(f"Document Type: {self.document_type}")
-        print(f"Code: {self.code.name if self.code else None}")
-        print(f"Slides: {self.slides}")
-        print(f"Abstract: {self.abstract}")
-        print(f"Keywords: {self.keywords}")
-        print(f"JCR: {self.jcr}")
-        print(f"License: {self.license}")
-        print(f"Copyright: {self.copyright}")
-        citation = self.build_apa_citation()
-        print(f"Citation: {citation}")
+    def __str__(self) -> str:
+        string = f"Title: {self.title}\n"
+        string += f"Authors: {self.authors}\n"
+        string += f"Year: {self.year}\n"
+        string += f"Source: {self.source}\n"
+        string += f"Volume: {self.volume}\n"
+        string += f"Issue: {self.issue}\n"
+        string += f"Art. No.: {self.artno}\n"
+        string += f"Page start: {self.page_start}\n"
+        string += f"Page end: {self.page_end}\n"
+        string += f"DOI: {self.doi}\n"
+        string += f"Preprint DOI: {self.preprint_doi}\n"
+        string += f"Document Type: {self.document_type}\n"
+        string += f"Code: {self.code.name if self.code else None}\n"
+        string += f"Slides: {self.slides}\n"
+        string += f"Abstract: {self.abstract}\n"
+        string += f"Keywords: {self.keywords}\n"
+        string += f"JCR: {self.jcr}\n"
+        string += f"License: {self.license}\n"
+        string += f"Copyright: {self.copyright}\n\n"
+        return string
+
+    def __repr__(self) -> str:
+        repr = f"PublicationsData(authors={self.authors}, title={self.title}, year={self.year}, source={self.source}, volume={self.volume}, issue={self.issue}, artno={self.artno}, page_start={self.page_start}, page_end={self.page_end}, doi={self.doi}, preprint_doi={self.preprint_doi}, document_type={self.document_type}, code={self.code}, slides={self.slides}, abstract={self.abstract}, keywords={self.keywords}, jcr={self.jcr}, license={self.license}, copyright={self.copyright})"
+        return repr
 
 
 class Publications():
     def __init__(self, filename, cv):
         self._filename = filename
         self._cv = cv
         self._publications = self._load_publications()
@@ -290,15 +293,16 @@
         return min(years), max(years)
 
     def _load_publications(self):
         publications_df = pd.read_excel(
             self.filename, sheet_name="Publications")
         return [PublicationsData(row, self.cv) for index, row in publications_df.iterrows()]
 
-    def print(self):
-        print(f"Publications in {self.filename}")
+    def __str__(self):
+        string = ""
         for publication in self.publications:
-            publication.print()
-        # print the number of publications and unique sources
-        print(f"Total publications: {self.get_publications_count()}")
-        print(f"Unique sources: {self.get_unique_sources()}")
-        print(f"Document types: {self.get_document_types()}")
+            string += str(publication)
+        return string
+
+    def __repr__(self):
+        repr = f"Publications(filename={self.filename}, cv={self.cv}, publications={self.publications})\n"
+        return repr
```

### Comparing `cvprocessor-0.0.24/src/cvprocessor/research_interests.py` & `cvprocessor-0.0.25/src/cvprocessor/research_interests.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,18 +17,22 @@
         return self._keywords
 
     @property
     def research_interests(self):
         return self._research_interests
 
     def _load_interests(self):
-        self._filename = pd.read_excel(
+        research_interests_pd = pd.read_excel(
             self.filename, sheet_name="Research_Interests")
-        self._research_interests = self.filename["Interests"].values[0]
-        keywords = self.filename["Keywords"]
+        self._research_interests = research_interests_pd["Interests"].values[0]
+        keywords = research_interests_pd["Keywords"]
         for keyword in keywords:
             self._keywords.append(keyword)
 
-    def print(self):
-        print(f"Research Interests: {self._research_interests}")
-        print(f"Keywords: {self._keywords}")
-        print("\n")
+    def __str__(self):
+        string = f"Research Interests: {self.research_interests}\n"
+        string += f"Keywords: {self.keywords}\n\n"
+        return string
+
+    def __repr__(self):
+        repr = f"ResearchInterests(filename={self.filename}, research_interests={self.research_interests}, keywords={self.keywords})"
+        return repr
```

### Comparing `cvprocessor-0.0.24/src/cvprocessor/software.py` & `cvprocessor-0.0.25/src/cvprocessor/grants_awards.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,118 +1,91 @@
 import pandas as pd
 
 
-class SofwareData:
+class GrantsAwardsData:
     def __init__(self, filename):
         self._filename = filename
-        self._id = None
-        self._name = None
-        self._version = None
+        self._year = None
         self._description = None
-        self._repository = None
-        self._demo = None
-        self._website = None
-        self._summary = None
-        self._license = None
-        self._load_software()
+        self._institution = None
+        self._country = None
+        self._value = None
+        self._load_grants_awards()
 
     @property
     def filename(self):
         return self._filename
 
     @property
-    def id(self):
-        return self._id
-
-    @property
-    def name(self):
-        return self._name
-
-    @property
-    def version(self):
-        return self._version
+    def year(self):
+        return self._year
 
     @property
     def description(self):
         return self._description
 
     @property
-    def repository(self):
-        return self._repository
-
-    @property
-    def demo(self):
-        return self._demo
-
-    @property
-    def website(self):
-        return self._website
+    def institution(self):
+        return self._institution
 
     @property
-    def summary(self):
-        return self._summary
+    def country(self):
+        return self._country
 
     @property
-    def license(self):
-        return self._license
+    def value(self):
+        return self._value
 
-    # @property
-    # def doi(self):
-    #     return self._doi
-
-    def _load_software(self):
-        self._id = self.filename["id"]
-        self._name = self.filename["Name"]
-        self._version = self.filename["Version"]
+    def _load_grants_awards(self):
+        self._year = self.filename["Year"]
+        self._year = pd.to_datetime(self.year, format="%Y").year
         self._description = self.filename["Description"]
-        self._repository = self.filename["Repository"]
-        self._demo = self.filename["Demo"]
-        self._website = self.filename["Website"]
-        self._summary = self.filename["Summary"]
-        self._license = self.filename["License"]
-
-    def print(self):
-        print(f"ID: {self.id}")
-        print(f"Name: {self.name}")
-        print(f"Version: {self.version}")
-        print(f"Description: {self.description}")
-        print(f"repository: {self.repository}")
-        print(f"Demo: {self.demo}")
-        print(f"Website: {self.website}")
-        print(f"Summary: {self.summary}")
-        print(f"License: {self.license}")
-        print("\n")
+        self._institution = self.filename["Institution"]
+        self._country = self.filename["Country"]
+        self._value = self.filename["Value"]
+
+    def __str__(self) -> str:
+        string = f"Year: {self.year}\n"
+        string += f"Description: {self.description}\n"
+        string += f"Institution: {self.institution}\n"
+        string += f"Country: {self.country}\n"
+        string += f"Value: {self.value}\n\n"
+        return string
+
+    def __repr__(self) -> str:
+        string = f"GrantsAwardsData(year={self.year}, description={self.description}, institution={self.institution}, country={self.country}, value={self.value})"
+        return string
 
 
-class Software:
+class GrantsAwards:
     def __init__(self, filename):
         self._filename = filename
-        self._software = self._load_software()
+        self._grants_awards = self._load_grants_awards()
+        # sort the grants_awards data by year
+        self._grants_awards = sorted(
+            self.grants_awards, key=lambda x: x.year, reverse=True)
 
     @property
     def filename(self):
         return self._filename
 
     @property
-    def software(self):
-        return self._software
+    def grants_awards(self):
+        return self._grants_awards
+
+    def get_oldest_year(self):
+        return self.grants_awards[-1].year
 
-    def get_software(self, software_id):
-        if not software_id:
-            return None
-        if isinstance(software_id, str):
-            software_id = int(software_id)
-        for software in self.software:
-            if software.id == software_id:
-                return software
-        return None
-
-    def get_software_alphabetically(self):
-        return sorted(self.software, key=lambda x: x.name)
-
-    def _load_software(self):
-        software_df = pd.read_excel(self.filename, sheet_name="Software")
-        return [SofwareData(software) for index, software in software_df.iterrows()]
-
-    def print(self):
-        for software in self.software:
-            software.print()
+    def _load_grants_awards(self):
+        grants_rewards_df = pd.read_excel(
+            self.filename, sheet_name="Grants_awards")
+        return [GrantsAwardsData(row) for _, row in grants_rewards_df.iterrows()]
+
+    def __str__(self) -> str:
+        string = ""
+        for grants_award in self.grants_awards:
+            string += str(grants_award)
+        return string
+
+    def __repr__(self) -> str:
+        string = f"GrantsAwards(filename={self.filename}, grants_awards={self.grants_awards})"
+        return string
```

### Comparing `cvprocessor-0.0.24/src/cvprocessor/teaching.py` & `cvprocessor-0.0.25/src/cvprocessor/teaching.py`

 * *Files 14% similar despite different names*

```diff
@@ -126,28 +126,32 @@
         self._type = self.filename["Type"]
         self._institution = self.filename["Institution"]
         self._department = self.filename["Department"]
         self._country = self.filename["Country"]
         self._supervisor = self.filename["Supervisor"]
         self._responsibilities = self.filename["Responsibilities"]
 
-    def print(self):
-        print(f"Year: {self.year}")
-        print(f"Start year: {self.start_year}")
-        print(f"End year: {self.end_year}")
-        print(f"Position: {self.position}")
-        print(f"Course: {self.course}")
-        print(f"Link: {self.link}")
-        print(f"Type: {self.type}")
-        print(f"Institution: {self.institution}")
-        print(f"Department: {self.department}")
-        print(f"Country: {self.country}")
-        print(f"Supervisor: {self.supervisor}")
-        print(f"Responsibilities: {self.responsibilities}")
-        print("\n")
+    def __str__(self):
+        string = f"Year: {self.year}\n"
+        string += f"Start year: {self.start_year}\n"
+        string += f"End year: {self.end_year}\n"
+        string += f"Position: {self.position}\n"
+        string += f"Course: {self.course}\n"
+        string += f"Link: {self.link}\n"
+        string += f"Type: {self.type}\n"
+        string += f"Institution: {self.institution}\n"
+        string += f"Department: {self.department}\n"
+        string += f"Country: {self.country}\n"
+        string += f"Supervisor: {self.supervisor}\n"
+        string += f"Responsibilities: {self.responsibilities}\n\n"
+        return string
+
+    def __repr__(self):
+        string = f"TeachingData(year={self.year}, start_year={self.start_year}, end_year={self.end_year}, position={self.position}, course={self.course}, link={self.link}, type={self.type}, institution={self.institution}, department={self.department}, country={self.country}, supervisor={self.supervisor}, responsibilities={self.responsibilities})"
+        return string
 
 
 class Teaching:
     def __init__(self, filename):
         self._filename = filename
         self._teaching = self._load_teaching()
         # Sort the teaching data by type then by year
@@ -176,10 +180,16 @@
                 count += 1
         return count
 
     def _load_teaching(self):
         teaching_df = pd.read_excel(self.filename, sheet_name="Teaching")
         return [TeachingData(teaching) for _, teaching in teaching_df.iterrows()]
 
-    def print(self):
+    def __str__(self):
+        string = ""
         for teaching in self.teaching:
-            teaching.print()
+            string += str(teaching)
+        return string
+
+    def __repr__(self):
+        string = f"Teaching(filename={self.filename}, teaching={self.teaching})\n"
+        return string
```

### Comparing `cvprocessor-0.0.24/src/cvprocessor.egg-info/PKG-INFO` & `cvprocessor-0.0.25/src/cvprocessor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvprocessor
-Version: 0.0.24
+Version: 0.0.25
 Summary: CVProcessor is a Python library for processing CV (Curriculum Vitae) or resume documents.
 Author-email: "F. Fernando Jurado-Lasso" <fdo.jurado@gmail.com>
 Project-URL: Homepage, https://github.com/fdojurado/CVProcessor
 Project-URL: Issues, https://github.com/fdojurado/CVProcessor/issues
 Keywords: CV,Curriculum Vitae,Resume,xslx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -43,10 +43,12 @@
 ```python
 from cvprocessor.cv import CV
 
 # Load a CV file
 cv_file = "cv.xlsx"
 cv = CV(cv_file)
 
-# print CV details
-cv.print()
+# print education details
+print(cv.education)
+# Print teaching experience
+print(cv.teaching)
 ```
```

### Comparing `cvprocessor-0.0.24/src/cvprocessor.egg-info/SOURCES.txt` & `cvprocessor-0.0.25/src/cvprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

