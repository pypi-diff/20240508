# Comparing `tmp/task-queue-2.8.7.tar.gz` & `tmp/task-queue-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task-queue-2.8.7.tar", last modified: Fri May 14 15:02:12 2021, max compression
+gzip compressed data, was "task-queue-2.9.0.tar", last modified: Fri May 14 22:13:12 2021, max compression
```

## Comparing `task-queue-2.8.7.tar` & `task-queue-2.9.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2021-05-14 15:02:12.442882 task-queue-2.8.7/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2021-05-14 15:02:12.436170 task-queue-2.8.7/.github/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2021-05-14 15:02:12.438070 task-queue-2.8.7/.github/workflows/
--rw-r--r--   0 wms        (501) staff       (20)      908 2021-02-10 02:40:42.000000 task-queue-2.8.7/.github/workflows/python-package.yml
--rw-r--r--   0 wms        (501) staff       (20)      222 2021-05-14 15:02:12.000000 task-queue-2.8.7/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     7494 2021-05-14 15:02:12.000000 task-queue-2.8.7/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)     1535 2021-01-11 02:50:56.000000 task-queue-2.8.7/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       46 2021-01-11 02:50:56.000000 task-queue-2.8.7/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)    24870 2021-05-14 15:02:12.443059 task-queue-2.8.7/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)    21112 2021-03-25 17:39:55.000000 task-queue-2.8.7/README.md
--rw-r--r--   0 wms        (501) staff       (20)      123 2021-01-11 02:50:56.000000 task-queue-2.8.7/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)       17 2021-05-10 17:11:46.000000 task-queue-2.8.7/requirements_dev.txt
--rw-r--r--   0 wms        (501) staff       (20)      833 2021-05-14 15:02:12.443486 task-queue-2.8.7/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      238 2021-01-11 02:50:56.000000 task-queue-2.8.7/setup.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2021-05-14 15:02:12.439295 task-queue-2.8.7/task_queue.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)    24870 2021-05-14 15:02:12.000000 task-queue-2.8.7/task_queue.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      850 2021-05-14 15:02:12.000000 task-queue-2.8.7/task_queue.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2021-05-14 15:02:12.000000 task-queue-2.8.7/task_queue.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       44 2021-05-14 15:02:12.000000 task-queue-2.8.7/task_queue.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2021-02-09 20:36:23.000000 task-queue-2.8.7/task_queue.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2021-05-14 15:02:12.000000 task-queue-2.8.7/task_queue.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)      124 2021-05-14 15:02:12.000000 task-queue-2.8.7/task_queue.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       24 2021-05-14 15:02:12.000000 task-queue-2.8.7/task_queue.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2021-05-14 15:02:12.441733 task-queue-2.8.7/taskqueue/
--rw-r--r--   0 wms        (501) staff       (20)      298 2021-05-14 15:01:07.000000 task-queue-2.8.7/taskqueue/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     4564 2021-02-09 23:07:16.000000 task-queue-2.8.7/taskqueue/aws_queue_api.py
--rw-r--r--   0 wms        (501) staff       (20)    11666 2021-05-14 14:54:41.000000 task-queue-2.8.7/taskqueue/file_queue_api.py
--rw-r--r--   0 wms        (501) staff       (20)     2946 2021-01-11 02:50:56.000000 task-queue-2.8.7/taskqueue/lib.py
--rw-r--r--   0 wms        (501) staff       (20)     1067 2021-01-11 02:50:56.000000 task-queue-2.8.7/taskqueue/paths.py
--rw-r--r--   0 wms        (501) staff       (20)     3499 2021-05-10 17:16:29.000000 task-queue-2.8.7/taskqueue/queueablefns.py
--rw-r--r--   0 wms        (501) staff       (20)     1104 2021-01-11 02:50:56.000000 task-queue-2.8.7/taskqueue/queueables.py
--rw-r--r--   0 wms        (501) staff       (20)     3167 2021-01-11 02:50:56.000000 task-queue-2.8.7/taskqueue/registered_task.py
--rw-r--r--   0 wms        (501) staff       (20)     2623 2021-05-10 17:11:46.000000 task-queue-2.8.7/taskqueue/scheduler.py
--rw-r--r--   0 wms        (501) staff       (20)     3585 2021-01-11 02:50:56.000000 task-queue-2.8.7/taskqueue/secrets.py
--rw-r--r--   0 wms        (501) staff       (20)    17379 2021-05-14 14:56:47.000000 task-queue-2.8.7/taskqueue/taskqueue.py
--rw-r--r--   0 wms        (501) staff       (20)     7173 2021-01-11 02:50:56.000000 task-queue-2.8.7/taskqueue/threaded_queue.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2021-05-14 15:02:12.442164 task-queue-2.8.7/taskqueue_cli/
--rw-r--r--   0 wms        (501) staff       (20)     1535 2021-01-11 02:50:56.000000 task-queue-2.8.7/taskqueue_cli/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       28 2021-01-11 02:50:56.000000 task-queue-2.8.7/taskqueue_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     1609 2021-01-11 02:50:56.000000 task-queue-2.8.7/taskqueue_cli/taskqueue_cli.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2021-05-14 15:02:12.442597 task-queue-2.8.7/test/
--rw-r--r--   0 wms        (501) staff       (20)      416 2021-01-11 02:50:56.000000 task-queue-2.8.7/test/pathos_issue.py
--rw-r--r--   0 wms        (501) staff       (20)     2616 2021-03-25 17:42:56.000000 task-queue-2.8.7/test/test_filequeue.py
--rw-r--r--   0 wms        (501) staff       (20)     6828 2021-05-10 17:16:42.000000 task-queue-2.8.7/test/test_taskqueue.py
--rw-r--r--   0 wms        (501) staff       (20)      186 2021-01-11 02:50:56.000000 task-queue-2.8.7/tox.ini
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2021-05-14 22:13:12.438275 task-queue-2.9.0/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2021-05-14 22:13:12.431190 task-queue-2.9.0/.github/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2021-05-14 22:13:12.433253 task-queue-2.9.0/.github/workflows/
+-rw-r--r--   0 wms        (501) staff       (20)      908 2021-02-10 02:40:42.000000 task-queue-2.9.0/.github/workflows/python-package.yml
+-rw-r--r--   0 wms        (501) staff       (20)      222 2021-05-14 22:13:12.000000 task-queue-2.9.0/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     7679 2021-05-14 22:13:12.000000 task-queue-2.9.0/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)     1535 2021-01-11 02:50:56.000000 task-queue-2.9.0/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       46 2021-01-11 02:50:56.000000 task-queue-2.9.0/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)    24870 2021-05-14 22:13:12.438459 task-queue-2.9.0/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)    21112 2021-03-25 17:39:55.000000 task-queue-2.9.0/README.md
+-rw-r--r--   0 wms        (501) staff       (20)      123 2021-01-11 02:50:56.000000 task-queue-2.9.0/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)       17 2021-05-10 17:11:46.000000 task-queue-2.9.0/requirements_dev.txt
+-rw-r--r--   0 wms        (501) staff       (20)      833 2021-05-14 22:13:12.438877 task-queue-2.9.0/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      238 2021-01-11 02:50:56.000000 task-queue-2.9.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2021-05-14 22:13:12.434537 task-queue-2.9.0/task_queue.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)    24870 2021-05-14 22:13:12.000000 task-queue-2.9.0/task_queue.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      850 2021-05-14 22:13:12.000000 task-queue-2.9.0/task_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2021-05-14 22:13:12.000000 task-queue-2.9.0/task_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       44 2021-05-14 22:13:12.000000 task-queue-2.9.0/task_queue.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2021-02-09 20:36:23.000000 task-queue-2.9.0/task_queue.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2021-05-14 22:13:12.000000 task-queue-2.9.0/task_queue.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)      124 2021-05-14 22:13:12.000000 task-queue-2.9.0/task_queue.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       24 2021-05-14 22:13:12.000000 task-queue-2.9.0/task_queue.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2021-05-14 22:13:12.437027 task-queue-2.9.0/taskqueue/
+-rw-r--r--   0 wms        (501) staff       (20)      298 2021-05-14 22:12:29.000000 task-queue-2.9.0/taskqueue/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     4564 2021-02-09 23:07:16.000000 task-queue-2.9.0/taskqueue/aws_queue_api.py
+-rw-r--r--   0 wms        (501) staff       (20)    11666 2021-05-14 14:54:41.000000 task-queue-2.9.0/taskqueue/file_queue_api.py
+-rw-r--r--   0 wms        (501) staff       (20)     2946 2021-01-11 02:50:56.000000 task-queue-2.9.0/taskqueue/lib.py
+-rw-r--r--   0 wms        (501) staff       (20)     1067 2021-01-11 02:50:56.000000 task-queue-2.9.0/taskqueue/paths.py
+-rw-r--r--   0 wms        (501) staff       (20)     3499 2021-05-10 17:16:29.000000 task-queue-2.9.0/taskqueue/queueablefns.py
+-rw-r--r--   0 wms        (501) staff       (20)     1104 2021-01-11 02:50:56.000000 task-queue-2.9.0/taskqueue/queueables.py
+-rw-r--r--   0 wms        (501) staff       (20)     3167 2021-01-11 02:50:56.000000 task-queue-2.9.0/taskqueue/registered_task.py
+-rw-r--r--   0 wms        (501) staff       (20)     2623 2021-05-10 17:11:46.000000 task-queue-2.9.0/taskqueue/scheduler.py
+-rw-r--r--   0 wms        (501) staff       (20)     3585 2021-01-11 02:50:56.000000 task-queue-2.9.0/taskqueue/secrets.py
+-rw-r--r--   0 wms        (501) staff       (20)    17379 2021-05-14 14:56:47.000000 task-queue-2.9.0/taskqueue/taskqueue.py
+-rw-r--r--   0 wms        (501) staff       (20)     7173 2021-01-11 02:50:56.000000 task-queue-2.9.0/taskqueue/threaded_queue.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2021-05-14 22:13:12.437435 task-queue-2.9.0/taskqueue_cli/
+-rw-r--r--   0 wms        (501) staff       (20)     1535 2021-01-11 02:50:56.000000 task-queue-2.9.0/taskqueue_cli/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       28 2021-01-11 02:50:56.000000 task-queue-2.9.0/taskqueue_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     2029 2021-05-14 22:07:44.000000 task-queue-2.9.0/taskqueue_cli/taskqueue_cli.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2021-05-14 22:13:12.438023 task-queue-2.9.0/test/
+-rw-r--r--   0 wms        (501) staff       (20)      416 2021-01-11 02:50:56.000000 task-queue-2.9.0/test/pathos_issue.py
+-rw-r--r--   0 wms        (501) staff       (20)     2616 2021-03-25 17:42:56.000000 task-queue-2.9.0/test/test_filequeue.py
+-rw-r--r--   0 wms        (501) staff       (20)     6828 2021-05-10 17:16:42.000000 task-queue-2.9.0/test/test_taskqueue.py
+-rw-r--r--   0 wms        (501) staff       (20)      186 2021-01-11 02:50:56.000000 task-queue-2.9.0/tox.ini
```

### Comparing `task-queue-2.8.7/.github/workflows/python-package.yml` & `task-queue-2.9.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/ChangeLog` & `task-queue-2.9.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGES
 =======
 
+2.9.0
+-----
+
+* release(2.9.0): adds cp command to ptq
+* refactor: rename copy to cp
+* docs: describe restrictions on copying sqs
+* chore: update ChangeLog
+* feat(cli): add copy to ptq
+
 2.8.7
 -----
 
 * release(2.8.7): more robust is\_empty for FileQueue
 * fix(fq): iter dies if file deleted between scan and read
 * fix: no need for is\_empty to actually read the files
```

### Comparing `task-queue-2.8.7/LICENSE` & `task-queue-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/PKG-INFO` & `task-queue-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task-queue
-Version: 2.8.7
+Version: 2.9.0
 Summary: Multithreaded cloud queue client.
 Home-page: https://github.com/seung-lab/python-task-queue/
 Author: Ignacio Tartavull, William Silversmith, and others
 Author-email: ws9@princeton.edu
 License: BSD
 Description: [![Build Status](https://travis-ci.org/seung-lab/python-task-queue.svg?branch=master)](https://travis-ci.org/seung-lab/python-task-queue) [![PyPI version](https://badge.fury.io/py/task-queue.svg)](https://badge.fury.io/py/task-queue)
```

### Comparing `task-queue-2.8.7/README.md` & `task-queue-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/setup.cfg` & `task-queue-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/task_queue.egg-info/PKG-INFO` & `task-queue-2.9.0/task_queue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: task-queue
-Version: 2.8.7
+Version: 2.9.0
 Summary: Multithreaded cloud queue client.
 Home-page: https://github.com/seung-lab/python-task-queue/
 Author: Ignacio Tartavull, William Silversmith, and others
 Author-email: ws9@princeton.edu
 License: BSD
 Description: [![Build Status](https://travis-ci.org/seung-lab/python-task-queue.svg?branch=master)](https://travis-ci.org/seung-lab/python-task-queue) [![PyPI version](https://badge.fury.io/py/task-queue.svg)](https://badge.fury.io/py/task-queue)
```

### Comparing `task-queue-2.8.7/task_queue.egg-info/SOURCES.txt` & `task-queue-2.9.0/task_queue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/taskqueue/aws_queue_api.py` & `task-queue-2.9.0/taskqueue/aws_queue_api.py`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/taskqueue/file_queue_api.py` & `task-queue-2.9.0/taskqueue/file_queue_api.py`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/taskqueue/lib.py` & `task-queue-2.9.0/taskqueue/lib.py`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/taskqueue/paths.py` & `task-queue-2.9.0/taskqueue/paths.py`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/taskqueue/queueablefns.py` & `task-queue-2.9.0/taskqueue/queueablefns.py`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/taskqueue/queueables.py` & `task-queue-2.9.0/taskqueue/queueables.py`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/taskqueue/registered_task.py` & `task-queue-2.9.0/taskqueue/registered_task.py`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/taskqueue/scheduler.py` & `task-queue-2.9.0/taskqueue/scheduler.py`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/taskqueue/secrets.py` & `task-queue-2.9.0/taskqueue/secrets.py`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/taskqueue/taskqueue.py` & `task-queue-2.9.0/taskqueue/taskqueue.py`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/taskqueue/threaded_queue.py` & `task-queue-2.9.0/taskqueue/threaded_queue.py`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/taskqueue_cli/LICENSE` & `task-queue-2.9.0/taskqueue_cli/LICENSE`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/taskqueue_cli/taskqueue_cli.py` & `task-queue-2.9.0/taskqueue_cli/taskqueue_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -57,7 +57,30 @@
     print(f"Leased: {leased} (--%) of queue")
 
 @main.command()
 @click.argument("queuepath")
 def release(queuepath):
   """Release all tasks from their leases."""
   TaskQueue(normalize_path(queuepath)).release_all()
+
+@main.command()
+@click.argument("src")
+@click.argument("dest")
+def cp(src, dest):
+  """
+  Copy the contents of a queue to another
+  service or location. Do not run this
+  process while a queue is being worked.
+
+  Currently sqs queues are not copiable,
+  but you can copy an fq to sqs.
+  """
+  src = normalize_path(src)
+  dest = normalize_path(dest)
+
+  tqd = TaskQueue(dest)
+  tqs = TaskQueue(src)
+
+  tqd.insert(tqs)
+
+
+
```

### Comparing `task-queue-2.8.7/test/test_filequeue.py` & `task-queue-2.9.0/test/test_filequeue.py`

 * *Files identical despite different names*

### Comparing `task-queue-2.8.7/test/test_taskqueue.py` & `task-queue-2.9.0/test/test_taskqueue.py`

 * *Files identical despite different names*

