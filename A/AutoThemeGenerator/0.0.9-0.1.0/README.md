# Comparing `tmp/autothemegenerator-0.0.9.tar.gz` & `tmp/autothemegenerator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autothemegenerator-0.0.9.tar", last modified: Wed May  8 06:04:49 2024, max compression
+gzip compressed data, was "autothemegenerator-0.1.0.tar", last modified: Wed May  8 06:06:37 2024, max compression
```

## Comparing `autothemegenerator-0.0.9.tar` & `autothemegenerator-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 06:04:49.882809 autothemegenerator-0.0.9/
-drwxrwxrwx   0        0        0        0 2024-05-08 06:04:49.867172 autothemegenerator-0.0.9/AutoThemeGenerator/
--rw-rw-rw-   0        0        0    29815 2024-05-08 06:04:22.000000 autothemegenerator-0.0.9/AutoThemeGenerator/AutoThemeGenerator.py
--rw-rw-rw-   0        0        0       86 2024-05-07 12:19:43.000000 autothemegenerator-0.0.9/AutoThemeGenerator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 06:04:49.882809 autothemegenerator-0.0.9/AutoThemeGenerator.egg-info/
--rw-rw-rw-   0        0        0     5170 2024-05-08 06:04:49.000000 autothemegenerator-0.0.9/AutoThemeGenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-08 06:04:49.000000 autothemegenerator-0.0.9/AutoThemeGenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 06:04:49.000000 autothemegenerator-0.0.9/AutoThemeGenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2024-05-08 06:04:49.000000 autothemegenerator-0.0.9/AutoThemeGenerator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-08 06:04:49.000000 autothemegenerator-0.0.9/AutoThemeGenerator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      757 2024-05-08 06:04:17.000000 autothemegenerator-0.0.9/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2024-05-07 12:08:17.000000 autothemegenerator-0.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-05-07 12:08:18.000000 autothemegenerator-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     5170 2024-05-08 06:04:49.882809 autothemegenerator-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     4217 2024-05-08 06:04:07.000000 autothemegenerator-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 06:04:49.882809 autothemegenerator-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1348 2024-05-08 06:04:26.000000 autothemegenerator-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:06:37.401714 autothemegenerator-0.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-08 06:06:37.396708 autothemegenerator-0.1.0/AutoThemeGenerator/
+-rw-rw-rw-   0        0        0    29815 2024-05-08 06:04:22.000000 autothemegenerator-0.1.0/AutoThemeGenerator/AutoThemeGenerator.py
+-rw-rw-rw-   0        0        0       86 2024-05-07 12:19:43.000000 autothemegenerator-0.1.0/AutoThemeGenerator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:06:37.401714 autothemegenerator-0.1.0/AutoThemeGenerator.egg-info/
+-rw-rw-rw-   0        0        0     5170 2024-05-08 06:06:37.000000 autothemegenerator-0.1.0/AutoThemeGenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-08 06:06:37.000000 autothemegenerator-0.1.0/AutoThemeGenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 06:06:37.000000 autothemegenerator-0.1.0/AutoThemeGenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2024-05-08 06:06:37.000000 autothemegenerator-0.1.0/AutoThemeGenerator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-08 06:06:37.000000 autothemegenerator-0.1.0/AutoThemeGenerator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      834 2024-05-08 06:05:49.000000 autothemegenerator-0.1.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2024-05-07 12:08:17.000000 autothemegenerator-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-07 12:08:18.000000 autothemegenerator-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5170 2024-05-08 06:06:37.401714 autothemegenerator-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4217 2024-05-08 06:06:09.000000 autothemegenerator-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 06:06:37.401714 autothemegenerator-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2024-05-08 06:05:35.000000 autothemegenerator-0.1.0/setup.py
```

### Comparing `autothemegenerator-0.0.9/AutoThemeGenerator/AutoThemeGenerator.py` & `autothemegenerator-0.1.0/AutoThemeGenerator/AutoThemeGenerator.py`

 * *Files identical despite different names*

### Comparing `autothemegenerator-0.0.9/AutoThemeGenerator.egg-info/PKG-INFO` & `autothemegenerator-0.1.0/AutoThemeGenerator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoThemeGenerator
-Version: 0.0.9
+Version: 0.1.0
 Summary: Performing thematic analysis with OpenAI's GPT-4 models
 Author: Charles Alba
 Author-email: alba@wustl.edu
 Keywords: GPT models,Thematic analysis,OpenAI,Qualitiative studies,transcripts,interviews
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 Requires-Dist: tqdm
 Requires-Dist: zipfile
 Requires-Dist: requests
 
 AutoThemeGenerator is a package that allows you to perform thematic analysis in qualitative studies using OpenAI's GPT models. 
 
 
-[![Documentation](https://img.shields.io/badge/Documentation-v0.0.8-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.0.8-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
+[![Documentation](https://img.shields.io/badge/Documentation-v0.1.0-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.0-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
 
 
 ## User inputs
 Users are only required to specify the folder location where their interview transcripts are stored. Accepted formats of transcripts include `PDF`, `.docx`, and `.txt` (prefered). `AutoThemeGenerator` assumes that each document is a transcript of one interviewed participant.
 
 ## Requirements
 ### Required packages
```

### Comparing `autothemegenerator-0.0.9/CHANGELOG.txt` & `autothemegenerator-0.1.0/CHANGELOG.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Change Log
 ==========
 
+0.1.0 (05/08/2024)
+-----------------------------
+- Bugs in the readme
+
+
 0.0.9 (05/08/2024)
 -----------------------------
 - Bugs in the readme
 
 0.0.8 (05/08/2024)
 -----------------------------
 - Bugs in the readme
```

### Comparing `autothemegenerator-0.0.9/LICENSE.txt` & `autothemegenerator-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autothemegenerator-0.0.9/PKG-INFO` & `autothemegenerator-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoThemeGenerator
-Version: 0.0.9
+Version: 0.1.0
 Summary: Performing thematic analysis with OpenAI's GPT-4 models
 Author: Charles Alba
 Author-email: alba@wustl.edu
 Keywords: GPT models,Thematic analysis,OpenAI,Qualitiative studies,transcripts,interviews
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 Requires-Dist: tqdm
 Requires-Dist: zipfile
 Requires-Dist: requests
 
 AutoThemeGenerator is a package that allows you to perform thematic analysis in qualitative studies using OpenAI's GPT models. 
 
 
-[![Documentation](https://img.shields.io/badge/Documentation-v0.0.8-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.0.8-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
+[![Documentation](https://img.shields.io/badge/Documentation-v0.1.0-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.0-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
 
 
 ## User inputs
 Users are only required to specify the folder location where their interview transcripts are stored. Accepted formats of transcripts include `PDF`, `.docx`, and `.txt` (prefered). `AutoThemeGenerator` assumes that each document is a transcript of one interviewed participant.
 
 ## Requirements
 ### Required packages
```

### Comparing `autothemegenerator-0.0.9/README.md` & `autothemegenerator-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 AutoThemeGenerator is a package that allows you to perform thematic analysis in qualitative studies using OpenAI's GPT models. 
 
 
-[![Documentation](https://img.shields.io/badge/Documentation-v0.0.8-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.0.8-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
+[![Documentation](https://img.shields.io/badge/Documentation-v0.1.0-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.0-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
 
 
 ## User inputs
 Users are only required to specify the folder location where their interview transcripts are stored. Accepted formats of transcripts include `PDF`, `.docx`, and `.txt` (prefered). `AutoThemeGenerator` assumes that each document is a transcript of one interviewed participant.
 
 ## Requirements
 ### Required packages
```

### Comparing `autothemegenerator-0.0.9/setup.py` & `autothemegenerator-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 readme_path = os.path.join(here, "README.md")
 with codecs.open(readme_path, encoding="utf-8") as fh:
     long_description = fh.read()
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 DESCRIPTION = 'Performing thematic analysis with OpenAI\'s GPT-4 models'
 LONG_DESCRIPTION = 'A package uses openAI\'s GPT-4 model to perform thematic analysis using interview transcripts from qualititative studies'
 
 # Setting up
 setup(
     name="AutoThemeGenerator",
     version=VERSION,
```

