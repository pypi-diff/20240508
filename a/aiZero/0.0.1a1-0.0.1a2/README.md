# Comparing `tmp/aiZero-0.0.1a1.tar.gz` & `tmp/aiZero-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiZero-0.0.1a1.tar", last modified: Tue May  7 07:27:53 2024, max compression
+gzip compressed data, was "aiZero-0.0.1a2.tar", last modified: Wed May  8 02:02:17 2024, max compression
```

## Comparing `aiZero-0.0.1a1.tar` & `aiZero-0.0.1a2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:27:53.611857 aiZero-0.0.1a1/
--rw-r--r--   0 emhang     (501) staff       (20)       71 2024-05-07 05:21:12.000000 aiZero-0.0.1a1/MANIFEST.in
--rw-r--r--   0 emhang     (501) staff       (20)     9594 2024-05-07 07:27:53.611724 aiZero-0.0.1a1/PKG-INFO
--rw-r--r--   0 emhang     (501) staff       (20)     9047 2024-05-07 07:27:48.000000 aiZero-0.0.1a1/README.md
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:27:53.607744 aiZero-0.0.1a1/aiZero/
--rw-r--r--   0 emhang     (501) staff       (20)    18346 2024-05-07 07:22:32.000000 aiZero-0.0.1a1/aiZero/__init__.py
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:27:53.607065 aiZero-0.0.1a1/aiZero/static/
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:27:53.608868 aiZero-0.0.1a1/aiZero/static/audios/
--rw-r--r--   0 emhang     (501) staff       (20)   276040 2024-05-07 07:22:42.000000 aiZero-0.0.1a1/aiZero/static/audios/1a32d899-90f3-46e7-a26c-7a744b1516a7.wav
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:27:53.610754 aiZero-0.0.1a1/aiZero/static/js/
--rw-r--r--   0 emhang     (501) staff       (20)    35418 2024-04-10 09:16:03.000000 aiZero-0.0.1a1/aiZero/static/js/marked.min.js
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:27:53.611287 aiZero-0.0.1a1/aiZero/templates/
--rw-r--r--   0 emhang     (501) staff       (20)    28097 2024-04-17 06:07:29.000000 aiZero-0.0.1a1/aiZero/templates/index.html
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:27:53.608721 aiZero-0.0.1a1/aiZero.egg-info/
--rw-r--r--   0 emhang     (501) staff       (20)     9594 2024-05-07 07:27:53.000000 aiZero-0.0.1a1/aiZero.egg-info/PKG-INFO
--rw-r--r--   0 emhang     (501) staff       (20)      319 2024-05-07 07:27:53.000000 aiZero-0.0.1a1/aiZero.egg-info/SOURCES.txt
--rw-r--r--   0 emhang     (501) staff       (20)        1 2024-05-07 07:27:53.000000 aiZero-0.0.1a1/aiZero.egg-info/dependency_links.txt
--rw-r--r--   0 emhang     (501) staff       (20)       48 2024-05-07 07:27:53.000000 aiZero-0.0.1a1/aiZero.egg-info/requires.txt
--rw-r--r--   0 emhang     (501) staff       (20)        7 2024-05-07 07:27:53.000000 aiZero-0.0.1a1/aiZero.egg-info/top_level.txt
--rw-r--r--   0 emhang     (501) staff       (20)       38 2024-05-07 07:27:53.611906 aiZero-0.0.1a1/setup.cfg
--rw-r--r--   0 emhang     (501) staff       (20)      828 2024-05-07 07:27:34.000000 aiZero-0.0.1a1/setup.py
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-08 02:02:17.361850 aiZero-0.0.1a2/
+-rw-r--r--   0 emhang     (501) staff       (20)       71 2024-05-07 05:21:12.000000 aiZero-0.0.1a2/MANIFEST.in
+-rw-r--r--   0 emhang     (501) staff       (20)     9594 2024-05-08 02:02:17.361704 aiZero-0.0.1a2/PKG-INFO
+-rw-r--r--   0 emhang     (501) staff       (20)     9047 2024-05-07 07:27:48.000000 aiZero-0.0.1a2/README.md
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-08 02:02:17.358474 aiZero-0.0.1a2/aiZero/
+-rw-r--r--   0 emhang     (501) staff       (20)    18346 2024-05-07 07:22:32.000000 aiZero-0.0.1a2/aiZero/__init__.py
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-08 02:02:17.357761 aiZero-0.0.1a2/aiZero/static/
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-08 02:02:17.359614 aiZero-0.0.1a2/aiZero/static/audios/
+-rw-r--r--   0 emhang     (501) staff       (20)   276040 2024-05-07 07:22:42.000000 aiZero-0.0.1a2/aiZero/static/audios/1a32d899-90f3-46e7-a26c-7a744b1516a7.wav
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-08 02:02:17.360895 aiZero-0.0.1a2/aiZero/static/js/
+-rw-r--r--   0 emhang     (501) staff       (20)    35418 2024-04-10 09:16:03.000000 aiZero-0.0.1a2/aiZero/static/js/marked.min.js
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-08 02:02:17.361273 aiZero-0.0.1a2/aiZero/templates/
+-rw-r--r--   0 emhang     (501) staff       (20)    28097 2024-04-17 06:07:29.000000 aiZero-0.0.1a2/aiZero/templates/index.html
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-08 02:02:17.359486 aiZero-0.0.1a2/aiZero.egg-info/
+-rw-r--r--   0 emhang     (501) staff       (20)     9594 2024-05-08 02:02:17.000000 aiZero-0.0.1a2/aiZero.egg-info/PKG-INFO
+-rw-r--r--   0 emhang     (501) staff       (20)      319 2024-05-08 02:02:17.000000 aiZero-0.0.1a2/aiZero.egg-info/SOURCES.txt
+-rw-r--r--   0 emhang     (501) staff       (20)        1 2024-05-08 02:02:17.000000 aiZero-0.0.1a2/aiZero.egg-info/dependency_links.txt
+-rw-r--r--   0 emhang     (501) staff       (20)       40 2024-05-08 02:02:17.000000 aiZero-0.0.1a2/aiZero.egg-info/requires.txt
+-rw-r--r--   0 emhang     (501) staff       (20)        7 2024-05-08 02:02:17.000000 aiZero-0.0.1a2/aiZero.egg-info/top_level.txt
+-rw-r--r--   0 emhang     (501) staff       (20)       38 2024-05-08 02:02:17.361892 aiZero-0.0.1a2/setup.cfg
+-rw-r--r--   0 emhang     (501) staff       (20)      820 2024-05-08 02:02:02.000000 aiZero-0.0.1a2/setup.py
```

### Comparing `aiZero-0.0.1a1/PKG-INFO` & `aiZero-0.0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiZero
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A simple and easy-to-use library that connects to common artificial intelligence interfaces, allowing for quick development of local web applications. It includes mainstream AI capabilities such as LLM text interaction, image understanding, audio understanding, image generation, speech recognition, and speech synthesis.
 Home-page: UNKNOWN
 Author: emhang
 Author-email: emhang@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `aiZero-0.0.1a1/README.md` & `aiZero-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `aiZero-0.0.1a1/aiZero/__init__.py` & `aiZero-0.0.1a2/aiZero/__init__.py`

 * *Files identical despite different names*

### Comparing `aiZero-0.0.1a1/aiZero/static/audios/1a32d899-90f3-46e7-a26c-7a744b1516a7.wav` & `aiZero-0.0.1a2/aiZero/static/audios/1a32d899-90f3-46e7-a26c-7a744b1516a7.wav`

 * *Files identical despite different names*

### Comparing `aiZero-0.0.1a1/aiZero/static/js/marked.min.js` & `aiZero-0.0.1a2/aiZero/static/js/marked.min.js`

 * *Files identical despite different names*

### Comparing `aiZero-0.0.1a1/aiZero/templates/index.html` & `aiZero-0.0.1a2/aiZero/templates/index.html`

 * *Files identical despite different names*

### Comparing `aiZero-0.0.1a1/aiZero.egg-info/PKG-INFO` & `aiZero-0.0.1a2/aiZero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiZero
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A simple and easy-to-use library that connects to common artificial intelligence interfaces, allowing for quick development of local web applications. It includes mainstream AI capabilities such as LLM text interaction, image understanding, audio understanding, image generation, speech recognition, and speech synthesis.
 Home-page: UNKNOWN
 Author: emhang
 Author-email: emhang@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `aiZero-0.0.1a1/setup.py` & `aiZero-0.0.1a2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aiZero",
-    version="0.0.1a1",
+    version="0.0.1a2",
     author="emhang",
     author_email="emhang@126.com",
     description="A simple and easy-to-use library that connects to common artificial intelligence interfaces, "
                 "allowing for quick development of local web applications. "
                 "It includes mainstream AI capabilities such as LLM text interaction, image understanding, audio understanding, image generation, speech recognition, and speech synthesis.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
     python_requires='>=3.6',
     install_requires=[
         "flask>=3.0.0",
-        "requests>=2.82.2",
+        "requests",
         "dashscope==1.13.6"
     ]
 )
```

