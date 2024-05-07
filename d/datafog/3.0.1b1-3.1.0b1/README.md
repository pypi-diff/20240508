# Comparing `tmp/datafog-3.0.1b1.tar.gz` & `tmp/datafog-3.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.0.1b1.tar", last modified: Mon May  6 17:48:55 2024, max compression
+gzip compressed data, was "datafog-3.1.0b1.tar", last modified: Tue May  7 23:49:31 2024, max compression
```

## Comparing `datafog-3.0.1b1.tar` & `datafog-3.1.0b1.tar`

### file list

```diff
@@ -1,24 +1,12 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-06 17:48:55.022077 datafog-3.0.1b1/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-06 15:35:25.000000 datafog-3.0.1b1/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     7843 2024-05-06 17:48:55.021793 datafog-3.0.1b1/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     6349 2024-05-06 15:35:48.000000 datafog-3.0.1b1/README.md
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-06 17:48:55.022127 datafog-3.0.1b1/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1792 2024-05-06 17:48:48.000000 datafog-3.0.1b1/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-06 17:48:55.016617 datafog-3.0.1b1/src/
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-06 17:48:55.019067 datafog-3.0.1b1/src/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       22 2024-05-06 17:46:59.000000 datafog-3.0.1b1/src/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      436 2024-05-06 15:51:40.000000 datafog-3.0.1b1/src/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1273 2024-05-06 15:35:48.000000 datafog-3.0.1b1/src/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     4324 2024-05-06 15:35:48.000000 datafog-3.0.1b1/src/datafog/donuttransformer.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     3017 2024-05-06 15:51:40.000000 datafog-3.0.1b1/src/datafog/main.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1709 2024-05-06 15:35:48.000000 datafog-3.0.1b1/src/datafog/pii_annotation.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-06 17:48:55.021420 datafog-3.0.1b1/src/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     7843 2024-05-06 17:48:54.000000 datafog-3.0.1b1/src/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      434 2024-05-06 17:48:54.000000 datafog-3.0.1b1/src/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-06 17:48:54.000000 datafog-3.0.1b1/src/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      128 2024-05-06 17:48:54.000000 datafog-3.0.1b1/src/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-05-06 17:48:54.000000 datafog-3.0.1b1/src/datafog.egg-info/top_level.txt
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-06 17:48:55.021051 datafog-3.0.1b1/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1217 2024-05-06 15:35:49.000000 datafog-3.0.1b1/tests/test_donuttransformer.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1978 2024-05-06 15:35:49.000000 datafog-3.0.1b1/tests/test_main.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1926 2024-05-06 15:51:40.000000 datafog-3.0.1b1/tests/test_textpiiannotator.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-07 23:49:31.418947 datafog-3.1.0b1/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-06 15:35:25.000000 datafog-3.1.0b1/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6034 2024-05-07 23:49:31.418827 datafog-3.1.0b1/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     4813 2024-05-06 18:39:55.000000 datafog-3.1.0b1/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-07 23:49:31.418620 datafog-3.1.0b1/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6034 2024-05-07 23:49:31.000000 datafog-3.1.0b1/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      180 2024-05-07 23:49:31.000000 datafog-3.1.0b1/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-07 23:49:31.000000 datafog-3.1.0b1/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      165 2024-05-07 23:49:31.000000 datafog-3.1.0b1/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-07 23:49:31.000000 datafog-3.1.0b1/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-07 23:49:31.418994 datafog-3.1.0b1/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1829 2024-05-07 23:33:52.000000 datafog-3.1.0b1/setup.py
```

### Comparing `datafog-3.0.1b1/LICENSE` & `datafog-3.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.0.1b1/PKG-INFO` & `datafog-3.1.0b1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,37 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.0.1b1
+Version: 3.1.0b1
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
 Project-URL: Homepage, https://datafog.ai
 Project-URL: Documentation, https://docs.datafog.ai
 Project-URL: Discord, https://discord.gg/bzDth394R4
 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python
 Keywords: pii,redaction,nlp,rag,retrieval augmented generation
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: tox
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas==2.2.2
-Requires-Dist: Requests==2.31.0
-Requires-Dist: spacy==3.4.4
-Requires-Dist: en_spacy_pii_fast
-Requires-Dist: transformers
-Requires-Dist: torch
-Requires-Dist: pyspark
-Requires-Dist: pydantic
-Requires-Dist: Pillow
-Requires-Dist: sentencepiece
-Requires-Dist: protobuf
 
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
@@ -103,55 +93,18 @@
 
 DataFog can be installed via pip:
 
 ```bash
 pip install datafog
 ```
 
-and in your python environment:
-
-```
-from datafog import PresidioEngine as presidio
-datafog = datafog.DataFog()
-
-```
-
-## Examples
-
-Here are some examples of datafog being used to redact information in business contexts. Please see '/examples' for our [Getting Started](examples/getting-started.ipynb) notebook. We'll be regularly updating content and providing comprehensive guides to using DataFog in production contexts. If you have any ideas for a tutorial or guide that you would like to see, please let us know!
-
-### Scanning a single string
-
-```
-  ceo_email_chunk = "I'm announcing on Friday that Jeff is going to be CTO."
-
-  scan_results1 = presidio.scan(ceo_email_chunk)
-  print("PII Detected - base case:", scan_results1)
-  # PII Detected - base case: [type: PERSON, start: 30, end: 34, score: 0.85]
+## Examples - Updated for v3
 
+Check out for examples to get started with datafog v3: https://colab.research.google.com/drive/1k3HPaOTur3iDfBdWXh7O_EjzsjI_K6wT#scrollTo=WNtUZ497_0kd
 
-  scan_results2 = presidio.scan(ceo_email_chunk, deny_list=['CTO'])
-  print("PII Detected with deny list:", scan_results2)
-  # PII Detected with deny list: [type: CUSTOM_PII, start: 50, end: 53, score: 1.0, type: PERSON, start: 30, end: 34, score: 0.85]
-
-```
-
-### Scanning a list of PDFs
-
-```
-file_dir = ["/Users/sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/agi-builder-meetup.pdf",
-           "/Users/sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/pypdf-readthedocs-io-en-stable.pdf"]
-datafog = datafog.DataFog()
-result = datafog.upload_files(uploaded_files=file_dir)
-print(result)
-```
-
-The output here will be a dictionary where the keys are the file names and the values are the scan results for that file.
-for ex:
-`{'agi-builder-meetup.pdf': "2/26/24, 2:16 PM\nAGI Builders Meetup SF · Luma\nContact the HostReport Event29\nEvent FullIf youʼd like"}`
 
 ## Contributing
 
 DataFog is a community-driven **open-source** platform and we've been fortunate to have a small and growing contributor base. We'd love to hear ideas, feedback, suggestions for improvement - anything on your mind about what you think can be done to make DataFog better! Join our [Discord](https://discord.gg/bzDth394R4) and join our growing community.
 
 ### Dev Notes
 
@@ -169,7 +122,9 @@
 
 ```
 
 ## License
 
 This software is published under the [MIT
 license](https://en.wikipedia.org/wiki/MIT_License).
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,27 +1,24 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.0.1b1 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.1.0b1 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
-pii,redaction,nlp,rag,retrieval augmented generation Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Framework :: tox Classifier: Framework :: Pytest
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Science/Research Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pandas==2.2.2 Requires-Dist: Requests==2.31.0 Requires-Dist: spacy==3.4.4
-Requires-Dist: en_spacy_pii_fast Requires-Dist: transformers Requires-Dist:
-torch Requires-Dist: pyspark Requires-Dist: pydantic Requires-Dist: Pillow
-Requires-Dist: sentencepiece Requires-Dist: protobuf
+pii,redaction,nlp,rag,retrieval augmented generation Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Framework :: tox
+Classifier: Framework :: Pytest Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: Information Technology Classifier: Intended Audience :: System
+Administrators Requires-Python: >=3.10 Description-Content-Type: text/markdown
+License-File: LICENSE
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
@@ -49,39 +46,19 @@
 needs of the open-source community as they tackle this challenge. ### Roadmap
 DataFog is an active project with regular weekly releases to production
 (typically on/around Monday evenings US PT). Here's a snapshot of our coming
 roadmap; if you have questions or would like to weigh in, join our discord and
 let us know what we can do to make the product better! ![image](https://
 github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-
 0cc99de2ba92) ## Installation DataFog can be installed via pip: ```bash pip
-install datafog ``` and in your python environment: ``` from datafog import
-PresidioEngine as presidio datafog = datafog.DataFog() ``` ## Examples Here are
-some examples of datafog being used to redact information in business contexts.
-Please see '/examples' for our [Getting Started](examples/getting-
-started.ipynb) notebook. We'll be regularly updating content and providing
-comprehensive guides to using DataFog in production contexts. If you have any
-ideas for a tutorial or guide that you would like to see, please let us know!
-### Scanning a single string ``` ceo_email_chunk = "I'm announcing on Friday
-that Jeff is going to be CTO." scan_results1 = presidio.scan(ceo_email_chunk)
-print("PII Detected - base case:", scan_results1) # PII Detected - base case:
-[type: PERSON, start: 30, end: 34, score: 0.85] scan_results2 = presidio.scan
-(ceo_email_chunk, deny_list=['CTO']) print("PII Detected with deny list:",
-scan_results2) # PII Detected with deny list: [type: CUSTOM_PII, start: 50,
-end: 53, score: 1.0, type: PERSON, start: 30, end: 34, score: 0.85] ``` ###
-Scanning a list of PDFs ``` file_dir = ["/Users/sidmohan/Desktop/datafog-
-v2.4.0/datafog-python/tests/files/input_files/agi-builder-meetup.pdf", "/Users/
-sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/pypdf-
-readthedocs-io-en-stable.pdf"] datafog = datafog.DataFog() result =
-datafog.upload_files(uploaded_files=file_dir) print(result) ``` The output here
-will be a dictionary where the keys are the file names and the values are the
-scan results for that file. for ex: `{'agi-builder-meetup.pdf': "2/26/24, 2:16
-PM\nAGI Builders Meetup SF Â· Luma\nContact the HostReport Event29\nEvent
-FullIf youÊ¼d like"}` ## Contributing DataFog is a community-driven **open-
-source** platform and we've been fortunate to have a small and growing
-contributor base. We'd love to hear ideas, feedback, suggestions for
-improvement - anything on your mind about what you think can be done to make
-DataFog better! Join our [Discord](https://discord.gg/bzDth394R4) and join our
-growing community. ### Dev Notes - Justfile commands: - `just format` to apply
-formatting. - `just lint` to check formatting and style. ### Testing To run the
-datafog unit tests, check out this repository and do ``` tox ``` ## License
-This software is published under the [MIT license](https://en.wikipedia.org/
-wiki/MIT_License).
+install datafog ``` ## Examples - Updated for v3 Check out for examples to get
+started with datafog v3: https://colab.research.google.com/drive/
+1k3HPaOTur3iDfBdWXh7O_EjzsjI_K6wT#scrollTo=WNtUZ497_0kd ## Contributing DataFog
+is a community-driven **open-source** platform and we've been fortunate to have
+a small and growing contributor base. We'd love to hear ideas, feedback,
+suggestions for improvement - anything on your mind about what you think can be
+done to make DataFog better! Join our [Discord](https://discord.gg/bzDth394R4)
+and join our growing community. ### Dev Notes - Justfile commands: - `just
+format` to apply formatting. - `just lint` to check formatting and style. ###
+Testing To run the datafog unit tests, check out this repository and do ``` tox
+``` ## License This software is published under the [MIT license](https://
+en.wikipedia.org/wiki/MIT_License).
```

### Comparing `datafog-3.0.1b1/README.md` & `datafog-3.1.0b1/datafog.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+Metadata-Version: 2.1
+Name: datafog
+Version: 3.1.0b1
+Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
+Home-page: https://datafog.ai
+Author: DataFog
+Author-email: hi@datafog.ai
+Maintainer: DataFog
+Maintainer-email: hi@datafog.ai
+License: MIT
+Project-URL: Homepage, https://datafog.ai
+Project-URL: Documentation, https://docs.datafog.ai
+Project-URL: Discord, https://discord.gg/bzDth394R4
+Project-URL: Twitter, https://twitter.com/datafoginc
+Project-URL: GitHub, https://github.com/datafog/datafog-python
+Keywords: pii,redaction,nlp,rag,retrieval augmented generation
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: tox
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
 </p>
@@ -62,55 +93,18 @@
 
 DataFog can be installed via pip:
 
 ```bash
 pip install datafog
 ```
 
-and in your python environment:
-
-```
-from datafog import PresidioEngine as presidio
-datafog = datafog.DataFog()
-
-```
-
-## Examples
-
-Here are some examples of datafog being used to redact information in business contexts. Please see '/examples' for our [Getting Started](examples/getting-started.ipynb) notebook. We'll be regularly updating content and providing comprehensive guides to using DataFog in production contexts. If you have any ideas for a tutorial or guide that you would like to see, please let us know!
-
-### Scanning a single string
-
-```
-  ceo_email_chunk = "I'm announcing on Friday that Jeff is going to be CTO."
-
-  scan_results1 = presidio.scan(ceo_email_chunk)
-  print("PII Detected - base case:", scan_results1)
-  # PII Detected - base case: [type: PERSON, start: 30, end: 34, score: 0.85]
-
-
-  scan_results2 = presidio.scan(ceo_email_chunk, deny_list=['CTO'])
-  print("PII Detected with deny list:", scan_results2)
-  # PII Detected with deny list: [type: CUSTOM_PII, start: 50, end: 53, score: 1.0, type: PERSON, start: 30, end: 34, score: 0.85]
-
-```
-
-### Scanning a list of PDFs
+## Examples - Updated for v3
 
-```
-file_dir = ["/Users/sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/agi-builder-meetup.pdf",
-           "/Users/sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/pypdf-readthedocs-io-en-stable.pdf"]
-datafog = datafog.DataFog()
-result = datafog.upload_files(uploaded_files=file_dir)
-print(result)
-```
+Check out for examples to get started with datafog v3: https://colab.research.google.com/drive/1k3HPaOTur3iDfBdWXh7O_EjzsjI_K6wT#scrollTo=WNtUZ497_0kd
 
-The output here will be a dictionary where the keys are the file names and the values are the scan results for that file.
-for ex:
-`{'agi-builder-meetup.pdf': "2/26/24, 2:16 PM\nAGI Builders Meetup SF · Luma\nContact the HostReport Event29\nEvent FullIf youʼd like"}`
 
 ## Contributing
 
 DataFog is a community-driven **open-source** platform and we've been fortunate to have a small and growing contributor base. We'd love to hear ideas, feedback, suggestions for improvement - anything on your mind about what you think can be done to make DataFog better! Join our [Discord](https://discord.gg/bzDth394R4) and join our growing community.
 
 ### Dev Notes
 
@@ -128,7 +122,9 @@
 
 ```
 
 ## License
 
 This software is published under the [MIT
 license](https://en.wikipedia.org/wiki/MIT_License).
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1 Name: datafog Version: 3.1.0b1 Summary: Scan, redact, and
+manage PII in your documents before they get uploaded to a Retrieval Augmented
+Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
+email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
+License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
+Documentation, https://docs.datafog.ai Project-URL: Discord, https://
+discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
+Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
+pii,redaction,nlp,rag,retrieval augmented generation Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Framework :: tox
+Classifier: Framework :: Pytest Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
+:: Information Technology Classifier: Intended Audience :: System
+Administrators Requires-Python: >=3.10 Description-Content-Type: text/markdown
+License-File: LICENSE
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
@@ -29,39 +46,19 @@
 needs of the open-source community as they tackle this challenge. ### Roadmap
 DataFog is an active project with regular weekly releases to production
 (typically on/around Monday evenings US PT). Here's a snapshot of our coming
 roadmap; if you have questions or would like to weigh in, join our discord and
 let us know what we can do to make the product better! ![image](https://
 github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-
 0cc99de2ba92) ## Installation DataFog can be installed via pip: ```bash pip
-install datafog ``` and in your python environment: ``` from datafog import
-PresidioEngine as presidio datafog = datafog.DataFog() ``` ## Examples Here are
-some examples of datafog being used to redact information in business contexts.
-Please see '/examples' for our [Getting Started](examples/getting-
-started.ipynb) notebook. We'll be regularly updating content and providing
-comprehensive guides to using DataFog in production contexts. If you have any
-ideas for a tutorial or guide that you would like to see, please let us know!
-### Scanning a single string ``` ceo_email_chunk = "I'm announcing on Friday
-that Jeff is going to be CTO." scan_results1 = presidio.scan(ceo_email_chunk)
-print("PII Detected - base case:", scan_results1) # PII Detected - base case:
-[type: PERSON, start: 30, end: 34, score: 0.85] scan_results2 = presidio.scan
-(ceo_email_chunk, deny_list=['CTO']) print("PII Detected with deny list:",
-scan_results2) # PII Detected with deny list: [type: CUSTOM_PII, start: 50,
-end: 53, score: 1.0, type: PERSON, start: 30, end: 34, score: 0.85] ``` ###
-Scanning a list of PDFs ``` file_dir = ["/Users/sidmohan/Desktop/datafog-
-v2.4.0/datafog-python/tests/files/input_files/agi-builder-meetup.pdf", "/Users/
-sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/pypdf-
-readthedocs-io-en-stable.pdf"] datafog = datafog.DataFog() result =
-datafog.upload_files(uploaded_files=file_dir) print(result) ``` The output here
-will be a dictionary where the keys are the file names and the values are the
-scan results for that file. for ex: `{'agi-builder-meetup.pdf': "2/26/24, 2:16
-PM\nAGI Builders Meetup SF Â· Luma\nContact the HostReport Event29\nEvent
-FullIf youÊ¼d like"}` ## Contributing DataFog is a community-driven **open-
-source** platform and we've been fortunate to have a small and growing
-contributor base. We'd love to hear ideas, feedback, suggestions for
-improvement - anything on your mind about what you think can be done to make
-DataFog better! Join our [Discord](https://discord.gg/bzDth394R4) and join our
-growing community. ### Dev Notes - Justfile commands: - `just format` to apply
-formatting. - `just lint` to check formatting and style. ### Testing To run the
-datafog unit tests, check out this repository and do ``` tox ``` ## License
-This software is published under the [MIT license](https://en.wikipedia.org/
-wiki/MIT_License).
+install datafog ``` ## Examples - Updated for v3 Check out for examples to get
+started with datafog v3: https://colab.research.google.com/drive/
+1k3HPaOTur3iDfBdWXh7O_EjzsjI_K6wT#scrollTo=WNtUZ497_0kd ## Contributing DataFog
+is a community-driven **open-source** platform and we've been fortunate to have
+a small and growing contributor base. We'd love to hear ideas, feedback,
+suggestions for improvement - anything on your mind about what you think can be
+done to make DataFog better! Join our [Discord](https://discord.gg/bzDth394R4)
+and join our growing community. ### Dev Notes - Justfile commands: - `just
+format` to apply formatting. - `just lint` to check formatting and style. ###
+Testing To run the datafog unit tests, check out this repository and do ``` tox
+``` ## License This software is published under the [MIT license](https://
+en.wikipedia.org/wiki/MIT_License).
```

### Comparing `datafog-3.0.1b1/setup.py` & `datafog-3.1.0b1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.0.1b1"
+    return "3.1.0b1"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
@@ -26,19 +26,19 @@
     description="Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "pandas==2.2.2",
         "Requests==2.31.0",
         "spacy==3.4.4",
-        "en_spacy_pii_fast",
-        "transformers",
-        "torch",
-        "pyspark",
-        "pydantic",
+        "en_spacy_pii_fast==0.0.0",
+        "transformers==4.40.1",
+        "torch==2.2.2",
+        "pyspark==3.4.1",
+        "pydantic==1.10.8",
         "Pillow",
         "sentencepiece",
         "protobuf",
     ],
     python_requires=">=3.10",
     classifiers=[
         "Programming Language :: Python :: 3.10",
```

