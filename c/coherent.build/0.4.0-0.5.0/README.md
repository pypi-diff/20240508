# Comparing `tmp/coherent_build-0.4.0.tar.gz` & `tmp/coherent_build-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherent_build-0.4.0.tar", last modified: Tue May  7 20:56:49 2024, max compression
+gzip compressed data, was "coherent_build-0.5.0.tar", last modified: Wed May  8 12:58:36 2024, max compression
```

## Comparing `coherent_build-0.4.0.tar` & `coherent_build-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-07 20:48:20.139500 coherent_build-0.4.0/
--rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.4.0/README.md
--rw-r--r--   0 jaraco     (501) staff       (20)     5556 2024-05-07 20:53:13.349675 coherent_build-0.4.0/__init__.py
--rw-r--r--   0 jaraco     (501) staff       (20)     8550 2024-05-07 20:37:24.092828 coherent_build-0.4.0/__init__.py.orig
--rw-r--r--   0 jaraco     (501) staff       (20)      495 2024-05-02 02:13:39.559121 coherent_build-0.4.0/__main__.py
--rw-r--r--   0 jaraco     (501) staff       (20)     3035 2024-05-07 20:55:49.864191 coherent_build-0.4.0/discovery.py
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      509 2024-05-07 20:56:49.143335 coherent_build-0.4.0/PKG-INFO
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-08 12:58:34.967964 coherent_build-0.5.0/
+-rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.5.0/README.md
+-rw-r--r--   0 jaraco     (501) staff       (20)     5574 2024-05-08 12:57:14.008323 coherent_build-0.5.0/__init__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     8550 2024-05-07 20:37:24.092828 coherent_build-0.5.0/__init__.py.orig
+-rw-r--r--   0 jaraco     (501) staff       (20)      492 2024-05-08 12:56:54.105638 coherent_build-0.5.0/__main__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     3232 2024-05-08 12:36:43.178900 coherent_build-0.5.0/discovery.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-08 12:58:34.968043 coherent_build-0.5.0/pyproject.toml
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.5.0/system.toml
+-rw-r--r--   0        0        0      509 2024-05-08 12:58:36.669853 coherent_build-0.5.0/PKG-INFO
```

### Comparing `coherent_build-0.4.0/__init__.py` & `coherent_build-0.5.0/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     namespace(name='foo/bar/dist')
     """
 
     ignored = ['dist', r'(.*[/])?__pycache__$', r'(.*[/])?[.]']
 
 
 class Wheel(Filter):
-    ignored = ['docs', 'tests', 'README.*', 'PKG-INFO', '(meta)']
+    ignored = ['docs', 'tests', 'README.*', 'PKG-INFO', '(meta)', 'pyproject.toml']
 
 
 class ZipInfo(types.SimpleNamespace):
     def __init__(self, path):
         zip_name = path.replace(os.pathsep, posixpath.sep)
         super().__init__(path=path, name=zip_name)
```

### Comparing `coherent_build-0.4.0/__init__.py.orig` & `coherent_build-0.5.0/__init__.py.orig`

 * *Files identical despite different names*

### Comparing `coherent_build-0.4.0/discovery.py` & `coherent_build-0.5.0/discovery.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import json
 import pathlib
 import subprocess
 import types
 import mimetypes
 
 import requests
@@ -73,20 +74,28 @@
         return f'"{self.name}" <{self.email}>'
 
 
 @suppress(Exception)
 def author_from_vcs():
     # run git-fame twice to get both name and email
     cmd = ['git-fame', '--format', 'json']
-    names_data = json.loads(subprocess.check_output(cmd, text=True, encoding='utf-8'))
+    names_data = json.loads(
+        subprocess.check_output(
+            cmd,
+            text=True,
+            encoding='utf-8',
+            stderr=subprocess.DEVNULL,
+        )
+    )
     emails_data = json.loads(
         subprocess.check_output(
             cmd + ['--show-email'],
             text=True,
             encoding='utf-8',
+            stderr=subprocess.DEVNULL,
         )
     )
     names_data['columns'][0] = 'name'
     emails_data['columns'][0] = 'email'
     emails_contribs = _to_mapping(emails_data)
     names_contribs = _to_mapping(names_data)
 
@@ -109,14 +118,14 @@
     >>> guess_content_type('foo')
     'text/plain'
     """
     type, _ = mimetypes.guess_type(str(path))
     return type
 
 
-@suppress(ValueError, AssertionError)
 def description_from_readme():
-    (readme,) = pathlib.Path().glob('README*')
-    ct = guess_content_type(readme)
-    assert ct
-    yield 'Description-Content-Type', ct
-    yield 'Description', readme.read_text(encoding='utf-8')
+    with contextlib.suppress(ValueError, AssertionError):
+        (readme,) = pathlib.Path().glob('README*')
+        ct = guess_content_type(readme)
+        assert ct
+        yield 'Description-Content-Type', ct
+        yield 'Description', readme.read_text(encoding='utf-8')
```

