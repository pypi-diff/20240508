# Comparing `tmp/mozilla-taskgraph-1.5.0.tar.gz` & `tmp/mozilla-taskgraph-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-taskgraph-1.5.0.tar", last modified: Thu Apr 11 18:21:49 2024, max compression
+gzip compressed data, was "mozilla-taskgraph-2.0.0.tar", last modified: Wed May  8 16:25:29 2024, max compression
```

## Comparing `mozilla-taskgraph-1.5.0.tar` & `mozilla-taskgraph-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.662467 mozilla-taskgraph-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-11 18:21:49.662467 mozilla-taskgraph-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 18:21:49.662467 mozilla-taskgraph-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.658467 mozilla-taskgraph-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.658467 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.658467 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/actions/release_promotion.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.658467 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.658467 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.658467 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/worker_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.658467 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-11 18:21:49.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-11 18:21:49.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:21:49.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 18:21:49.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 18:21:49.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.662467 mozilla-taskgraph-1.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/test/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/test/test_worker_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.011829 mozilla-taskgraph-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-08 16:25:29.011829 mozilla-taskgraph-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:25:29.011829 mozilla-taskgraph-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.007829 mozilla-taskgraph-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.007829 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.007829 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/actions/release_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.007829 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.007829 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.007829 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/worker_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.007829 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-08 16:25:28.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-08 16:25:29.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:25:28.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 16:25:28.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 16:25:28.000000 mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:25:29.011829 mozilla-taskgraph-2.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/test/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-05-08 16:25:26.000000 mozilla-taskgraph-2.0.0/test/test_worker_types.py
```

### Comparing `mozilla-taskgraph-1.5.0/LICENSE` & `mozilla-taskgraph-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.5.0/PKG-INFO` & `mozilla-taskgraph-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-taskgraph
-Version: 1.5.0
+Version: 2.0.0
 Summary: Mozilla-specific transforms and utilities for Taskgraph
 Home-page: https://github.com/mozilla-releng/mozilla-taskgraph
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mozilla-taskgraph-1.5.0/README.md` & `mozilla-taskgraph-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.5.0/pyproject.toml` & `mozilla-taskgraph-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.5.0/setup.py` & `mozilla-taskgraph-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/__init__.py` & `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/actions/__init__.py` & `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/actions/release_promotion.py` & `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/actions/release_promotion.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/config.py` & `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py` & `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py` & `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/PKG-INFO` & `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-taskgraph
-Version: 1.5.0
+Version: 2.0.0
 Summary: Mozilla-specific transforms and utilities for Taskgraph
 Home-page: https://github.com/mozilla-releng/mozilla-taskgraph
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/SOURCES.txt` & `mozilla-taskgraph-2.0.0/src/mozilla_taskgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.5.0/test/test_register.py` & `mozilla-taskgraph-2.0.0/test/test_register.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.5.0/test/test_worker_types.py` & `mozilla-taskgraph-2.0.0/test/test_worker_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,24 +8,44 @@
 from mozilla_taskgraph import worker_types
 
 
 @pytest.mark.parametrize(
     "worker,extra_params,expected",
     (
         pytest.param({}, {}, Exception, id="missing bitrise"),
-        pytest.param({"bitrise": {"workflows": []}}, {}, Exception, id="missing app"),
+        pytest.param(
+            {"bitrise": {"workflows": ["foo"]}}, {}, Exception, id="missing app"
+        ),
         pytest.param(
             {"bitrise": {"app": "foo"}}, {}, Exception, id="missing workflows"
         ),
         pytest.param(
+            {"bitrise": {"app": "foo", "workflows": {"err": "nope"}}},
+            {},
+            Exception,
+            id="wrong workflows format",
+        ),
+        pytest.param(
+            {"bitrise": {"app": "foo", "workflows": [{"nope": ["wut"]}]}},
+            {},
+            Exception,
+            id="wrong workflows format2",
+        ),
+        pytest.param(
+            {"bitrise": {"app": "foo", "workflows": [{"foo": {"bar": ["oops"]}}]}},
+            {},
+            Exception,
+            id="wrong workflows format3",
+        ),
+        pytest.param(
             {"bitrise": {"app": "some-app", "workflows": ["bar", "baz"]}},
             {},
             {
                 "payload": {
-                    "build_params": {
+                    "global_params": {
                         "branch": "default",
                         "branch_repo_owner": "http://example.com/head/repo",
                         "commit_hash": "abcdef",
                     },
                 },
                 "scopes": [
                     "foo:bitrise:app:some-app",
@@ -37,15 +57,15 @@
             id="default params",
         ),
         pytest.param(
             {"bitrise": {"app": "some-app", "workflows": ["bar"]}},
             {"tasks_for": "github-pull-request"},
             {
                 "payload": {
-                    "build_params": {
+                    "global_params": {
                         "branch": "default",
                         "branch_dest": "123456",
                         "branch_dest_repo_owner": "http://example.com/base/repo",
                         "branch_repo_owner": "http://example.com/head/repo",
                         "commit_hash": "abcdef",
                         "pull_request_author": "some-owner",
                     },
@@ -62,15 +82,15 @@
                 "base_repository": "",
                 "head_ref": "",
                 "head_tag": "some-tag",
                 "tasks_for": "github-pull-request",
             },
             {
                 "payload": {
-                    "build_params": {
+                    "global_params": {
                         "branch_repo_owner": "http://example.com/head/repo",
                         "commit_hash": "abcdef",
                         "pull_request_author": "some-owner",
                         "tag": "some-tag",
                     }
                 },
                 "scopes": ["foo:bitrise:app:some-app", "foo:bitrise:workflow:bar"],
@@ -85,15 +105,15 @@
                 "base_repository": "",
                 "head_ref": "refs/heads/bar",
                 "head_tag": "refs/tags/some-tag",
                 "tasks_for": "github-pull-request",
             },
             {
                 "payload": {
-                    "build_params": {
+                    "global_params": {
                         "branch": "bar",
                         "branch_dest": "foo",
                         "branch_repo_owner": "http://example.com/head/repo",
                         "commit_hash": "abcdef",
                         "pull_request_author": "some-owner",
                         "tag": "some-tag",
                     }
@@ -110,54 +130,65 @@
                 "base_repository": "",
                 "head_ref": "refs/tags/bar",
                 "head_tag": "refs/heads/some-tag",
                 "tasks_for": "github-pull-request",
             },
             {
                 "payload": {
-                    "build_params": {
+                    "global_params": {
                         "branch_repo_owner": "http://example.com/head/repo",
                         "commit_hash": "abcdef",
                         "pull_request_author": "some-owner",
                     }
                 },
                 "scopes": ["foo:bitrise:app:some-app", "foo:bitrise:workflow:bar"],
                 "tags": {"worker-implementation": "scriptworker"},
             },
             id="normalize refs wrong type",
         ),
         pytest.param(
             {
                 "bitrise": {
                     "app": "some-app",
-                    "env": {
-                        "FOO": "bar",
-                        "PATH": {"artifact-reference": "<build/target.zip>"},
-                    },
-                    "workflows": ["bar"],
+                    "workflows": [
+                        "foo",
+                        {
+                            "bar": {
+                                "FOO": "bar",
+                                "PATH": {"artifact-reference": "<build/target.zip>"},
+                            }
+                        },
+                    ],
                 }
             },
             {},
             {
                 "payload": {
-                    "build_params": {
+                    "global_params": {
                         "branch": "default",
                         "branch_repo_owner": "http://example.com/head/repo",
                         "commit_hash": "abcdef",
-                        "environments": [
-                            {"mapped_to": "FOO", "value": "bar"},
-                            {
-                                "mapped_to": "PATH",
-                                "value": {"artifact-reference": "<build/target.zip>"},
-                            },
-                        ],
+                    },
+                    "workflow_params": {
+                        "bar": {
+                            "environments": [
+                                {"mapped_to": "FOO", "value": "bar"},
+                                {
+                                    "mapped_to": "PATH",
+                                    "value": {
+                                        "artifact-reference": "<build/target.zip>"
+                                    },
+                                },
+                            ]
+                        }
                     },
                 },
                 "scopes": [
                     "foo:bitrise:app:some-app",
+                    "foo:bitrise:workflow:foo",
                     "foo:bitrise:workflow:bar",
                 ],
                 "tags": {"worker-implementation": "scriptworker"},
             },
             id="environments",
         ),
         pytest.param(
@@ -168,15 +199,15 @@
                     "workflows": ["bar"],
                 }
             },
             {},
             {
                 "payload": {
                     "artifact_prefix": "public",
-                    "build_params": {
+                    "global_params": {
                         "branch": "default",
                         "branch_repo_owner": "http://example.com/head/repo",
                         "commit_hash": "abcdef",
                     },
                 },
                 "scopes": [
                     "foo:bitrise:app:some-app",
```

