# Comparing `tmp/messages_local-0.0.49.tar.gz` & `tmp/messages_local-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messages_local-0.0.49.tar", last modified: Sun Apr 28 05:51:08 2024, max compression
+gzip compressed data, was "messages_local-0.0.50.tar", last modified: Wed May  8 02:10:14 2024, max compression
```

## Comparing `messages_local-0.0.49.tar` & `messages_local-0.0.50.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:51:08.363937 messages_local-0.0.49/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-28 05:51:08.363937 messages_local-0.0.49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-28 05:50:27.000000 messages_local-0.0.49/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:51:08.359937 messages_local-0.0.49/messages_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:51:08.363937 messages_local-0.0.49/messages_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-04-28 05:50:27.000000 messages_local-0.0.49/messages_local/src/MessagesLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:50:27.000000 messages_local-0.0.49/messages_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:51:08.363937 messages_local-0.0.49/messages_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-28 05:51:08.000000 messages_local-0.0.49/messages_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-28 05:51:08.000000 messages_local-0.0.49/messages_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 05:51:08.000000 messages_local-0.0.49/messages_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-28 05:51:08.000000 messages_local-0.0.49/messages_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-28 05:51:08.000000 messages_local-0.0.49/messages_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-28 05:50:27.000000 messages_local-0.0.49/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 05:51:08.363937 messages_local-0.0.49/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-28 05:50:27.000000 messages_local-0.0.49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:10:14.658078 messages_local-0.0.50/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-08 02:10:14.658078 messages_local-0.0.50/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-08 02:09:35.000000 messages_local-0.0.50/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:10:14.654078 messages_local-0.0.50/messages_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:10:14.654078 messages_local-0.0.50/messages_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12497 2024-05-08 02:09:35.000000 messages_local-0.0.50/messages_local/src/MessagesLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 02:09:35.000000 messages_local-0.0.50/messages_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:10:14.654078 messages_local-0.0.50/messages_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-08 02:10:14.000000 messages_local-0.0.50/messages_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-08 02:10:14.000000 messages_local-0.0.50/messages_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 02:10:14.000000 messages_local-0.0.50/messages_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-08 02:10:14.000000 messages_local-0.0.50/messages_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 02:10:14.000000 messages_local-0.0.50/messages_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-08 02:09:35.000000 messages_local-0.0.50/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 02:10:14.658078 messages_local-0.0.50/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 02:09:35.000000 messages_local-0.0.50/setup.py
```

### Comparing `messages_local-0.0.49/PKG-INFO` & `messages_local-0.0.50/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.49
+Version: 0.0.50
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
-Author-email: info@circles.life
+Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: item-local
-Requires-Dist: message-local>=0.0.118
+Requires-Dist: item-local>=0.0.9
 Requires-Dist: queue-worker-local>=0.0.37
-Requires-Dist: label-message-local>=0.0.2
-Requires-Dist: whatsapp-message-vonage-local
-Requires-Dist: whataspp-inforu-local
-Requires-Dist: email-message-aws-ses-local
-Requires-Dist: sms-message-aws-sns-local>=0.0.8
+Requires-Dist: label-message-local>=0.0.4
+Requires-Dist: message-local>=0.0.121
+Requires-Dist: whatsapp-message-vonage-local>=0.0.19
+Requires-Dist: whataspp-inforu-local>=0.0.12
+Requires-Dist: sms-message-aws-sns-local>=0.0.35
+Requires-Dist: email-message-aws-ses-local>=0.0.13
 
 messages-local
```

### Comparing `messages_local-0.0.49/README.md` & `messages_local-0.0.50/README.md`

 * *Files identical despite different names*

### Comparing `messages_local-0.0.49/messages_local/src/MessagesLocal.py` & `messages_local-0.0.50/messages_local/src/MessagesLocal.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from queue_worker_local.queue_worker import QueueWorker
 from sms_message_aws_sns_local.sms_message_aws_sns import SmsMessageAwsSnsLocal
 from whataspp_inforu_local.WhatsAppMessageInforuLocal import WhatsAppMessageInforuLocal
 from whatsapp_message_vonage_local.vonage_whatsapp_message_local import WhatsAppMessageVonageLocal
 
 # TODO Replace Magic Number with enum in a separate file in this repo which will be created by Sql2Code in the future
 MESSAGES_API_TYPE_ID = 5
+# TODO What is this action?
 SEND_SYNC_ACTION_ID = 15
 MESSAGE_LOCAL_PYTHON_COMPONENT_ID = 259
 MESSAGE_LOCAL_PYTHON_COMPONENT_COMPONENT_NAME = 'messages-local-python-package'
 DEVELOPER_EMAIL = 'akiva.s@circ.zone'
 
 logger_object_message = {
     'component_id': MESSAGE_LOCAL_PYTHON_COMPONENT_ID,
```

### Comparing `messages_local-0.0.49/messages_local.egg-info/PKG-INFO` & `messages_local-0.0.50/messages_local.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.49
+Version: 0.0.50
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
-Author-email: info@circles.life
+Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: item-local
-Requires-Dist: message-local>=0.0.118
+Requires-Dist: item-local>=0.0.9
 Requires-Dist: queue-worker-local>=0.0.37
-Requires-Dist: label-message-local>=0.0.2
-Requires-Dist: whatsapp-message-vonage-local
-Requires-Dist: whataspp-inforu-local
-Requires-Dist: email-message-aws-ses-local
-Requires-Dist: sms-message-aws-sns-local>=0.0.8
+Requires-Dist: label-message-local>=0.0.4
+Requires-Dist: message-local>=0.0.121
+Requires-Dist: whatsapp-message-vonage-local>=0.0.19
+Requires-Dist: whataspp-inforu-local>=0.0.12
+Requires-Dist: sms-message-aws-sns-local>=0.0.35
+Requires-Dist: email-message-aws-ses-local>=0.0.13
 
 messages-local
```

### Comparing `messages_local-0.0.49/setup.py` & `messages_local-0.0.50/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 
 PACKAGE_NAME = "messages-local"
 
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.49', # https://pypi.org/project/messages-local
+    version='0.0.50',  # https://pypi.org/project/messages-local
     author="Circles",
-    author_email="info@circles.life",
-    url=f"https://github.com/circles-zone/messages-local-python-package",
+    author_email="info@circles.ai",
+    url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="messages-local",
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["item-local",
-                      "message-local>=0.0.118",
-                      "queue-worker-local>=0.0.37",
-                      "label-message-local>=0.0.2",
-                      "whatsapp-message-vonage-local",
-                      "whataspp-inforu-local",
-                      "email-message-aws-ses-local",
-                      "sms-message-aws-sns-local>=0.0.8",
-                      ]
+    install_requires=[
+        "item-local>=0.0.9",
+        "queue-worker-local>=0.0.37",
+        "label-message-local>=0.0.4",
+        "message-local>=0.0.121",
+        "whatsapp-message-vonage-local>=0.0.19",
+        "whataspp-inforu-local>=0.0.12",
+        "sms-message-aws-sns-local>=0.0.35",
+        "email-message-aws-ses-local>=0.0.13"
+    ]
 )
```

