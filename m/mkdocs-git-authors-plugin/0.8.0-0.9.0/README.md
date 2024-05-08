# Comparing `tmp/mkdocs-git-authors-plugin-0.8.0.tar.gz` & `tmp/mkdocs_git_authors_plugin-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-git-authors-plugin-0.8.0.tar", last modified: Tue Mar 12 21:53:48 2024, max compression
+gzip compressed data, was "mkdocs_git_authors_plugin-0.9.0.tar", last modified: Wed May  8 14:21:17 2024, max compression
```

## Comparing `mkdocs-git-authors-plugin-0.8.0.tar` & `mkdocs_git_authors_plugin-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:53:48.109220 mkdocs-git-authors-plugin-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-03-12 21:53:48.109220 mkdocs-git-authors-plugin-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:53:48.105220 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/exclude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:53:48.109220 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/git/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/git/author.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/git/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/git/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/git/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:53:48.109220 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-03-12 21:53:48.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-12 21:53:48.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 21:53:48.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-12 21:53:48.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-12 21:53:48.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-12 21:53:48.000000 mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 21:53:48.109220 mkdocs-git-authors-plugin-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:53:48.109220 mkdocs-git-authors-plugin-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-03-12 21:53:21.000000 mkdocs-git-authors-plugin-0.8.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:21:17.573513 mkdocs_git_authors_plugin-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-08 14:21:17.573513 mkdocs_git_authors_plugin-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:21:17.569513 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/exclude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:21:17.569513 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/git/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/git/author.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/git/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/git/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/git/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:21:17.569513 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-08 14:21:17.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-08 14:21:17.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:21:17.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 14:21:17.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 14:21:17.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 14:21:17.000000 mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:21:17.573513 mkdocs_git_authors_plugin-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:21:17.569513 mkdocs_git_authors_plugin-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14710 2024-05-08 14:20:51.000000 mkdocs_git_authors_plugin-0.9.0/tests/test_util.py
```

### Comparing `mkdocs-git-authors-plugin-0.8.0/LICENSE` & `mkdocs_git_authors_plugin-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.8.0/PKG-INFO` & `mkdocs_git_authors_plugin-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-git-authors-plugin
-Version: 0.8.0
+Version: 0.9.0
 Summary: Mkdocs plugin to display git authors of a page
 Home-page: https://github.com/timvink/mkdocs-git-authors-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs git contributors committers authors plugin
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocs-git-authors-plugin-0.8.0/README.md` & `mkdocs_git_authors_plugin-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/ci.py` & `mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/ci.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/exclude.py` & `mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/exclude.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/git/author.py` & `mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/git/author.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/git/command.py` & `mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/git/command.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/git/commit.py` & `mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/git/commit.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/git/page.py` & `mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/git/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,23 +142,30 @@
             ---
         Returns:
             --- (this method works through side effects)
         """
 
         re_sha = re.compile(r"^\w{40}")
 
-        cmd = GitCommand("blame", ["--porcelain", str(self._path)])
+        args = []
+        if self.repo().config("ignore_commits"):
+            args.append("--ignore-revs-file")
+            args.append(self.repo().config("ignore_commits"))
+        args.append("--porcelain")
+        args.append(str(self._path))
+        cmd = GitCommand("blame", args)
         cmd.run()
 
         lines = cmd.stdout()
 
         # in case of empty, non-committed files, raise error
         if len(lines) == 0:
             raise GitCommandError
 
+        ignore_authors = self.repo().config("ignore_authors")
         commit_data = {}
         for line in lines:
             key = line.split(" ")[0]
             m = re_sha.match(key)
             if m:
                 commit_data = {"sha": key}
             elif key in [
@@ -179,15 +186,15 @@
                     # so they can be used for creating a Commit object.
                     author_name=commit_data.get("author"),
                     author_email=commit_data.get("author-mail"),
                     author_time=commit_data.get("author-time"),
                     author_tz=commit_data.get("author-tz"),
                     summary=commit_data.get("summary"),
                 )
-                if len(line) > 1 or self.repo().config("count_empty_lines"):
+                if commit.author().email() not in ignore_authors and (len(line) > 1 or self.repo().config("count_empty_lines")):
                     author = commit.author()
                     if author not in self._authors:
                         self._authors.append(author)
                     author.add_lines(self, commit)
                     self.add_total_lines()
                     self.repo().add_total_lines()
```

### Comparing `mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/git/repo.py` & `mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/git/repo.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/plugin.py` & `mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         ("show_contribution", config_options.Type(bool, default=False)),
         ("show_line_count", config_options.Type(bool, default=False)),
         ("show_email_address", config_options.Type(bool, default=True)),
         ("href", config_options.Type(str, default='mailto:{email}')),
         ("count_empty_lines", config_options.Type(bool, default=True)),
         ("fallback_to_empty", config_options.Type(bool, default=False)),
         ("exclude", config_options.Type(list, default=[])),
+        ("ignore_commits", config_options.Type(str, default=None)),
+        ("ignore_authors", config_options.Type(list, default=[])),
         ("enabled", config_options.Type(bool, default=True)),
         ("enabled_on_serve", config_options.Type(bool, default=True)),
         ("sort_authors_by", config_options.Type(str, default="name")),
         ("authorship_threshold_percent", config_options.Type(int, default=0)),
         ("strict", config_options.Type(bool, default=True)),
         # ('sort_authors_by_name', config_options.Type(bool, default=True)),
         # ('sort_reverse', config_options.Type(bool, default=False))
```

### Comparing `mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin/util.py` & `mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin.egg-info/PKG-INFO` & `mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-git-authors-plugin
-Version: 0.8.0
+Version: 0.9.0
 Summary: Mkdocs plugin to display git authors of a page
 Home-page: https://github.com/timvink/mkdocs-git-authors-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs git contributors committers authors plugin
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocs-git-authors-plugin-0.8.0/mkdocs_git_authors_plugin.egg-info/SOURCES.txt` & `mkdocs_git_authors_plugin-0.9.0/mkdocs_git_authors_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.8.0/setup.py` & `mkdocs_git_authors_plugin-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mkdocs-git-authors-plugin",
-    version="0.8.0",
+    version="0.9.0",
     description="Mkdocs plugin to display git authors of a page",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs git contributors committers authors plugin",
     url="https://github.com/timvink/mkdocs-git-authors-plugin",
     author="Tim Vink",
     author_email="vinktim@gmail.com",
```

### Comparing `mkdocs-git-authors-plugin-0.8.0/tests/test_basic.py` & `mkdocs_git_authors_plugin-0.9.0/tests/test_basic.py`

 * *Files 5% similar despite different names*

```diff
@@ -142,14 +142,31 @@
     assert page_file.exists(), "%s does not exist" % page_file
 
     contents = page_file.read_text()
     assert not re.search("<span class='git-page-authors", contents)
 
 
 
+def test_ignore_authors_working(tmp_path):
+
+    result = build_docs_setup("tests/basic_setup/mkdocs_ignore_authors.yml", tmp_path)
+    assert result.exit_code == 0, (
+            "'mkdocs build' command failed. Error: %s" % result.stdout
+    )
+
+    page_file = tmp_path / "page_with_tag/index.html"
+    assert page_file.exists(), "%s does not exist" % page_file
+
+    contents = page_file.read_text()
+    assert re.search("<span class='git-page-authors", contents)
+    assert re.search("<a href='mailto:vinktim@gmail.com'>Tim Vink</a>", contents)
+    assert not re.search("Julien", contents)
+
+
+
 def test_exclude_working_with_genfiles(tmp_path):
     """
     A warning for uncommited files should not show up
     when those uncommited files are excluded.
     """
     
     testproject_path = tmp_path / "testproject_genfiles"
```

### Comparing `mkdocs-git-authors-plugin-0.8.0/tests/test_util.py` & `mkdocs_git_authors_plugin-0.9.0/tests/test_util.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "show_line_count": False,
     "show_email_address": True,
     "count_empty_lines": True,
     "sort_authors_by_name": True,
     "sort_reverse": False,
     "sort_authors_by": "name",
     "authorship_threshold_percent": 0,
+    "ignore_authors": [],
 }
 
 #### Helpers ####
 
 
 def setup_clean_mkdocs_folder(mkdocs_yml_path, output_path):
     """
@@ -271,14 +272,156 @@
             "contribution": "66.67%",
             "contribution_all_pages": "66.67%",
         },
     ]
     os.chdir(cwd)
 
 
+def test_retrieve_authors_ignoring_commits(tmp_path):
+    """
+    Builds a fake git project with some commits.
+
+    Args:
+        tmp_path (PosixPath): Directory of a tempdir
+    """
+    cwd = os.getcwd()
+    os.chdir(str(tmp_path))
+
+    # Create file
+    file_name = str(tmp_path / "new-file")
+    with open(file_name, "w") as the_file:
+        the_file.write("line 1\n")
+        the_file.write("line 2\n")
+
+    # Create git repo and commit file
+    r = gitpython.Repo.init(tmp_path)
+    r.index.add([file_name])
+    author = gitpython.Actor("Tim", "abc@abc.com")
+    r.index.commit("initial commit", author=author)
+
+    # Update the file
+    with open(file_name, "w") as the_file:
+        the_file.write("line 1.1\n")
+        the_file.write("line 2.1\n")
+    r.index.add([file_name])
+    author = gitpython.Actor("John", "john@abc.com")
+    commit = r.index.commit("second commit", author=author)
+
+    repo_instance = repo.Repo()
+    repo_instance.set_config(DEFAULT_CONFIG)
+    repo_instance.page(file_name)
+    authors = repo_instance.get_authors()
+    authors = util.page_authors(authors, file_name)
+    authors[0]["last_datetime"] = None
+
+    assert authors == [
+        {
+            "name": "John",
+            "email": "john@abc.com",
+            "last_datetime": None,
+            "lines": 2,
+            "lines_all_pages": 2,
+            "contribution": "100.0%",
+            "contribution_all_pages": "100.0%",
+        }
+    ]
+
+    # Get the authors while ignoring the last commit
+    ignored_commits_files = str(tmp_path / "ignored_commits.txt")
+    with open(ignored_commits_files, "w") as the_file:
+        the_file.write(commit.hexsha + "\n")
+    repo_instance = repo.Repo()
+    config = DEFAULT_CONFIG.copy()
+    config['ignore_commits'] = ignored_commits_files
+    repo_instance.set_config(config)
+    repo_instance.page(file_name)
+    authors = repo_instance.get_authors()
+    authors = util.page_authors(authors, file_name)
+    authors[0]["last_datetime"] = None
+
+    assert authors == [
+        {
+            "name": "Tim",
+            "email": "abc@abc.com",
+            "last_datetime": None,
+            "lines": 2,
+            "lines_all_pages": 2,
+            "contribution": "100.0%",
+            "contribution_all_pages": "100.0%",
+        },
+    ]
+
+    os.chdir(cwd)
+
+
+def test_retrieve_authors_ignoring_emails(tmp_path):
+    """
+    Builds a fake git project with some commits.
+
+    Args:
+        tmp_path (PosixPath): Directory of a tempdir
+    """
+    cwd = os.getcwd()
+    os.chdir(str(tmp_path))
+
+    # Create file
+    file_name = str(tmp_path / "new-file")
+    with open(file_name, "w") as the_file:
+        the_file.write("line 1\n")
+        the_file.write("line 2\n")
+
+    # Create git repo and commit file
+    r = gitpython.Repo.init(tmp_path)
+    r.index.add([file_name])
+    author = gitpython.Actor("Tim", "abc@abc.com")
+    r.index.commit("initial commit", author=author)
+
+    # Add more content
+    with open(file_name, "a+") as the_file:
+        the_file.write("line 3\n")
+        the_file.write("line 4\n")
+    r.index.add([file_name])
+    author = gitpython.Actor("John", "john@abc.com")
+    r.index.commit("second commit", author=author)
+
+    # Get the authors while ignoring john@abc.com user
+    repo_instance = repo.Repo()
+    config = DEFAULT_CONFIG.copy()
+    config['ignore_authors'] = ['john@abc.com']
+    repo_instance.set_config(config)
+    repo_instance.page(file_name)
+    authors = repo_instance.get_authors()
+    authors = util.page_authors(authors, file_name)
+    authors[0]["last_datetime"] = None
+    authors[1]["last_datetime"] = None
+
+    assert authors == [
+        {
+            "contribution": "0.0%",
+            "contribution_all_pages": "0.0%",
+            "email": "john@abc.com",
+            "last_datetime": None,
+            "lines": 0,
+            "lines_all_pages": 0,
+            "name": "John"
+        },
+        {
+            "name": "Tim",
+            "email": "abc@abc.com",
+            "last_datetime": None,
+            "lines": 2,
+            "lines_all_pages": 2,
+            "contribution": "100.0%",
+            "contribution_all_pages": "100.0%",
+        },
+    ]
+
+    os.chdir(cwd)
+
+
 def test_mkdocs_in_git_subdir(tmp_path):
     """
     Sometimes `mkdocs.yml` is not in the root of the repo.
     We need to make sure things still work in this edge case.
 
     tmp_path/testproject
     website/
```

