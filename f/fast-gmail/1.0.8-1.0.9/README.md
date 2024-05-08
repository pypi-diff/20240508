# Comparing `tmp/fast_gmail-1.0.8.tar.gz` & `tmp/fast_gmail-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_gmail-1.0.8.tar", last modified: Sat Apr 20 07:22:34 2024, max compression
+gzip compressed data, was "fast_gmail-1.0.9.tar", last modified: Wed May  8 13:01:40 2024, max compression
```

## Comparing `fast_gmail-1.0.8.tar` & `fast_gmail-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-20 07:22:34.665839 fast_gmail-1.0.8/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.0.8/LICENSE
--rw-r--r--   0 aleti     (1000) aleti     (1000)    15624 2024-04-20 07:22:34.665839 fast_gmail-1.0.8/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    14864 2024-04-20 07:12:16.000000 fast_gmail-1.0.8/README.md
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-20 07:22:34.665839 fast_gmail-1.0.8/fast_gmail/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       30 2024-04-15 08:44:02.000000 fast_gmail-1.0.8/fast_gmail/__init__.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.0.8/fast_gmail/draft.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    21980 2024-04-20 06:58:56.000000 fast_gmail-1.0.8/fast_gmail/gmail.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     7203 2024-04-19 12:04:22.000000 fast_gmail-1.0.8/fast_gmail/helpers.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    25256 2024-04-20 07:20:24.000000 fast_gmail-1.0.8/fast_gmail/message.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.0.8/fast_gmail/search.py
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-20 07:22:34.665839 fast_gmail-1.0.8/fast_gmail.egg-info/
--rw-r--r--   0 aleti     (1000) aleti     (1000)    15624 2024-04-20 07:22:34.000000 fast_gmail-1.0.8/fast_gmail.egg-info/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-04-20 07:22:34.000000 fast_gmail-1.0.8/fast_gmail.egg-info/SOURCES.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-04-20 07:22:34.000000 fast_gmail-1.0.8/fast_gmail.egg-info/dependency_links.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-04-20 07:22:34.000000 fast_gmail-1.0.8/fast_gmail.egg-info/requires.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-04-20 07:22:34.000000 fast_gmail-1.0.8/fast_gmail.egg-info/top_level.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-04-20 07:22:34.665839 fast_gmail-1.0.8/setup.cfg
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1074 2024-04-20 07:22:18.000000 fast_gmail-1.0.8/setup.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-08 13:01:40.682925 fast_gmail-1.0.9/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.0.9/LICENSE
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    15624 2024-05-08 13:01:40.682925 fast_gmail-1.0.9/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    14864 2024-04-20 07:12:16.000000 fast_gmail-1.0.9/README.md
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-08 13:01:40.682925 fast_gmail-1.0.9/fast_gmail/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       30 2024-04-15 08:44:02.000000 fast_gmail-1.0.9/fast_gmail/__init__.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.0.9/fast_gmail/draft.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    22026 2024-05-08 12:44:06.000000 fast_gmail-1.0.9/fast_gmail/gmail.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     7203 2024-04-19 12:04:22.000000 fast_gmail-1.0.9/fast_gmail/helpers.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    25256 2024-04-20 07:20:24.000000 fast_gmail-1.0.9/fast_gmail/message.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.0.9/fast_gmail/search.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-08 13:01:40.682925 fast_gmail-1.0.9/fast_gmail.egg-info/
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    15624 2024-05-08 13:01:40.000000 fast_gmail-1.0.9/fast_gmail.egg-info/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-05-08 13:01:40.000000 fast_gmail-1.0.9/fast_gmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-05-08 13:01:40.000000 fast_gmail-1.0.9/fast_gmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-05-08 13:01:40.000000 fast_gmail-1.0.9/fast_gmail.egg-info/requires.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-05-08 13:01:40.000000 fast_gmail-1.0.9/fast_gmail.egg-info/top_level.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-05-08 13:01:40.682925 fast_gmail-1.0.9/setup.cfg
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1074 2024-05-08 12:44:38.000000 fast_gmail-1.0.9/setup.py
```

### Comparing `fast_gmail-1.0.8/LICENSE` & `fast_gmail-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.8/PKG-INFO` & `fast_gmail-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.0.8
+Version: 1.0.9
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `fast_gmail-1.0.8/README.md` & `fast_gmail-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.8/fast_gmail/gmail.py` & `fast_gmail-1.0.9/fast_gmail/gmail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Optional
 from typing import Union
 from typing import List
-from typing import Any
 import mimetypes
 import base64
 import os
 import json
 
 from email.message import EmailMessage
 from email.header import Header
 from email import utils
 
 from googleapiclient.discovery import build
 from google.oauth2.credentials import Credentials
 from googleapiclient.errors import HttpError
-from google_auth_oauthlib.flow import InstalledAppFlow, Flow
+from google_auth_oauthlib.flow import InstalledAppFlow
+from google_auth_oauthlib.flow import Flow
 
 from fast_gmail.message import MessagePartBody
 from fast_gmail.message import Message
 from fast_gmail.search import SearchParams
 from fast_gmail.draft import Draft
 from fast_gmail.helpers import *
 
@@ -35,14 +35,15 @@
 class GmailApi(object):
 	"""https://googleapis.github.io/google-api-python-client/docs/dyn/gmail_v1.users.html"""
 	credentials: Optional[Credentials] = None
 	google_service: GoogleService
 	max_results: int = MAX_RESULTS
 	SEPARATOR_SYMBOL: str
 	profile_data: Optional[GmailProfile] = None
+	redirect_uri: Optional[str] = None
 
 	def __init__(
 		self,
 		token_file_path: str = "token.json",
 		credentials_file_path: str = "credentials.json",
 		port: int = 3000, # set the local server port for Authorized redirect URI
 		separator_symbol: str = ", ",
@@ -105,15 +106,15 @@
 						self.flow = Flow.from_client_secrets_file(
 							credentials_file_path,
 							SCOPES,
                             redirect_uri=self.redirect_uri
                         )
 						if code:
 							self.flow.fetch_token(code=code)
-							self.credentials: str = self.flow.credentials
+							self.credentials = self.flow.credentials
 						else:
 							self.auth_url = f"{self.flow.authorization_url()[0]}&prompt=consent"
 							return
 			# Save the credentials for the next run
 			with open(token_file_path, "w") as token:
 				token.write(self.credentials.to_json())
 		try:
@@ -629,8 +630,8 @@
 			request = build("people", "v1", credentials = self.credentials).otherContacts().search(
 				pageSize=30,
 				readMask="emailAddresses",
 				query = query
 			).execute()
 			return request["results"] if "results" in request else None
 		except HttpError as e:
-			raise e
+			raise e
```

### Comparing `fast_gmail-1.0.8/fast_gmail/helpers.py` & `fast_gmail-1.0.9/fast_gmail/helpers.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.8/fast_gmail/message.py` & `fast_gmail-1.0.9/fast_gmail/message.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.8/fast_gmail/search.py` & `fast_gmail-1.0.9/fast_gmail/search.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.8/fast_gmail.egg-info/PKG-INFO` & `fast_gmail-1.0.9/fast_gmail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.0.8
+Version: 1.0.9
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `fast_gmail-1.0.8/setup.py` & `fast_gmail-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as f:
     long_descrition=f.read()
 
 setup(
     name="fast_gmail",
-    version="1.0.8",
+    version="1.0.9",
     description="GmailApi wrapper",
     long_description=long_descrition,
     long_description_content_type='text/markdown',
     author="Aleti",
     author_email="aleti.open.source@gmail.com",
     url="https://github.com/aleti1/fast_gmail",
     license="MIT",
```

