# Comparing `tmp/autothemegenerator-0.1.0.tar.gz` & `tmp/autothemegenerator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autothemegenerator-0.1.0.tar", last modified: Wed May  8 06:06:37 2024, max compression
+gzip compressed data, was "autothemegenerator-0.1.1.tar", last modified: Wed May  8 06:29:40 2024, max compression
```

## Comparing `autothemegenerator-0.1.0.tar` & `autothemegenerator-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 06:06:37.401714 autothemegenerator-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-05-08 06:06:37.396708 autothemegenerator-0.1.0/AutoThemeGenerator/
--rw-rw-rw-   0        0        0    29815 2024-05-08 06:04:22.000000 autothemegenerator-0.1.0/AutoThemeGenerator/AutoThemeGenerator.py
--rw-rw-rw-   0        0        0       86 2024-05-07 12:19:43.000000 autothemegenerator-0.1.0/AutoThemeGenerator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 06:06:37.401714 autothemegenerator-0.1.0/AutoThemeGenerator.egg-info/
--rw-rw-rw-   0        0        0     5170 2024-05-08 06:06:37.000000 autothemegenerator-0.1.0/AutoThemeGenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-08 06:06:37.000000 autothemegenerator-0.1.0/AutoThemeGenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 06:06:37.000000 autothemegenerator-0.1.0/AutoThemeGenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2024-05-08 06:06:37.000000 autothemegenerator-0.1.0/AutoThemeGenerator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-08 06:06:37.000000 autothemegenerator-0.1.0/AutoThemeGenerator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      834 2024-05-08 06:05:49.000000 autothemegenerator-0.1.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2024-05-07 12:08:17.000000 autothemegenerator-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-05-07 12:08:18.000000 autothemegenerator-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5170 2024-05-08 06:06:37.401714 autothemegenerator-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4217 2024-05-08 06:06:09.000000 autothemegenerator-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 06:06:37.401714 autothemegenerator-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1348 2024-05-08 06:05:35.000000 autothemegenerator-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:29:40.038963 autothemegenerator-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-08 06:29:40.025402 autothemegenerator-0.1.1/AutoThemeGenerator/
+-rw-rw-rw-   0        0        0    29815 2024-05-08 06:04:22.000000 autothemegenerator-0.1.1/AutoThemeGenerator/AutoThemeGenerator.py
+-rw-rw-rw-   0        0        0       86 2024-05-07 12:19:43.000000 autothemegenerator-0.1.1/AutoThemeGenerator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:29:40.038963 autothemegenerator-0.1.1/AutoThemeGenerator.egg-info/
+-rw-rw-rw-   0        0        0     5246 2024-05-08 06:29:39.000000 autothemegenerator-0.1.1/AutoThemeGenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-08 06:29:39.000000 autothemegenerator-0.1.1/AutoThemeGenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 06:29:39.000000 autothemegenerator-0.1.1/AutoThemeGenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2024-05-08 06:29:39.000000 autothemegenerator-0.1.1/AutoThemeGenerator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-08 06:29:39.000000 autothemegenerator-0.1.1/AutoThemeGenerator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      904 2024-05-08 06:18:19.000000 autothemegenerator-0.1.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2024-05-07 12:08:17.000000 autothemegenerator-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-05-07 12:08:18.000000 autothemegenerator-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5246 2024-05-08 06:29:40.038963 autothemegenerator-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4293 2024-05-08 06:28:58.000000 autothemegenerator-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 06:29:40.038963 autothemegenerator-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2024-05-08 06:29:12.000000 autothemegenerator-0.1.1/setup.py
```

### Comparing `autothemegenerator-0.1.0/AutoThemeGenerator/AutoThemeGenerator.py` & `autothemegenerator-0.1.1/AutoThemeGenerator/AutoThemeGenerator.py`

 * *Files identical despite different names*

### Comparing `autothemegenerator-0.1.0/AutoThemeGenerator.egg-info/PKG-INFO` & `autothemegenerator-0.1.1/AutoThemeGenerator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoThemeGenerator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Performing thematic analysis with OpenAI's GPT-4 models
 Author: Charles Alba
 Author-email: alba@wustl.edu
 Keywords: GPT models,Thematic analysis,OpenAI,Qualitiative studies,transcripts,interviews
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -22,38 +22,38 @@
 Requires-Dist: tqdm
 Requires-Dist: zipfile
 Requires-Dist: requests
 
 AutoThemeGenerator is a package that allows you to perform thematic analysis in qualitative studies using OpenAI's GPT models. 
 
 
-[![Documentation](https://img.shields.io/badge/Documentation-v0.1.0-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.0-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
+[![Documentation](https://img.shields.io/badge/Documentation-v0.1.1-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.1-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
 
 
 ## User inputs
 Users are only required to specify the folder location where their interview transcripts are stored. Accepted formats of transcripts include `PDF`, `.docx`, and `.txt` (prefered). `AutoThemeGenerator` assumes that each document is a transcript of one interviewed participant.
 
 ## Requirements
 ### Required packages
 To use `AutoThemeGenerator`, you are required to have the following packages installed:  
 - `openai`  
 - `docx`    
 - `tqdm`    
 - `nltk`    
-- `nltk.tokenize`    
+- `nltk.tokenize` (submodule of `nltk`)   
 - `python-docx`  
 - `textract`  
-- `zipfile`  
-- `shutil`  
 - `requests`  
-- `json`  
+- `zipfile` (Python standard library)   
+- `shutil`  (Python standard library)  
+- `json`  (Python standard library)  
 
 If you do not have this packages installed in python, you can do the following:
 ```bash
-pip install openai docx tqdm nltk nltk.tokenize python-docx textract zipfile shutil requests json
+pip install openai==1.12.0 python-docx docx tqdm nltk textract requests
 ```
 ### OpenAI API key
 You also need an OpenAI key to be able to use this package. If you do not have one, you can apply for an OpenAI API key at [platform.openai.com/api-keys](https://platform.openai.com/api-keys). 
 
 ## Installation
 To install in python, simply do the following: 
 ```bash
```

### Comparing `autothemegenerator-0.1.0/CHANGELOG.txt` & `autothemegenerator-0.1.1/CHANGELOG.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Change Log
 ==========
 
+
+0.1.1 (05/08/2024)
+-----------------------------
+- Fixed typos
+
 0.1.0 (05/08/2024)
 -----------------------------
 - Bugs in the readme
 
 
 0.0.9 (05/08/2024)
 -----------------------------
```

### Comparing `autothemegenerator-0.1.0/LICENSE.txt` & `autothemegenerator-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autothemegenerator-0.1.0/PKG-INFO` & `autothemegenerator-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoThemeGenerator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Performing thematic analysis with OpenAI's GPT-4 models
 Author: Charles Alba
 Author-email: alba@wustl.edu
 Keywords: GPT models,Thematic analysis,OpenAI,Qualitiative studies,transcripts,interviews
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
@@ -22,38 +22,38 @@
 Requires-Dist: tqdm
 Requires-Dist: zipfile
 Requires-Dist: requests
 
 AutoThemeGenerator is a package that allows you to perform thematic analysis in qualitative studies using OpenAI's GPT models. 
 
 
-[![Documentation](https://img.shields.io/badge/Documentation-v0.1.0-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.0-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
+[![Documentation](https://img.shields.io/badge/Documentation-v0.1.1-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.1-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
 
 
 ## User inputs
 Users are only required to specify the folder location where their interview transcripts are stored. Accepted formats of transcripts include `PDF`, `.docx`, and `.txt` (prefered). `AutoThemeGenerator` assumes that each document is a transcript of one interviewed participant.
 
 ## Requirements
 ### Required packages
 To use `AutoThemeGenerator`, you are required to have the following packages installed:  
 - `openai`  
 - `docx`    
 - `tqdm`    
 - `nltk`    
-- `nltk.tokenize`    
+- `nltk.tokenize` (submodule of `nltk`)   
 - `python-docx`  
 - `textract`  
-- `zipfile`  
-- `shutil`  
 - `requests`  
-- `json`  
+- `zipfile` (Python standard library)   
+- `shutil`  (Python standard library)  
+- `json`  (Python standard library)  
 
 If you do not have this packages installed in python, you can do the following:
 ```bash
-pip install openai docx tqdm nltk nltk.tokenize python-docx textract zipfile shutil requests json
+pip install openai==1.12.0 python-docx docx tqdm nltk textract requests
 ```
 ### OpenAI API key
 You also need an OpenAI key to be able to use this package. If you do not have one, you can apply for an OpenAI API key at [platform.openai.com/api-keys](https://platform.openai.com/api-keys). 
 
 ## Installation
 To install in python, simply do the following: 
 ```bash
```

### Comparing `autothemegenerator-0.1.0/README.md` & `autothemegenerator-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 AutoThemeGenerator is a package that allows you to perform thematic analysis in qualitative studies using OpenAI's GPT models. 
 
 
-[![Documentation](https://img.shields.io/badge/Documentation-v0.1.0-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.0-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
+[![Documentation](https://img.shields.io/badge/Documentation-v0.1.1-orange)](https://cja5553.github.io/ReadTheDocs_AutoThemeGenerator/) [![pypi package](https://img.shields.io/badge/pypi_package-v0.1.1-brightgreen)](https://pypi.org/project/AutoThemeGenerator/) [![GitHub Source Code](https://img.shields.io/badge/github_source_code-source_code?logo=github&color=green)](https://github.com/cja5553/AutoThemeGenerator) [![Colab Example](https://img.shields.io/badge/-Colab_Example-grey?logo=google&logoColor=F9AB00)](https://colab.research.google.com/drive/1BoAI-QNL-yL8j8hUJ3K8cJkbyp4spoQ3)
 
 
 ## User inputs
 Users are only required to specify the folder location where their interview transcripts are stored. Accepted formats of transcripts include `PDF`, `.docx`, and `.txt` (prefered). `AutoThemeGenerator` assumes that each document is a transcript of one interviewed participant.
 
 ## Requirements
 ### Required packages
 To use `AutoThemeGenerator`, you are required to have the following packages installed:  
 - `openai`  
 - `docx`    
 - `tqdm`    
 - `nltk`    
-- `nltk.tokenize`    
+- `nltk.tokenize` (submodule of `nltk`)   
 - `python-docx`  
 - `textract`  
-- `zipfile`  
-- `shutil`  
 - `requests`  
-- `json`  
+- `zipfile` (Python standard library)   
+- `shutil`  (Python standard library)  
+- `json`  (Python standard library)  
 
 If you do not have this packages installed in python, you can do the following:
 ```bash
-pip install openai docx tqdm nltk nltk.tokenize python-docx textract zipfile shutil requests json
+pip install openai==1.12.0 python-docx docx tqdm nltk textract requests
 ```
 ### OpenAI API key
 You also need an OpenAI key to be able to use this package. If you do not have one, you can apply for an OpenAI API key at [platform.openai.com/api-keys](https://platform.openai.com/api-keys). 
 
 ## Installation
 To install in python, simply do the following: 
 ```bash
```

### Comparing `autothemegenerator-0.1.0/setup.py` & `autothemegenerator-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 readme_path = os.path.join(here, "README.md")
 with codecs.open(readme_path, encoding="utf-8") as fh:
     long_description = fh.read()
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Performing thematic analysis with OpenAI\'s GPT-4 models'
 LONG_DESCRIPTION = 'A package uses openAI\'s GPT-4 model to perform thematic analysis using interview transcripts from qualititative studies'
 
 # Setting up
 setup(
     name="AutoThemeGenerator",
     version=VERSION,
```

