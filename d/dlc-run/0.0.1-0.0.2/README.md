# Comparing `tmp/dlc_run-0.0.1.tar.gz` & `tmp/dlc_run-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dlc_run-0.0.1.tar", last modified: Fri Apr 26 13:06:11 2024, max compression
+gzip compressed data, was "dist/dlc_run-0.0.2.tar", last modified: Wed May  8 03:33:53 2024, max compression
```

## Comparing `dlc_run-0.0.1.tar` & `dlc_run-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:06:11.000000 dlc_run-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 13:06:11.000000 dlc_run-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 13:06:07.000000 dlc_run-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:06:11.000000 dlc_run-0.0.1/dlc_run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:06:07.000000 dlc_run-0.0.1/dlc_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-04-26 13:06:07.000000 dlc_run-0.0.1/dlc_run/dlc_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-26 13:06:07.000000 dlc_run-0.0.1/dlc_run/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:06:11.000000 dlc_run-0.0.1/dlc_run.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 13:06:11.000000 dlc_run-0.0.1/dlc_run.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-26 13:06:11.000000 dlc_run-0.0.1/dlc_run.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:06:11.000000 dlc_run-0.0.1/dlc_run.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 13:06:11.000000 dlc_run-0.0.1/dlc_run.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 13:06:11.000000 dlc_run-0.0.1/dlc_run.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:06:11.000000 dlc_run-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-26 13:06:07.000000 dlc_run-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:33:53.000000 dlc_run-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-08 03:33:53.000000 dlc_run-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 03:33:49.000000 dlc_run-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:33:53.000000 dlc_run-0.0.2/dlc_run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:33:49.000000 dlc_run-0.0.2/dlc_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-05-08 03:33:49.000000 dlc_run-0.0.2/dlc_run/dlc_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-08 03:33:49.000000 dlc_run-0.0.2/dlc_run/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:33:53.000000 dlc_run-0.0.2/dlc_run.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-08 03:33:52.000000 dlc_run-0.0.2/dlc_run.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 03:33:53.000000 dlc_run-0.0.2/dlc_run.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 03:33:52.000000 dlc_run-0.0.2/dlc_run.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 03:33:52.000000 dlc_run-0.0.2/dlc_run.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 03:33:52.000000 dlc_run-0.0.2/dlc_run.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 03:33:53.000000 dlc_run-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-08 03:33:49.000000 dlc_run-0.0.2/setup.py
```

### Comparing `dlc_run-0.0.1/dlc_run/dlc_run.py` & `dlc_run-0.0.2/dlc_run/dlc_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 import re
 import subprocess
 from pathlib import Path
 
 HOME = f'/cpfs01/user/{os.getenv("USER")}'
 
 
-def get_workspace_id(partition: str, config_path: str) -> str:
+def get_workspace_id(partition: str, config_path: str, dlc_path: str) -> str:
     """Extract the workspace ID for the specified partition using dlc
     command."""
+    config_path = os.path.expanduser(config_path)
+    dlc_path = os.path.expanduser(dlc_path)
     try:
-        result = subprocess.run(['dlc', 'get', 'workspace', '-c', config_path],
+        result = subprocess.run([dlc_path, 'get', 'workspace', '-c', config_path],
                                 capture_output=True,
                                 text=True,
                                 check=True)
         regex = rf'\|\s*{re.escape(partition)}\s*\|\s*([\w]+)\s*\|'
         match = re.search(regex, result.stdout, re.MULTILINE)
         if match:
             return match.group(1).strip()
@@ -137,15 +139,15 @@
     parser.add_argument(
         'task_cmds',
         # required=True,
         nargs=argparse.REMAINDER,
         help='Command line to execute, similar to typing in the shell.')
     args = parser.parse_args()
 
-    workspace_id = get_workspace_id(args.partition, args.config)
+    workspace_id = get_workspace_id(args.partition, args.config, args.dlc_path)
     if not workspace_id:
         print('Failed to retrieve workspace ID.')
         exit(1)
 
     home_cmd = f'export HOME={HOME}'
     shell_cmd = (f'{args.shell} -c "source ~/.{args.shell}rc'
                  if args.shell != 'none' else '')
```

### Comparing `dlc_run-0.0.1/dlc_run/version.py` & `dlc_run-0.0.2/dlc_run/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 
 def parse_version_info(version_str: str, length: int = 4) -> tuple:
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
```

### Comparing `dlc_run-0.0.1/setup.py` & `dlc_run-0.0.2/setup.py`

 * *Files identical despite different names*

