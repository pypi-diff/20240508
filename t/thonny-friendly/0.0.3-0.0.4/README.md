# Comparing `tmp/thonny-friendly-0.0.3.tar.gz` & `tmp/thonny_friendly-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thonny-friendly-0.0.3.tar", last modified: Sat Feb 17 22:40:34 2024, max compression
+gzip compressed data, was "thonny_friendly-0.0.4.tar", last modified: Tue May  7 20:51:15 2024, max compression
```

## Comparing `thonny-friendly-0.0.3.tar` & `thonny_friendly-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-02-17 22:40:34.828655 thonny-friendly-0.0.3/
--rw-rw-rw-   0        0        0     1700 2024-02-17 22:40:34.828655 thonny-friendly-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      105 2024-02-17 22:24:15.000000 thonny-friendly-0.0.3/README.md
--rw-rw-rw-   0        0        0     1584 2024-02-17 22:40:08.000000 thonny-friendly-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       33 2024-02-17 22:22:36.000000 thonny-friendly-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       88 2024-02-17 22:40:34.831673 thonny-friendly-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      602 2024-02-17 22:24:45.000000 thonny-friendly-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-17 22:40:34.827655 thonny-friendly-0.0.3/thonny_friendly.egg-info/
--rw-rw-rw-   0        0        0     1700 2024-02-17 22:40:34.000000 thonny-friendly-0.0.3/thonny_friendly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2024-02-17 22:40:34.000000 thonny-friendly-0.0.3/thonny_friendly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-17 22:40:34.000000 thonny-friendly-0.0.3/thonny_friendly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-02-17 22:40:34.000000 thonny-friendly-0.0.3/thonny_friendly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-02-17 22:40:34.000000 thonny-friendly-0.0.3/thonny_friendly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-17 22:40:34.784136 thonny-friendly-0.0.3/thonnycontrib/
-drwxrwxrwx   0        0        0        0 2024-02-17 22:40:34.825657 thonny-friendly-0.0.3/thonnycontrib/thonny_friendly/
--rw-rw-rw-   0        0        0     7168 2024-02-17 22:39:52.000000 thonny-friendly-0.0.3/thonnycontrib/thonny_friendly/__init__.py
--rw-rw-rw-   0        0        0     3742 2024-02-17 17:42:22.000000 thonny-friendly-0.0.3/thonnycontrib/thonny_friendly/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:51:15.268736 thonny_friendly-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-07 20:51:15.268736 thonny_friendly-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 20:51:11.000000 thonny_friendly-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-07 20:51:11.000000 thonny_friendly-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 20:51:11.000000 thonny_friendly-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 20:51:15.268736 thonny_friendly-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-07 20:51:11.000000 thonny_friendly-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:51:15.268736 thonny_friendly-0.0.4/thonny_friendly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-07 20:51:15.000000 thonny_friendly-0.0.4/thonny_friendly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-07 20:51:15.000000 thonny_friendly-0.0.4/thonny_friendly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:51:15.000000 thonny_friendly-0.0.4/thonny_friendly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 20:51:15.000000 thonny_friendly-0.0.4/thonny_friendly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 20:51:15.000000 thonny_friendly-0.0.4/thonny_friendly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:51:15.268736 thonny_friendly-0.0.4/thonnycontrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:51:15.268736 thonny_friendly-0.0.4/thonnycontrib/thonny_friendly/
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-05-07 20:51:11.000000 thonny_friendly-0.0.4/thonnycontrib/thonny_friendly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-07 20:51:11.000000 thonny_friendly-0.0.4/thonnycontrib/thonny_friendly/parser.py
```

### Comparing `thonny-friendly-0.0.3/PKG-INFO` & `thonny_friendly-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-Metadata-Version: 2.1
-Name: thonny-friendly
-Version: 0.0.3
-Summary: A plug-in which offers primitive support (for now ) for Friendly_traceback python package in Thonny IDE .
-Home-page: https://github.com/selmen2004/thonny-friendly
-Author: Selmen Arous
-Author-email: Selmen Arous <selmen.arous@gmail.com>
-License: GPL version 3
-Keywords: Friendly,Friendly_traceback,beginner,Tunisia,School,Teaching,Education
-Platform: Windows
-Platform: macOS
-Platform: Linux
-Classifier: Environment :: MacOS X
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: Environment :: X11 Applications
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: Freeware
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Education
-Classifier: Topic :: Software Development
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-Requires-Dist: thonny>=3.2.1
-
-A plug-in which offers primitive support (for now ) for Friendly_traceback python package in Thonny IDE .
+Metadata-Version: 2.1
+Name: thonny-friendly
+Version: 0.0.4
+Summary: A plug-in which offers primitive support (for now ) for Friendly_traceback python package in Thonny IDE .
+Home-page: https://github.com/selmen2004/thonny-friendly
+Author: Selmen Arous
+Author-email: Selmen Arous <selmen.arous@gmail.com>
+License: GPL version 3
+Keywords: Friendly,Friendly_traceback,beginner,Tunisia,School,Teaching,Education
+Platform: Windows
+Platform: macOS
+Platform: Linux
+Classifier: Environment :: MacOS X
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Environment :: X11 Applications
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: Freeware
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Education
+Classifier: Topic :: Software Development
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+Requires-Dist: thonny>=3.2.1
+Requires-Dist: friendly_traceback
+
+A plug-in which offers primitive support (for now ) for Friendly_traceback python package in Thonny IDE .
+It needs to be installed to the interpetter (not only as thonny plugin ) because of the parser that needs to called (thonnycontrib.thonny_friendly.parser.parseable)
```

### Comparing `thonny-friendly-0.0.3/setup.py` & `thonny_friendly-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `thonny-friendly-0.0.3/thonny_friendly.egg-info/PKG-INFO` & `thonny_friendly-0.0.4/thonny_friendly.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-Metadata-Version: 2.1
-Name: thonny-friendly
-Version: 0.0.3
-Summary: A plug-in which offers primitive support (for now ) for Friendly_traceback python package in Thonny IDE .
-Home-page: https://github.com/selmen2004/thonny-friendly
-Author: Selmen Arous
-Author-email: Selmen Arous <selmen.arous@gmail.com>
-License: GPL version 3
-Keywords: Friendly,Friendly_traceback,beginner,Tunisia,School,Teaching,Education
-Platform: Windows
-Platform: macOS
-Platform: Linux
-Classifier: Environment :: MacOS X
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: Environment :: X11 Applications
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: Freeware
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Education
-Classifier: Topic :: Software Development
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-Requires-Dist: thonny>=3.2.1
-
-A plug-in which offers primitive support (for now ) for Friendly_traceback python package in Thonny IDE .
+Metadata-Version: 2.1
+Name: thonny-friendly
+Version: 0.0.4
+Summary: A plug-in which offers primitive support (for now ) for Friendly_traceback python package in Thonny IDE .
+Home-page: https://github.com/selmen2004/thonny-friendly
+Author: Selmen Arous
+Author-email: Selmen Arous <selmen.arous@gmail.com>
+License: GPL version 3
+Keywords: Friendly,Friendly_traceback,beginner,Tunisia,School,Teaching,Education
+Platform: Windows
+Platform: macOS
+Platform: Linux
+Classifier: Environment :: MacOS X
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Environment :: X11 Applications
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: Freeware
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Education
+Classifier: Topic :: Software Development
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+Requires-Dist: thonny>=3.2.1
+Requires-Dist: friendly_traceback
+
+A plug-in which offers primitive support (for now ) for Friendly_traceback python package in Thonny IDE .
+It needs to be installed to the interpetter (not only as thonny plugin ) because of the parser that needs to called (thonnycontrib.thonny_friendly.parser.parseable)
```

### Comparing `thonny-friendly-0.0.3/thonnycontrib/thonny_friendly/__init__.py` & `thonny_friendly-0.0.4/thonnycontrib/thonny_friendly/__init__.py`

 * *Files identical despite different names*

