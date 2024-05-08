# Comparing `tmp/pyintelowl-5.0.0.tar.gz` & `tmp/pyintelowl-5.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyintelowl-5.0.0.tar", last modified: Wed May  8 14:27:04 2024, max compression
+gzip compressed data, was "pyintelowl-5.0.0rc0.tar", last modified: Wed Mar  6 11:17:16 2024, max compression
```

## Comparing `pyintelowl-5.0.0.tar` & `pyintelowl-5.0.0rc0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:27:04.729881 pyintelowl-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-08 14:27:04.729881 pyintelowl-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:27:04.721881 pyintelowl-5.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:27:04.721881 pyintelowl-5.0.0/pyintelowl/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyintelowl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:27:04.725881 pyintelowl-5.0.0/pyintelowl/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyintelowl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyintelowl/cli/_jobs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyintelowl/cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyintelowl/cli/analyse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyintelowl/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyintelowl/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    52097 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyintelowl/cli/domain_checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyintelowl/cli/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyintelowl/cli/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyintelowl/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1286 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyintelowl/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    37749 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyintelowl/pyintelowl.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyintelowl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:27:04.725881 pyintelowl-5.0.0/pyintelowl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-08 14:27:04.000000 pyintelowl-5.0.0/pyintelowl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-08 14:27:04.000000 pyintelowl-5.0.0/pyintelowl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:27:04.000000 pyintelowl-5.0.0/pyintelowl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 14:27:04.000000 pyintelowl-5.0.0/pyintelowl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-08 14:27:04.000000 pyintelowl-5.0.0/pyintelowl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 14:27:04.000000 pyintelowl-5.0.0/pyintelowl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:27:04.729881 pyintelowl-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:27:04.725881 pyintelowl-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/tests/mocked_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/tests/test_general.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-08 14:26:55.000000 pyintelowl-5.0.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:17:16.058015 pyintelowl-5.0.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-03-06 11:17:16.058015 pyintelowl-5.0.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:17:16.050015 pyintelowl-5.0.0rc0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:17:16.050015 pyintelowl-5.0.0rc0/pyintelowl/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyintelowl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:17:16.054015 pyintelowl-5.0.0rc0/pyintelowl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyintelowl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyintelowl/cli/_jobs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyintelowl/cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyintelowl/cli/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyintelowl/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyintelowl/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52097 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyintelowl/cli/domain_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyintelowl/cli/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyintelowl/cli/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyintelowl/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1286 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyintelowl/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37817 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyintelowl/pyintelowl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyintelowl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:17:16.054015 pyintelowl-5.0.0rc0/pyintelowl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-03-06 11:17:16.000000 pyintelowl-5.0.0rc0/pyintelowl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-06 11:17:16.000000 pyintelowl-5.0.0rc0/pyintelowl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 11:17:16.000000 pyintelowl-5.0.0rc0/pyintelowl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-06 11:17:16.000000 pyintelowl-5.0.0rc0/pyintelowl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-06 11:17:16.000000 pyintelowl-5.0.0rc0/pyintelowl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-06 11:17:16.000000 pyintelowl-5.0.0rc0/pyintelowl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 11:17:16.058015 pyintelowl-5.0.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 11:17:16.054015 pyintelowl-5.0.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/tests/mocked_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-03-06 11:17:06.000000 pyintelowl-5.0.0rc0/tests/utils.py
```

### Comparing `pyintelowl-5.0.0/LICENSE` & `pyintelowl-5.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/PKG-INFO` & `pyintelowl-5.0.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintelowl
-Version: 5.0.0
+Version: 5.0.0rc0
 Summary: Robust Python SDK and CLI for IntelOwl's API
 Home-page: https://github.com/intelowlproject/pyintelowl
 Author: Matteo Lodi
 Project-URL: Documentation, https://github.com/intelowlproject/pyintelowl
 Project-URL: Funding, https://liberapay.com/IntelOwlProject/
 Project-URL: Source, https://github.com/intelowlproject/pyintelowl
 Project-URL: Tracker, https://github.com/intelowlproject/pyintelowl/issues
```

### Comparing `pyintelowl-5.0.0/README.md` & `pyintelowl-5.0.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/docs/conf.py` & `pyintelowl-5.0.0rc0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 
-VERSION = "5.0.0"
+VERSION = "4.4.7"
 GITHUB_URL = "https://github.com/intelowlproject/pyintelowl"
 
 sys.path.append(os.path.abspath("../"))
 
 
 # -- Project information -----------------------------------------------------
```

### Comparing `pyintelowl-5.0.0/pyintelowl/cli/_jobs_utils.py` & `pyintelowl-5.0.0rc0/pyintelowl/cli/_jobs_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     for el in rows:
         cols = [
             el["name"],
             get_success_text((el["status"])),
         ]
         if verbose:
             for field in ["report", "errors", "runtime_configuration"]:
-                cols.append(get_json_syntax(el[field]) if el.get(field, "") else None)
+                cols.append(get_json_syntax(el[field]) if el[field] else None)
         table.add_row(*cols)
     return table
 
 
 def _render_job_attributes(data):
     style = "[bold #31DDCF]"
     tags = get_tags_str(data["tags"])
```

### Comparing `pyintelowl-5.0.0/pyintelowl/cli/_utils.py` & `pyintelowl-5.0.0rc0/pyintelowl/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/pyintelowl/cli/analyse.py` & `pyintelowl-5.0.0rc0/pyintelowl/cli/analyse.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,16 +76,27 @@
     ),
 ]
 
 __playbook_analyse_options = __analyse_options.copy()
 # doing it twice to remove --analyzers-list and --connectors-list
 __playbook_analyse_options.pop(0)
 __playbook_analyse_options.pop(0)
-__playbook_analyse_options.pop(3)
-__playbook_analyse_options.pop(2)
+
+__playbook_analyse_options.append(
+    click.option(
+        "-pl",
+        "--playbooks-list",
+        type=str,
+        default="",
+        help="""
+        Comma separated list of playbook names to invoke.
+        Defaults to all configured playbooks.
+        """,
+    ),
+)
 
 
 @click.group("analyse")
 def analyse():
     """
     Send new analysis request
     """
@@ -169,75 +180,81 @@
         )
     except IntelOwlClientException as e:
         ctx.obj.logger.fatal(str(e))
 
 
 @analyse.command(help="Send playbook analysis request for an observable")
 @click.argument("value")
-@click.argument("playbook")
 @add_options(__playbook_analyse_options)
 @click.pass_context
 def playbook_observable(
     ctx: ClickContext,
     value: str,
-    playbook: str,
+    playbooks_list: str,
     tags_list: str,
     tlp: str,
+    check,
+    check_minutes_ago: int,
     runtime_config,
     should_poll: bool,
 ):
+    playbooks_list = playbooks_list.split(",") if len(playbooks_list) else []
     tags_labels = tags_list.split(",") if len(tags_list) else []
     if runtime_config:
         runtime_config = get_json_data(runtime_config)
     else:
         runtime_config = {}
     try:
-        print("here")
         ctx.obj._new_analysis_playbook_cli(
             value,
             "observable",
-            playbook,
+            check,
             tlp,
+            playbooks_list,
             runtime_config,
             tags_labels,
             should_poll,
+            check_minutes_ago,
         )
-        print("here3")
     except IntelOwlClientException as e:
         ctx.obj.logger.fatal(str(e))
 
 
 @analyse.command(help="Send playbook analysis request for an observable")
 @click.argument("filepath", type=click.Path(exists=True, resolve_path=True))
-@click.argument("playbook")
 @add_options(__playbook_analyse_options)
 @click.pass_context
 def playbook_file(
     ctx: ClickContext,
     filepath: str,
-    playbook: str,
+    playbooks_list: str,
     tags_list: str,
     tlp: str,
+    check,
+    check_minutes_ago: int,
     runtime_config,
     should_poll: bool,
 ):
+    playbooks_list = playbooks_list.split(",") if len(playbooks_list) else []
     tags_labels = tags_list.split(",") if len(tags_list) else []
     if runtime_config:
         runtime_config = get_json_data(runtime_config)
     else:
         runtime_config = {}
     try:
         ctx.obj._new_analysis_playbook_cli(
             filepath,
             "file",
-            playbook,
+            check,
             tlp,
+            playbooks_list,
             runtime_config,
             tags_labels,
             should_poll,
+            check_minutes_ago,
         )
     except IntelOwlClientException as e:
         ctx.obj.logger.fatal(str(e))
 
 
 @analyse.command(
     help="Send multiple analysis requests. Reads file (csv or json) for inputs."
```

### Comparing `pyintelowl-5.0.0/pyintelowl/cli/commands.py` & `pyintelowl-5.0.0rc0/pyintelowl/cli/commands.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/pyintelowl/cli/config.py` & `pyintelowl-5.0.0rc0/pyintelowl/cli/config.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/pyintelowl/cli/domain_checkers.py` & `pyintelowl-5.0.0rc0/pyintelowl/cli/domain_checkers.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/pyintelowl/cli/jobs.py` & `pyintelowl-5.0.0rc0/pyintelowl/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/pyintelowl/cli/tags.py` & `pyintelowl-5.0.0rc0/pyintelowl/cli/tags.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/pyintelowl/exceptions.py` & `pyintelowl-5.0.0rc0/pyintelowl/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/pyintelowl/main.py` & `pyintelowl-5.0.0rc0/pyintelowl/main.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/pyintelowl/pyintelowl.py` & `pyintelowl-5.0.0rc0/pyintelowl/pyintelowl.py`

 * *Files 0% similar despite different names*

```diff
@@ -765,52 +765,56 @@
                 """
             )
 
     def _new_analysis_playbook_cli(
         self,
         obj: str,
         type_: str,
+        check,
         playbook: str,
         tlp: TLPType = None,
         runtime_configuration: Dict = None,
         tags_labels: List[str] = None,
         should_poll: bool = False,
+        minutes_ago: int = None,
     ) -> None:
         """
         For internal use by the pyintelowl CLI.
         """
         if not runtime_configuration:
             runtime_configuration = {}
         if not tags_labels:
             tags_labels = []
 
+            return
+
         self.logger.info(
             f"""Requesting analysis..
             {type_}: [blue]{obj}[/]
             playbook: [i green]{playbook}[/]
             tags: [i green]{tags_labels}[/]
             """
         )
 
         # 1st step, make request
         if type_ == "observable":
             resp = self.send_observable_analysis_playbook_request(
                 observable_name=obj,
-                playbook_requested=playbook,
                 tlp=tlp,
+                playbook_requested=playbook,
                 runtime_configuration=runtime_configuration,
                 tags_labels=tags_labels,
             )
         else:
             path = pathlib.Path(obj)
             resp = self.send_file_analysis_playbook_request(
                 filename=path.name,
                 binary=path.read_bytes(),
-                playbook_requested=playbook,
                 tlp=tlp,
+                playbook_requested=playbook,
                 runtime_configuration=runtime_configuration,
                 tags_labels=tags_labels,
             )
 
         # 2nd step: poll for result
         if should_poll:
             if resp.get("status", "") != "accepted":
```

### Comparing `pyintelowl-5.0.0/pyintelowl.egg-info/PKG-INFO` & `pyintelowl-5.0.0rc0/pyintelowl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintelowl
-Version: 5.0.0
+Version: 5.0.0rc0
 Summary: Robust Python SDK and CLI for IntelOwl's API
 Home-page: https://github.com/intelowlproject/pyintelowl
 Author: Matteo Lodi
 Project-URL: Documentation, https://github.com/intelowlproject/pyintelowl
 Project-URL: Funding, https://liberapay.com/IntelOwlProject/
 Project-URL: Source, https://github.com/intelowlproject/pyintelowl
 Project-URL: Tracker, https://github.com/intelowlproject/pyintelowl/issues
```

### Comparing `pyintelowl-5.0.0/pyintelowl.egg-info/SOURCES.txt` & `pyintelowl-5.0.0rc0/pyintelowl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/pyintelowl.egg-info/requires.txt` & `pyintelowl-5.0.0rc0/pyintelowl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/setup.py` & `pyintelowl-5.0.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/tests/mocked_requests.py` & `pyintelowl-5.0.0rc0/tests/mocked_requests.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/tests/test_general.py` & `pyintelowl-5.0.0rc0/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/tests/test_jobs.py` & `pyintelowl-5.0.0rc0/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/tests/test_tags.py` & `pyintelowl-5.0.0rc0/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-5.0.0/tests/utils.py` & `pyintelowl-5.0.0rc0/tests/utils.py`

 * *Files identical despite different names*

