# Comparing `tmp/ansar-create-0.1.76.tar.gz` & `tmp/ansar_create-0.1.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar-create-0.1.76.tar", last modified: Thu Mar 28 02:35:34 2024, max compression
+gzip compressed data, was "ansar_create-0.1.77.tar", last modified: Wed May  8 01:34:39 2024, max compression
```

## Comparing `ansar-create-0.1.76.tar` & `ansar_create-0.1.77.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-28 02:35:34.288097 ansar-create-0.1.76/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:18.000000 ansar-create-0.1.76/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-03-28 02:35:34.288097 ansar-create-0.1.76/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      901 2023-06-17 21:18:11.000000 ansar-create-0.1.76/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      718 2024-03-27 05:56:05.000000 ansar-create-0.1.76/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-03-28 02:35:34.288097 ansar-create-0.1.76/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     2139 2024-03-27 05:55:54.000000 ansar-create-0.1.76/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-28 02:35:34.284097 ansar-create-0.1.76/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-28 02:35:34.284097 ansar-create-0.1.76/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-28 02:35:34.288097 ansar-create-0.1.76/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    13081 2024-01-02 02:57:04.000000 ansar-create-0.1.76/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8950 2024-02-25 02:39:34.000000 ansar-create-0.1.76/src/ansar/command/ansar_group.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-28 02:35:34.288097 ansar-create-0.1.76/src/ansar/create/
--rw-rw-r--   0 scott     (1000) scott     (1000)     5722 2024-03-28 02:34:59.000000 ansar-create-0.1.76/src/ansar/create/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2654 2023-07-13 04:39:47.000000 ansar-create-0.1.76/src/ansar/create/binding.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1989 2023-12-23 01:56:16.000000 ansar-create-0.1.76/src/ansar/create/coding.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1857 2024-01-19 15:16:48.000000 ansar-create-0.1.76/src/ansar/create/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    13837 2024-02-24 20:57:36.000000 ansar-create-0.1.76/src/ansar/create/home.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3607 2024-02-14 21:31:28.000000 ansar-create-0.1.76/src/ansar/create/latching.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7383 2024-03-24 15:57:41.000000 ansar-create-0.1.76/src/ansar/create/lifecycle.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     4061 2024-01-25 13:13:42.000000 ansar-create-0.1.76/src/ansar/create/locking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6164 2023-07-13 04:40:10.000000 ansar-create-0.1.76/src/ansar/create/log.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8495 2023-07-13 04:40:11.000000 ansar-create-0.1.76/src/ansar/create/machine.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    29599 2024-03-26 20:00:39.000000 ansar-create-0.1.76/src/ansar/create/object.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9071 2024-01-18 15:23:10.000000 ansar-create-0.1.76/src/ansar/create/pending.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    29472 2024-02-28 13:52:41.000000 ansar-create-0.1.76/src/ansar/create/point.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    79049 2024-02-27 21:07:28.000000 ansar-create-0.1.76/src/ansar/create/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    31841 2024-01-22 04:26:11.000000 ansar-create-0.1.76/src/ansar/create/processing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3099 2024-03-26 19:19:48.000000 ansar-create-0.1.76/src/ansar/create/properties.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3741 2024-03-07 07:59:16.000000 ansar-create-0.1.76/src/ansar/create/retry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5938 2024-02-27 14:04:16.000000 ansar-create-0.1.76/src/ansar/create/rolling.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7477 2023-12-23 15:53:02.000000 ansar-create-0.1.76/src/ansar/create/root.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14196 2024-03-22 18:43:05.000000 ansar-create-0.1.76/src/ansar/create/space.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    19735 2024-03-22 18:43:09.000000 ansar-create-0.1.76/src/ansar/create/storage.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3959 2024-01-15 15:55:19.000000 ansar-create-0.1.76/src/ansar/create/test.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5100 2024-01-26 08:38:29.000000 ansar-create-0.1.76/src/ansar/create/timing.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-03-28 02:35:34.288097 ansar-create-0.1.76/src/ansar_create.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-03-28 02:35:34.000000 ansar-create-0.1.76/src/ansar_create.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      986 2024-03-28 02:35:34.000000 ansar-create-0.1.76/src/ansar_create.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-03-28 02:35:34.000000 ansar-create-0.1.76/src/ansar_create.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      104 2024-03-28 02:35:34.000000 ansar-create-0.1.76/src/ansar_create.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       22 2024-03-28 02:35:34.000000 ansar-create-0.1.76/src/ansar_create.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-03-28 02:35:34.000000 ansar-create-0.1.76/src/ansar_create.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:34:39.536899 ansar_create-0.1.77/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:18.000000 ansar_create-0.1.77/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-08 01:34:39.536899 ansar_create-0.1.77/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      901 2023-06-17 21:18:11.000000 ansar_create-0.1.77/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      718 2024-03-27 05:56:05.000000 ansar_create-0.1.77/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-08 01:34:39.536899 ansar_create-0.1.77/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2139 2024-03-27 05:55:54.000000 ansar_create-0.1.77/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:34:39.532899 ansar_create-0.1.77/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:34:39.532899 ansar_create-0.1.77/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:34:39.532899 ansar_create-0.1.77/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13081 2024-01-02 02:57:04.000000 ansar_create-0.1.77/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8950 2024-02-25 02:39:34.000000 ansar_create-0.1.77/src/ansar/command/ansar_group.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:34:39.536899 ansar_create-0.1.77/src/ansar/create/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5706 2024-05-08 01:34:36.000000 ansar_create-0.1.77/src/ansar/create/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2654 2023-07-13 04:39:47.000000 ansar_create-0.1.77/src/ansar/create/binding.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1989 2023-12-23 01:56:16.000000 ansar_create-0.1.77/src/ansar/create/coding.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1857 2024-01-19 15:16:48.000000 ansar_create-0.1.77/src/ansar/create/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13837 2024-02-24 20:57:36.000000 ansar_create-0.1.77/src/ansar/create/home.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3607 2024-02-14 21:31:28.000000 ansar_create-0.1.77/src/ansar/create/latching.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7383 2024-03-24 15:57:41.000000 ansar_create-0.1.77/src/ansar/create/lifecycle.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4061 2024-01-25 13:13:42.000000 ansar_create-0.1.77/src/ansar/create/locking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6164 2023-07-13 04:40:10.000000 ansar_create-0.1.77/src/ansar/create/log.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8495 2023-07-13 04:40:11.000000 ansar_create-0.1.77/src/ansar/create/machine.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    29638 2024-05-07 19:48:13.000000 ansar_create-0.1.77/src/ansar/create/object.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9071 2024-01-18 15:23:10.000000 ansar_create-0.1.77/src/ansar/create/pending.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    29472 2024-02-28 13:52:41.000000 ansar_create-0.1.77/src/ansar/create/point.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    79049 2024-04-14 03:56:16.000000 ansar_create-0.1.77/src/ansar/create/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    31841 2024-01-22 04:26:11.000000 ansar_create-0.1.77/src/ansar/create/processing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3099 2024-03-26 19:19:48.000000 ansar_create-0.1.77/src/ansar/create/properties.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3741 2024-03-07 07:59:16.000000 ansar_create-0.1.77/src/ansar/create/retry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5938 2024-02-27 14:04:16.000000 ansar_create-0.1.77/src/ansar/create/rolling.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7477 2023-12-23 15:53:02.000000 ansar_create-0.1.77/src/ansar/create/root.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14196 2024-03-22 18:43:05.000000 ansar_create-0.1.77/src/ansar/create/space.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    19735 2024-03-22 18:43:09.000000 ansar_create-0.1.77/src/ansar/create/storage.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3959 2024-01-15 15:55:19.000000 ansar_create-0.1.77/src/ansar/create/test.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5100 2024-01-26 08:38:29.000000 ansar_create-0.1.77/src/ansar/create/timing.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:34:39.536899 ansar_create-0.1.77/src/ansar_create.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-08 01:34:39.000000 ansar_create-0.1.77/src/ansar_create.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      986 2024-05-08 01:34:39.000000 ansar_create-0.1.77/src/ansar_create.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-08 01:34:39.000000 ansar_create-0.1.77/src/ansar_create.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      104 2024-05-08 01:34:39.000000 ansar_create-0.1.77/src/ansar_create.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       22 2024-05-08 01:34:39.000000 ansar_create-0.1.77/src/ansar_create.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-08 01:34:39.000000 ansar_create-0.1.77/src/ansar_create.egg-info/top_level.txt
```

### Comparing `ansar-create-0.1.76/LICENSE` & `ansar_create-0.1.77/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/PKG-INFO` & `ansar_create-0.1.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-create
-Version: 0.1.76
+Version: 0.1.77
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com>
 Project-URL: Documentation, https://ansar-create-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-create-0.1.76/README.md` & `ansar_create-0.1.77/README.md`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/pyproject.toml` & `ansar_create-0.1.77/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/setup.py` & `ansar_create-0.1.77/setup.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/command/ansar_command.py` & `ansar_create-0.1.77/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/command/ansar_group.py` & `ansar_create-0.1.77/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/__init__.py` & `ansar_create-0.1.77/src/ansar/create/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-create.git
 Branch: main
-Commit: 6776fd1ae0db923d4c04136ff27d8b50a2677e50
-Version: 0.1.75 (2024-03-28@15:34:59+NZDT)
+Commit: 2ee07a3418bfb17144225b665bb2322407b12435
+Version: 0.1.76 (2024-05-08@13:34:36+NZST)
 """
 
 from ansar.encode import *
 
 from .coding import cannot, lor
 from .space import NO_SUCH_ADDRESS
 from .space import create_an_object, find_object, destroy_an_object
@@ -98,15 +98,15 @@
 from .procedure import procedure_get, procedure_set, procedure_edit
 from .procedure import procedure_deploy, procedure_snapshot
 
 from .object import POINT_OF_ORIGIN, start_origin, run_origin
 from .object import LOG_NUMBER
 from .object import ObjectSettings, object_settings
 from .object import object_role, object_args, object_variables, object_executable, object_words
-from .object import object_custom_settings, object_unknown, store_settings
+from .object import object_custom_settings, store_settings
 from .object import object_input
 from .object import object_resource_folder, object_tmp_folder, object_model_folder
 from .object import object_resource_path, object_tmp_path, object_model_path
 from .object import object_passing, sub_object_passing
 from .object import co
 from .object import create_object
```

### Comparing `ansar-create-0.1.76/src/ansar/create/binding.py` & `ansar_create-0.1.77/src/ansar/create/binding.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/coding.py` & `ansar_create-0.1.77/src/ansar/create/coding.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/grouping.py` & `ansar_create-0.1.77/src/ansar/create/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/home.py` & `ansar_create-0.1.77/src/ansar/create/home.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/latching.py` & `ansar_create-0.1.77/src/ansar/create/latching.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/lifecycle.py` & `ansar_create-0.1.77/src/ansar/create/lifecycle.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/locking.py` & `ansar_create-0.1.77/src/ansar/create/locking.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/log.py` & `ansar_create-0.1.77/src/ansar/create/log.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/machine.py` & `ansar_create-0.1.77/src/ansar/create/machine.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/object.py` & `ansar_create-0.1.77/src/ansar/create/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 	'object_role',
 	'object_resolve',
 	'object_args',
 	'object_variables',
 	'object_executable',
 	'object_words',
 	'object_custom_settings',
-	'object_unknown',
 	'store_settings',
 	'object_input',
 	'object_resource_folder',
 	'object_tmp_folder',
 	'object_model_folder',
 	'object_resource_path',
 	'object_tmp_path',
@@ -216,18 +215,14 @@
 	"""Global access to the words appearing on the command-line. Returns a list of words."""
 	return co.command_words
 
 def object_custom_settings():
 	"""Global access to the values decoded from persistent configuration. Returns the values or None."""
 	return co.custom_settings
 
-def object_unknown():
-	"""Global access to the values decoded from persistent configuration. Returns the values or None."""
-	return co.unknown_args
-
 def store_settings(settings):
 	"""Global mechanism for updating the persistent configuration. Returns indication of success."""
 	if co.role.role_settings is not None:
 		co.role.role_settings[1].store(settings)
 		co.role.role_settings[2] = settings
 		return True
 	return False
@@ -392,18 +387,14 @@
 
 	executable = os.path.abspath(sys.argv[0])
 	self.trace('Executable "%s" as object process (%d)' % (executable, os.getpid()))
 	self.trace('Working folder "%s"' % (os.getcwd()))
 	self.trace('Running object "%s"' % (object_type.__art__.path,))
 	self.trace('Class threads (%d) %s' % (len(pt.thread_classes), ','.join(name_counts)))
 
-	unknown = object_unknown()
-	if unknown is not None:
-		self.warning(f'Unknown settings ({unknown}) ignored')
-
 	pa = ()
 	if settings is not None:
 		pa = pa + (settings,)
 	if input is not None:
 		pa = pa + (input,)
 	if variables is not None:
 		pa = pa + (variables,)
@@ -576,18 +567,27 @@
 
 		x, r = ar.extract_args(settings, args, None)
 		if len(r[0]) > 0 or len(r[1]) > 0:
 			lf, sf = r
 			lk, sk = lf.keys(), sf.keys()
 			ld = [k for k in lk]
 			sd = [k for k in sk]
-			ld.extend(sd)
-			unknown = ', '.join(ld)
-			#f = ar.Failed(object_args=(None, f'unknown ({unknown}) settings detected in arguments'))
-			#raise ar.Incomplete(f)
+			# Workaround to allow group_port from ansar-group process to
+			# be ignored but still flag anything else. Allows create_object
+			# apps to run under ansar-group.
+			if len(ld) == 1 and ld[1] == 'group-port' and len(sd) == 0:
+				pass
+			elif len(sd) == 1 and sd[1] == 'gp' and len(ld) == 0:
+				pass
+			else:
+				ld.extend(sd)
+				unknown = ', '.join(ld)
+				f = ar.Failed(object_args=(None, f'unknown ({unknown}) settings detected in arguments'))
+				raise ar.Incomplete(f)
+
 		change = len(x[0]) or len(x[1])
 		if change:
 			ar.arg_values(settings, x)
 	except (ar.FileFailure, ar.CodecFailed) as e:
 		f = ar.Failed(settings_load=(e, None))
 		raise ar.Incomplete(f)
 	except ar.CommandError as e:
```

### Comparing `ansar-create-0.1.76/src/ansar/create/pending.py` & `ansar_create-0.1.77/src/ansar/create/pending.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/point.py` & `ansar_create-0.1.77/src/ansar/create/point.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/procedure.py` & `ansar_create-0.1.77/src/ansar/create/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/processing.py` & `ansar_create-0.1.77/src/ansar/create/processing.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/properties.py` & `ansar_create-0.1.77/src/ansar/create/properties.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/retry.py` & `ansar_create-0.1.77/src/ansar/create/retry.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/rolling.py` & `ansar_create-0.1.77/src/ansar/create/rolling.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/root.py` & `ansar_create-0.1.77/src/ansar/create/root.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/space.py` & `ansar_create-0.1.77/src/ansar/create/space.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/storage.py` & `ansar_create-0.1.77/src/ansar/create/storage.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/test.py` & `ansar_create-0.1.77/src/ansar/create/test.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar/create/timing.py` & `ansar_create-0.1.77/src/ansar/create/timing.py`

 * *Files identical despite different names*

### Comparing `ansar-create-0.1.76/src/ansar_create.egg-info/PKG-INFO` & `ansar_create-0.1.77/src/ansar_create.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-create
-Version: 0.1.76
+Version: 0.1.77
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com>
 Project-URL: Documentation, https://ansar-create-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar-create-0.1.76/src/ansar_create.egg-info/SOURCES.txt` & `ansar_create-0.1.77/src/ansar_create.egg-info/SOURCES.txt`

 * *Files identical despite different names*

