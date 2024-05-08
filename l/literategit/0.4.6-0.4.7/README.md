# Comparing `tmp/literategit-0.4.6.tar.gz` & `tmp/literategit-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literategit-0.4.6.tar", max compression
+gzip compressed data, was "literategit-0.4.7.tar", max compression
```

## Comparing `literategit-0.4.6.tar` & `literategit-0.4.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1930 2024-04-08 15:49:49.991908 literategit-0.4.6/COPYING
--rw-r--r--   0        0        0    35147 2024-04-06 16:10:11.658789 literategit-0.4.6/LICENCE.txt
--rw-r--r--   0        0        0      512 2024-04-08 15:49:49.991908 literategit-0.4.6/README-short.md
--rw-r--r--   0        0        0     9443 2024-04-08 15:49:49.991908 literategit-0.4.6/literategit/__init__.py
--rw-r--r--   0        0        0       47 2024-04-08 15:49:49.991908 literategit-0.4.6/literategit/_version.py
--rw-r--r--   0        0        0      141 2024-04-08 15:49:49.991908 literategit-0.4.6/literategit/cli/__init__.py
--rw-r--r--   0        0        0     2182 2024-04-08 15:49:49.991908 literategit-0.4.6/literategit/cli/dump_all_trees.py
--rw-r--r--   0        0        0     2770 2024-04-08 15:49:49.991908 literategit-0.4.6/literategit/cli/render.py
--rw-r--r--   0        0        0      986 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/cli/repo_for_path.py
--rw-r--r--   0        0        0      268 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/content.html.tmpl
--rw-r--r--   0        0        0      787 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/diff.html.tmpl
--rw-r--r--   0        0        0     3405 2024-04-08 15:49:49.991908 literategit-0.4.6/literategit/dump_all_trees.py
--rw-r--r--   0        0        0      475 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/example_create_url.py
--rw-r--r--   0        0        0     6333 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/literate-git.css
--rw-r--r--   0        0        0     8346 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/literate-git.js
--rw-r--r--   0        0        0      988 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/node.html.tmpl
--rw-r--r--   0        0        0     1513 2024-04-06 16:10:11.662789 literategit-0.4.6/literategit/page.html.tmpl
--rw-r--r--   0        0        0     1046 2024-04-08 15:49:49.991908 literategit-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     1634 1970-01-01 00:00:00.000000 literategit-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1930 2024-04-08 15:49:49.991908 literategit-0.4.7/COPYING
+-rw-r--r--   0        0        0    35147 2024-04-06 16:10:11.658789 literategit-0.4.7/LICENCE.txt
+-rw-r--r--   0        0        0      512 2024-04-08 15:49:49.991908 literategit-0.4.7/README-short.md
+-rw-r--r--   0        0        0     9443 2024-04-08 15:49:49.991908 literategit-0.4.7/literategit/__init__.py
+-rw-r--r--   0        0        0       47 2024-05-08 09:16:37.980771 literategit-0.4.7/literategit/_version.py
+-rw-r--r--   0        0        0      141 2024-04-08 15:49:49.991908 literategit-0.4.7/literategit/cli/__init__.py
+-rw-r--r--   0        0        0     2182 2024-04-08 15:49:49.991908 literategit-0.4.7/literategit/cli/dump_all_trees.py
+-rw-r--r--   0        0        0     2770 2024-04-08 15:49:49.991908 literategit-0.4.7/literategit/cli/render.py
+-rw-r--r--   0        0        0      986 2024-04-06 16:10:11.662789 literategit-0.4.7/literategit/cli/repo_for_path.py
+-rw-r--r--   0        0        0      268 2024-04-06 16:10:11.662789 literategit-0.4.7/literategit/content.html.tmpl
+-rw-r--r--   0        0        0      787 2024-04-06 16:10:11.662789 literategit-0.4.7/literategit/diff.html.tmpl
+-rw-r--r--   0        0        0     3405 2024-04-08 15:49:49.991908 literategit-0.4.7/literategit/dump_all_trees.py
+-rw-r--r--   0        0        0      475 2024-04-06 16:10:11.662789 literategit-0.4.7/literategit/example_create_url.py
+-rw-r--r--   0        0        0     6333 2024-04-06 16:10:11.662789 literategit-0.4.7/literategit/literate-git.css
+-rw-r--r--   0        0        0     8346 2024-04-06 16:10:11.662789 literategit-0.4.7/literategit/literate-git.js
+-rw-r--r--   0        0        0      988 2024-04-06 16:10:11.662789 literategit-0.4.7/literategit/node.html.tmpl
+-rw-r--r--   0        0        0     1513 2024-04-06 16:10:11.662789 literategit-0.4.7/literategit/page.html.tmpl
+-rw-r--r--   0        0        0     1046 2024-05-08 09:16:37.980771 literategit-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     1634 1970-01-01 00:00:00.000000 literategit-0.4.7/PKG-INFO
```

### Comparing `literategit-0.4.6/COPYING` & `literategit-0.4.7/COPYING`

 * *Files identical despite different names*

### Comparing `literategit-0.4.6/LICENCE.txt` & `literategit-0.4.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `literategit-0.4.6/README-short.md` & `literategit-0.4.7/README-short.md`

 * *Files identical despite different names*

### Comparing `literategit-0.4.6/literategit/__init__.py` & `literategit-0.4.7/literategit/__init__.py`

 * *Files identical despite different names*

### Comparing `literategit-0.4.6/literategit/cli/dump_all_trees.py` & `literategit-0.4.7/literategit/cli/dump_all_trees.py`

 * *Files identical despite different names*

### Comparing `literategit-0.4.6/literategit/cli/render.py` & `literategit-0.4.7/literategit/cli/render.py`

 * *Files identical despite different names*

### Comparing `literategit-0.4.6/literategit/cli/repo_for_path.py` & `literategit-0.4.7/literategit/cli/repo_for_path.py`

 * *Files identical despite different names*

### Comparing `literategit-0.4.6/literategit/diff.html.tmpl` & `literategit-0.4.7/literategit/diff.html.tmpl`

 * *Files identical despite different names*

### Comparing `literategit-0.4.6/literategit/dump_all_trees.py` & `literategit-0.4.7/literategit/dump_all_trees.py`

 * *Files identical despite different names*

### Comparing `literategit-0.4.6/literategit/literate-git.css` & `literategit-0.4.7/literategit/literate-git.css`

 * *Files identical despite different names*

### Comparing `literategit-0.4.6/literategit/literate-git.js` & `literategit-0.4.7/literategit/literate-git.js`

 * *Files identical despite different names*

### Comparing `literategit-0.4.6/literategit/node.html.tmpl` & `literategit-0.4.7/literategit/node.html.tmpl`

 * *Files identical despite different names*

### Comparing `literategit-0.4.6/literategit/page.html.tmpl` & `literategit-0.4.7/literategit/page.html.tmpl`

 * *Files identical despite different names*

### Comparing `literategit-0.4.6/pyproject.toml` & `literategit-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "literategit"
-version = "0.4.6"
+version = "0.4.7"
 description = "Render a structured git history as an interactive web page"
 homepage = "https://github.com/bennorth/literate-git"
 authors = ["Ben North <ben@redfrontdoor.org>"]
 license = "GPLv3"
 readme = "README-short.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `literategit-0.4.6/PKG-INFO` & `literategit-0.4.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: literategit
-Version: 0.4.6
+Version: 0.4.7
 Summary: Render a structured git history as an interactive web page
 Home-page: https://github.com/bennorth/literate-git
 License: GPLv3
 Author: Ben North
 Author-email: ben@redfrontdoor.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

