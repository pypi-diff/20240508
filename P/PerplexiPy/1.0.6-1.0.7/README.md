# Comparing `tmp/PerplexiPy-1.0.6-py3-none-any.whl.zip` & `tmp/PerplexiPy-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12541 bytes, number of entries: 10
--rw-r--r--  2.0 unx     9853 b- defN 24-May-05 02:03 perplexipy/__init__.py
--rw-r--r--  2.0 unx    13411 b- defN 24-May-05 02:08 perplexipy/codex.py
+Zip file size: 12557 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     9961 b- defN 24-May-08 14:30 perplexipy/__init__.py
+-rw-r--r--  2.0 unx    13411 b- defN 24-May-05 02:46 perplexipy/codex.py
 -rw-r--r--  2.0 unx      283 b- defN 24-Mar-01 20:13 perplexipy/errors.py
 -rw-r--r--  2.0 unx      684 b- defN 24-Apr-13 17:06 perplexipy/responses.py
--rw-r--r--  2.0 unx     1514 b- defN 24-May-05 02:11 PerplexiPy-1.0.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6968 b- defN 24-May-05 02:11 PerplexiPy-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-05 02:11 PerplexiPy-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-May-05 02:11 PerplexiPy-1.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-May-05 02:11 PerplexiPy-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      814 b- defN 24-May-05 02:11 PerplexiPy-1.0.6.dist-info/RECORD
-10 files, 33679 bytes uncompressed, 11149 bytes compressed:  66.9%
+-rw-r--r--  2.0 unx     1514 b- defN 24-May-08 14:31 PerplexiPy-1.0.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6968 b- defN 24-May-08 14:31 PerplexiPy-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 14:31 PerplexiPy-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-May-08 14:31 PerplexiPy-1.0.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-May-08 14:31 PerplexiPy-1.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      814 b- defN 24-May-08 14:31 PerplexiPy-1.0.7.dist-info/RECORD
+10 files, 33787 bytes uncompressed, 11165 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: perplexipy/errors.py
 Comment: 
 
 Filename: perplexipy/responses.py
 Comment: 
 
-Filename: PerplexiPy-1.0.6.dist-info/LICENSE.txt
+Filename: PerplexiPy-1.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.6.dist-info/METADATA
+Filename: PerplexiPy-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: PerplexiPy-1.0.6.dist-info/WHEEL
+Filename: PerplexiPy-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: PerplexiPy-1.0.6.dist-info/entry_points.txt
+Filename: PerplexiPy-1.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.6.dist-info/top_level.txt
+Filename: PerplexiPy-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.6.dist-info/RECORD
+Filename: PerplexiPy-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perplexipy/__init__.py

```diff
@@ -28,25 +28,22 @@
 
 load_dotenv()
 
 import os
 
 
 _CLAUDE_MODEL = 'claude-3-haiku'
+PERPLEXITY_API_KEY = os.environ.get('PERPLEXITY_API_KEY', default = '')
 """
 `PERPLEXITY_API_KEY` is set to the environment variable of the same name if
-present, otherwise it's set to the empty string `''`.
+present, otherwise it's set to the empty string `''`.  PerplexiPy uses the
+`dotenv` module to load environment settings from `$PWD/.env` if present.
 """
-PERPLEXITY_API_KEY = os.environ.get('PERPLEXITY_API_KEY', default = '')
 PERPLEXITY_API_PREFIX = 'pplx-'
 PERPLEXITY_API_URL = 'https://api.perplexity.ai'
-"""
-The default model is **mistral-7b-instruct** because of it's efficiency and
-performance qualities.  Ref:  https://arxiv.org/abs/2310.06825
-"""
 PERPLEXITY_DEFAULT_MODEL = 'llama-3-sonar-small-32k-chat'
 PERPLEXITY_DEFAULT_ROLE = 'user'
 PERPLEXITY_TIMEOUT = 30.0 # seconds
 PERPLEXITY_VALID_ROLES = { 'assistant', 'system', 'user', } # future proofing.
 
 
 """
@@ -94,15 +91,17 @@
             PerplexityClientError
         If the API key is empty, or doesn't match one of the valid API prefixes
         per the documentation.
         """
         if not key:
             raise PerplexityClientError('Provide a valid key argument during instantiation')
         if not PERPLEXITY_API_PREFIX in key:
-            raise PerplexityClientError('The key %s i missing the pplx- prefix - invalid API key')
+            raise PerplexityClientError('The key %s is missing the pplx- prefix - invalid API key' % key)
+        if not all(ord(' ') <= ord(c) <= ord('~') for c in key):
+            raise PerplexityClientError('The key %s contains invalid characters' % key)
 
         self._endpoint = endpoint
         self._key = key
         self._role = PERPLEXITY_DEFAULT_ROLE
         self._model = PERPLEXITY_DEFAULT_MODEL
         self._client = OpenAI(
             api_key = self._key,
```

## Comparing `PerplexiPy-1.0.6.dist-info/LICENSE.txt` & `PerplexiPy-1.0.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PerplexiPy-1.0.6.dist-info/METADATA` & `PerplexiPy-1.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PerplexiPy
-Version: 1.0.6
+Version: 1.0.7
 Summary: PerplexiPy - A robust Perplexity AI API client
 Author-email: CIME Software Ltd <perplexipy@cime.net>
 License: BSD-3
 Project-URL: homepage, https://cime-software.github.io/perplexipy/
 Project-URL: Documentation, https://cime-software.github.io/perplexipy/
 Project-URL: Bug Tracker, https://github.com/CIME-Software/perplexipy/issues
 Project-URL: Source, https://github.com/CIME-Software/perplexipy
@@ -22,15 +22,15 @@
 Requires-Dist: appdirs
 Requires-Dist: click
 Requires-Dist: openai (>=1.12.0)
 Requires-Dist: prompt-toolkit
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 
-% perplexipy(3) Version 1.0.6 | Perplexity AI high level API documentation
+% perplexipy(3) Version 1.0.7 | Perplexity AI high level API documentation
 
 Name
 ====
 
 **PerplexiPy** - Perplexity AI high level library
```

### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.6 Summary: PerplexiPy - A
+Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.7 Summary: PerplexiPy - A
 robust Perplexity AI API client Author-email: CIME Software Ltd
 cime.net> License: BSD-3 Project-URL: homepage, https://cime-
 software.github.io/perplexipy/ Project-URL: Documentation, https://cime-
 software.github.io/perplexipy/ Project-URL: Bug Tracker, https://github.com/
 CIME-Software/perplexipy/issues Project-URL: Source, https://github.com/CIME-
 Software/perplexipy Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: appdirs Requires-Dist: click Requires-Dist: openai
 (>=1.12.0) Requires-Dist: prompt-toolkit Requires-Dist: python-dotenv Requires-
-Dist: pyyaml % perplexipy(3) Version 1.0.6 | Perplexity AI high level API
+Dist: pyyaml % perplexipy(3) Version 1.0.7 | Perplexity AI high level API
 documentation Name ==== **PerplexiPy** - Perplexity AI high level library
 [https://images2.imgbox.com/57/94/AsI1WSfy_o.png]Synopsis ======== ```python
 client = PerplexityClient() \ print(client.query('What is the meaning of 42?')
 \ for result in client.queryStreamable('List of all US presidents'): \ print
 (result) ``` Description =========== **PerplexiPy** is a high-level,
 convenience library for interacting with the Perplexity API from any Python
 3.9+ application. The library aims to simplify interactions with Perplexity
```

## Comparing `PerplexiPy-1.0.6.dist-info/RECORD` & `PerplexiPy-1.0.7.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-perplexipy/__init__.py,sha256=7E09bh_YwfZHEQhIe6dWTJG28MHh1wl_57GOAa8_ws0,9853
+perplexipy/__init__.py,sha256=Kw2CPH3DHV8ukgVaWXOLjPWQe8Y0KOJIC0abJCU7oo8,9961
 perplexipy/codex.py,sha256=ZVTXxNkxACxtqkbn3yGd2f-xVx2jhdWWtZBbgQZL2H8,13411
 perplexipy/errors.py,sha256=YM4dVV9q2aLm_ZJdhyCjhejLXdo8mEffx93zlP_7lOs,283
 perplexipy/responses.py,sha256=1OrBpZxGHaVvlE5x9ZtdQhoXP5RbmKOXtHGt6Nm7g2I,684
-PerplexiPy-1.0.6.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
-PerplexiPy-1.0.6.dist-info/METADATA,sha256=WvRg-ifsD6yTpBZaQCvGuOXWNC-a73B-7Qr_u-1E0f4,6968
-PerplexiPy-1.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-PerplexiPy-1.0.6.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
-PerplexiPy-1.0.6.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
-PerplexiPy-1.0.6.dist-info/RECORD,,
+PerplexiPy-1.0.7.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
+PerplexiPy-1.0.7.dist-info/METADATA,sha256=b1QO73ooLp1OP-zK3CFlyy5dTrw-kuCC4DAwywfm7_s,6968
+PerplexiPy-1.0.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+PerplexiPy-1.0.7.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
+PerplexiPy-1.0.7.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
+PerplexiPy-1.0.7.dist-info/RECORD,,
```

