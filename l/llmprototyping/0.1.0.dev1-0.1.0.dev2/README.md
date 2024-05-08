# Comparing `tmp/llmprototyping-0.1.0.dev1.tar.gz` & `tmp/llmprototyping-0.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmprototyping-0.1.0.dev1.tar", last modified: Tue May  7 22:56:31 2024, max compression
+gzip compressed data, was "llmprototyping-0.1.0.dev2.tar", last modified: Tue May  7 23:17:42 2024, max compression
```

## Comparing `llmprototyping-0.1.0.dev1.tar` & `llmprototyping-0.1.0.dev2.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-07 22:56:31.891361 llmprototyping-0.1.0.dev1/
--rw-r--r--   0 alejandro   (501) staff       (20)    11357 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev1/LICENSE
--rw-r--r--   0 alejandro   (501) staff       (20)     1723 2024-05-07 22:56:31.891287 llmprototyping-0.1.0.dev1/PKG-INFO
--rw-r--r--   0 alejandro   (501) staff       (20)     1059 2024-05-07 22:56:12.000000 llmprototyping-0.1.0.dev1/README.md
--rw-r--r--   0 alejandro   (501) staff       (20)       74 2024-05-07 22:56:31.891578 llmprototyping-0.1.0.dev1/setup.cfg
--rw-r--r--   0 alejandro   (501) staff       (20)     1119 2024-05-07 22:51:08.000000 llmprototyping-0.1.0.dev1/setup.py
-drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-07 22:56:31.886356 llmprototyping-0.1.0.dev1/src/
-drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-07 22:56:31.889997 llmprototyping-0.1.0.dev1/src/llmprototyping/
--rw-r--r--   0 alejandro   (501) staff       (20)      543 2024-05-07 22:50:14.000000 llmprototyping-0.1.0.dev1/src/llmprototyping/__init__.py
--rw-r--r--   0 alejandro   (501) staff       (20)      684 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev1/src/llmprototyping/conversation.py
--rw-r--r--   0 alejandro   (501) staff       (20)     1919 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev1/src/llmprototyping/embeddings_interface.py
--rw-r--r--   0 alejandro   (501) staff       (20)     3150 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev1/src/llmprototyping/embeddings_openai.py
--rw-r--r--   0 alejandro   (501) staff       (20)     1163 2024-05-07 22:50:21.000000 llmprototyping-0.1.0.dev1/src/llmprototyping/error.py
--rw-r--r--   0 alejandro   (501) staff       (20)     1348 2024-05-07 22:50:24.000000 llmprototyping-0.1.0.dev1/src/llmprototyping/factory.py
--rw-r--r--   0 alejandro   (501) staff       (20)     3256 2024-05-07 22:50:30.000000 llmprototyping-0.1.0.dev1/src/llmprototyping/llm_groq.py
--rw-r--r--   0 alejandro   (501) staff       (20)     2834 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev1/src/llmprototyping/llm_interface.py
--rw-r--r--   0 alejandro   (501) staff       (20)     3634 2024-05-07 22:50:31.000000 llmprototyping-0.1.0.dev1/src/llmprototyping/llm_openai.py
--rw-r--r--   0 alejandro   (501) staff       (20)      434 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev1/src/llmprototyping/serializable.py
--rw-r--r--   0 alejandro   (501) staff       (20)     1930 2024-05-07 22:50:32.000000 llmprototyping-0.1.0.dev1/src/llmprototyping/vectordb.py
-drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-07 22:56:31.891034 llmprototyping-0.1.0.dev1/src/llmprototyping.egg-info/
--rw-r--r--   0 alejandro   (501) staff       (20)     1723 2024-05-07 22:56:31.000000 llmprototyping-0.1.0.dev1/src/llmprototyping.egg-info/PKG-INFO
--rw-r--r--   0 alejandro   (501) staff       (20)      618 2024-05-07 22:56:31.000000 llmprototyping-0.1.0.dev1/src/llmprototyping.egg-info/SOURCES.txt
--rw-r--r--   0 alejandro   (501) staff       (20)        1 2024-05-07 22:56:31.000000 llmprototyping-0.1.0.dev1/src/llmprototyping.egg-info/dependency_links.txt
--rw-r--r--   0 alejandro   (501) staff       (20)       41 2024-05-07 22:56:31.000000 llmprototyping-0.1.0.dev1/src/llmprototyping.egg-info/requires.txt
--rw-r--r--   0 alejandro   (501) staff       (20)       15 2024-05-07 22:56:31.000000 llmprototyping-0.1.0.dev1/src/llmprototyping.egg-info/top_level.txt
+drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-07 23:17:42.372852 llmprototyping-0.1.0.dev2/
+-rw-r--r--   0 alejandro   (501) staff       (20)    11357 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev2/LICENSE
+-rw-r--r--   0 alejandro   (501) staff       (20)     1730 2024-05-07 23:17:42.372792 llmprototyping-0.1.0.dev2/PKG-INFO
+-rw-r--r--   0 alejandro   (501) staff       (20)     1066 2024-05-07 23:08:48.000000 llmprototyping-0.1.0.dev2/README.md
+-rw-r--r--   0 alejandro   (501) staff       (20)       74 2024-05-07 23:17:42.373035 llmprototyping-0.1.0.dev2/setup.cfg
+-rw-r--r--   0 alejandro   (501) staff       (20)     1119 2024-05-07 23:12:11.000000 llmprototyping-0.1.0.dev2/setup.py
+drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-07 23:17:42.368697 llmprototyping-0.1.0.dev2/src/
+drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-07 23:17:42.371740 llmprototyping-0.1.0.dev2/src/llmprototyping/
+-rw-r--r--   0 alejandro   (501) staff       (20)      543 2024-05-07 22:50:14.000000 llmprototyping-0.1.0.dev2/src/llmprototyping/__init__.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     1919 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev2/src/llmprototyping/embeddings_interface.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     3150 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev2/src/llmprototyping/embeddings_openai.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     1163 2024-05-07 22:50:21.000000 llmprototyping-0.1.0.dev2/src/llmprototyping/error.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     1348 2024-05-07 22:50:24.000000 llmprototyping-0.1.0.dev2/src/llmprototyping/factory.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     3256 2024-05-07 22:50:30.000000 llmprototyping-0.1.0.dev2/src/llmprototyping/llm_groq.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     2834 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev2/src/llmprototyping/llm_interface.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     3634 2024-05-07 22:50:31.000000 llmprototyping-0.1.0.dev2/src/llmprototyping/llm_openai.py
+-rw-r--r--   0 alejandro   (501) staff       (20)      434 2024-05-07 22:37:54.000000 llmprototyping-0.1.0.dev2/src/llmprototyping/serializable.py
+-rw-r--r--   0 alejandro   (501) staff       (20)     1930 2024-05-07 22:50:32.000000 llmprototyping-0.1.0.dev2/src/llmprototyping/vectordb.py
+drwxr-xr-x   0 alejandro   (501) staff       (20)        0 2024-05-07 23:17:42.372588 llmprototyping-0.1.0.dev2/src/llmprototyping.egg-info/
+-rw-r--r--   0 alejandro   (501) staff       (20)     1730 2024-05-07 23:17:42.000000 llmprototyping-0.1.0.dev2/src/llmprototyping.egg-info/PKG-INFO
+-rw-r--r--   0 alejandro   (501) staff       (20)      583 2024-05-07 23:17:42.000000 llmprototyping-0.1.0.dev2/src/llmprototyping.egg-info/SOURCES.txt
+-rw-r--r--   0 alejandro   (501) staff       (20)        1 2024-05-07 23:17:42.000000 llmprototyping-0.1.0.dev2/src/llmprototyping.egg-info/dependency_links.txt
+-rw-r--r--   0 alejandro   (501) staff       (20)       41 2024-05-07 23:17:42.000000 llmprototyping-0.1.0.dev2/src/llmprototyping.egg-info/requires.txt
+-rw-r--r--   0 alejandro   (501) staff       (20)       15 2024-05-07 23:17:42.000000 llmprototyping-0.1.0.dev2/src/llmprototyping.egg-info/top_level.txt
```

### Comparing `llmprototyping-0.1.0.dev1/LICENSE` & `llmprototyping-0.1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev1/PKG-INFO` & `llmprototyping-0.1.0.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmprototyping
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: A simple set of tools to access llm apis
 Home-page: https://github.com/alejandrolc/llmprototyping
 Author: Alejandro López Correa
 Keywords: llm,rag,openai,groq
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -39,15 +39,16 @@
 
 ```bash
 pip install llmprototyping
 ```
 
 ## Usage
 
-```import os
+```python
+import os
 from dotenv import load_dotenv
 load_dotenv()
 
 groq_api_key = os.getenv('GROQ_API_KEY')
 
 import llmprototyping as llmp
 factory = llmp.LLMChatCompletionFactory
```

### Comparing `llmprototyping-0.1.0.dev1/README.md` & `llmprototyping-0.1.0.dev2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 ```bash
 pip install llmprototyping
 ```
 
 ## Usage
 
-```import os
+```python
+import os
 from dotenv import load_dotenv
 load_dotenv()
 
 groq_api_key = os.getenv('GROQ_API_KEY')
 
 import llmprototyping as llmp
 factory = llmp.LLMChatCompletionFactory
```

### Comparing `llmprototyping-0.1.0.dev1/setup.py` & `llmprototyping-0.1.0.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name="llmprototyping",
     # https://packaging.python.org/en/latest/discussions/versioning/
-    version="0.1.0.dev1",
+    version="0.1.0.dev2",
     description="A simple set of tools to access llm apis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alejandrolc/llmprototyping",
     author="Alejandro López Correa",
     #author_email="...",
     classifiers=[
```

### Comparing `llmprototyping-0.1.0.dev1/src/llmprototyping/__init__.py` & `llmprototyping-0.1.0.dev2/src/llmprototyping/__init__.py`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev1/src/llmprototyping/embeddings_interface.py` & `llmprototyping-0.1.0.dev2/src/llmprototyping/embeddings_interface.py`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev1/src/llmprototyping/embeddings_openai.py` & `llmprototyping-0.1.0.dev2/src/llmprototyping/embeddings_openai.py`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev1/src/llmprototyping/error.py` & `llmprototyping-0.1.0.dev2/src/llmprototyping/error.py`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev1/src/llmprototyping/factory.py` & `llmprototyping-0.1.0.dev2/src/llmprototyping/factory.py`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev1/src/llmprototyping/llm_groq.py` & `llmprototyping-0.1.0.dev2/src/llmprototyping/llm_groq.py`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev1/src/llmprototyping/llm_interface.py` & `llmprototyping-0.1.0.dev2/src/llmprototyping/llm_interface.py`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev1/src/llmprototyping/llm_openai.py` & `llmprototyping-0.1.0.dev2/src/llmprototyping/llm_openai.py`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev1/src/llmprototyping/vectordb.py` & `llmprototyping-0.1.0.dev2/src/llmprototyping/vectordb.py`

 * *Files identical despite different names*

### Comparing `llmprototyping-0.1.0.dev1/src/llmprototyping.egg-info/PKG-INFO` & `llmprototyping-0.1.0.dev2/src/llmprototyping.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmprototyping
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: A simple set of tools to access llm apis
 Home-page: https://github.com/alejandrolc/llmprototyping
 Author: Alejandro López Correa
 Keywords: llm,rag,openai,groq
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -39,15 +39,16 @@
 
 ```bash
 pip install llmprototyping
 ```
 
 ## Usage
 
-```import os
+```python
+import os
 from dotenv import load_dotenv
 load_dotenv()
 
 groq_api_key = os.getenv('GROQ_API_KEY')
 
 import llmprototyping as llmp
 factory = llmp.LLMChatCompletionFactory
```

### Comparing `llmprototyping-0.1.0.dev1/src/llmprototyping.egg-info/SOURCES.txt` & `llmprototyping-0.1.0.dev2/src/llmprototyping.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 src/llmprototyping/__init__.py
-src/llmprototyping/conversation.py
 src/llmprototyping/embeddings_interface.py
 src/llmprototyping/embeddings_openai.py
 src/llmprototyping/error.py
 src/llmprototyping/factory.py
 src/llmprototyping/llm_groq.py
 src/llmprototyping/llm_interface.py
 src/llmprototyping/llm_openai.py
```

