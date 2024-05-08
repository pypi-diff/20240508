# Comparing `tmp/darklock-0.1.2.tar.gz` & `tmp/darklock-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darklock-0.1.2.tar", last modified: Thu Apr 25 17:38:21 2024, max compression
+gzip compressed data, was "darklock-0.1.3.tar", last modified: Wed May  8 18:16:28 2024, max compression
```

## Comparing `darklock-0.1.2.tar` & `darklock-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:21.623223 darklock-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 17:38:17.000000 darklock-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-25 17:38:21.623223 darklock-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-25 17:38:17.000000 darklock-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:38:21.623223 darklock-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-25 17:38:17.000000 darklock-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:21.619223 darklock-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:21.619223 darklock-0.1.2/src/darklock/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-25 17:38:17.000000 darklock-0.1.2/src/darklock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-25 17:38:17.000000 darklock-0.1.2/src/darklock/log_disc_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-25 17:38:17.000000 darklock-0.1.2/src/darklock/no_internet_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-25 17:38:17.000000 darklock-0.1.2/src/darklock/restrict_network_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-25 17:38:17.000000 darklock-0.1.2/src/darklock/restrict_os_access.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-25 17:38:17.000000 darklock-0.1.2/src/darklock/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:21.623223 darklock-0.1.2/src/darklock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-25 17:38:21.000000 darklock-0.1.2/src/darklock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-25 17:38:21.000000 darklock-0.1.2/src/darklock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:38:21.000000 darklock-0.1.2/src/darklock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 17:38:21.000000 darklock-0.1.2/src/darklock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:38:21.623223 darklock-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-25 17:38:17.000000 darklock-0.1.2/tests/test_no_internet_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-25 17:38:17.000000 darklock-0.1.2/tests/test_restrict_internet_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-25 17:38:17.000000 darklock-0.1.2/tests/test_restrict_os.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:28.422464 darklock-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 18:16:24.000000 darklock-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-08 18:16:28.422464 darklock-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-08 18:16:24.000000 darklock-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:16:28.422464 darklock-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-08 18:16:24.000000 darklock-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:28.418464 darklock-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:28.418464 darklock-0.1.3/src/darklock/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-08 18:16:24.000000 darklock-0.1.3/src/darklock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-08 18:16:24.000000 darklock-0.1.3/src/darklock/log_disc_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-08 18:16:24.000000 darklock-0.1.3/src/darklock/no_internet_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-08 18:16:24.000000 darklock-0.1.3/src/darklock/restrict_network_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-08 18:16:24.000000 darklock-0.1.3/src/darklock/restrict_os_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-08 18:16:24.000000 darklock-0.1.3/src/darklock/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:28.422464 darklock-0.1.3/src/darklock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-08 18:16:28.000000 darklock-0.1.3/src/darklock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-08 18:16:28.000000 darklock-0.1.3/src/darklock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:16:28.000000 darklock-0.1.3/src/darklock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 18:16:28.000000 darklock-0.1.3/src/darklock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:28.422464 darklock-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-08 18:16:24.000000 darklock-0.1.3/tests/test_no_internet_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 18:16:24.000000 darklock-0.1.3/tests/test_restrict_internet_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-08 18:16:24.000000 darklock-0.1.3/tests/test_restrict_os.py
```

### Comparing `darklock-0.1.2/LICENSE` & `darklock-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `darklock-0.1.2/PKG-INFO` & `darklock-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darklock
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://github.com/Capsize-Games/darklock
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `darklock-0.1.2/README.md` & `darklock-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `darklock-0.1.2/setup.py` & `darklock-0.1.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="darklock",
-    version="0.1.2",
+    version="0.1.3",
     author="Capsize LLC",
     description="",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="",
     license="GPL-3.0",
     author_email="contact@capsizegames.com",
```

### Comparing `darklock-0.1.2/src/darklock/__init__.py` & `darklock-0.1.3/src/darklock/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 def activate(
     whitelisted_operations: list = None,
     whitelisted_filenames: list = None,
     whitelisted_imports: list = None,
     blacklisted_filenames: list = None,
 ):
-    network.activate()
+    # network.activate(
+    #     allowed_port=4222
+    # )
     os.activate(
         whitelisted_operations,
         whitelisted_filenames,
         whitelisted_imports,
         blacklisted_filenames,
     )
```

### Comparing `darklock-0.1.2/src/darklock/no_internet_socket.py` & `darklock-0.1.3/src/darklock/no_internet_socket.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,41 @@
 import logging
+import socket
 
-
-class NoInternetSocket:
+class NoInternetSocket(socket.socket):
     """
-    A custom socket class that prevents any form of internet connections.
-
-    This class overrides the default socket object in Python's socket module to ensure that
-    no outgoing or incoming internet connections can be established. Attempting to create
-    or use a socket connection will result in a ConnectionError.
-
-    Methods:
-        __init__(*args, **kwargs): Constructor for the socket object that raises an error.
-        connect(*args, **kwargs): Method that simulates the connect functionality and raises an error.
+    A custom socket class that prevents any form of internet connections except for localhost on a specified port.
     """
 
     def __init__(self, *args, **kwargs):
-        """
-        Initializes a new instance of the socket object and logs the attempt.
-
-        Args:
-            *args: Variable length argument list.
-            **kwargs: Arbitrary keyword arguments.
-
-        Raises:
-            ConnectionError: Always thrown to indicate that network connections are disabled.
-        """
+        super().__init__(*args, **kwargs)
         self.__init_logger()
-        self.logger.info("Socket creation attempted and blocked.")
-        raise ConnectionError("This application does not allow internet connections.")
 
     def __init_logger(self):
         self.logger = logging.getLogger(__name__)
         handler = logging.FileHandler('network_access_attempts.log')
         formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
         handler.setFormatter(formatter)
         self.logger.addHandler(handler)
         self.logger.setLevel(logging.INFO)
 
-    def connect(self, *args, **kwargs):
+    def connect(self, address):
         """
-        Simulates the behavior of the socket's `connect` method. This override is specifically
-        designed to log and block any attempts to establish a connection using the socket object.
+        Overrides the socket's `connect` method to allow connections only to localhost on a specific port.
 
         Args:
-            *args: Variable length argument list.
-            **kwargs: Arbitrary keyword arguments.
+            address (tuple): A tuple of (host, port)
 
         Raises:
-            ConnectionError: Always thrown to prevent any form of network connection.
+            ConnectionError: If the connection attempt is to an address other than localhost on the allowed port.
         """
-        self.__init_logger()
-        self.logger.info("Connection attempt blocked.")
-        raise ConnectionError("This application does not allow internet connections.")
+        host, port = address
+        if host == '127.0.0.1' and port == self.allowed_port:
+            super().connect(address)
+            self.logger.info(f"Allowed connection to {host} on port {port}.")
+        else:
+            self.logger.info(f"Blocked connection attempt to {host} on port {port}.")
+            raise ConnectionError(f"Connection to {host} on port {port} is not allowed.")
+
+    @classmethod
+    def set_allowed_port(cls, port):
+        cls.allowed_port = port
```

### Comparing `darklock-0.1.2/src/darklock/restrict_network_access.py` & `darklock-0.1.3/src/darklock/restrict_network_access.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 import socket
 import logging
+
 from darklock.no_internet_socket import NoInternetSocket
 from darklock.singleton import Singleton
 
-
 class RestrictNetworkAccess(metaclass=Singleton):
     def __init__(self):
         self.__init_logger()
         self.original_socket = socket.socket
-        self.original_socket_type = socket.SocketType
 
     def __init_logger(self):
         """
         Initializes the logger with a file handler and a specific format.
         """
         logging.basicConfig(level=logging.INFO)
         self.logger = logging.getLogger(__name__)
-        # handler = logging.FileHandler('network_access_attempts.log')
         handler = logging.StreamHandler()
-        handler.setLevel(logging.INFO)  # Set the handler's level to INFO
         formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
         handler.setFormatter(formatter)
         self.logger.addHandler(handler)
         self.logger.setLevel(logging.INFO)
 
-    def activate(self):
-        self.logger.info("Installing network restrictions.")
-        self.original_socket = socket.socket
-        self.original_socket_type = socket.SocketType
+    def activate(self, allowed_port):
+        self.logger.info("Activating network restrictions")
+        NoInternetSocket.set_allowed_port(allowed_port)
         socket.socket = NoInternetSocket
-        socket.SocketType = NoInternetSocket
 
     def deactivate(self):
-        self.logger.info("Uninstalling network restrictions.")
+        self.logger.info("Deactivating network restrictions")
         socket.socket = self.original_socket
-        socket.SocketType = self.original_socket_type
```

### Comparing `darklock-0.1.2/src/darklock/restrict_os_access.py` & `darklock-0.1.3/src/darklock/restrict_os_access.py`

 * *Files identical despite different names*

### Comparing `darklock-0.1.2/src/darklock.egg-info/PKG-INFO` & `darklock-0.1.3/src/darklock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darklock
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://github.com/Capsize-Games/darklock
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `darklock-0.1.2/tests/test_restrict_internet_access.py` & `darklock-0.1.3/tests/test_restrict_internet_access.py`

 * *Files identical despite different names*

### Comparing `darklock-0.1.2/tests/test_restrict_os.py` & `darklock-0.1.3/tests/test_restrict_os.py`

 * *Files identical despite different names*

