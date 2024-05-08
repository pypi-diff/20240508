# Comparing `tmp/scratchcommunication-2.7.1.tar.gz` & `tmp/scratchcommunication-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.7.1.tar", last modified: Thu May  2 16:46:34 2024, max compression
+gzip compressed data, was "scratchcommunication-2.7.2.tar", last modified: Wed May  8 13:42:22 2024, max compression
```

## Comparing `scratchcommunication-2.7.1.tar` & `scratchcommunication-2.7.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:46:34.226773 scratchcommunication-2.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16430 2024-05-02 16:46:34.226773 scratchcommunication-2.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:46:34.226773 scratchcommunication-2.7.1/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/cloud_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:46:34.226773 scratchcommunication-2.7.1/scratchcommunication/cloudrequests/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/cloudrequests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/cloudrequests/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/cloudrequests/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:46:34.226773 scratchcommunication-2.7.1/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16430 2024-05-02 16:46:34.000000 scratchcommunication-2.7.1/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-02 16:46:34.000000 scratchcommunication-2.7.1/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:46:34.000000 scratchcommunication-2.7.1/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 16:46:34.000000 scratchcommunication-2.7.1/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 16:46:34.000000 scratchcommunication-2.7.1/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:46:34.226773 scratchcommunication-2.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:46:34.226773 scratchcommunication-2.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-02 16:46:30.000000 scratchcommunication-2.7.1/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:42:22.975186 scratchcommunication-2.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16430 2024-05-08 13:42:22.975186 scratchcommunication-2.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:42:22.971186 scratchcommunication-2.7.2/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:42:22.975186 scratchcommunication-2.7.2/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:42:22.975186 scratchcommunication-2.7.2/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16430 2024-05-08 13:42:22.000000 scratchcommunication-2.7.2/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-08 13:42:22.000000 scratchcommunication-2.7.2/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:42:22.000000 scratchcommunication-2.7.2/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 13:42:22.000000 scratchcommunication-2.7.2/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 13:42:22.000000 scratchcommunication-2.7.2/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:42:22.975186 scratchcommunication-2.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:42:22.975186 scratchcommunication-2.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 13:42:14.000000 scratchcommunication-2.7.2/tests/test1.py
```

### Comparing `scratchcommunication-2.7.1/LICENSE` & `scratchcommunication-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.7.1/PKG-INFO` & `scratchcommunication-2.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.7.1
+Version: 2.7.2
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.7.1/README.md` & `scratchcommunication-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.7.1/scratchcommunication/cloud.py` & `scratchcommunication-2.7.2/scratchcommunication/cloud.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.7.1/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.7.2/scratchcommunication/cloud_socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .cloud import CloudConnection
 from . import security as sec
+from threading import Lock
 from typing import Union, Any, Self
 import random, time
 from itertools import islice
 from .exceptions import NotSupported
 
 alphabet = "abcdefghijklmnopqrstuvwxyz"
 special_characters = " .,-:;_'#!\"§$%&/()=?{[]}\\0123456789<>ß*"
@@ -14,14 +15,19 @@
     # batched('ABCDEFG', 3) --> ABC DEF G
     if n < 1:
         raise ValueError('n must be at least one')
     it = iter(iterable)
     while batch := tuple(islice(it, n)):
         yield batch
         
+class BaseCloudSocketMSG:
+    """
+    Base class for cloud socket messages.
+    """
+        
 class BaseCloudSocketClient:
     """
     Base class for connecting with cloud sockets
     """
     def __init__(self, *, cloud : CloudConnection, username : str = "user1000", packet_size : int = 220, security : Union[None, tuple] = None):
         raise NotImplementedError
     
@@ -63,14 +69,23 @@
         """
         raise NotImplementedError
 
 class BaseCloudSocket:
     """
     Base Class for creating cloud sockets with projects
     """
+    security : sec.RSAKeys
+    cloud : CloudConnection
+    clients : dict
+    new_clients : list
+    connecting_clients : list
+    key_parts : dict
+    last_timestamp : float
+    packet_size : int
+    accepting : Lock
     def __init__(self, *, cloud : CloudConnection, packet_size : int = 220, security : Union[None, tuple] = None):
         raise NotImplementedError
 
     def __enter__(self) -> Self:
         raise NotImplementedError
     
     def __exit__(self, exc_type, exc_value, traceback):
@@ -96,14 +111,24 @@
         """
         raise NotImplementedError
 
 class BaseCloudSocketConnection:
     """
     Base Class for handling incoming connections from a cloud socket
     """
+    cloud_socket : BaseCloudSocket
+    client_id : str
+    username : str
+    security : str
+    encrypter : sec.SymmetricEncryption
+    secure : bool
+    new_msgs : list
+    current_msg : BaseCloudSocketMSG
+    receiving : Lock
+    sending : Lock
     def __init__(self, *, cloud_socket : BaseCloudSocket, client_id : str, username : str = None, security : str = None):
         raise NotImplementedError
     
     def __enter__(self) -> Self:
         raise NotImplementedError
     
     def __exit__(self, exc_type, exc_value, traceback):
@@ -130,14 +155,15 @@
         self.cloud = cloud
         self.clients = {}
         self.new_clients = []
         self.connecting_clients = []
         self.key_parts = {}
         self.last_timestamp = time.time()
         self.packet_size = packet_size
+        self.accepting = Lock()
         
     def listen(self):
         """
         Start the cloud socket.
         """
         @self.cloud.on("set")
         def on_packet(event):
@@ -247,36 +273,44 @@
                 encoded += char_to_idx["?"]
         return int(encoded)
     
     def accept(self, timeout : Union[float, None] = 10) -> tuple[BaseCloudSocketConnection, str]:
         """
         Returns a new client
         """
-        endtime = time.time() + timeout if timeout is not None else None
-        while (not self.new_clients) and (timeout is None or time.time() < endtime): 
-            pass
-        try:
-            new_client = self.new_clients.pop(0)
-            return new_client
-        except IndexError:
+        endtime = (time.time() + timeout) if timeout is not None else None
+        result = self.accepting.acquire(timeout=timeout if timeout is not None else -1)
+        if not result:
             raise TimeoutError("The timeout expired (consider setting timeout=None)")
+        try:
+            while (not self.new_clients) and (timeout is None or time.time() < endtime): 
+                pass
+            try:
+                new_client = self.new_clients.pop(0)
+                return new_client
+            except IndexError:
+                raise TimeoutError("The timeout expired (consider setting timeout=None)")
+        finally:
+            self.accepting.release()
     
 class CloudSocketConnection(BaseCloudSocketConnection):
     """
     Class for handling incoming connections from a cloud socket
     """
     def __init__(self, *, cloud_socket : BaseCloudSocket, client_id : str, username : str = None, security : str = None):
         self.cloud_socket = cloud_socket
         self.client_id = client_id
         self.username = username
         self.security = security
         self.encrypter = sec.SymmetricEncryption(self.security)
         self.secure = bool(self.security)
         self.new_msgs = []
         self.current_msg = CloudSocketMSG()
+        self.receiving = Lock()
+        self.sending = Lock()
 
     def __enter__(self):
         return self
     
     def __exit__(self, exc_type, exc_value, traceback):
         pass
     
@@ -295,39 +329,49 @@
         packet = self.cloud_socket._encode(self.encrypter.encrypt(packets[-1], salt=salt))
         self.cloud_socket.cloud.set_variable(name=f"TO_CLIENT_{random.randint(1, 4)}", value=f"{packet}{str(salt).zfill(15)}.{self.client_id}{packet_idx}")
     
     def send(self, data : str):
         """
         Use for sending data to the client
         """
-        if self.secure:
-            self._secure_send(data)
-            return
-        data = str(self.cloud_socket._encode(data))
-        packets = ["".join(i) for i in batched(data, self.cloud_socket.packet_size)]
-        packet_idx = 0
-        for packet in packets[:-1]:
-            self.cloud_socket.cloud.set_variable(name=f"TO_CLIENT_{random.randint(1, 4)}", value=f"-{packet}.{self.client_id}{packet_idx}")
-            packet_idx += 1
-        self.cloud_socket.cloud.set_variable(name=f"TO_CLIENT_{random.randint(1, 4)}", value=f"{packets[-1]}.{self.client_id}{packet_idx}")
+        with self.sending:
+            if self.secure:
+                self._secure_send(data)
+                return
+            data = str(self.cloud_socket._encode(data))
+            packets = ["".join(i) for i in batched(data, self.cloud_socket.packet_size)]
+            packet_idx = 0
+            for packet in packets[:-1]:
+                self.cloud_socket.cloud.set_variable(name=f"TO_CLIENT_{random.randint(1, 4)}", value=f"-{packet}.{self.client_id}{packet_idx}")
+                packet_idx += 1
+            self.cloud_socket.cloud.set_variable(name=f"TO_CLIENT_{random.randint(1, 4)}", value=f"{packets[-1]}.{self.client_id}{packet_idx}")
 
     def recv(self, timeout : Union[float, None] = 10) -> str:
         """
         Use for receiving data from the client
         timeout defaults to 10 (seconds) but can be set to None if you do not want timeout.
         """
-        endtime = time.time() + timeout if timeout is not None else None
-        while (not self.new_msgs) and (timeout is None or time.time() < endtime):
-            pass
-        try:
-            return self.new_msgs.pop(0).message
-        except IndexError:
+        endtime = (time.time() + timeout) if timeout is not None else None
+        result = self.receiving.acquire(timeout=timeout if timeout is not None else -1)
+        if not result:
             raise TimeoutError("The timeout expired (consider setting timeout=None)")
+        try:
+            while (not self.new_msgs) and (timeout is None or time.time() < endtime):
+                pass
+            try:
+                return self.new_msgs.pop(0).message
+            except IndexError:
+                raise TimeoutError("The timeout expired (consider setting timeout=None)")
+        finally:
+            self.receiving.release()
     
-class CloudSocketMSG:
+class CloudSocketMSG(BaseCloudSocketMSG):
+    """
+    Class for cloud socket messages.
+    """
     def __init__(self, message : str = "", complete : bool = False):
         self.message = message
         self.complete = complete
         
     def add(self, data):
         self.message += data[1:]
```

### Comparing `scratchcommunication-2.7.1/scratchcommunication/cloudrequests/basetypes.py` & `scratchcommunication-2.7.2/scratchcommunication/cloudrequests/basetypes.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.7.1/scratchcommunication/cloudrequests/requests.py` & `scratchcommunication-2.7.2/scratchcommunication/cloudrequests/requests.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.7.1/scratchcommunication/security.py` & `scratchcommunication-2.7.2/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.7.1/scratchcommunication/session.py` & `scratchcommunication-2.7.2/scratchcommunication/session.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.7.1/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.7.2/scratchcommunication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.7.1
+Version: 2.7.2
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.7.1/scratchcommunication.egg-info/SOURCES.txt` & `scratchcommunication-2.7.2/scratchcommunication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.7.1/setup.py` & `scratchcommunication-2.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '2.7.1'
+VERSION = '2.7.2'
 
 setup(
     name='scratchcommunication',
     version=VERSION,
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
```

### Comparing `scratchcommunication-2.7.1/tests/test1.py` & `scratchcommunication-2.7.2/tests/test1.py`

 * *Files identical despite different names*
