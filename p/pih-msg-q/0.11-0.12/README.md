# Comparing `tmp/pih-msg_q-0.11.tar.gz` & `tmp/pih-msg_q-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-msg_q-0.11.tar", last modified: Wed Apr 10 01:50:57 2024, max compression
+gzip compressed data, was "pih-msg_q-0.12.tar", last modified: Wed May  8 06:45:25 2024, max compression
```

## Comparing `pih-msg_q-0.11.tar` & `pih-msg_q-0.12.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 01:50:57.889932 pih-msg_q-0.11/
-drwxrwxrwx   0        0        0        0 2024-04-10 01:50:57.529487 pih-msg_q-0.11/MessageQueueService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-msg_q-0.11/MessageQueueService/__init__.py
--rw-rw-rw-   0        0        0      156 2024-02-15 00:45:45.000000 pih-msg_q-0.11/MessageQueueService/__main__.py
--rw-rw-rw-   0        0        0      441 2024-04-10 00:33:19.000000 pih-msg_q-0.11/MessageQueueService/const.py
--rw-rw-rw-   0        0        0     3184 2024-04-10 00:34:39.000000 pih-msg_q-0.11/MessageQueueService/service.py
--rw-rw-rw-   0        0        0      275 2024-04-10 01:50:57.858682 pih-msg_q-0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 01:50:57.826376 pih-msg_q-0.11/pih_msg_q.egg-info/
--rw-rw-rw-   0        0        0      275 2024-04-10 01:50:57.000000 pih-msg_q-0.11/pih_msg_q.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-10 01:50:57.000000 pih-msg_q-0.11/pih_msg_q.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 01:50:57.000000 pih-msg_q-0.11/pih_msg_q.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-10 01:50:57.000000 pih-msg_q-0.11/pih_msg_q.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 01:50:57.000000 pih-msg_q-0.11/pih_msg_q.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-10 01:50:57.000000 pih-msg_q-0.11/pih_msg_q.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 01:50:57.905562 pih-msg_q-0.11/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 06:45:25.335511 pih-msg_q-0.12/
+drwxrwxrwx   0        0        0        0 2024-05-08 06:45:24.895866 pih-msg_q-0.12/MessageQueueService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-msg_q-0.12/MessageQueueService/__init__.py
+-rw-rw-rw-   0        0        0      156 2024-02-15 00:45:45.000000 pih-msg_q-0.12/MessageQueueService/__main__.py
+-rw-rw-rw-   0        0        0      441 2024-05-08 06:42:36.000000 pih-msg_q-0.12/MessageQueueService/const.py
+-rw-rw-rw-   0        0        0     3701 2024-05-08 06:43:07.000000 pih-msg_q-0.12/MessageQueueService/service.py
+-rw-rw-rw-   0        0        0      275 2024-05-08 06:45:25.304254 pih-msg_q-0.12/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-08 06:45:25.257383 pih-msg_q-0.12/pih_msg_q.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-05-08 06:45:24.000000 pih-msg_q-0.12/pih_msg_q.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-08 06:45:24.000000 pih-msg_q-0.12/pih_msg_q.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 06:45:24.000000 pih-msg_q-0.12/pih_msg_q.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-08 06:45:24.000000 pih-msg_q-0.12/pih_msg_q.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-08 06:45:24.000000 pih-msg_q-0.12/pih_msg_q.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-08 06:45:24.000000 pih-msg_q-0.12/pih_msg_q.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 06:45:25.335511 pih-msg_q-0.12/setup.cfg
```

### Comparing `pih-msg_q-0.11/MessageQueueService/service.py` & `pih-msg_q-0.12/MessageQueueService/service.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import ipih
 
 from pih import A, PIHThread
 from pih.collections import Message
 from MessageQueueService.const import SD
-from pih.tools import ParameterList, while_not_do, ne, j, js
+from pih.tools import ParameterList, while_not_do, ne, js, nn, j
 
 
 SC = A.CT_SC
 
-ISOLATED: bool = False
+ISOLATED: bool = True
 
 from collections import defaultdict
 from time import sleep
 import random
 
+
 class DH:
     message_buffer_list: dict[str, list[Message]] = defaultdict(list)
 
 
 def service_call_handler(sc: SC, pl: ParameterList) -> bool | None:
     if sc == SC.add_message_to_queue:
         message: Message | None = pl.next(Message())
@@ -30,15 +31,30 @@
             return True
     return None
 
 
 def send_message(message: Message) -> None:
     if ne((message.message or "").strip()):
         recipient: str = A.S_P.test_recipient(message.sender) or message.recipient
-        while_not_do(lambda: A.ME_WH_W.send(recipient, message.message, message.sender))
+
+        def send() -> bool:
+            if nn(message.location):
+                return A.ME_WH_W.send_location(
+                    recipient, message.location, message.message, message.sender
+                )
+            if nn(message.image_url):
+                return A.ME_WH_W.send_image(
+                    recipient,
+                    message.message,
+                    A.D_CO.file_to_base64(message.image_url),
+                    message.sender,
+                )
+            return A.ME_WH_W.send(recipient, message.message, message.sender)
+
+        while_not_do(send)
 
 
 def complete_buffered_message_sending_action(message: Message) -> bool:
     A.L.polibase(js(("Сообщение было отправлено аббоненту:", message.recipient)))
     return True
```

