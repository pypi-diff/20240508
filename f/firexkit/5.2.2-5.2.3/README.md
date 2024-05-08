# Comparing `tmp/firexkit-5.2.2.tar.gz` & `tmp/firexkit-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firexkit-5.2.2.tar", last modified: Fri Apr 19 21:52:42 2024, max compression
+gzip compressed data, was "firexkit-5.2.3.tar", last modified: Wed May  8 21:23:24 2024, max compression
```

## Comparing `firexkit-5.2.2.tar` & `firexkit-5.2.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-19 21:52:42.083270 firexkit-5.2.2/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1513 2024-04-19 21:52:17.000000 firexkit-5.2.2/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       73 2024-04-19 21:52:17.000000 firexkit-5.2.2/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      262 2024-04-19 21:52:42.083270 firexkit-5.2.2/PKG-INFO
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       38 2024-04-19 21:52:17.000000 firexkit-5.2.2/README.md
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-19 21:52:42.084270 firexkit-5.2.2/firexkit/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/__init__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      497 2024-04-19 21:52:42.084270 firexkit-5.2.2/firexkit/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    11286 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/argument_conversion.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6941 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/bag_of_goodies.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2957 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/broker.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     8370 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/chain.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1327 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/firex_exceptions.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1004 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/firexkit_common.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3178 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/inspect.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-19 21:52:42.082270 firexkit-5.2.2/firexkit/install_resources/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      482 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/install_resources/cloud-ci-install-configs.json
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1938 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/memory_utils.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       82 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/permissions.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3315 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/proc_utils.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-19 21:52:42.083270 firexkit-5.2.2/firexkit/resources/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3448 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/resources/firex.css
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7676 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/resources/firex_logo.png
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      836 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/resources.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    34337 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/result.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3358 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/revoke.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70465 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/task.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-19 21:52:42.083270 firexkit-5.2.2/firexkit/templates/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      300 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/templates/link.html
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2874 2024-04-19 21:52:18.000000 firexkit-5.2.2/firexkit/templates/log_template.html
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-19 21:52:42.082270 firexkit-5.2.2/firexkit.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      262 2024-04-19 21:52:42.000000 firexkit-5.2.2/firexkit.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)      833 2024-04-19 21:52:42.000000 firexkit-5.2.2/firexkit.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-04-19 21:52:42.000000 firexkit-5.2.2/firexkit.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       34 2024-04-19 21:52:42.000000 firexkit-5.2.2/firexkit.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       21 2024-04-19 21:52:42.000000 firexkit-5.2.2/firexkit.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        9 2024-04-19 21:52:42.000000 firexkit-5.2.2/firexkit.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-04-19 21:52:42.000000 firexkit-5.2.2/firexkit.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      268 2024-04-19 21:52:42.084270 firexkit-5.2.2/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      681 2024-04-19 21:52:18.000000 firexkit-5.2.2/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2024-04-19 21:52:18.000000 firexkit-5.2.2/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-08 21:23:24.214448 firexkit-5.2.3/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1513 2024-05-08 21:23:00.000000 firexkit-5.2.3/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       73 2024-05-08 21:23:00.000000 firexkit-5.2.3/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      262 2024-05-08 21:23:24.214448 firexkit-5.2.3/PKG-INFO
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       38 2024-05-08 21:23:00.000000 firexkit-5.2.3/README.md
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-08 21:23:24.215448 firexkit-5.2.3/firexkit/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/__init__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      497 2024-05-08 21:23:24.215448 firexkit-5.2.3/firexkit/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    11286 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/argument_conversion.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6941 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/bag_of_goodies.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2957 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/broker.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     8370 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/chain.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1327 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/firex_exceptions.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1004 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/firexkit_common.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3178 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/inspect.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-08 21:23:24.213448 firexkit-5.2.3/firexkit/install_resources/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      482 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/install_resources/cloud-ci-install-configs.json
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1938 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/memory_utils.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       82 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/permissions.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3315 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/proc_utils.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-08 21:23:24.213448 firexkit-5.2.3/firexkit/resources/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3448 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/resources/firex.css
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7676 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/resources/firex_logo.png
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      836 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/resources.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    34337 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/result.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3358 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/revoke.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    71247 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/task.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-08 21:23:24.214448 firexkit-5.2.3/firexkit/templates/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      300 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/templates/link.html
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2874 2024-05-08 21:23:00.000000 firexkit-5.2.3/firexkit/templates/log_template.html
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-08 21:23:24.213448 firexkit-5.2.3/firexkit.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      262 2024-05-08 21:23:24.000000 firexkit-5.2.3/firexkit.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)      833 2024-05-08 21:23:24.000000 firexkit-5.2.3/firexkit.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-05-08 21:23:24.000000 firexkit-5.2.3/firexkit.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       34 2024-05-08 21:23:24.000000 firexkit-5.2.3/firexkit.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       21 2024-05-08 21:23:24.000000 firexkit-5.2.3/firexkit.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        9 2024-05-08 21:23:24.000000 firexkit-5.2.3/firexkit.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-05-08 21:23:24.000000 firexkit-5.2.3/firexkit.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      268 2024-05-08 21:23:24.214448 firexkit-5.2.3/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      681 2024-05-08 21:23:00.000000 firexkit-5.2.3/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2024-05-08 21:23:00.000000 firexkit-5.2.3/versioneer.py
```

### Comparing `firexkit-5.2.2/LICENSE` & `firexkit-5.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/argument_conversion.py` & `firexkit-5.2.3/firexkit/argument_conversion.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/bag_of_goodies.py` & `firexkit-5.2.3/firexkit/bag_of_goodies.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/broker.py` & `firexkit-5.2.3/firexkit/broker.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/chain.py` & `firexkit-5.2.3/firexkit/chain.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/firex_exceptions.py` & `firexkit-5.2.3/firexkit/firex_exceptions.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/firexkit_common.py` & `firexkit-5.2.3/firexkit/firexkit_common.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/inspect.py` & `firexkit-5.2.3/firexkit/inspect.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/memory_utils.py` & `firexkit-5.2.3/firexkit/memory_utils.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/proc_utils.py` & `firexkit-5.2.3/firexkit/proc_utils.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/resources/firex.css` & `firexkit-5.2.3/firexkit/resources/firex.css`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/resources/firex_logo.png` & `firexkit-5.2.3/firexkit/resources/firex_logo.png`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/resources.py` & `firexkit-5.2.3/firexkit/resources.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/result.py` & `firexkit-5.2.3/firexkit/result.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/revoke.py` & `firexkit-5.2.3/firexkit/revoke.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit/task.py` & `firexkit-5.2.3/firexkit/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import os
 import textwrap
 from collections import OrderedDict
 import inspect
 from datetime import datetime
 from functools import partial
-from typing import Callable, Iterable, Optional, Union
+from typing import Callable, Iterable, Optional, Union, Any
 from urllib.parse import urljoin
 from copy import deepcopy
 import dataclasses
 
 from celery.canvas import Signature, _chain
 from celery.result import AsyncResult
 from celery.states import REVOKED
@@ -48,14 +48,21 @@
 logger = get_task_logger(__name__)
 
 ################################################################
 # Monkey patching
 _orig_chain_apply_async__ = _chain.apply_async
 
 
+@dataclasses.dataclass
+class TaskConfig:
+    signature: Signature
+    inject_abog: bool = True
+    enqueue_opts: Optional[dict[str, Any]] = None
+
+
 def _chain_apply_async(self: _chain, *args: tuple, **kwargs: dict) -> AsyncResult:
     try:
         chain_depth = 0
         for task in self.tasks:
             task.kwargs['chain_depth'] = chain_depth
             chain_depth += 1
     except AttributeError:
@@ -1237,14 +1244,28 @@
             scheduled.append(promise)
             promises.append(promise)
         if wait_for_completion or raise_exception_on_failure:
             # Wait for all children to complete
             self.wait_for_specific_children(promises, raise_exception_on_failure=raise_exception_on_failure)
         return promises
 
+    def enqueue_task_config(self,
+                            task_config: TaskConfig,
+                            inject_args: Optional[dict] = None):
+        enqueue_opts = task_config.enqueue_opts or dict()
+        chain = task_config.signature
+        args_to_inject = self.abog.copy() if task_config.inject_abog else {}
+        if inject_args:
+            args_to_inject.update(inject_args)
+        if args_to_inject:
+            from firexkit.chain import InjectArgs
+            chain = InjectArgs(**args_to_inject) | chain
+        logger.debug(f'Enqueuing {task_config}')
+        self.enqueue_child(chain, **enqueue_opts)
+
     def revoke_nonready_children(self):
         nonready_children = self.nonready_enqueued_children
         if nonready_children:
             logger.info('Nonready children of current task exist.')
             revoked = [self.revoke_child(child_result) for child_result in nonready_children]
             wait_for_running_tasks_from_results([result for result_list in revoked for result in result_list])
```

### Comparing `firexkit-5.2.2/firexkit/templates/log_template.html` & `firexkit-5.2.3/firexkit/templates/log_template.html`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/firexkit.egg-info/SOURCES.txt` & `firexkit-5.2.3/firexkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/setup.py` & `firexkit-5.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `firexkit-5.2.2/versioneer.py` & `firexkit-5.2.3/versioneer.py`

 * *Files identical despite different names*

