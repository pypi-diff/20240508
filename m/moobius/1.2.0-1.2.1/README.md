# Comparing `tmp/moobius-1.2.0.tar.gz` & `tmp/moobius-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moobius-1.2.0.tar", last modified: Fri Apr 26 06:14:47 2024, max compression
+gzip compressed data, was "moobius-1.2.1.tar", last modified: Wed May  8 03:40:28 2024, max compression
```

## Comparing `moobius-1.2.0.tar` & `moobius-1.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 06:14:47.241967 moobius-1.2.0/
--rw-rw-rw-   0        0        0     8910 2024-04-26 06:14:47.240970 moobius-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2024-03-24 16:36:44.000000 moobius-1.2.0/license.md
--rw-rw-rw-   0        0        0      647 2024-04-26 06:06:56.000000 moobius-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     8055 2024-03-17 18:58:55.000000 moobius-1.2.0/readme.md
--rw-rw-rw-   0        0        0       42 2024-04-26 06:14:47.241967 moobius-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 06:14:47.220204 moobius-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 06:14:47.223898 moobius-1.2.0/src/moobius/
--rw-rw-rw-   0        0        0      184 2024-03-05 05:12:19.000000 moobius-1.2.0/src/moobius/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:14:47.231846 moobius-1.2.0/src/moobius/core/
--rw-rw-rw-   0        0        0    57654 2024-04-24 21:24:30.000000 moobius-1.2.0/src/moobius/core/sdk.py
--rw-rw-rw-   0        0        0     4170 2024-04-01 21:02:47.000000 moobius-1.2.0/src/moobius/core/wand.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:14:47.235837 moobius-1.2.0/src/moobius/database/
--rw-rw-rw-   0        0        0     2655 2024-03-13 15:36:04.000000 moobius-1.2.0/src/moobius/database/database_interface.py
--rw-rw-rw-   0        0        0     4435 2024-04-26 04:20:23.000000 moobius-1.2.0/src/moobius/database/json_database.py
--rw-rw-rw-   0        0        0      902 2024-02-16 02:53:33.000000 moobius-1.2.0/src/moobius/database/null_database.py
--rw-rw-rw-   0        0        0     1517 2024-03-25 06:01:03.000000 moobius-1.2.0/src/moobius/database/redis_database.py
--rw-rw-rw-   0        0        0     9708 2024-04-26 05:53:24.000000 moobius-1.2.0/src/moobius/database/storage.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:14:47.238977 moobius-1.2.0/src/moobius/network/
--rw-rw-rw-   0        0        0    14222 2024-04-01 23:40:33.000000 moobius-1.2.0/src/moobius/network/asserts.py
--rw-rw-rw-   0        0        0    45076 2024-04-24 18:33:19.000000 moobius-1.2.0/src/moobius/network/http_api_wrapper.py
--rw-rw-rw-   0        0        0    25652 2024-04-10 03:05:43.000000 moobius-1.2.0/src/moobius/network/ws_client.py
--rw-rw-rw-   0        0        0     7154 2024-04-08 21:51:19.000000 moobius-1.2.0/src/moobius/types.py
--rw-rw-rw-   0        0        0     7399 2024-04-23 19:30:39.000000 moobius-1.2.0/src/moobius/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-26 06:14:47.239979 moobius-1.2.0/src/moobius.egg-info/
--rw-rw-rw-   0        0        0     8910 2024-04-26 06:14:47.000000 moobius-1.2.0/src/moobius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2024-04-26 06:14:47.000000 moobius-1.2.0/src/moobius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 06:14:47.000000 moobius-1.2.0/src/moobius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2024-04-26 06:14:47.000000 moobius-1.2.0/src/moobius.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-26 06:14:47.000000 moobius-1.2.0/src/moobius.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      329 2024-04-08 18:24:26.000000 moobius-1.2.0/src/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:40:28.503814 moobius-1.2.1/
+-rw-rw-rw-   0        0        0     8946 2024-05-08 03:40:28.502841 moobius-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2024-03-25 06:01:03.000000 moobius-1.2.1/license.md
+-rw-rw-rw-   0        0        0      647 2024-05-08 03:33:36.000000 moobius-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     8091 2024-03-26 23:06:54.000000 moobius-1.2.1/readme.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 03:40:28.503814 moobius-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 03:40:28.483356 moobius-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 03:40:28.486276 moobius-1.2.1/src/moobius/
+-rw-rw-rw-   0        0        0      184 2024-03-05 05:12:19.000000 moobius-1.2.1/src/moobius/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:40:28.493088 moobius-1.2.1/src/moobius/core/
+-rw-rw-rw-   0        0        0    57654 2024-04-24 21:24:30.000000 moobius-1.2.1/src/moobius/core/sdk.py
+-rw-rw-rw-   0        0        0     4170 2024-05-04 16:47:45.000000 moobius-1.2.1/src/moobius/core/wand.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:40:28.496982 moobius-1.2.1/src/moobius/database/
+-rw-rw-rw-   0        0        0     2655 2024-03-13 15:36:04.000000 moobius-1.2.1/src/moobius/database/database_interface.py
+-rw-rw-rw-   0        0        0     4435 2024-04-26 06:18:04.000000 moobius-1.2.1/src/moobius/database/json_database.py
+-rw-rw-rw-   0        0        0      902 2024-02-16 02:53:33.000000 moobius-1.2.1/src/moobius/database/null_database.py
+-rw-rw-rw-   0        0        0     1517 2024-03-25 06:01:03.000000 moobius-1.2.1/src/moobius/database/redis_database.py
+-rw-rw-rw-   0        0        0     9708 2024-04-26 06:18:04.000000 moobius-1.2.1/src/moobius/database/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:40:28.500881 moobius-1.2.1/src/moobius/network/
+-rw-rw-rw-   0        0        0    14222 2024-04-01 23:40:33.000000 moobius-1.2.1/src/moobius/network/asserts.py
+-rw-rw-rw-   0        0        0    45076 2024-04-24 18:33:19.000000 moobius-1.2.1/src/moobius/network/http_api_wrapper.py
+-rw-rw-rw-   0        0        0    25820 2024-05-04 17:20:19.000000 moobius-1.2.1/src/moobius/network/ws_client.py
+-rw-rw-rw-   0        0        0     7154 2024-04-08 21:51:19.000000 moobius-1.2.1/src/moobius/types.py
+-rw-rw-rw-   0        0        0     7399 2024-04-23 19:30:39.000000 moobius-1.2.1/src/moobius/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:40:28.501867 moobius-1.2.1/src/moobius.egg-info/
+-rw-rw-rw-   0        0        0     8946 2024-05-08 03:40:28.000000 moobius-1.2.1/src/moobius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2024-05-08 03:40:28.000000 moobius-1.2.1/src/moobius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 03:40:28.000000 moobius-1.2.1/src/moobius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2024-05-08 03:40:28.000000 moobius-1.2.1/src/moobius.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-08 03:40:28.000000 moobius-1.2.1/src/moobius.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      329 2024-04-08 18:24:26.000000 moobius-1.2.1/src/setup.py
```

### Comparing `moobius-1.2.0/PKG-INFO` & `moobius-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moobius
-Version: 1.2.0
+Version: 1.2.1
 Summary: Moobius Platform SDK
 Author-email: Kevin Kostlan <sdk@moobius.app>
 Project-URL: Homepage, https://github.com/groupultra/sdk-public
 Project-URL: Issues, https://github.com/groupultra/sdk-public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 Requires-Dist: APScheduler>=3.10.4
 Requires-Dist: dacite>=1.8.1
 Requires-Dist: redis>=5.0.1
 Requires-Dist: Requests>=2.31.0
 Requires-Dist: websockets>=12.0
 Requires-Dist: loguru>=0.7.2
 
-# Welcome to Moobius Python SDK (Version 1.0.0)!
+# Welcome to Moobius Python SDK (Version 1.x.y)!
 
 ## Quick Start (Requires Python 3.10+)
 
 **Setup your account**
 
 Register an account on [Moobius](http://www.moobius.net). You have to enter an email and password to use this SDK. Third-party logins are not supported.
 
@@ -59,15 +59,15 @@
 
 ## Glossery / Reference
 
 1. **Tutorials:** In `projects/demo` there are `DemoServiceTutorial.md` and `DemoAgentTutorial.md` walkthroughs.
 
 2. **Service:** The Service handles most of the interaction with the platform SDK. This includes sending and responding to messages, controlling the look and feel, and uploading assets. Callbacks have the format `on_xyz` and actuators have the format `send_xyz`. JSON is automatically converted to and from *dataclasses* within `types.py`.
 
-3. **Agent:** Like *service*, the agent overrides the `Moobius` class and is constructed with `is_agent` set to True. However, the agent is more limited in it's functionality: it cannot do much besides sending and recieving messages and modifying itself. Most other functions will generate an error. To use an agent under a given account requires knowing the secret credentials. Services call `send_message_down` while users and agents call `send_message_up`.
+3. **Agent:** Like *service*, the agent overrides the `Moobius` class and is constructed with `is_agent` set to True. However, the agent is more limited in it's functionality: it cannot do much besides sending and recieving messages and modifying itself. Most other functions will generate an error. To use an agent under a given account requires knowing the secret credentials. Services internally call `self.ws_client.message_down` while users and agents call `self.ws_client.send_message_up`.
 
 4. **Databases:** Databases are client-side and represented as `MoobiusStorage` instances. The structure is determined by a configuration file (usually `./config/db.json`). Each element has a `name` that is *directly written instance's attributes*. Each element also contains an `implementation` which determines the database engine; currently "json" and "redis" is supported. The Demo by default will only run "redis" on Linux and Mac.
 
 5. **Logging:** Logging uses [Loguru](https://loguru.readthedocs.io/en/stable/), a colorful, comprehensive logging system. Simply replace `print` with `logging.info()`, `logging.error()`, or `logging.error()` for a thread-safe logging that also saves to the disk. It has plenty of other [features](https://loguru.readthedocs.io/en/stable/) as well.
 
 6. **Wand:** The `MoobiusWand` class launches and manages one or more services. The services can either run on the Wand's process (recommended for simple tasks) or on a seperate process with `background=True`. Using a background service requires moving initialization of unpickable objects to `on_start()`. Use `wand.spell()` or `await wand.aspell()` to have the wand interact with the service by calling the `on_spell()` callback.
```

### Comparing `moobius-1.2.0/license.md` & `moobius-1.2.1/license.md`

 * *Files identical despite different names*

### Comparing `moobius-1.2.0/pyproject.toml` & `moobius-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "moobius"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Kevin Kostlan", email="sdk@moobius.app"},
 ]
 description = "Moobius Platform SDK"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `moobius-1.2.0/readme.md` & `moobius-1.2.1/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Welcome to Moobius Python SDK (Version 1.0.0)!
+# Welcome to Moobius Python SDK (Version 1.x.y)!
 
 ## Quick Start (Requires Python 3.10+)
 
 **Setup your account**
 
 Register an account on [Moobius](http://www.moobius.net). You have to enter an email and password to use this SDK. Third-party logins are not supported.
 
@@ -37,15 +37,15 @@
 
 ## Glossery / Reference
 
 1. **Tutorials:** In `projects/demo` there are `DemoServiceTutorial.md` and `DemoAgentTutorial.md` walkthroughs.
 
 2. **Service:** The Service handles most of the interaction with the platform SDK. This includes sending and responding to messages, controlling the look and feel, and uploading assets. Callbacks have the format `on_xyz` and actuators have the format `send_xyz`. JSON is automatically converted to and from *dataclasses* within `types.py`.
 
-3. **Agent:** Like *service*, the agent overrides the `Moobius` class and is constructed with `is_agent` set to True. However, the agent is more limited in it's functionality: it cannot do much besides sending and recieving messages and modifying itself. Most other functions will generate an error. To use an agent under a given account requires knowing the secret credentials. Services call `send_message_down` while users and agents call `send_message_up`.
+3. **Agent:** Like *service*, the agent overrides the `Moobius` class and is constructed with `is_agent` set to True. However, the agent is more limited in it's functionality: it cannot do much besides sending and recieving messages and modifying itself. Most other functions will generate an error. To use an agent under a given account requires knowing the secret credentials. Services internally call `self.ws_client.message_down` while users and agents call `self.ws_client.send_message_up`.
 
 4. **Databases:** Databases are client-side and represented as `MoobiusStorage` instances. The structure is determined by a configuration file (usually `./config/db.json`). Each element has a `name` that is *directly written instance's attributes*. Each element also contains an `implementation` which determines the database engine; currently "json" and "redis" is supported. The Demo by default will only run "redis" on Linux and Mac.
 
 5. **Logging:** Logging uses [Loguru](https://loguru.readthedocs.io/en/stable/), a colorful, comprehensive logging system. Simply replace `print` with `logging.info()`, `logging.error()`, or `logging.error()` for a thread-safe logging that also saves to the disk. It has plenty of other [features](https://loguru.readthedocs.io/en/stable/) as well.
 
 6. **Wand:** The `MoobiusWand` class launches and manages one or more services. The services can either run on the Wand's process (recommended for simple tasks) or on a seperate process with `background=True`. Using a background service requires moving initialization of unpickable objects to `on_start()`. Use `wand.spell()` or `await wand.aspell()` to have the wand interact with the service by calling the `on_spell()` callback.
```

### Comparing `moobius-1.2.0/src/moobius/core/sdk.py` & `moobius-1.2.1/src/moobius/core/sdk.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.0/src/moobius/core/wand.py` & `moobius-1.2.1/src/moobius/core/wand.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.0/src/moobius/database/database_interface.py` & `moobius-1.2.1/src/moobius/database/database_interface.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.0/src/moobius/database/json_database.py` & `moobius-1.2.1/src/moobius/database/json_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.0/src/moobius/database/null_database.py` & `moobius-1.2.1/src/moobius/database/null_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.0/src/moobius/database/redis_database.py` & `moobius-1.2.1/src/moobius/database/redis_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.0/src/moobius/database/storage.py` & `moobius-1.2.1/src/moobius/database/storage.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.0/src/moobius/network/asserts.py` & `moobius-1.2.1/src/moobius/network/asserts.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.0/src/moobius/network/http_api_wrapper.py` & `moobius-1.2.1/src/moobius/network/http_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.0/src/moobius/network/ws_client.py` & `moobius-1.2.1/src/moobius/network/ws_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,21 +75,25 @@
         asserts.socket_assert(json.loads(message))
         try:
             logger.opt(colors=True).info(f"<fg 128,0,240>{message.replace('<', '&lt;').replace('>', '&gt;')}</>")
             while self.is_reconnecting: # Cannot use an async.lock() for this b/c doing so would make self.send() block itself.
                 await asyncio.sleep(0.01)
             await self.websocket.send(message)  # Don't use asyncio.create_task() here, or the message could not be sent in order
         except websockets.exceptions.ConnectionClosed as e:
+            if self.is_reconnecting: # Already reconnecting.
+                return
             self.is_reconnecting = True
             logger.info(f"Connection closed: {e}. Attempting to reconnect...")
             await self.connect()
             logger.info("Reconnected! Attempting to send message again...")
             self.is_reconnecting = False
             await self.websocket.send(message)
         except Exception as e:
+            if self.is_reconnecting: # Already reconnecting.
+                return
             logger.error(f'Error with websocket.send: {e}')
             await self.connect()
             logger.info("Reconnected! Attempting to send message again, which is a long shot for non ConnectionClosed Exceptions...")
             await self.websocket.send(message)
 
     async def receive(self):
         """
```

### Comparing `moobius-1.2.0/src/moobius/types.py` & `moobius-1.2.1/src/moobius/types.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.0/src/moobius/utils.py` & `moobius-1.2.1/src/moobius/utils.py`

 * *Files identical despite different names*

### Comparing `moobius-1.2.0/src/moobius.egg-info/PKG-INFO` & `moobius-1.2.1/src/moobius.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moobius
-Version: 1.2.0
+Version: 1.2.1
 Summary: Moobius Platform SDK
 Author-email: Kevin Kostlan <sdk@moobius.app>
 Project-URL: Homepage, https://github.com/groupultra/sdk-public
 Project-URL: Issues, https://github.com/groupultra/sdk-public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 Requires-Dist: APScheduler>=3.10.4
 Requires-Dist: dacite>=1.8.1
 Requires-Dist: redis>=5.0.1
 Requires-Dist: Requests>=2.31.0
 Requires-Dist: websockets>=12.0
 Requires-Dist: loguru>=0.7.2
 
-# Welcome to Moobius Python SDK (Version 1.0.0)!
+# Welcome to Moobius Python SDK (Version 1.x.y)!
 
 ## Quick Start (Requires Python 3.10+)
 
 **Setup your account**
 
 Register an account on [Moobius](http://www.moobius.net). You have to enter an email and password to use this SDK. Third-party logins are not supported.
 
@@ -59,15 +59,15 @@
 
 ## Glossery / Reference
 
 1. **Tutorials:** In `projects/demo` there are `DemoServiceTutorial.md` and `DemoAgentTutorial.md` walkthroughs.
 
 2. **Service:** The Service handles most of the interaction with the platform SDK. This includes sending and responding to messages, controlling the look and feel, and uploading assets. Callbacks have the format `on_xyz` and actuators have the format `send_xyz`. JSON is automatically converted to and from *dataclasses* within `types.py`.
 
-3. **Agent:** Like *service*, the agent overrides the `Moobius` class and is constructed with `is_agent` set to True. However, the agent is more limited in it's functionality: it cannot do much besides sending and recieving messages and modifying itself. Most other functions will generate an error. To use an agent under a given account requires knowing the secret credentials. Services call `send_message_down` while users and agents call `send_message_up`.
+3. **Agent:** Like *service*, the agent overrides the `Moobius` class and is constructed with `is_agent` set to True. However, the agent is more limited in it's functionality: it cannot do much besides sending and recieving messages and modifying itself. Most other functions will generate an error. To use an agent under a given account requires knowing the secret credentials. Services internally call `self.ws_client.message_down` while users and agents call `self.ws_client.send_message_up`.
 
 4. **Databases:** Databases are client-side and represented as `MoobiusStorage` instances. The structure is determined by a configuration file (usually `./config/db.json`). Each element has a `name` that is *directly written instance's attributes*. Each element also contains an `implementation` which determines the database engine; currently "json" and "redis" is supported. The Demo by default will only run "redis" on Linux and Mac.
 
 5. **Logging:** Logging uses [Loguru](https://loguru.readthedocs.io/en/stable/), a colorful, comprehensive logging system. Simply replace `print` with `logging.info()`, `logging.error()`, or `logging.error()` for a thread-safe logging that also saves to the disk. It has plenty of other [features](https://loguru.readthedocs.io/en/stable/) as well.
 
 6. **Wand:** The `MoobiusWand` class launches and manages one or more services. The services can either run on the Wand's process (recommended for simple tasks) or on a seperate process with `background=True`. Using a background service requires moving initialization of unpickable objects to `on_start()`. Use `wand.spell()` or `await wand.aspell()` to have the wand interact with the service by calling the `on_spell()` callback.
```

### Comparing `moobius-1.2.0/src/moobius.egg-info/SOURCES.txt` & `moobius-1.2.1/src/moobius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

