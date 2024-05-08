# Comparing `tmp/orangebox-0.3.0.tar.gz` & `tmp/orangebox-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orangebox-0.3.0.tar", last modified: Sun Feb  4 19:11:50 2024, max compression
+gzip compressed data, was "orangebox-0.3.1.tar", last modified: Wed May  8 18:32:37 2024, max compression
```

## Comparing `orangebox-0.3.0.tar` & `orangebox-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 kiri      (1000) kiri      (1002)        0 2024-02-04 19:11:50.142345 orangebox-0.3.0/
--rw-rw-r--   0 kiri      (1000) kiri      (1002)    35148 2024-02-02 07:53:51.000000 orangebox-0.3.0/LICENSE
--rw-r--r--   0 kiri      (1000) kiri      (1002)      628 2024-02-04 19:11:50.142345 orangebox-0.3.0/PKG-INFO
--rw-rw-r--   0 kiri      (1000) kiri      (1002)     3184 2024-02-04 16:55:59.000000 orangebox-0.3.0/README.md
-drwxrwxr-x   0 kiri      (1000) kiri      (1002)        0 2024-02-04 19:11:50.138345 orangebox-0.3.0/orangebox/
--rw-rw-r--   0 kiri      (1000) kiri      (1002)      789 2024-02-04 16:17:06.000000 orangebox-0.3.0/orangebox/__init__.py
--rw-rw-r--   0 kiri      (1000) kiri      (1002)     4893 2024-02-04 16:17:06.000000 orangebox-0.3.0/orangebox/context.py
--rw-rw-r--   0 kiri      (1000) kiri      (1002)     6509 2024-02-04 16:24:06.000000 orangebox-0.3.0/orangebox/decoders.py
--rw-rw-r--   0 kiri      (1000) kiri      (1002)     2507 2024-02-04 16:23:06.000000 orangebox-0.3.0/orangebox/events.py
--rw-rw-r--   0 kiri      (1000) kiri      (1002)    10555 2024-02-04 16:24:06.000000 orangebox-0.3.0/orangebox/parser.py
--rw-rw-r--   0 kiri      (1000) kiri      (1002)     2893 2024-02-04 16:20:47.000000 orangebox-0.3.0/orangebox/predictors.py
--rw-rw-r--   0 kiri      (1000) kiri      (1002)     9323 2024-02-04 16:24:06.000000 orangebox-0.3.0/orangebox/reader.py
--rw-rw-r--   0 kiri      (1000) kiri      (1002)     2249 2024-02-02 07:53:51.000000 orangebox-0.3.0/orangebox/tools.py
--rw-rw-r--   0 kiri      (1000) kiri      (1002)     3806 2024-02-02 07:53:51.000000 orangebox-0.3.0/orangebox/types.py
-drwxrwxr-x   0 kiri      (1000) kiri      (1002)        0 2024-02-04 19:11:50.142345 orangebox-0.3.0/orangebox.egg-info/
--rw-r--r--   0 kiri      (1000) kiri      (1002)      628 2024-02-04 19:11:50.000000 orangebox-0.3.0/orangebox.egg-info/PKG-INFO
--rw-rw-r--   0 kiri      (1000) kiri      (1002)      376 2024-02-04 19:11:50.000000 orangebox-0.3.0/orangebox.egg-info/SOURCES.txt
--rw-rw-r--   0 kiri      (1000) kiri      (1002)        1 2024-02-04 19:11:50.000000 orangebox-0.3.0/orangebox.egg-info/dependency_links.txt
--rw-rw-r--   0 kiri      (1000) kiri      (1002)       10 2024-02-04 19:11:50.000000 orangebox-0.3.0/orangebox.egg-info/top_level.txt
-drwxrwxr-x   0 kiri      (1000) kiri      (1002)        0 2024-02-04 19:11:50.142345 orangebox-0.3.0/scripts/
--rwxrwxr-x   0 kiri      (1000) kiri      (1002)     2422 2024-02-02 07:53:51.000000 orangebox-0.3.0/scripts/bb2csv
--rwxrwxr-x   0 kiri      (1000) kiri      (1002)     3473 2024-02-02 07:53:51.000000 orangebox-0.3.0/scripts/bbsplit
--rw-rw-r--   0 kiri      (1000) kiri      (1002)       38 2024-02-04 19:11:50.142345 orangebox-0.3.0/setup.cfg
--rwxrwxr-x   0 kiri      (1000) kiri      (1002)      822 2024-02-02 07:53:51.000000 orangebox-0.3.0/setup.py
+drwxrwxr-x   0 kiri      (1000) kiri      (1002)        0 2024-05-08 18:32:37.477621 orangebox-0.3.1/
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)    35148 2024-02-02 07:53:51.000000 orangebox-0.3.1/LICENSE
+-rw-r--r--   0 kiri      (1000) kiri      (1002)      628 2024-05-08 18:32:37.477621 orangebox-0.3.1/PKG-INFO
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)     3252 2024-05-08 18:19:07.000000 orangebox-0.3.1/README.md
+drwxrwxr-x   0 kiri      (1000) kiri      (1002)        0 2024-05-08 18:32:37.477621 orangebox-0.3.1/orangebox/
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)      789 2024-05-08 07:05:48.000000 orangebox-0.3.1/orangebox/__init__.py
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)     4893 2024-02-04 16:17:06.000000 orangebox-0.3.1/orangebox/context.py
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)     6509 2024-02-04 16:24:06.000000 orangebox-0.3.1/orangebox/decoders.py
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)     2507 2024-02-04 16:23:06.000000 orangebox-0.3.1/orangebox/events.py
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)    10555 2024-02-04 16:24:06.000000 orangebox-0.3.1/orangebox/parser.py
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)     2893 2024-02-04 16:20:47.000000 orangebox-0.3.1/orangebox/predictors.py
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)     9323 2024-02-04 16:24:06.000000 orangebox-0.3.1/orangebox/reader.py
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)     2249 2024-02-02 07:53:51.000000 orangebox-0.3.1/orangebox/tools.py
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)     3806 2024-02-02 07:53:51.000000 orangebox-0.3.1/orangebox/types.py
+drwxrwxr-x   0 kiri      (1000) kiri      (1002)        0 2024-05-08 18:32:37.477621 orangebox-0.3.1/orangebox.egg-info/
+-rw-r--r--   0 kiri      (1000) kiri      (1002)      628 2024-05-08 18:32:37.000000 orangebox-0.3.1/orangebox.egg-info/PKG-INFO
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)      391 2024-05-08 18:32:37.000000 orangebox-0.3.1/orangebox.egg-info/SOURCES.txt
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)        1 2024-05-08 18:32:37.000000 orangebox-0.3.1/orangebox.egg-info/dependency_links.txt
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)       10 2024-05-08 18:32:37.000000 orangebox-0.3.1/orangebox.egg-info/top_level.txt
+drwxrwxr-x   0 kiri      (1000) kiri      (1002)        0 2024-05-08 18:32:37.477621 orangebox-0.3.1/scripts/
+-rwxrwxr-x   0 kiri      (1000) kiri      (1002)     2422 2024-05-08 18:22:07.000000 orangebox-0.3.1/scripts/bb2csv
+-rwxrwxr-x   0 kiri      (1000) kiri      (1002)     5366 2024-05-08 18:21:00.000000 orangebox-0.3.1/scripts/bb2gpx
+-rwxrwxr-x   0 kiri      (1000) kiri      (1002)     3473 2024-02-02 07:53:51.000000 orangebox-0.3.1/scripts/bbsplit
+-rw-rw-r--   0 kiri      (1000) kiri      (1002)       38 2024-05-08 18:32:37.477621 orangebox-0.3.1/setup.cfg
+-rwxrwxr-x   0 kiri      (1000) kiri      (1002)      840 2024-05-08 07:01:48.000000 orangebox-0.3.1/setup.py
```

### Comparing `orangebox-0.3.0/LICENSE` & `orangebox-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `orangebox-0.3.0/PKG-INFO` & `orangebox-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orangebox
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Cleanflight/Betaflight blackbox log parser written in Python 3
 Home-page: https://github.com/atomgomba/orangebox
 Author: Károly Kiripolszky
 Author-email: karcsi@ekezet.com
 Keywords: blackbox cleanflight betaflight
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
```

### Comparing `orangebox-0.3.0/README.md` & `orangebox-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 
 * Contributions are very welcome!
 * Please follow the [PEP8](https://www.python.org/dev/peps/pep-0008/) Style Guido.
 * [More info](https://orangebox.readthedocs.io/#development) in the docs.
 
 ## Changelog
 
+### 0.3.1
+
+* Add `bb2gpx` utility for converting GPS data into GPX
+
 ### 0.3.0
 
 * Add support for GPS frames (thanks to [@tblaha](https://github.com/tblaha)!)
 
 ### 0.2.0
 
 * Improved `Reader` class can now handle multiple logs in a single file
```

### Comparing `orangebox-0.3.0/orangebox/__init__.py` & `orangebox-0.3.1/orangebox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from .parser import Parser
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

### Comparing `orangebox-0.3.0/orangebox/context.py` & `orangebox-0.3.1/orangebox/context.py`

 * *Files identical despite different names*

### Comparing `orangebox-0.3.0/orangebox/decoders.py` & `orangebox-0.3.1/orangebox/decoders.py`

 * *Files identical despite different names*

### Comparing `orangebox-0.3.0/orangebox/events.py` & `orangebox-0.3.1/orangebox/events.py`

 * *Files identical despite different names*

### Comparing `orangebox-0.3.0/orangebox/parser.py` & `orangebox-0.3.1/orangebox/parser.py`

 * *Files identical despite different names*

### Comparing `orangebox-0.3.0/orangebox/predictors.py` & `orangebox-0.3.1/orangebox/predictors.py`

 * *Files identical despite different names*

### Comparing `orangebox-0.3.0/orangebox/reader.py` & `orangebox-0.3.1/orangebox/reader.py`

 * *Files identical despite different names*

### Comparing `orangebox-0.3.0/orangebox/tools.py` & `orangebox-0.3.1/orangebox/tools.py`

 * *Files identical despite different names*

### Comparing `orangebox-0.3.0/orangebox/types.py` & `orangebox-0.3.1/orangebox/types.py`

 * *Files identical despite different names*

### Comparing `orangebox-0.3.0/orangebox.egg-info/PKG-INFO` & `orangebox-0.3.1/orangebox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orangebox
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Cleanflight/Betaflight blackbox log parser written in Python 3
 Home-page: https://github.com/atomgomba/orangebox
 Author: Károly Kiripolszky
 Author-email: karcsi@ekezet.com
 Keywords: blackbox cleanflight betaflight
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
```

### Comparing `orangebox-0.3.0/scripts/bb2csv` & `orangebox-0.3.1/scripts/bb2csv`

 * *Files identical despite different names*

### Comparing `orangebox-0.3.0/scripts/bbsplit` & `orangebox-0.3.1/scripts/bbsplit`

 * *Files identical despite different names*

### Comparing `orangebox-0.3.0/setup.py` & `orangebox-0.3.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import orangebox
 
 setup(
     name="orangebox",
     version=orangebox.__version__,
     packages=["orangebox"],
-    scripts=["scripts/bb2csv", "scripts/bbsplit"],
+    scripts=["scripts/bb2csv", "scripts/bbsplit", "scripts/bb2gpx"],
     author="Károly Kiripolszky",
     author_email="karcsi@ekezet.com",
     description="A Cleanflight/Betaflight blackbox log parser written in Python 3",
     keywords="blackbox cleanflight betaflight",
     url="https://github.com/atomgomba/orangebox",
     classifiers=[
         "Programming Language :: Python :: 3 :: Only",
```

