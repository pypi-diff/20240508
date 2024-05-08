# Comparing `tmp/discorudo-1.2.tar.gz` & `tmp/discorudo-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discorudo-1.2.tar", last modified: Sat May  4 07:46:38 2024, max compression
+gzip compressed data, was "discorudo-1.3.tar", last modified: Wed May  8 12:06:35 2024, max compression
```

## Comparing `discorudo-1.2.tar` & `discorudo-1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 07:46:38.793629 discorudo-1.2/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1096 2024-05-04 07:46:38.793629 discorudo-1.2/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2024-05-01 15:04:25.000000 discorudo-1.2/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 07:46:38.793629 discorudo-1.2/discorudo/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       44 2024-05-04 07:44:49.000000 discorudo-1.2/discorudo/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       87 2024-05-04 07:44:36.000000 discorudo-1.2/discorudo/main.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-04 07:46:38.793629 discorudo-1.2/discorudo.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1096 2024-05-04 07:46:38.000000 discorudo-1.2/discorudo.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      222 2024-05-04 07:46:38.000000 discorudo-1.2/discorudo.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-05-04 07:46:38.000000 discorudo-1.2/discorudo.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       43 2024-05-04 07:46:38.000000 discorudo-1.2/discorudo.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       10 2024-05-04 07:46:38.000000 discorudo-1.2/discorudo.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-05-04 07:46:38.793629 discorudo-1.2/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2375 2024-05-04 07:46:06.000000 discorudo-1.2/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-08 12:06:35.898876 discorudo-1.3/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1096 2024-05-08 12:06:35.898876 discorudo-1.3/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2024-05-01 15:04:25.000000 discorudo-1.3/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-08 12:06:35.894876 discorudo-1.3/discorudo/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       75 2024-05-08 12:05:44.000000 discorudo-1.3/discorudo/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      983 2024-05-08 12:05:23.000000 discorudo-1.3/discorudo/main.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-08 12:06:35.898876 discorudo-1.3/discorudo.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1096 2024-05-08 12:06:35.000000 discorudo-1.3/discorudo.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      222 2024-05-08 12:06:35.000000 discorudo-1.3/discorudo.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-05-08 12:06:35.000000 discorudo-1.3/discorudo.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       43 2024-05-08 12:06:35.000000 discorudo-1.3/discorudo.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       10 2024-05-08 12:06:35.000000 discorudo-1.3/discorudo.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-05-08 12:06:35.898876 discorudo-1.3/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2375 2024-05-08 12:05:54.000000 discorudo-1.3/setup.py
```

### Comparing `discorudo-1.2/PKG-INFO` & `discorudo-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discorudo
-Version: 1.2
+Version: 1.3
 Summary: Just script on to discord
 Home-page: https://github.com/rizkychi/discorudo
 Author: rizkychi
 Author-email: rizkynhae@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/rizkychi/discorudo/
 Project-URL: Funding, https://www.paypal.me/rizkychi
```

### Comparing `discorudo-1.2/discorudo.egg-info/PKG-INFO` & `discorudo-1.3/discorudo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discorudo
-Version: 1.2
+Version: 1.3
 Summary: Just script on to discord
 Home-page: https://github.com/rizkychi/discorudo
 Author: rizkychi
 Author-email: rizkynhae@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/rizkychi/discorudo/
 Project-URL: Funding, https://www.paypal.me/rizkychi
```

### Comparing `discorudo-1.2/setup.py` & `discorudo-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = 'discorudo',         # How you named your package folder (MyLib)
     packages = ['discorudo'],   # Chose the same as "name"
-    version = '1.2',      # Start with a small number and increase it with every change you make
+    version = '1.3',      # Start with a small number and increase it with every change you make
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Just script on to discord',   # Give a short description about your library
     long_description=long_description,            # Give a long description about your library
     long_description_content_type='text/markdown',
     author = 'rizkychi',                   # Type in your name
     author_email = 'rizkynhae@gmail.com',      # Type in your E-Mail
     url = 'https://github.com/rizkychi/discorudo',   # Provide either the link to your github or to your website
```

