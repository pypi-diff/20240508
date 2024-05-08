# Comparing `tmp/whataspp-inforu-local-0.0.8.tar.gz` & `tmp/whataspp-inforu-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whataspp-inforu-local-0.0.8.tar", last modified: Mon Jan 29 21:52:40 2024, max compression
+gzip compressed data, was "whataspp-inforu-local-0.0.9.tar", last modified: Wed Jan 31 20:09:04 2024, max compression
```

## Comparing `whataspp-inforu-local-0.0.8.tar` & `whataspp-inforu-local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:52:40.226046 whataspp-inforu-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-29 21:52:40.226046 whataspp-inforu-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-01-29 21:52:03.000000 whataspp-inforu-local-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-29 21:52:03.000000 whataspp-inforu-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 21:52:40.226046 whataspp-inforu-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-01-29 21:52:03.000000 whataspp-inforu-local-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:52:40.222046 whataspp-inforu-local-0.0.8/whataspp_inforu_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:52:40.226046 whataspp-inforu-local-0.0.8/whataspp_inforu_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-01-29 21:52:03.000000 whataspp-inforu-local-0.0.8/whataspp_inforu_local/src/WhatsAppLocalConstants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-01-29 21:52:03.000000 whataspp-inforu-local-0.0.8/whataspp_inforu_local/src/WhatsAppMessageInforuLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 21:52:03.000000 whataspp-inforu-local-0.0.8/whataspp_inforu_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:52:40.226046 whataspp-inforu-local-0.0.8/whataspp_inforu_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-29 21:52:40.000000 whataspp-inforu-local-0.0.8/whataspp_inforu_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-29 21:52:40.000000 whataspp-inforu-local-0.0.8/whataspp_inforu_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 21:52:40.000000 whataspp-inforu-local-0.0.8/whataspp_inforu_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-29 21:52:40.000000 whataspp-inforu-local-0.0.8/whataspp_inforu_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-29 21:52:40.000000 whataspp-inforu-local-0.0.8/whataspp_inforu_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 20:09:04.115009 whataspp-inforu-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-31 20:09:04.115009 whataspp-inforu-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-01-31 20:08:26.000000 whataspp-inforu-local-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-31 20:08:26.000000 whataspp-inforu-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 20:09:04.115009 whataspp-inforu-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-01-31 20:08:26.000000 whataspp-inforu-local-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 20:09:04.111009 whataspp-inforu-local-0.0.9/whataspp_inforu_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 20:09:04.111009 whataspp-inforu-local-0.0.9/whataspp_inforu_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-01-31 20:08:26.000000 whataspp-inforu-local-0.0.9/whataspp_inforu_local/src/WhatsAppLocalConstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-01-31 20:08:26.000000 whataspp-inforu-local-0.0.9/whataspp_inforu_local/src/WhatsAppMessageInforuLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 20:08:26.000000 whataspp-inforu-local-0.0.9/whataspp_inforu_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 20:09:04.111009 whataspp-inforu-local-0.0.9/whataspp_inforu_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-31 20:09:04.000000 whataspp-inforu-local-0.0.9/whataspp_inforu_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-31 20:09:04.000000 whataspp-inforu-local-0.0.9/whataspp_inforu_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 20:09:04.000000 whataspp-inforu-local-0.0.9/whataspp_inforu_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-31 20:09:04.000000 whataspp-inforu-local-0.0.9/whataspp_inforu_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-31 20:09:04.000000 whataspp-inforu-local-0.0.9/whataspp_inforu_local.egg-info/top_level.txt
```

### Comparing `whataspp-inforu-local-0.0.8/PKG-INFO` & `whataspp-inforu-local-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whataspp-inforu-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles whataspp_inforu_local Python
 Home-page: https://github.com/circles-zone/whatsapp-message-inforu-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `whataspp-inforu-local-0.0.8/README.md` & `whataspp-inforu-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `whataspp-inforu-local-0.0.8/pyproject.toml` & `whataspp-inforu-local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whataspp-inforu-local-0.0.8/setup.py` & `whataspp-inforu-local-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "whataspp-inforu-local"
 # Since all PACAKGE_NAMEs are with an underscore, we don't need this. Why do we need it?
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # update only the minor version each time # https://pypi.org/project/whataspp-inforu-local/
+    version='0.0.9',  # update only the minor version each time # https://pypi.org/project/whataspp-inforu-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles whataspp_inforu_local Python",
     long_description="This is a package for sharing common whataspp_inforu_local function used in different repositories",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/whatsapp-message-inforu-local-python-package",
     # packages=setuptools.find_packages(),
```

### Comparing `whataspp-inforu-local-0.0.8/whataspp_inforu_local/src/WhatsAppLocalConstants.py` & `whataspp-inforu-local-0.0.9/whataspp_inforu_local/src/WhatsAppLocalConstants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
 WHATSAPP_MESSAGE_INFORU_API_TYPE_ID = 8
 
 WHATSAPP_API_URL = 'https://capi.inforu.co.il/api/v2/WhatsApp/SendWhatsAppChat'
 
-WHATSAPP_HEADERS = {
-    'Content-Type': 'application/json',
-}
-
 WHATSAPP_LOGGER_COMPONENT_ID = 208
 WHATSAPP_LOGGER_COMPONENT_NAME = "WhatsApp_InforU_LOCAL_PYTHON_PACKAGE"
 WHATSAPP_DEVELOPER_EMAIL = "emad.a@circ.zone"
 
 
 def get_logger_object(category: str = LoggerComponentEnum.ComponentCategory.Code):
     if category == LoggerComponentEnum.ComponentCategory.Code:
```

### Comparing `whataspp-inforu-local-0.0.8/whataspp_inforu_local/src/WhatsAppMessageInforuLocal.py` & `whataspp-inforu-local-0.0.9/whataspp_inforu_local/src/WhatsAppMessageInforuLocal.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from typing import List
 
 import requests
 from python_sdk_remote.utilities import our_get_env
 from logger_local.LoggerLocal import Logger
 from message_local.MessageLocal import MessageLocal
 from message_local.Recipient import Recipient
+from python_sdk_remote.utilities import create_return_http_headers
 
-from .WhatsAppLocalConstants import (WHATSAPP_API_URL, WHATSAPP_HEADERS,
+from .WhatsAppLocalConstants import (WHATSAPP_API_URL,
                                      WHATSAPP_MESSAGE_INFORU_API_TYPE_ID,
                                      get_logger_object)
 
 INFORU_AUTH_TOKEN = our_get_env("INFORU_AUTH_TOKEN")
 
 
 class WhatsAppMessageInforuLocal(MessageLocal):
@@ -52,15 +53,15 @@
                     "Recipients": recipients_details
                 }
             }
             if message_media:
                 payload["Data"]["messageMedia"] = message_media
             url = WHATSAPP_API_URL
             headers = {
-                **WHATSAPP_HEADERS,
+                **create_return_http_headers(),
                 'Authorization': INFORU_AUTH_TOKEN
             }
             payload_json = json.dumps(payload)
             if (our_get_env("REALLY_SEND_WHATSAPP") and
                     self.can_send(api_data=payload, outgoing_body=payload,
                                   sender_profile_id=self.get_sender_profile_id())):
                 response = requests.post(url, headers=headers, json=payload_json)
```

### Comparing `whataspp-inforu-local-0.0.8/whataspp_inforu_local.egg-info/PKG-INFO` & `whataspp-inforu-local-0.0.9/whataspp_inforu_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whataspp-inforu-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles whataspp_inforu_local Python
 Home-page: https://github.com/circles-zone/whatsapp-message-inforu-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

