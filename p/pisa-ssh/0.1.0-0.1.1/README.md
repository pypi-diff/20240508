# Comparing `tmp/pisa_ssh-0.1.0.tar.gz` & `tmp/pisa_ssh-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisa_ssh-0.1.0.tar", last modified: Wed May  8 10:47:01 2024, max compression
+gzip compressed data, was "pisa_ssh-0.1.1.tar", last modified: Wed May  8 18:11:00 2024, max compression
```

## Comparing `pisa_ssh-0.1.0.tar` & `pisa_ssh-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:47:01.152060 pisa_ssh-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/src/pisa/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/src/pisa/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/dispatcher/cluster_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/dispatcher/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/dispatcher/task_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/src/pisa/runner/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/runner/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/src/pisa/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/src/pisa_ssh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-08 10:47:01.000000 pisa_ssh-0.1.0/src/pisa_ssh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-08 10:47:01.000000 pisa_ssh-0.1.0/src/pisa_ssh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:47:01.000000 pisa_ssh-0.1.0/src/pisa_ssh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 10:47:01.000000 pisa_ssh-0.1.0/src/pisa_ssh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 10:47:01.000000 pisa_ssh-0.1.0/src/pisa_ssh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 10:47:01.000000 pisa_ssh-0.1.0/src/pisa_ssh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:11:00.956626 pisa_ssh-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 18:10:44.000000 pisa_ssh-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-08 18:11:00.952626 pisa_ssh-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-08 18:10:44.000000 pisa_ssh-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-08 18:10:44.000000 pisa_ssh-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:11:00.956626 pisa_ssh-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:11:00.952626 pisa_ssh-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:11:00.952626 pisa_ssh-0.1.1/src/pisa/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 18:10:44.000000 pisa_ssh-0.1.1/src/pisa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-08 18:10:44.000000 pisa_ssh-0.1.1/src/pisa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-08 18:10:44.000000 pisa_ssh-0.1.1/src/pisa/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:11:00.952626 pisa_ssh-0.1.1/src/pisa/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-08 18:10:44.000000 pisa_ssh-0.1.1/src/pisa/dispatcher/cluster_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-08 18:10:44.000000 pisa_ssh-0.1.1/src/pisa/dispatcher/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-08 18:10:44.000000 pisa_ssh-0.1.1/src/pisa/dispatcher/task_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:11:00.952626 pisa_ssh-0.1.1/src/pisa/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-08 18:10:44.000000 pisa_ssh-0.1.1/src/pisa/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:11:00.952626 pisa_ssh-0.1.1/src/pisa_ssh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-08 18:11:00.000000 pisa_ssh-0.1.1/src/pisa_ssh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-08 18:11:00.000000 pisa_ssh-0.1.1/src/pisa_ssh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:11:00.000000 pisa_ssh-0.1.1/src/pisa_ssh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 18:11:00.000000 pisa_ssh-0.1.1/src/pisa_ssh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 18:11:00.000000 pisa_ssh-0.1.1/src/pisa_ssh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 18:11:00.000000 pisa_ssh-0.1.1/src/pisa_ssh.egg-info/top_level.txt
```

### Comparing `pisa_ssh-0.1.0/LICENSE` & `pisa_ssh-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.0/PKG-INFO` & `pisa_ssh-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisa-ssh
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pseudo Infrastructure for Scalable Applications (PISA)
 Author-email: Michael Hohenstein <michael@hohenste.in>
 License: MIT
 Project-URL: Homepage, https://github.com/MitchiLaser/pisa/blob/main/docs/README.md
 Project-URL: Repository, https://github.com/MitchiLaser/pisa
 Keywords: data,analysis,education,university,students,physics
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pisa_ssh-0.1.0/README.md` & `pisa_ssh-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.0/pyproject.toml` & `pisa_ssh-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.0/src/pisa/__main__.py` & `pisa_ssh-0.1.1/src/pisa/__main__.py`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.0/src/pisa/dispatcher/cluster_conf.py` & `pisa_ssh-0.1.1/src/pisa/dispatcher/cluster_conf.py`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.0/src/pisa/dispatcher/dispatcher.py` & `pisa_ssh-0.1.1/src/pisa/dispatcher/dispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from . import task_list
 import threading
 import logging as log
 import queue
 import subprocess
 import sys
 
-import random  # TODO: remove
-
 
 def run_dispatcher(cluster: cluster_conf.cluster_conf, tasks: queue.Queue[task_list.task]):
     # Start a thread for each connection to every device (task_limit for each node). Then these start taking tasks from the queue.
     for node in cluster.node_list():
         for _ in range(node.get_task_limit()):
             threading.Thread(target=node_connection, args=(node, tasks)).start()
 
@@ -34,15 +32,15 @@
 
             ssh.Session(node.get_address()) \
                 .connect() \
                 .send_command(f"cd {task.w_dir}") \
                 .send_command(f"./{task.env}/bin/activate") \
                 .send_command(f"mkdir -p {task.out}") \
                 .send_command(f"mkdir -p {task.err}") \
-                .send_command(f"{task.cmd} >{task.out}/{task.num}.out 2>{task.err}/{task.num}.err &") \
+                .send_command(f"{task.cmd} >{task.out}/{task.num}.out 2>{task.err}/{task.num}.err") \
                 .close()
             # log.debug(f"{task.cmd} >{task.out}/{task.num}.out 2>{task.err}/{task.num}.err &")  # TODO: remove
         except queue.Empty:  # queue is empty: exit thread
             has_task = False
             break
         except FileNotFoundError as e:  # file not found: program is not available
             log.error(f"file not found: {e}")
```

### Comparing `pisa_ssh-0.1.0/src/pisa/dispatcher/task_list.py` & `pisa_ssh-0.1.1/src/pisa/dispatcher/task_list.py`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.0/src/pisa_ssh.egg-info/PKG-INFO` & `pisa_ssh-0.1.1/src/pisa_ssh.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisa-ssh
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pseudo Infrastructure for Scalable Applications (PISA)
 Author-email: Michael Hohenstein <michael@hohenste.in>
 License: MIT
 Project-URL: Homepage, https://github.com/MitchiLaser/pisa/blob/main/docs/README.md
 Project-URL: Repository, https://github.com/MitchiLaser/pisa
 Keywords: data,analysis,education,university,students,physics
 Classifier: Development Status :: 5 - Production/Stable
```

