# Comparing `tmp/mozilla-taskgraph-2.0.0.tar.gz` & `tmp/mozilla-taskgraph-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-taskgraph-2.0.0.tar", last modified: Wed May  8 16:25:29 2024, max compression
+gzip compressed data, was "mozilla-taskgraph-2.0.1.tar", last modified: Wed May  8 20:55:50 2024, max compression
```

## Comparing `mozilla-taskgraph-2.0.0.tar` & `mozilla-taskgraph-2.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.011829 mozilla-taskgraph-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-08 16:25:29.011829 mozilla-taskgraph-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:25:29.011829 mozilla-taskgraph-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.007829 mozilla-taskgraph-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.007829 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.007829 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/actions/release_promotion.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.007829 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.007829 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.007829 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/worker_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.007829 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-08 16:25:28.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-08 16:25:29.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:25:28.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 16:25:28.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 16:25:28.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.011829 mozilla-taskgraph-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/test/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/test/test_worker_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:55:50.228180 mozilla-taskgraph-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-08 20:55:50.228180 mozilla-taskgraph-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:55:50.228180 mozilla-taskgraph-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:55:50.224180 mozilla-taskgraph-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:55:50.224180 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:55:50.224180 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/actions/release_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:55:50.224180 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:55:50.224180 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/transforms/scriptworker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/transforms/scriptworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:55:50.224180 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/transforms/scriptworker/shipit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/transforms/scriptworker/shipit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/worker_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:55:50.224180 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-08 20:55:50.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-08 20:55:50.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:55:50.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 20:55:50.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 20:55:50.000000 mozilla-taskgraph-2.0.1/src/mozilla_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:55:50.228180 mozilla-taskgraph-2.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/test/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-05-08 20:55:46.000000 mozilla-taskgraph-2.0.1/test/test_worker_types.py
```

### Comparing `mozilla-taskgraph-2.0.0/LICENSE` & `mozilla-taskgraph-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-2.0.0/PKG-INFO` & `mozilla-taskgraph-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-taskgraph
-Version: 2.0.0
+Version: 2.0.1
 Summary: Mozilla-specific transforms and utilities for Taskgraph
 Home-page: https://github.com/mozilla-releng/mozilla-taskgraph
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mozilla-taskgraph-2.0.0/README.md` & `mozilla-taskgraph-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-2.0.0/pyproject.toml` & `mozilla-taskgraph-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-2.0.0/setup.py` & `mozilla-taskgraph-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/__init__.py` & `mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/actions/__init__.py` & `mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/actions/release_promotion.py` & `mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/actions/release_promotion.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/config.py` & `mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py` & `mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py` & `mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/worker_types.py` & `mozilla-taskgraph-2.0.1/src/mozilla_taskgraph/worker_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,32 +76,34 @@
 
     # Set some global_params implicitly from Taskcluster params.
     global_params = {
         "commit_hash": config.params["head_rev"],
         "branch_repo_owner": config.params["head_repository"],
     }
 
-    head_ref = normref(config.params["head_ref"])
-    head_tag = normref(config.params["head_tag"], type="tags")
-    base_ref = normref(config.params["base_ref"])
-
-    if head_ref:
+    if head_ref := normref(config.params["head_ref"]):
         global_params["branch"] = head_ref
 
-    if head_tag:
+    if head_tag := normref(config.params["head_tag"], type="tags"):
         global_params["tag"] = head_tag
 
+    if commit_message := config.params.get("commit_message"):
+        global_params["commit_message"] = commit_message
+
+    if pull_request_number := config.params.get("pull_request_number"):
+        global_params["pull_request_id"] = pull_request_number
+
     if config.params["tasks_for"] == "github-pull-request":
         global_params["pull_request_author"] = config.params["owner"]
 
-        if base_ref:
+        if base_ref := normref(config.params["base_ref"]):
             global_params["branch_dest"] = base_ref
 
-        if config.params["base_repository"]:
-            global_params["branch_dest_repo_owner"] = config.params["base_repository"]
+        if base_repository := config.params["base_repository"]:
+            global_params["branch_dest_repo_owner"] = base_repository
 
     task_def["payload"] = {"global_params": global_params}
     if workflow_params:
         task_def["payload"]["workflow_params"] = workflow_params
 
     if bitrise.get("artifact_prefix"):
         task_def["payload"]["artifact_prefix"] = bitrise["artifact_prefix"]
```

### Comparing `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/PKG-INFO` & `mozilla-taskgraph-2.0.1/src/mozilla_taskgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-taskgraph
-Version: 2.0.0
+Version: 2.0.1
 Summary: Mozilla-specific transforms and utilities for Taskgraph
 Home-page: https://github.com/mozilla-releng/mozilla-taskgraph
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/SOURCES.txt` & `mozilla-taskgraph-2.0.1/src/mozilla_taskgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-2.0.0/test/test_register.py` & `mozilla-taskgraph-2.0.1/test/test_register.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-2.0.0/test/test_worker_types.py` & `mozilla-taskgraph-2.0.1/test/test_worker_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,24 +54,30 @@
                 ],
                 "tags": {"worker-implementation": "scriptworker"},
             },
             id="default params",
         ),
         pytest.param(
             {"bitrise": {"app": "some-app", "workflows": ["bar"]}},
-            {"tasks_for": "github-pull-request"},
+            {
+                "tasks_for": "github-pull-request",
+                "commit_message": "This is a commit",
+                "pull_request_number": "123",
+            },
             {
                 "payload": {
                     "global_params": {
                         "branch": "default",
                         "branch_dest": "123456",
                         "branch_dest_repo_owner": "http://example.com/base/repo",
                         "branch_repo_owner": "http://example.com/head/repo",
                         "commit_hash": "abcdef",
                         "pull_request_author": "some-owner",
+                        "commit_message": "This is a commit",
+                        "pull_request_id": "123",
                     },
                 },
                 "scopes": ["foo:bitrise:app:some-app", "foo:bitrise:workflow:bar"],
                 "tags": {"worker-implementation": "scriptworker"},
             },
             id="pull request",
         ),
@@ -79,22 +85,26 @@
             {"bitrise": {"app": "some-app", "workflows": ["bar"]}},
             {
                 "base_ref": "",
                 "base_repository": "",
                 "head_ref": "",
                 "head_tag": "some-tag",
                 "tasks_for": "github-pull-request",
+                "commit_message": "This is a commit",
+                "pull_request_number": "123",
             },
             {
                 "payload": {
                     "global_params": {
                         "branch_repo_owner": "http://example.com/head/repo",
                         "commit_hash": "abcdef",
                         "pull_request_author": "some-owner",
                         "tag": "some-tag",
+                        "commit_message": "This is a commit",
+                        "pull_request_id": "123",
                     }
                 },
                 "scopes": ["foo:bitrise:app:some-app", "foo:bitrise:workflow:bar"],
                 "tags": {"worker-implementation": "scriptworker"},
             },
             id="opposite params",  # this test helps hit other half of if statements
         ),
@@ -102,24 +112,28 @@
             {"bitrise": {"app": "some-app", "workflows": ["bar"]}},
             {
                 "base_ref": "refs/heads/foo",
                 "base_repository": "",
                 "head_ref": "refs/heads/bar",
                 "head_tag": "refs/tags/some-tag",
                 "tasks_for": "github-pull-request",
+                "commit_message": "This is a commit",
+                "pull_request_number": "123",
             },
             {
                 "payload": {
                     "global_params": {
                         "branch": "bar",
                         "branch_dest": "foo",
                         "branch_repo_owner": "http://example.com/head/repo",
                         "commit_hash": "abcdef",
                         "pull_request_author": "some-owner",
                         "tag": "some-tag",
+                        "commit_message": "This is a commit",
+                        "pull_request_id": "123",
                     }
                 },
                 "scopes": ["foo:bitrise:app:some-app", "foo:bitrise:workflow:bar"],
                 "tags": {"worker-implementation": "scriptworker"},
             },
             id="normalize refs",
         ),
@@ -127,21 +141,25 @@
             {"bitrise": {"app": "some-app", "workflows": ["bar"]}},
             {
                 "base_ref": "refs/tags/foo",
                 "base_repository": "",
                 "head_ref": "refs/tags/bar",
                 "head_tag": "refs/heads/some-tag",
                 "tasks_for": "github-pull-request",
+                "commit_message": "This is a commit",
+                "pull_request_number": "123",
             },
             {
                 "payload": {
                     "global_params": {
                         "branch_repo_owner": "http://example.com/head/repo",
                         "commit_hash": "abcdef",
                         "pull_request_author": "some-owner",
+                        "commit_message": "This is a commit",
+                        "pull_request_id": "123",
                     }
                 },
                 "scopes": ["foo:bitrise:app:some-app", "foo:bitrise:workflow:bar"],
                 "tags": {"worker-implementation": "scriptworker"},
             },
             id="normalize refs wrong type",
         ),
```

