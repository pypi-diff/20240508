# Comparing `tmp/pop_cli-7.0.0.tar.gz` & `tmp/pop_cli-7.0.1.tar.gz`

## Comparing `pop_cli-7.0.0.tar` & `pop_cli-7.0.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pop_cli-7.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pop_cli-7.0.0/setup.py
--rwxr-xr-x   0        0        0     1000 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/hub/__main__.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/config.yaml
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/cli.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/completer.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/config.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/console.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/init.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/legacy.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/ref.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/state.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/conftest.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/integration/test_cli.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/integration/test_config.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/integration/test_console.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/integration/test_init.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/integration/test_ref.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/integration/test_state.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/tpath/plugin/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/tpath/plugin/src/init.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/tpath/plugin/src/mod.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-7.0.0/.gitignore
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-7.0.0/README.rst
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pop_cli-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pop_cli-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pop_cli-7.0.1/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     1028 2020-02-02 00:00:00.000000 pop_cli-7.0.1/src/hub/__main__.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pop_cli-7.0.1/src/pop_cli/config.yaml
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 pop_cli-7.0.1/src/pop_cli/plugin/cli.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 pop_cli-7.0.1/src/pop_cli/plugin/completer.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 pop_cli-7.0.1/src/pop_cli/plugin/config.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pop_cli-7.0.1/src/pop_cli/plugin/console.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pop_cli-7.0.1/src/pop_cli/plugin/init.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 pop_cli-7.0.1/src/pop_cli/plugin/legacy.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 pop_cli-7.0.1/src/pop_cli/plugin/ref.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pop_cli-7.0.1/src/pop_cli/plugin/state.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pop_cli-7.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-7.0.1/tests/integration/test_cli.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-7.0.1/tests/integration/test_config.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-7.0.1/tests/integration/test_console.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-7.0.1/tests/integration/test_init.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pop_cli-7.0.1/tests/integration/test_ref.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pop_cli-7.0.1/tests/integration/test_state.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-7.0.1/tests/tpath/plugin/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-7.0.1/tests/tpath/plugin/src/init.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-7.0.1/tests/tpath/plugin/src/mod.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-7.0.1/.gitignore
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-7.0.1/README.rst
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pop_cli-7.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pop_cli-7.0.1/PKG-INFO
```

### Comparing `pop_cli-7.0.0/.pre-commit-config.yaml` & `pop_cli-7.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/src/hub/__main__.py` & `pop_cli-7.0.1/src/hub/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,30 +15,30 @@
         loop.close()
 
 
 async def amain(loop):
     async with cpop.hub.Hub(cli="cli") as hub:
         await hub.log.debug("Initialized the hub")
 
+        hold = asyncio.create_task(hub._holder())
+
         if "legacy" in hub.cli:
             await hub.cli.legacy.patch(loop=loop)
 
-        # Start the hub cli
-        hold = asyncio.create_task(hub._holder())
-
         try:
+            # Start the hub cli
             await hub.cli.init.run()
         except KeyboardInterrupt:
             await hub.log.error("Caught keyboard interrupt.  Cancelling...")
         except SystemExit:
             ...
         finally:
             await hub.log.debug("Cleaning up")
             await hub._tasks.put(cpop.hub.SHUTDOWN_SIGNAL)
             await asyncio.sleep(0)
-
-            await hold
+            if hold:
+                await hold
             await loop.shutdown_asyncgens()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pop_cli-7.0.0/src/pop_cli/config.yaml` & `pop_cli-7.0.1/src/pop_cli/config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/src/pop_cli/plugin/cli.py` & `pop_cli-7.0.1/src/pop_cli/plugin/cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/src/pop_cli/plugin/completer.py` & `pop_cli-7.0.1/src/pop_cli/plugin/completer.py`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/src/pop_cli/plugin/config.py` & `pop_cli-7.0.1/src/pop_cli/plugin/config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/src/pop_cli/plugin/console.py` & `pop_cli-7.0.1/src/pop_cli/plugin/console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/src/pop_cli/plugin/init.py` & `pop_cli-7.0.1/src/pop_cli/plugin/init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/src/pop_cli/plugin/legacy.py` & `pop_cli-7.0.1/src/pop_cli/plugin/legacy.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,30 +19,32 @@
     hub.legacy.pop.loop.CURRENT_LOOP = loop
 
     await hub.log.debug("Loading all dynes under legacy hub")
     for dyne in hub.legacy._dynamic:
         hub.legacy.pop.sub.add(dyne_name=dyne)
         hub.legacy.pop.sub.load_subdirs(hub.legacy[dyne], recurse=True)
 
-    # Patch the legacy hub's logger with a log eater for pop-config's noisy logger
+    # Patch the legacy hub's logger with trace logging for pop-config's noisy logger
     for name in LOG_NAMES:
-        setattr(hub.legacy.log, name, lambda *_, **__: ...)
+        setattr(
+            hub.legacy.log, name, lambda *a, **kw: hub._auto(hub.log.trace(*a, **kw))
+        )
 
     # Populate the legacy hub's OPT
     dyne_names = list(hub.legacy._dynamic.keys())
 
     config_dynes = hub.legacy.config.dirs.find_configs(dyne_names)
     hub.legacy.pop.config.load(
         list(config_dynes.keys()), "pop_config", dyne_names, parse_cli=False, logs=False
     )
 
     # Patch the legacy hub's logger with cpop's logger
     for name in LOG_NAMES:
         setattr(
-            hub.legacy.log, name, lambda *a, **kw: hub._auto(hub.log[name](*a, **kw))
+            hub.legacy.log, name, lambda *a, __name=name, **kw: hub._auto(hub.log[__name](*a, **kw))
         )
 
     # Add the legacy hub's subs to the search path of the main hub
     hub += hub.legacy._subs
 
     # Extend subs from both pop versions
     await hub.log.debug("Extending cpop hub attrs with pop hub attrs")
```

### Comparing `pop_cli-7.0.0/src/pop_cli/plugin/ref.py` & `pop_cli-7.0.1/src/pop_cli/plugin/ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/src/pop_cli/plugin/state.py` & `pop_cli-7.0.1/src/pop_cli/plugin/state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/tests/conftest.py` & `pop_cli-7.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/tests/integration/test_cli.py` & `pop_cli-7.0.1/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/tests/integration/test_config.py` & `pop_cli-7.0.1/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/tests/integration/test_console.py` & `pop_cli-7.0.1/tests/integration/test_console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/tests/integration/test_init.py` & `pop_cli-7.0.1/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/tests/integration/test_ref.py` & `pop_cli-7.0.1/tests/integration/test_ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/tests/integration/test_state.py` & `pop_cli-7.0.1/tests/integration/test_state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/.gitignore` & `pop_cli-7.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/README.rst` & `pop_cli-7.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pop_cli-7.0.0/pyproject.toml` & `pop_cli-7.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "setuptools"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pop-cli"
-version = "7.0.0"
+version = "7.0.1"
 description = "A POP cli interface"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
 ]
 classifiers = [
     "Operating System :: OS Independent",
```

### Comparing `pop_cli-7.0.0/PKG-INFO` & `pop_cli-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pop-cli
-Version: 7.0.0
+Version: 7.0.1
 Summary: A POP cli interface
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

