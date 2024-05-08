# Comparing `tmp/pyircsdk-1.2.0.tar.gz` & `tmp/pyircsdk-1.3.0.tar.gz`

## Comparing `pyircsdk-1.2.0.tar` & `pyircsdk-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyircsdk/__about__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyircsdk/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyircsdk/command.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyircsdk/message.py
--rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyircsdk/pyircsdk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyircsdk/event/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyircsdk/event/event.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/LICENSE
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/README.md
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pyircsdk-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyircsdk-1.3.0/pyircsdk/__about__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyircsdk-1.3.0/pyircsdk/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 pyircsdk-1.3.0/pyircsdk/command.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pyircsdk-1.3.0/pyircsdk/message.py
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 pyircsdk-1.3.0/pyircsdk/pyircsdk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyircsdk-1.3.0/pyircsdk/event/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pyircsdk-1.3.0/pyircsdk/event/event.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyircsdk-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyircsdk-1.3.0/LICENSE
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyircsdk-1.3.0/README.md
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyircsdk-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pyircsdk-1.3.0/PKG-INFO
```

### Comparing `pyircsdk-1.2.0/pyircsdk/command.py` & `pyircsdk-1.3.0/pyircsdk/command.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.2.0/pyircsdk/message.py` & `pyircsdk-1.3.0/pyircsdk/message.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.2.0/pyircsdk/pyircsdk.py` & `pyircsdk-1.3.0/pyircsdk/pyircsdk.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,90 @@
 import socket
+import ssl
 import sys
+from dataclasses import dataclass
 
 from .event.event import Event
 from .message import Message
 
+@dataclass
 class IRCSDKConfig:
-    def __init__(self, host, port, nick, channel, user, realname):
-        self.host = host
-        self.port = port
-        self.nick = nick
-        self.channel = channel
-        self.user = user
-        self.realname = realname
+    host: str
+    port: int
+    nick: str
+    channel: str
+    user: str
+    realname: str
+    password: str
+    ssl: bool
+
+    def __init__(self,  **kwargs):
+        for k in self.__dataclass_fields__:
+            setattr(self, k, None)
+
+        for k, v in kwargs.items():
+            setattr(self, k, v)
+
 
     def __str__(self):
         return f'Host: {self.host}, Port: {self.port}, Nick: {self.nick}, Channel: {self.channel}, User: {self.user}'
 
     def __repr__(self):
         return f'Host: {self.host}, Port: {self.port}, Nick: {self.nick}, Channel: {self.channel}, User: {self.user}'
 
 
 class IRCSDK:
     def __init__(self, config: IRCSDKConfig = None) -> None:
         self.event: Event = Event()
         if config:
             self.config = config
             self.irc = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            if self.config.ssl:
+                self.sslContext = ssl.create_default_context()
 
     def privmsg(self, receiver: str, msg: str) -> None:
         command = "PRIVMSG %s :%s\r\n" % (receiver, msg)
         self.irc.send(command.encode('utf-8'))
 
     def sendRaw(self, msg: str) -> None:
         self.irc.send(msg.encode('utf-8'))
 
     def close(self) -> None:
         message = "QUIT :%s\r\n" % self.config.nick
         self.irc.send(message.encode('utf-8'))
         self.irc.close()
 
+    def sendPassword(self, password: str) -> None:
+        message = f"PASS {password}\r\n"
+        self.irc.send(message.encode('utf-8'))
+
+
     def connect(self, config: IRCSDKConfig = None) -> None:
         # if no config use __init__ config
         if not config:
             config = self.config
 
         # if no config is passed throw an error
         if not self.config:
             raise ValueError('No config passed to connect')
 
         self.irc: socket.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        if self.config.ssl:
+            self.irc: socket.socket = self.sslContext.wrap_socket(self.irc, server_hostname=self.config.host)
         # print config
         print(config)
 
         self.irc.connect((self.config.host, self.config.port))
         self.event.emit('connected', 'Connected to host %s:%s' % (self.config.host, self.config.port))
 
         self.event.on('raw', self.log)
         self.event.on('raw', self.handle_raw_message)
+        if self.config.password:
+            self.sendPassword(self.config.password)
+
         self.setUser(self.config.user, self.config.realname)
         self.setNick(self.config.nick)
 
         self.event.on('connected', lambda data: self.join(self.config.channel))
         self.startRecv()
 
     def startRecv(self) -> None:
```

### Comparing `pyircsdk-1.2.0/pyircsdk/event/event.py` & `pyircsdk-1.3.0/pyircsdk/event/event.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.2.0/.gitignore` & `pyircsdk-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.2.0/LICENSE` & `pyircsdk-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.2.0/README.md` & `pyircsdk-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.2.0/pyproject.toml` & `pyircsdk-1.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "pyircsdk"
 authors = [
   { name="Bludot", email="admin@floretos.com" },
 ]
-version = "1.2.0"
+version = "1.3.0"
 description = "pyIRCSDK is a Python library for creating IRC bots and clients. It is designed to provide granular access to raw mesages and to provide an event emitter like interface for handling messages."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyircsdk-1.2.0/PKG-INFO` & `pyircsdk-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyircsdk
-Version: 1.2.0
+Version: 1.3.0
 Summary: pyIRCSDK is a Python library for creating IRC bots and clients. It is designed to provide granular access to raw mesages and to provide an event emitter like interface for handling messages.
 Project-URL: Homepage, https://github.com/bludot/pyircsdk
 Project-URL: Issues, https://github.com/bludot/pyircsdk/issues
 Author-email: Bludot <admin@floretos.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

