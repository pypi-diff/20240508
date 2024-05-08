# Comparing `tmp/broadcastify_cli-0.1.0.tar.gz` & `tmp/broadcastify_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "broadcastify_cli-0.1.0.tar", last modified: Wed May  8 20:30:03 2024, max compression
+gzip compressed data, was "broadcastify_cli-0.1.1.tar", last modified: Wed May  8 20:40:11 2024, max compression
```

## Comparing `broadcastify_cli-0.1.0.tar` & `broadcastify_cli-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 johndoe    (501) staff       (20)        0 2024-05-08 20:30:03.107392 broadcastify_cli-0.1.0/
--rw-r--r--   0 johndoe    (501) staff       (20)    34570 2024-04-18 10:31:06.000000 broadcastify_cli-0.1.0/LICENSE
--rw-r--r--   0 johndoe    (501) staff       (20)    38929 2024-05-08 20:30:03.107159 broadcastify_cli-0.1.0/PKG-INFO
--rw-r--r--   0 johndoe    (501) staff       (20)     1564 2024-04-18 12:17:43.000000 broadcastify_cli-0.1.0/README.md
-drwxr-xr-x   0 johndoe    (501) staff       (20)        0 2024-05-08 20:30:03.105219 broadcastify_cli-0.1.0/broadcastify_cli/
--rw-r--r--   0 johndoe    (501) staff       (20)        0 2024-04-18 10:32:12.000000 broadcastify_cli-0.1.0/broadcastify_cli/__init__.py
--rw-r--r--   0 johndoe    (501) staff       (20)    11518 2024-04-18 19:59:15.000000 broadcastify_cli-0.1.0/broadcastify_cli/broadcastify_cli.py
-drwxr-xr-x   0 johndoe    (501) staff       (20)        0 2024-05-08 20:30:03.106800 broadcastify_cli-0.1.0/broadcastify_cli.egg-info/
--rw-r--r--   0 johndoe    (501) staff       (20)    38929 2024-05-08 20:30:03.000000 broadcastify_cli-0.1.0/broadcastify_cli.egg-info/PKG-INFO
--rw-r--r--   0 johndoe    (501) staff       (20)      372 2024-05-08 20:30:03.000000 broadcastify_cli-0.1.0/broadcastify_cli.egg-info/SOURCES.txt
--rw-r--r--   0 johndoe    (501) staff       (20)        1 2024-05-08 20:30:03.000000 broadcastify_cli-0.1.0/broadcastify_cli.egg-info/dependency_links.txt
--rw-r--r--   0 johndoe    (501) staff       (20)       75 2024-05-08 20:30:03.000000 broadcastify_cli-0.1.0/broadcastify_cli.egg-info/entry_points.txt
--rw-r--r--   0 johndoe    (501) staff       (20)      239 2024-05-08 20:30:03.000000 broadcastify_cli-0.1.0/broadcastify_cli.egg-info/requires.txt
--rw-r--r--   0 johndoe    (501) staff       (20)       17 2024-05-08 20:30:03.000000 broadcastify_cli-0.1.0/broadcastify_cli.egg-info/top_level.txt
--rw-r--r--   0 johndoe    (501) staff       (20)     1055 2024-04-18 18:19:36.000000 broadcastify_cli-0.1.0/pyproject.toml
--rw-r--r--   0 johndoe    (501) staff       (20)       38 2024-05-08 20:30:03.107438 broadcastify_cli-0.1.0/setup.cfg
-drwxr-xr-x   0 johndoe    (501) staff       (20)        0 2024-05-08 20:30:03.106137 broadcastify_cli-0.1.0/tests/
--rw-r--r--   0 johndoe    (501) staff       (20)      572 2024-04-18 18:00:04.000000 broadcastify_cli-0.1.0/tests/test_transcription_api.py
+drwxr-xr-x   0 johndoe    (501) staff       (20)        0 2024-05-08 20:40:11.455980 broadcastify_cli-0.1.1/
+-rw-r--r--   0 johndoe    (501) staff       (20)    34570 2024-04-18 10:31:06.000000 broadcastify_cli-0.1.1/LICENSE
+-rw-r--r--   0 johndoe    (501) staff       (20)    39003 2024-05-08 20:40:11.455787 broadcastify_cli-0.1.1/PKG-INFO
+-rw-r--r--   0 johndoe    (501) staff       (20)     1564 2024-04-18 12:17:43.000000 broadcastify_cli-0.1.1/README.md
+drwxr-xr-x   0 johndoe    (501) staff       (20)        0 2024-05-08 20:40:11.454085 broadcastify_cli-0.1.1/broadcastify_cli/
+-rw-r--r--   0 johndoe    (501) staff       (20)        0 2024-04-18 10:32:12.000000 broadcastify_cli-0.1.1/broadcastify_cli/__init__.py
+-rw-r--r--   0 johndoe    (501) staff       (20)    11518 2024-05-08 20:38:28.000000 broadcastify_cli-0.1.1/broadcastify_cli/broadcastify_cli.py
+drwxr-xr-x   0 johndoe    (501) staff       (20)        0 2024-05-08 20:40:11.455510 broadcastify_cli-0.1.1/broadcastify_cli.egg-info/
+-rw-r--r--   0 johndoe    (501) staff       (20)    39003 2024-05-08 20:40:11.000000 broadcastify_cli-0.1.1/broadcastify_cli.egg-info/PKG-INFO
+-rw-r--r--   0 johndoe    (501) staff       (20)      372 2024-05-08 20:40:11.000000 broadcastify_cli-0.1.1/broadcastify_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 johndoe    (501) staff       (20)        1 2024-05-08 20:40:11.000000 broadcastify_cli-0.1.1/broadcastify_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 johndoe    (501) staff       (20)       75 2024-05-08 20:40:11.000000 broadcastify_cli-0.1.1/broadcastify_cli.egg-info/entry_points.txt
+-rw-r--r--   0 johndoe    (501) staff       (20)      239 2024-05-08 20:40:11.000000 broadcastify_cli-0.1.1/broadcastify_cli.egg-info/requires.txt
+-rw-r--r--   0 johndoe    (501) staff       (20)       17 2024-05-08 20:40:11.000000 broadcastify_cli-0.1.1/broadcastify_cli.egg-info/top_level.txt
+-rw-r--r--   0 johndoe    (501) staff       (20)     1135 2024-05-08 20:38:17.000000 broadcastify_cli-0.1.1/pyproject.toml
+-rw-r--r--   0 johndoe    (501) staff       (20)       38 2024-05-08 20:40:11.456013 broadcastify_cli-0.1.1/setup.cfg
+drwxr-xr-x   0 johndoe    (501) staff       (20)        0 2024-05-08 20:40:11.455249 broadcastify_cli-0.1.1/tests/
+-rw-r--r--   0 johndoe    (501) staff       (20)      572 2024-04-18 18:00:04.000000 broadcastify_cli-0.1.1/tests/test_transcription_api.py
```

### Comparing `broadcastify_cli-0.1.0/LICENSE` & `broadcastify_cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `broadcastify_cli-0.1.0/PKG-INFO` & `broadcastify_cli-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broadcastify-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary:  CLI for interacting with the unoffical broadcastify API
 Author-email: NotJoeMartinez <notjoemartinez@protonmail.com>
 License: GNU GENERAL PUBLIC LICENSE 
         Version 3, 29 June 2007
         Copyright © 2007 Free Software Foundation, Inc. <http://fsf.org/>
         
         Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
@@ -231,14 +231,15 @@
         
         The hypothetical commands `show w' and `show c' should show the appropriate parts of the General Public License. Of course, your program's commands might be different; for a GUI interface, you would use an “about box”.
         
         You should also get your employer (if you work as a programmer) or school, if any, to sign a “copyright disclaimer” for the program, if necessary. For more information on this, and how to apply and follow the GNU GPL, see <http://www.gnu.org/licenses/>.
         
         The GNU General Public License does not permit incorporating your program into proprietary programs. If your program is a subroutine library, you may consider it more useful to permit linking proprietary applications with the library. If this is what you want to do, use the GNU Lesser General Public License instead of this License. But first, please read <http://www.gnu.org/philosophy/why-not-lgpl.html>.
         
+Project-URL: Homepage, https://github.com/NotJoeMartinez/broadcastify-cli
 Keywords: radio,cli,broadcastify
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `broadcastify_cli-0.1.0/README.md` & `broadcastify_cli-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `broadcastify_cli-0.1.0/broadcastify_cli/broadcastify_cli.py` & `broadcastify_cli-0.1.1/broadcastify_cli/broadcastify_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from dotenv import load_dotenv
 from pprint import pprint
 
 load_dotenv(".env")
 warnings.filterwarnings("ignore", module="whisper")
 
-BRODCASTIFY_CLI_VERSION = "0.1.0"
+BRODCASTIFY_CLI_VERSION = "0.1.1"
 
 console = Console()
 
 @click.group(context_settings={"help_option_names": ["-h", "--help"]})
 @click.version_option(BRODCASTIFY_CLI_VERSION, message='brodcastify-cli version: %(version)s')
 def cli():
     pass
```

### Comparing `broadcastify_cli-0.1.0/broadcastify_cli.egg-info/PKG-INFO` & `broadcastify_cli-0.1.1/broadcastify_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: broadcastify-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary:  CLI for interacting with the unoffical broadcastify API
 Author-email: NotJoeMartinez <notjoemartinez@protonmail.com>
 License: GNU GENERAL PUBLIC LICENSE 
         Version 3, 29 June 2007
         Copyright © 2007 Free Software Foundation, Inc. <http://fsf.org/>
         
         Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
@@ -231,14 +231,15 @@
         
         The hypothetical commands `show w' and `show c' should show the appropriate parts of the General Public License. Of course, your program's commands might be different; for a GUI interface, you would use an “about box”.
         
         You should also get your employer (if you work as a programmer) or school, if any, to sign a “copyright disclaimer” for the program, if necessary. For more information on this, and how to apply and follow the GNU GPL, see <http://www.gnu.org/licenses/>.
         
         The GNU General Public License does not permit incorporating your program into proprietary programs. If your program is a subroutine library, you may consider it more useful to permit linking proprietary applications with the library. If this is what you want to do, use the GNU Lesser General Public License instead of this License. But first, please read <http://www.gnu.org/philosophy/why-not-lgpl.html>.
         
+Project-URL: Homepage, https://github.com/NotJoeMartinez/broadcastify-cli
 Keywords: radio,cli,broadcastify
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `broadcastify_cli-0.1.0/pyproject.toml` & `broadcastify_cli-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=46.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "broadcastify-cli"
-version = "0.1.0" 
+version = "0.1.1" 
 description = " CLI for interacting with the unoffical broadcastify API"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
     { name = "NotJoeMartinez", email = "notjoemartinez@protonmail.com" }
 ]
@@ -35,8 +35,11 @@
     "urllib3==2.2.1",
     "pydub==0.25.1", 
     "openai-whisper==20231117",
     "openai==1.22.0"
 ]
 
 [project.scripts]
-broadcastify-cli = "broadcastify_cli.broadcastify_cli:cli"
+broadcastify-cli = "broadcastify_cli.broadcastify_cli:cli"
+
+[project.urls]
+Homepage = "https://github.com/NotJoeMartinez/broadcastify-cli"
```

### Comparing `broadcastify_cli-0.1.0/tests/test_transcription_api.py` & `broadcastify_cli-0.1.1/tests/test_transcription_api.py`

 * *Files identical despite different names*

