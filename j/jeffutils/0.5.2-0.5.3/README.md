# Comparing `tmp/jeffutils-0.5.2.tar.gz` & `tmp/jeffutils-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.5.2.tar", last modified: Wed May  1 21:06:04 2024, max compression
+gzip compressed data, was "jeffutils-0.5.3.tar", last modified: Wed May  8 21:33:56 2024, max compression
```

## Comparing `jeffutils-0.5.2.tar` & `jeffutils-0.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-01 21:06:04.766961 jeffutils-0.5.2/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.2/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-01 21:06:04.766961 jeffutils-0.5.2/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.2/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.2/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-01 21:06:04.766961 jeffutils-0.5.2/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-01 21:05:59.000000 jeffutils-0.5.2/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-01 21:06:04.766961 jeffutils-0.5.2/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-01 21:06:04.766961 jeffutils-0.5.2/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.2/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    16271 2024-05-01 21:05:36.000000 jeffutils-0.5.2/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-01 21:06:04.766961 jeffutils-0.5.2/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-01 21:06:04.000000 jeffutils-0.5.2/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-01 21:06:04.000000 jeffutils-0.5.2/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-01 21:06:04.000000 jeffutils-0.5.2/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-01 21:06:04.000000 jeffutils-0.5.2/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-08 21:33:56.065231 jeffutils-0.5.3/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.5.3/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-08 21:33:56.065231 jeffutils-0.5.3/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.5.3/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.5.3/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-08 21:33:56.065231 jeffutils-0.5.3/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-08 21:33:52.000000 jeffutils-0.5.3/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-08 21:33:56.061231 jeffutils-0.5.3/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-08 21:33:56.065231 jeffutils-0.5.3/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.5.3/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    16498 2024-05-08 21:33:36.000000 jeffutils-0.5.3/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-08 21:33:56.065231 jeffutils-0.5.3/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-08 21:33:56.000000 jeffutils-0.5.3/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-08 21:33:56.000000 jeffutils-0.5.3/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-08 21:33:56.000000 jeffutils-0.5.3/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-08 21:33:56.000000 jeffutils-0.5.3/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.5.2/LICENSE.txt` & `jeffutils-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.5.2/setup.py` & `jeffutils-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.5.2',
+    version='0.5.3',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.5.2/src/jeffutils/utils.py` & `jeffutils-0.5.3/src/jeffutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 def stack_trace(e):
     """returns a string representation of the stack trace to
     help with debugging and error messages
     """
     return "".join(traceback.TracebackException.from_exception(e).format())
 
 def curr_time_str(format="%m-%d-%Y"):
-    """returns the current time as a string YYYY-MM-DD"""
+    """returns the current time as a string MM-DD-YYYY"""
     now = datetime.now(timezone.utc)
     now_str = now.strftime(format)
     return now_str
 
-def current_time(utc=True, string=True, timestamp=False, hour_24=False):
+def current_time(utc=True, string=True, timestamp=False, hour_24=False, seconds=False):
     """prints the current time in YYYY-MM-DD HH:MM pm/am format
     can specify current utc time or current local time
     default local
     """
     if utc:
         now = datetime.now(timezone.utc)
     else:
@@ -49,23 +49,30 @@
 
     if timestamp:
         return now.timestamp()
 
     if not string:
         return now
 
-    if not hour_24:
-        format = "%Y-%m-%d %I:%M %p"
+    if seconds:
+        if not hour_24:
+            format = "%Y-%m-%d %I:%M:%S %p"
+        else:
+            format = "%Y-%m-%d %H:%M:%S"
     else:
-        format = "%Y-%m-%d %H:%M"
+        if not hour_24:
+            format = "%Y-%m-%d %I:%M %p"
+        else:
+            format = "%Y-%m-%d %H:%M"
         
     current_time_str = now.strftime(format)
     return current_time_str
 
-def log_print(*args, end="\n", flush=False, sep=" ", filepath="logs/live_log.txt", header=False, utc=False, only_log=False):
+def log_print(*args, end="\n", flush=False, sep=" ", filepath="logs/live_log.txt", 
+              header=False, utc=False, only_log=False, seconds=False):
     """functions like a normal print, but also sends whatever is printed to
     a specified file with './print_log.txt' set as the default
     """
     string = ""
     for i, a in enumerate(args):
         string += str(a)
         if i < len(args) - 1:
@@ -81,15 +88,15 @@
     # Create the directory if it doesn't exist
     if directory and not os.path.exists(directory):
         os.makedirs(directory)
 
     # add the output to the filepath specified
     with open(filepath, "a+") as file:
         if header:
-            file.write(current_time(string=True, utc=utc, timestamp=False))
+            file.write(current_time(string=True, utc=utc, timestamp=False, seconds=seconds))
             file.write("\n" + "-"*3 + "\n")
         file.write(string)
         file.write(end)
         if header:
             file.write("\n" + "-"*3 + "\n")
             
 def format_perc(perc):
```

