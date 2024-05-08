# Comparing `tmp/supersullytools-2.5.1.tar.gz` & `tmp/supersullytools-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supersullytools-2.5.1.tar", last modified: Tue May  7 18:03:05 2024, max compression
+gzip compressed data, was "supersullytools-2.5.2.tar", last modified: Tue May  7 18:07:27 2024, max compression
```

## Comparing `supersullytools-2.5.1.tar` & `supersullytools-2.5.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:03:05.522385 supersullytools-2.5.1/
--rw-r--r--   0 msull      (501) staff       (20)     1092 2023-11-08 05:22:30.000000 supersullytools-2.5.1/LICENSE
--rw-r--r--   0 msull      (501) staff       (20)     3185 2024-05-07 18:03:05.521978 supersullytools-2.5.1/PKG-INFO
--rw-r--r--   0 msull      (501) staff       (20)      297 2024-05-07 18:03:02.000000 supersullytools-2.5.1/README.md
--rw-r--r--   0 msull      (501) staff       (20)     2064 2024-05-07 18:03:02.000000 supersullytools-2.5.1/pyproject.toml
--rw-r--r--   0 msull      (501) staff       (20)       38 2024-05-07 18:03:05.522474 supersullytools-2.5.1/setup.cfg
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:03:05.509782 supersullytools-2.5.1/src/
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:03:05.511203 supersullytools-2.5.1/src/streamlit_app/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-30 16:56:26.000000 supersullytools-2.5.1/src/streamlit_app/Home.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:03:05.511893 supersullytools-2.5.1/src/streamlit_app/pages/
--rw-r--r--   0 msull      (501) staff       (20)     3497 2024-02-16 00:42:29.000000 supersullytools-2.5.1/src/streamlit_app/pages/AI Chat.py
--rw-r--r--   0 msull      (501) staff       (20)     1328 2024-02-15 00:27:25.000000 supersullytools-2.5.1/src/streamlit_app/pages/Item Paginator.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:03:05.512217 supersullytools-2.5.1/src/supersullytools/
--rw-r--r--   0 msull      (501) staff       (20)       26 2024-05-07 18:03:02.000000 supersullytools-2.5.1/src/supersullytools/__init__.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:03:05.514135 supersullytools-2.5.1/src/supersullytools/llm/
--rw-r--r--   0 msull      (501) staff       (20)        0 2024-05-06 20:11:38.000000 supersullytools-2.5.1/src/supersullytools/llm/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)    15063 2024-05-06 20:17:43.000000 supersullytools-2.5.1/src/supersullytools/llm/completions.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:03:05.514651 supersullytools-2.5.1/src/supersullytools/openai/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:46.000000 supersullytools-2.5.1/src/supersullytools/openai/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)     4329 2024-05-06 20:17:43.000000 supersullytools-2.5.1/src/supersullytools/openai/chat_session.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:03:05.515736 supersullytools-2.5.1/src/supersullytools/streamlit/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:34.000000 supersullytools-2.5.1/src/supersullytools/streamlit/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)      571 2024-03-21 19:38:09.000000 supersullytools-2.5.1/src/supersullytools/streamlit/misc.py
--rw-r--r--   0 msull      (501) staff       (20)     6115 2023-11-30 16:44:47.000000 supersullytools-2.5.1/src/supersullytools/streamlit/paginator.py
--rw-r--r--   0 msull      (501) staff       (20)    12606 2024-05-07 18:01:28.000000 supersullytools-2.5.1/src/supersullytools/streamlit/sessions.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:03:05.516771 supersullytools-2.5.1/src/supersullytools/utils/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 18:02:43.000000 supersullytools-2.5.1/src/supersullytools/utils/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)     7607 2024-05-06 23:02:18.000000 supersullytools-2.5.1/src/supersullytools/utils/fuzzy_search.py
--rw-r--r--   0 msull      (501) staff       (20)     1396 2024-02-15 22:47:53.000000 supersullytools-2.5.1/src/supersullytools/utils/misc.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:03:05.518798 supersullytools-2.5.1/src/supersullytools.egg-info/
--rw-r--r--   0 msull      (501) staff       (20)     3185 2024-05-07 18:03:05.000000 supersullytools-2.5.1/src/supersullytools.egg-info/PKG-INFO
--rw-r--r--   0 msull      (501) staff       (20)      906 2024-05-07 18:03:05.000000 supersullytools-2.5.1/src/supersullytools.egg-info/SOURCES.txt
--rw-r--r--   0 msull      (501) staff       (20)        1 2024-05-07 18:03:05.000000 supersullytools-2.5.1/src/supersullytools.egg-info/dependency_links.txt
--rw-r--r--   0 msull      (501) staff       (20)      289 2024-05-07 18:03:05.000000 supersullytools-2.5.1/src/supersullytools.egg-info/requires.txt
--rw-r--r--   0 msull      (501) staff       (20)       36 2024-05-07 18:03:05.000000 supersullytools-2.5.1/src/supersullytools.egg-info/top_level.txt
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:03:05.518436 supersullytools-2.5.1/src/tests/
--rw-r--r--   0 msull      (501) staff       (20)     5073 2024-05-06 20:18:38.000000 supersullytools-2.5.1/src/tests/conftest.py
--rw-r--r--   0 msull      (501) staff       (20)     4082 2024-05-06 22:59:37.000000 supersullytools-2.5.1/src/tests/test_fuzzy_search.py
--rw-r--r--   0 msull      (501) staff       (20)      795 2024-02-16 00:44:38.000000 supersullytools-2.5.1/src/tests/test_streamlit_session.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.226186 supersullytools-2.5.2/
+-rw-r--r--   0 msull      (501) staff       (20)     1092 2023-11-08 05:22:30.000000 supersullytools-2.5.2/LICENSE
+-rw-r--r--   0 msull      (501) staff       (20)     3185 2024-05-07 18:07:27.225614 supersullytools-2.5.2/PKG-INFO
+-rw-r--r--   0 msull      (501) staff       (20)      297 2024-05-07 18:07:24.000000 supersullytools-2.5.2/README.md
+-rw-r--r--   0 msull      (501) staff       (20)     2064 2024-05-07 18:07:24.000000 supersullytools-2.5.2/pyproject.toml
+-rw-r--r--   0 msull      (501) staff       (20)       38 2024-05-07 18:07:27.226302 supersullytools-2.5.2/setup.cfg
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.211516 supersullytools-2.5.2/src/
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.212907 supersullytools-2.5.2/src/streamlit_app/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-30 16:56:26.000000 supersullytools-2.5.2/src/streamlit_app/Home.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.213594 supersullytools-2.5.2/src/streamlit_app/pages/
+-rw-r--r--   0 msull      (501) staff       (20)     3497 2024-02-16 00:42:29.000000 supersullytools-2.5.2/src/streamlit_app/pages/AI Chat.py
+-rw-r--r--   0 msull      (501) staff       (20)     1328 2024-02-15 00:27:25.000000 supersullytools-2.5.2/src/streamlit_app/pages/Item Paginator.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.213966 supersullytools-2.5.2/src/supersullytools/
+-rw-r--r--   0 msull      (501) staff       (20)       26 2024-05-07 18:07:24.000000 supersullytools-2.5.2/src/supersullytools/__init__.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.216513 supersullytools-2.5.2/src/supersullytools/llm/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2024-05-06 20:11:38.000000 supersullytools-2.5.2/src/supersullytools/llm/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)    15063 2024-05-06 20:17:43.000000 supersullytools-2.5.2/src/supersullytools/llm/completions.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.217206 supersullytools-2.5.2/src/supersullytools/openai/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:46.000000 supersullytools-2.5.2/src/supersullytools/openai/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)     4329 2024-05-06 20:17:43.000000 supersullytools-2.5.2/src/supersullytools/openai/chat_session.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.218689 supersullytools-2.5.2/src/supersullytools/streamlit/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:34.000000 supersullytools-2.5.2/src/supersullytools/streamlit/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)      571 2024-03-21 19:38:09.000000 supersullytools-2.5.2/src/supersullytools/streamlit/misc.py
+-rw-r--r--   0 msull      (501) staff       (20)     6115 2023-11-30 16:44:47.000000 supersullytools-2.5.2/src/supersullytools/streamlit/paginator.py
+-rw-r--r--   0 msull      (501) staff       (20)    12742 2024-05-07 18:06:20.000000 supersullytools-2.5.2/src/supersullytools/streamlit/sessions.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.219771 supersullytools-2.5.2/src/supersullytools/utils/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 18:02:43.000000 supersullytools-2.5.2/src/supersullytools/utils/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)     7607 2024-05-06 23:02:18.000000 supersullytools-2.5.2/src/supersullytools/utils/fuzzy_search.py
+-rw-r--r--   0 msull      (501) staff       (20)     1396 2024-02-15 22:47:53.000000 supersullytools-2.5.2/src/supersullytools/utils/misc.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.221393 supersullytools-2.5.2/src/supersullytools.egg-info/
+-rw-r--r--   0 msull      (501) staff       (20)     3185 2024-05-07 18:07:27.000000 supersullytools-2.5.2/src/supersullytools.egg-info/PKG-INFO
+-rw-r--r--   0 msull      (501) staff       (20)      906 2024-05-07 18:07:27.000000 supersullytools-2.5.2/src/supersullytools.egg-info/SOURCES.txt
+-rw-r--r--   0 msull      (501) staff       (20)        1 2024-05-07 18:07:27.000000 supersullytools-2.5.2/src/supersullytools.egg-info/dependency_links.txt
+-rw-r--r--   0 msull      (501) staff       (20)      289 2024-05-07 18:07:27.000000 supersullytools-2.5.2/src/supersullytools.egg-info/requires.txt
+-rw-r--r--   0 msull      (501) staff       (20)       36 2024-05-07 18:07:27.000000 supersullytools-2.5.2/src/supersullytools.egg-info/top_level.txt
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-07 18:07:27.220909 supersullytools-2.5.2/src/tests/
+-rw-r--r--   0 msull      (501) staff       (20)     5073 2024-05-06 20:18:38.000000 supersullytools-2.5.2/src/tests/conftest.py
+-rw-r--r--   0 msull      (501) staff       (20)     4082 2024-05-06 22:59:37.000000 supersullytools-2.5.2/src/tests/test_fuzzy_search.py
+-rw-r--r--   0 msull      (501) staff       (20)      795 2024-02-16 00:44:38.000000 supersullytools-2.5.2/src/tests/test_streamlit_session.py
```

### Comparing `supersullytools-2.5.1/LICENSE` & `supersullytools-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.1/PKG-INFO` & `supersullytools-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supersullytools
-Version: 2.5.1
+Version: 2.5.2
 Summary: This is a Python package that brings together a suite of utilities and helpers across several domains of software development.
 Author-email: Sully <sully@sadburger.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -49,11 +49,11 @@
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 
 SuperSully Tools
 ================
 
-**Latest Version:** 2.5.1
+**Latest Version:** 2.5.2
 
 **SupersullyTools** is a Python package that brings together a suite of utilities and helpers across several domains of
 software development. My personal toolkit of things I want in every package I'm working on, compiled in one place.
```

### Comparing `supersullytools-2.5.1/pyproject.toml` & `supersullytools-2.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "supersullytools"
-version = "2.5.1"
+version = "2.5.2"
 description = "This is a Python package that brings together a suite of utilities and helpers across several domains of software development."
 readme = "README.md"
 authors = [{ name = "Sully", email = "sully@sadburger.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -62,15 +62,15 @@
 line-length = 120
 
 [tool.ruff]
 line-length = 120
 target-version = "py310"
 
 [tool.bumpver]
-current_version = "2.5.1"
+current_version = "2.5.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `supersullytools-2.5.1/src/streamlit_app/pages/AI Chat.py` & `supersullytools-2.5.2/src/streamlit_app/pages/AI Chat.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.1/src/streamlit_app/pages/Item Paginator.py` & `supersullytools-2.5.2/src/streamlit_app/pages/Item Paginator.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.1/src/supersullytools/llm/completions.py` & `supersullytools-2.5.2/src/supersullytools/llm/completions.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.1/src/supersullytools/openai/chat_session.py` & `supersullytools-2.5.2/src/supersullytools/openai/chat_session.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.1/src/supersullytools/streamlit/misc.py` & `supersullytools-2.5.2/src/supersullytools/streamlit/misc.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.1/src/supersullytools/streamlit/paginator.py` & `supersullytools-2.5.2/src/supersullytools/streamlit/paginator.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.1/src/supersullytools/streamlit/sessions.py` & `supersullytools-2.5.2/src/supersullytools/streamlit/sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,15 @@
                 match expiration:
                     case datetime():
                         expires_at = expiration.timestamp()
                     case timedelta():
                         expires_at = (datetime.utcnow() + expiration).timestamp()
                     case _:
                         raise ValueError("Invalid type for expiration")
+                expires_at = Decimal(str(expires_at).split(".")[0])
                 session = self.get_session_model()(expires_at=expires_at)
             else:
                 session = self.get_session_model()()
 
         session: StreamlitSessionBase
 
         if session.is_expired:
@@ -183,14 +184,15 @@
                 match expiration:
                     case datetime():
                         expires_at = expiration.timestamp()
                     case timedelta():
                         expires_at = (datetime.utcnow() + expiration).timestamp()
                     case _:
                         raise ValueError("Invalid type for expiration")
+                expires_at = Decimal(str(expires_at).split(".")[0])
                 session.expires_at = expires_at
         session.save_to_session_state()
         return session
 
     def clear_session_data(self):
         datakey = self.get_session_model().__name__
         st.session_state.pop(datakey, None)
```

### Comparing `supersullytools-2.5.1/src/supersullytools/utils/fuzzy_search.py` & `supersullytools-2.5.2/src/supersullytools/utils/fuzzy_search.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.1/src/supersullytools/utils/misc.py` & `supersullytools-2.5.2/src/supersullytools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.1/src/supersullytools.egg-info/PKG-INFO` & `supersullytools-2.5.2/src/supersullytools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supersullytools
-Version: 2.5.1
+Version: 2.5.2
 Summary: This is a Python package that brings together a suite of utilities and helpers across several domains of software development.
 Author-email: Sully <sully@sadburger.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -49,11 +49,11 @@
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 
 SuperSully Tools
 ================
 
-**Latest Version:** 2.5.1
+**Latest Version:** 2.5.2
 
 **SupersullyTools** is a Python package that brings together a suite of utilities and helpers across several domains of
 software development. My personal toolkit of things I want in every package I'm working on, compiled in one place.
```

### Comparing `supersullytools-2.5.1/src/supersullytools.egg-info/SOURCES.txt` & `supersullytools-2.5.2/src/supersullytools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.1/src/tests/conftest.py` & `supersullytools-2.5.2/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.1/src/tests/test_fuzzy_search.py` & `supersullytools-2.5.2/src/tests/test_fuzzy_search.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.1/src/tests/test_streamlit_session.py` & `supersullytools-2.5.2/src/tests/test_streamlit_session.py`

 * *Files identical despite different names*

