# Comparing `tmp/whatsapp-message-vonage-local-0.0.8.tar.gz` & `tmp/whatsapp-message-vonage-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-message-vonage-local-0.0.8.tar", last modified: Sun Dec 17 19:10:31 2023, max compression
+gzip compressed data, was "whatsapp-message-vonage-local-0.0.9.tar", last modified: Sun Dec 31 23:19:03 2023, max compression
```

## Comparing `whatsapp-message-vonage-local-0.0.8.tar` & `whatsapp-message-vonage-local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 19:10:31.198737 whatsapp-message-vonage-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-12-17 19:10:31.194737 whatsapp-message-vonage-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-12-17 19:09:35.000000 whatsapp-message-vonage-local-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-12-17 19:09:35.000000 whatsapp-message-vonage-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-17 19:10:31.198737 whatsapp-message-vonage-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-17 19:09:35.000000 whatsapp-message-vonage-local-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 19:10:31.194737 whatsapp-message-vonage-local-0.0.8/whatsapp_message_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 19:10:31.194737 whatsapp-message-vonage-local-0.0.8/whatsapp_message_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-17 19:09:35.000000 whatsapp-message-vonage-local-0.0.8/whatsapp_message_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2023-12-17 19:09:35.000000 whatsapp-message-vonage-local-0.0.8/whatsapp_message_local/src/vonage_whatsapp_message_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-12-17 19:09:35.000000 whatsapp-message-vonage-local-0.0.8/whatsapp_message_local/src/whatsappmessage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-17 19:10:31.194737 whatsapp-message-vonage-local-0.0.8/whatsapp_message_vonage_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-12-17 19:10:31.000000 whatsapp-message-vonage-local-0.0.8/whatsapp_message_vonage_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-17 19:10:31.000000 whatsapp-message-vonage-local-0.0.8/whatsapp_message_vonage_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-17 19:10:31.000000 whatsapp-message-vonage-local-0.0.8/whatsapp_message_vonage_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-17 19:10:31.000000 whatsapp-message-vonage-local-0.0.8/whatsapp_message_vonage_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-17 19:10:31.000000 whatsapp-message-vonage-local-0.0.8/whatsapp_message_vonage_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 23:19:03.581250 whatsapp-message-vonage-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2023-12-31 23:19:03.581250 whatsapp-message-vonage-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-12-31 23:18:21.000000 whatsapp-message-vonage-local-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2023-12-31 23:18:21.000000 whatsapp-message-vonage-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-31 23:19:03.581250 whatsapp-message-vonage-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-12-31 23:18:21.000000 whatsapp-message-vonage-local-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 23:19:03.581250 whatsapp-message-vonage-local-0.0.9/whatsapp_message_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 23:19:03.581250 whatsapp-message-vonage-local-0.0.9/whatsapp_message_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 23:18:21.000000 whatsapp-message-vonage-local-0.0.9/whatsapp_message_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2023-12-31 23:18:21.000000 whatsapp-message-vonage-local-0.0.9/whatsapp_message_local/src/vonage_whatsapp_message_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2023-12-31 23:18:21.000000 whatsapp-message-vonage-local-0.0.9/whatsapp_message_local/src/whatsapp_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 23:19:03.581250 whatsapp-message-vonage-local-0.0.9/whatsapp_message_vonage_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2023-12-31 23:19:03.000000 whatsapp-message-vonage-local-0.0.9/whatsapp_message_vonage_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2023-12-31 23:19:03.000000 whatsapp-message-vonage-local-0.0.9/whatsapp_message_vonage_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-31 23:19:03.000000 whatsapp-message-vonage-local-0.0.9/whatsapp_message_vonage_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-31 23:19:03.000000 whatsapp-message-vonage-local-0.0.9/whatsapp_message_vonage_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-31 23:19:03.000000 whatsapp-message-vonage-local-0.0.9/whatsapp_message_vonage_local.egg-info/top_level.txt
```

### Comparing `whatsapp-message-vonage-local-0.0.8/PKG-INFO` & `whatsapp-message-vonage-local-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: whatsapp-message-vonage-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles whatsapp-message-vonage-local
 Home-page: https://github.com/circles-zone/whatsapp-message-vonage-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: vonage>=3.11.0
 Requires-Dist: message-local>=0.0.3
 Requires-Dist: logger-local>=0.0.71
 Requires-Dist: database-mysql-local>=0.0.121
+Requires-Dist: api-management-local
 
 This is a package for sharing common whatsapp function used in different repositories
```

### Comparing `whatsapp-message-vonage-local-0.0.8/README.md` & `whatsapp-message-vonage-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp-message-vonage-local-0.0.8/pyproject.toml` & `whatsapp-message-vonage-local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whatsapp-message-vonage-local-0.0.8/setup.py` & `whatsapp-message-vonage-local-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "whatsapp-message-vonage-local"
 # Since all PACAKGE_NAMEs are with an underscore, we don't need this. Why do we need it?
 package_dir = "whatsapp_message_local"
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # https://pypi.org/project/whatsapp-message-vonage-local
+    version='0.0.9',  # https://pypi.org/project/whatsapp-message-vonage-local
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles whatsapp-message-vonage-local",
     long_description="This is a package for sharing common whatsapp function used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/circles-zone/whatsapp-message-vonage-local-python-package",
     packages=[package_dir],
@@ -21,10 +21,11 @@
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'vonage>=3.11.0',
         'message-local>=0.0.3',
         'logger-local>=0.0.71',
-        'database-mysql-local>=0.0.121'
+        'database-mysql-local>=0.0.121',
+        'api-management-local'
     ]
 )
```

### Comparing `whatsapp-message-vonage-local-0.0.8/whatsapp_message_local/src/vonage_whatsapp_message_local.py` & `whatsapp-message-vonage-local-0.0.9/whatsapp_message_local/src/vonage_whatsapp_message_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 "imports"
 import os
+
 import vonage
-from logger_local.LoggerComponentEnum import LoggerComponentEnum
-from logger_local.Logger import Logger
-from api_management_local.api_management_local import APIManagmentLocal
-from src.whatsappmessage import WHATSAPP_MESSAGE_VONAGE_LOCAL_PYTHON_COMPONENT_ID
-from src.whatsappmessage import WHATSAPP_MESSAGE_VONAGE_LOCAL_PYTHON_COMPONENT_NAME
 from dotenv import load_dotenv
+from logger_local.Logger import Logger
+from logger_local.LoggerComponentEnum import LoggerComponentEnum
+# from api_management_local.api_management_local import APIManagementsLocal
+from src.whatsapp_message import (
+    WHATSAPP_MESSAGE_VONAGE_LOCAL_PYTHON_COMPONENT_ID,
+    WHATSAPP_MESSAGE_VONAGE_LOCAL_PYTHON_COMPONENT_NAME)
 
 whatsapp_message_local_python_unit_tests_logger_object = {
     'component_id': WHATSAPP_MESSAGE_VONAGE_LOCAL_PYTHON_COMPONENT_ID,
     'component_name': WHATSAPP_MESSAGE_VONAGE_LOCAL_PYTHON_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
     "developer_email": "jenya.b@circ.zone"
 }
@@ -18,32 +20,34 @@
 logger = Logger.create_logger(
     object=whatsapp_message_local_python_unit_tests_logger_object)
 WHATSAPP_MESSAGE_VONAGE_API_TYPE_ID = 9
 load_dotenv()
 
 
 class VonageWhatsAppMessagesLocal(vonage.Messages):
-    "Vonage whatsapp message"
+    """Vonage whatsapp message"""
+
     def __init__(self, default_from_number: str, to_number: str) -> None:
         self.api_key = os.getenv("VONAGE_API_KEY")
         self.api_secret = os.getenv("VONAGE_API_SECRET")
         self.default_from_number = default_from_number
         self.to_number = to_number
         self.url = "https://messages-sandbox.nexmo.com/v1/messages"
         self.headers = {
             "Content-Type": "application/json",
             "Accept": "application/json"
         }
+        # super().__init__(client=vonage.Client(key=self.api_key, secret=self.api_secret))
 
     def send(self, person_id: int, message: str) -> None:
-        "send message use vonage api"
+        """send message use vonage api"""
         logger.start("send message to phone by id ", object={
-                     "profile_id": person_id, 'message': message})
+            "profile_id": person_id, 'message': message})
         data = {
             "from": self.default_from_number,
             "to": self.to_number,
             "message_type": "text",
             "text": message,
             "channel": "whatsapp"
         }
-        APIManagmentLocal()
+        # APIManagementsLocal()
         logger.end()
```

### Comparing `whatsapp-message-vonage-local-0.0.8/whatsapp_message_local/src/whatsappmessage.py` & `whatsapp-message-vonage-local-0.0.9/whatsapp_message_local/src/whatsapp_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import List
-from message_local.MessageLocal import MessageLocal
+
+from logger_local.Logger import Logger
+from logger_local.LoggerComponentEnum import LoggerComponentEnum
 from message_local.MessageImportance import MessageImportance
+from message_local.MessageLocal import MessageLocal
 from message_local.Recipient import Recipient
-from logger_local.LoggerComponentEnum import LoggerComponentEnum
-from logger_local.Logger import Logger
+
 # from api_management_local.api_call import APICallsLocal
 # from api_management_local.api_limit import APILimitsLocal
 
 
 WHATSAPP_MESSAGE_VONAGE_LOCAL_PYTHON_COMPONENT_ID = 173
 WHATSAPP_MESSAGE_VONAGE_LOCAL_PYTHON_COMPONENT_NAME = 'send whatsapp-message-local-python-package'
```

### Comparing `whatsapp-message-vonage-local-0.0.8/whatsapp_message_vonage_local.egg-info/PKG-INFO` & `whatsapp-message-vonage-local-0.0.9/whatsapp_message_vonage_local.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: whatsapp-message-vonage-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles whatsapp-message-vonage-local
 Home-page: https://github.com/circles-zone/whatsapp-message-vonage-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: vonage>=3.11.0
 Requires-Dist: message-local>=0.0.3
 Requires-Dist: logger-local>=0.0.71
 Requires-Dist: database-mysql-local>=0.0.121
+Requires-Dist: api-management-local
 
 This is a package for sharing common whatsapp function used in different repositories
```

