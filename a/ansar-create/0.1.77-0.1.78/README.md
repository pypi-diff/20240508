# Comparing `tmp/ansar_create-0.1.77.tar.gz` & `tmp/ansar_create-0.1.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_create-0.1.77.tar", last modified: Wed May  8 01:34:39 2024, max compression
+gzip compressed data, was "ansar_create-0.1.78.tar", last modified: Wed May  8 02:09:24 2024, max compression
```

## Comparing `ansar_create-0.1.77.tar` & `ansar_create-0.1.78.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:34:39.536899 ansar_create-0.1.77/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:18.000000 ansar_create-0.1.77/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-08 01:34:39.536899 ansar_create-0.1.77/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      901 2023-06-17 21:18:11.000000 ansar_create-0.1.77/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      718 2024-03-27 05:56:05.000000 ansar_create-0.1.77/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-08 01:34:39.536899 ansar_create-0.1.77/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     2139 2024-03-27 05:55:54.000000 ansar_create-0.1.77/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:34:39.532899 ansar_create-0.1.77/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:34:39.532899 ansar_create-0.1.77/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:34:39.532899 ansar_create-0.1.77/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    13081 2024-01-02 02:57:04.000000 ansar_create-0.1.77/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8950 2024-02-25 02:39:34.000000 ansar_create-0.1.77/src/ansar/command/ansar_group.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:34:39.536899 ansar_create-0.1.77/src/ansar/create/
--rw-rw-r--   0 scott     (1000) scott     (1000)     5706 2024-05-08 01:34:36.000000 ansar_create-0.1.77/src/ansar/create/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2654 2023-07-13 04:39:47.000000 ansar_create-0.1.77/src/ansar/create/binding.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1989 2023-12-23 01:56:16.000000 ansar_create-0.1.77/src/ansar/create/coding.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1857 2024-01-19 15:16:48.000000 ansar_create-0.1.77/src/ansar/create/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    13837 2024-02-24 20:57:36.000000 ansar_create-0.1.77/src/ansar/create/home.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3607 2024-02-14 21:31:28.000000 ansar_create-0.1.77/src/ansar/create/latching.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7383 2024-03-24 15:57:41.000000 ansar_create-0.1.77/src/ansar/create/lifecycle.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     4061 2024-01-25 13:13:42.000000 ansar_create-0.1.77/src/ansar/create/locking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6164 2023-07-13 04:40:10.000000 ansar_create-0.1.77/src/ansar/create/log.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8495 2023-07-13 04:40:11.000000 ansar_create-0.1.77/src/ansar/create/machine.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    29638 2024-05-07 19:48:13.000000 ansar_create-0.1.77/src/ansar/create/object.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9071 2024-01-18 15:23:10.000000 ansar_create-0.1.77/src/ansar/create/pending.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    29472 2024-02-28 13:52:41.000000 ansar_create-0.1.77/src/ansar/create/point.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    79049 2024-04-14 03:56:16.000000 ansar_create-0.1.77/src/ansar/create/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    31841 2024-01-22 04:26:11.000000 ansar_create-0.1.77/src/ansar/create/processing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3099 2024-03-26 19:19:48.000000 ansar_create-0.1.77/src/ansar/create/properties.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3741 2024-03-07 07:59:16.000000 ansar_create-0.1.77/src/ansar/create/retry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5938 2024-02-27 14:04:16.000000 ansar_create-0.1.77/src/ansar/create/rolling.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7477 2023-12-23 15:53:02.000000 ansar_create-0.1.77/src/ansar/create/root.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14196 2024-03-22 18:43:05.000000 ansar_create-0.1.77/src/ansar/create/space.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    19735 2024-03-22 18:43:09.000000 ansar_create-0.1.77/src/ansar/create/storage.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3959 2024-01-15 15:55:19.000000 ansar_create-0.1.77/src/ansar/create/test.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5100 2024-01-26 08:38:29.000000 ansar_create-0.1.77/src/ansar/create/timing.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:34:39.536899 ansar_create-0.1.77/src/ansar_create.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-08 01:34:39.000000 ansar_create-0.1.77/src/ansar_create.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      986 2024-05-08 01:34:39.000000 ansar_create-0.1.77/src/ansar_create.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-08 01:34:39.000000 ansar_create-0.1.77/src/ansar_create.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      104 2024-05-08 01:34:39.000000 ansar_create-0.1.77/src/ansar_create.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       22 2024-05-08 01:34:39.000000 ansar_create-0.1.77/src/ansar_create.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-08 01:34:39.000000 ansar_create-0.1.77/src/ansar_create.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 02:09:24.735219 ansar_create-0.1.78/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:18.000000 ansar_create-0.1.78/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-08 02:09:24.735219 ansar_create-0.1.78/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      901 2023-06-17 21:18:11.000000 ansar_create-0.1.78/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      718 2024-03-27 05:56:05.000000 ansar_create-0.1.78/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-08 02:09:24.735219 ansar_create-0.1.78/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2139 2024-03-27 05:55:54.000000 ansar_create-0.1.78/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 02:09:24.731219 ansar_create-0.1.78/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 02:09:24.731219 ansar_create-0.1.78/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 02:09:24.735219 ansar_create-0.1.78/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13081 2024-01-02 02:57:04.000000 ansar_create-0.1.78/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8950 2024-02-25 02:39:34.000000 ansar_create-0.1.78/src/ansar/command/ansar_group.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 02:09:24.735219 ansar_create-0.1.78/src/ansar/create/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5706 2024-05-08 02:09:21.000000 ansar_create-0.1.78/src/ansar/create/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2654 2023-07-13 04:39:47.000000 ansar_create-0.1.78/src/ansar/create/binding.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1989 2023-12-23 01:56:16.000000 ansar_create-0.1.78/src/ansar/create/coding.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1857 2024-01-19 15:16:48.000000 ansar_create-0.1.78/src/ansar/create/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13837 2024-02-24 20:57:36.000000 ansar_create-0.1.78/src/ansar/create/home.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3607 2024-02-14 21:31:28.000000 ansar_create-0.1.78/src/ansar/create/latching.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7383 2024-03-24 15:57:41.000000 ansar_create-0.1.78/src/ansar/create/lifecycle.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4061 2024-01-25 13:13:42.000000 ansar_create-0.1.78/src/ansar/create/locking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6164 2023-07-13 04:40:10.000000 ansar_create-0.1.78/src/ansar/create/log.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8495 2023-07-13 04:40:11.000000 ansar_create-0.1.78/src/ansar/create/machine.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    29699 2024-05-08 02:07:59.000000 ansar_create-0.1.78/src/ansar/create/object.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9071 2024-01-18 15:23:10.000000 ansar_create-0.1.78/src/ansar/create/pending.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    29472 2024-02-28 13:52:41.000000 ansar_create-0.1.78/src/ansar/create/point.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    79049 2024-04-14 03:56:16.000000 ansar_create-0.1.78/src/ansar/create/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    31841 2024-01-22 04:26:11.000000 ansar_create-0.1.78/src/ansar/create/processing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3099 2024-03-26 19:19:48.000000 ansar_create-0.1.78/src/ansar/create/properties.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3741 2024-03-07 07:59:16.000000 ansar_create-0.1.78/src/ansar/create/retry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5938 2024-02-27 14:04:16.000000 ansar_create-0.1.78/src/ansar/create/rolling.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7477 2023-12-23 15:53:02.000000 ansar_create-0.1.78/src/ansar/create/root.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14196 2024-03-22 18:43:05.000000 ansar_create-0.1.78/src/ansar/create/space.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    19735 2024-03-22 18:43:09.000000 ansar_create-0.1.78/src/ansar/create/storage.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3959 2024-01-15 15:55:19.000000 ansar_create-0.1.78/src/ansar/create/test.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5100 2024-01-26 08:38:29.000000 ansar_create-0.1.78/src/ansar/create/timing.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 02:09:24.735219 ansar_create-0.1.78/src/ansar_create.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-08 02:09:24.000000 ansar_create-0.1.78/src/ansar_create.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      986 2024-05-08 02:09:24.000000 ansar_create-0.1.78/src/ansar_create.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-08 02:09:24.000000 ansar_create-0.1.78/src/ansar_create.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      104 2024-05-08 02:09:24.000000 ansar_create-0.1.78/src/ansar_create.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       22 2024-05-08 02:09:24.000000 ansar_create-0.1.78/src/ansar_create.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-08 02:09:24.000000 ansar_create-0.1.78/src/ansar_create.egg-info/top_level.txt
```

### Comparing `ansar_create-0.1.77/LICENSE` & `ansar_create-0.1.78/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/PKG-INFO` & `ansar_create-0.1.78/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-create
-Version: 0.1.77
+Version: 0.1.78
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com>
 Project-URL: Documentation, https://ansar-create-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_create-0.1.77/README.md` & `ansar_create-0.1.78/README.md`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/pyproject.toml` & `ansar_create-0.1.78/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/setup.py` & `ansar_create-0.1.78/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/command/ansar_command.py` & `ansar_create-0.1.78/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/command/ansar_group.py` & `ansar_create-0.1.78/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/__init__.py` & `ansar_create-0.1.78/src/ansar/create/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-create.git
 Branch: main
-Commit: 2ee07a3418bfb17144225b665bb2322407b12435
-Version: 0.1.76 (2024-05-08@13:34:36+NZST)
+Commit: 113fa67042ed729bbea86f8b990670354a32355c
+Version: 0.1.77 (2024-05-08@14:09:21+NZST)
 """
 
 from ansar.encode import *
 
 from .coding import cannot, lor
 from .space import NO_SUCH_ADDRESS
 from .space import create_an_object, find_object, destroy_an_object
```

### Comparing `ansar_create-0.1.77/src/ansar/create/binding.py` & `ansar_create-0.1.78/src/ansar/create/binding.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/coding.py` & `ansar_create-0.1.78/src/ansar/create/coding.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/grouping.py` & `ansar_create-0.1.78/src/ansar/create/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/home.py` & `ansar_create-0.1.78/src/ansar/create/home.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/latching.py` & `ansar_create-0.1.78/src/ansar/create/latching.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/lifecycle.py` & `ansar_create-0.1.78/src/ansar/create/lifecycle.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/locking.py` & `ansar_create-0.1.78/src/ansar/create/locking.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/log.py` & `ansar_create-0.1.78/src/ansar/create/log.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/machine.py` & `ansar_create-0.1.78/src/ansar/create/machine.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/object.py` & `ansar_create-0.1.78/src/ansar/create/object.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,22 +28,24 @@
 __docformat__ = 'restructuredtext'
 
 import os
 import sys
 import signal
 import uuid
 import time
+import tempfile
 
 import ansar.encode as ar
 
 from .lifecycle import *
 from .point import *
 from .log import *
 from .rolling import *
 from .locking import *
+from .processing import *
 from .root import *
 from .home import *
 
 __all__ = [
 	'POINT_OF_ORIGIN',
 	'start_origin',
 	'run_origin',
@@ -130,28 +132,30 @@
 			debug_level=None,
 			home_path=None, role_name=None,	# Fully-homed only.
 			point_of_origin=None,			# Variants on home execution.
 			help=False,						# Administrative features.
 			dump_settings=False,
 			dump_input=False,
 			store_settings=False, store_input=False, factory_reset=False,
+			edit_settings=False,
 			settings_file=None, input_file=None, output_file=None,
 			group_pid=None):
 		self.pure_object = pure_object
 		self.call_signature = call_signature
 		self.debug_level = debug_level
 		self.home_path = home_path
 		self.role_name = role_name
 		self.point_of_origin = point_of_origin
 		self.help = help
 		self.dump_settings = dump_settings
 		self.dump_input = dump_input
 		self.store_settings = store_settings
 		self.store_input = store_input
 		self.factory_reset = factory_reset
+		self.edit_settings = edit_settings
 		self.settings_file = settings_file
 		self.input_file = input_file
 		self.output_file = output_file
 		self.group_pid = group_pid
 
 	def homed(self):
 		if self.home_path and self.role_name:
@@ -167,27 +171,28 @@
 	'point_of_origin': POINT_OF_ORIGIN,
 	'help': ar.Boolean(),
 	'dump_settings': ar.Boolean(),
 	'dump_input': ar.Boolean(),
 	'store_settings': ar.Boolean(),
 	'store_input': ar.Boolean(),
 	'factory_reset': ar.Boolean(),
+	'edit_settings': ar.Boolean(),
 	'settings_file': ar.Unicode(),
 	'input_file': ar.Unicode(),
 	'output_file': ar.Unicode(),
 	'group_pid': ar.Integer8(),
 }
 
 ar.bind_message(ObjectSettings, object_schema=OBJECT_SETTINGS_SCHEMA)
 
 object_settings = ObjectSettings()
 
 #
 #
-co = ar.Gas(command_args=[], environment_variables={}, command_executable=None, command_words=[], unknown=None, custom_settings=None, input=None, role=None, signal_received=None)
+co = ar.Gas(command_args=[], environment_variables={}, command_executable=None, command_words=[], custom_settings=None, input=None, role=None, signal_received=None)
 
 #
 #
 def object_role():
 	"""Global access to the runtime context assumed by create_object(). Returns a HomeRole."""
 	return co.role
 
@@ -570,17 +575,17 @@
 			lf, sf = r
 			lk, sk = lf.keys(), sf.keys()
 			ld = [k for k in lk]
 			sd = [k for k in sk]
 			# Workaround to allow group_port from ansar-group process to
 			# be ignored but still flag anything else. Allows create_object
 			# apps to run under ansar-group.
-			if len(ld) == 1 and ld[1] == 'group-port' and len(sd) == 0:
+			if len(ld) == 1 and ld[0] == 'group-port' and len(sd) == 0:
 				pass
-			elif len(sd) == 1 and sd[1] == 'gp' and len(ld) == 0:
+			elif len(sd) == 1 and sd[0] == 'gp' and len(ld) == 0:
 				pass
 			else:
 				ld.extend(sd)
 				unknown = ', '.join(ld)
 				f = ar.Failed(object_args=(None, f'unknown ({unknown}) settings detected in arguments'))
 				raise ar.Incomplete(f)
 
@@ -880,23 +885,23 @@
 			raise ar.Incomplete(None)
 
 		# Extract values from the words and args off the command
 		# line, with reference to the name/type ino in the
 		# settings object.
 		settings, unknown = load_settings(role, factory_settings, args, upgrade)
 
-		co.unknown_args = unknown
 		co.custom_settings = settings
 
 		# Non-operational features, i.e. command object not called.
 		# Place settings for this command on stdout.
 		if object_settings.help:
 			ar.command_help(object_type, settings, parameter_table)
 			raise ar.Incomplete(None)
-		elif object_settings.dump_settings:
+
+		if object_settings.dump_settings:
 			if settings is None:
 				f = ar.Failed(settings_dump=(None, 'no settings defined'))
 				raise ar.Incomplete(f)
 			try:
 				ar.output_encode(settings)
 			except ar.CodecFailed as e:
 				f = ar.Failed(settings_dump=(e, None))
@@ -913,15 +918,14 @@
 				f = ar.Failed(settings_changed=(e, None))
 				raise ar.Incomplete(f)
 
 		if object_settings.factory_reset:
 			if settings is None:
 				raise ar.Incomplete(Ack())
 			try:
-				ar.output_encode(settings)
 				decoration_store(role.role_settings, factory_settings)
 				raise ar.Incomplete(Ack())
 			except (ar.FileFailure, ar.CodecFailed) as e:
 				f = ar.Failed(settings_reset=(e, None))
 				raise ar.Incomplete(f)
 
 		# Primary input. Object expects to work on an instance of
```

### Comparing `ansar_create-0.1.77/src/ansar/create/pending.py` & `ansar_create-0.1.78/src/ansar/create/pending.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/point.py` & `ansar_create-0.1.78/src/ansar/create/point.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/procedure.py` & `ansar_create-0.1.78/src/ansar/create/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/processing.py` & `ansar_create-0.1.78/src/ansar/create/processing.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/properties.py` & `ansar_create-0.1.78/src/ansar/create/properties.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/retry.py` & `ansar_create-0.1.78/src/ansar/create/retry.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/rolling.py` & `ansar_create-0.1.78/src/ansar/create/rolling.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/root.py` & `ansar_create-0.1.78/src/ansar/create/root.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/space.py` & `ansar_create-0.1.78/src/ansar/create/space.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/storage.py` & `ansar_create-0.1.78/src/ansar/create/storage.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/test.py` & `ansar_create-0.1.78/src/ansar/create/test.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar/create/timing.py` & `ansar_create-0.1.78/src/ansar/create/timing.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.77/src/ansar_create.egg-info/PKG-INFO` & `ansar_create-0.1.78/src/ansar_create.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-create
-Version: 0.1.77
+Version: 0.1.78
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com>
 Project-URL: Documentation, https://ansar-create-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_create-0.1.77/src/ansar_create.egg-info/SOURCES.txt` & `ansar_create-0.1.78/src/ansar_create.egg-info/SOURCES.txt`

 * *Files identical despite different names*

