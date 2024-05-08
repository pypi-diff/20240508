# Comparing `tmp/receptorctl-1.4.5.tar.gz` & `tmp/receptorctl-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "receptorctl-1.4.5.tar", last modified: Thu Mar 21 17:27:51 2024, max compression
+gzip compressed data, was "receptorctl-1.4.6.tar", last modified: Wed May  8 15:52:41 2024, max compression
```

## Comparing `receptorctl-1.4.5.tar` & `receptorctl-1.4.6.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:27:51.359064 receptorctl-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-21 17:27:41.000000 receptorctl-1.4.5/.VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-21 17:27:38.000000 receptorctl-1.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-21 17:27:51.359064 receptorctl-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-21 17:27:38.000000 receptorctl-1.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-21 17:27:38.000000 receptorctl-1.4.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:27:51.359064 receptorctl-1.4.5/receptorctl/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-21 17:27:38.000000 receptorctl-1.4.5/receptorctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-21 17:27:38.000000 receptorctl-1.4.5/receptorctl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18191 2024-03-21 17:27:38.000000 receptorctl-1.4.5/receptorctl/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-03-21 17:27:38.000000 receptorctl-1.4.5/receptorctl/socket_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:27:51.359064 receptorctl-1.4.5/receptorctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-21 17:27:51.000000 receptorctl-1.4.5/receptorctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-21 17:27:51.000000 receptorctl-1.4.5/receptorctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 17:27:51.000000 receptorctl-1.4.5/receptorctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-21 17:27:51.000000 receptorctl-1.4.5/receptorctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-21 17:27:51.000000 receptorctl-1.4.5/receptorctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-21 17:27:51.000000 receptorctl-1.4.5/receptorctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-21 17:27:51.359064 receptorctl-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-21 17:27:38.000000 receptorctl-1.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:27:51.359064 receptorctl-1.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-21 17:27:38.000000 receptorctl-1.4.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-21 17:27:38.000000 receptorctl-1.4.5/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-21 17:27:38.000000 receptorctl-1.4.5/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-03-21 17:27:38.000000 receptorctl-1.4.5/tests/test_workunit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:52:41.343492 receptorctl-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 15:52:31.000000 receptorctl-1.4.6/.VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 15:52:26.000000 receptorctl-1.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-08 15:52:41.343492 receptorctl-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-08 15:52:26.000000 receptorctl-1.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-08 15:52:26.000000 receptorctl-1.4.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:52:41.343492 receptorctl-1.4.6/receptorctl/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-08 15:52:26.000000 receptorctl-1.4.6/receptorctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 15:52:26.000000 receptorctl-1.4.6/receptorctl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-05-08 15:52:26.000000 receptorctl-1.4.6/receptorctl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-05-08 15:52:26.000000 receptorctl-1.4.6/receptorctl/socket_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:52:41.343492 receptorctl-1.4.6/receptorctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-08 15:52:41.000000 receptorctl-1.4.6/receptorctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-08 15:52:41.000000 receptorctl-1.4.6/receptorctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:52:41.000000 receptorctl-1.4.6/receptorctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 15:52:41.000000 receptorctl-1.4.6/receptorctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-08 15:52:41.000000 receptorctl-1.4.6/receptorctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 15:52:41.000000 receptorctl-1.4.6/receptorctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 15:52:41.343492 receptorctl-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-08 15:52:26.000000 receptorctl-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:52:41.343492 receptorctl-1.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 15:52:26.000000 receptorctl-1.4.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-05-08 15:52:26.000000 receptorctl-1.4.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-08 15:52:26.000000 receptorctl-1.4.6/tests/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-08 15:52:26.000000 receptorctl-1.4.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-08 15:52:26.000000 receptorctl-1.4.6/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-08 15:52:26.000000 receptorctl-1.4.6/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-08 15:52:26.000000 receptorctl-1.4.6/tests/test_workunit.py
```

### Comparing `receptorctl-1.4.5/receptorctl/cli.py` & `receptorctl-1.4.6/receptorctl/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 @click.group(cls=IgnoreRequiredWithHelp)
 @click.pass_context
 @click.option(
     "--socket",
     envvar="RECEPTORCTL_SOCKET",
     required=True,
     show_envvar=True,
-    help="Control socket address to connect to Receptor (defaults to Unix socket, use tcp:// for TCP socket)",  # noqa: E501
+    help="Control socket address to for the Receptor connection (The default is 'unix:' for a Unix socket, use 'tcp://' for a TCP socket)",  # noqa: E501
 )
 @click.option(
     "--config",
     "-c",
     default=None,
     envvar="RECEPTORCTL_CONFIG",
     required=False,
```

### Comparing `receptorctl-1.4.5/receptorctl/socket_interface.py` & `receptorctl-1.4.6/receptorctl/socket_interface.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.5/setup.cfg` & `receptorctl-1.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.5/tests/test_cli.py` & `receptorctl-1.4.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.5/tests/test_connection.py` & `receptorctl-1.4.6/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.5/tests/test_mesh.py` & `receptorctl-1.4.6/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.5/tests/test_workunit.py` & `receptorctl-1.4.6/tests/test_workunit.py`

 * *Files identical despite different names*

