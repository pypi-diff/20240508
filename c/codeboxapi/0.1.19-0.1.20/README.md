# Comparing `tmp/codeboxapi-0.1.19.tar.gz` & `tmp/codeboxapi-0.1.20.tar.gz`

## Comparing `codeboxapi-0.1.19.tar` & `codeboxapi-0.1.20.tar`

### file list

```diff
@@ -1,41 +1,40 @@
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/.env.example
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/.pre-commit-config.yaml
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/mkdocs.yml
--rw-r--r--   0        0        0   272022 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/poetry.lock
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/requirements.lock
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/roadmap.todo
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/.github/workflows/auto-tests.yml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/.github/workflows/code-check.yml
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/.github/workflows/docs.yml
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/.vscode/settings.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/docs/api.md
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/docs/concepts.md
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/docs/examples.md
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/docs/index.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/docs/installation.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/docs/settings.md
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/docs/usage.md
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/examples/async_file_io.py
--rwxr-xr-x   0        0        0     2180 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/examples/async_plot_dataset.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/examples/file_io.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/examples/parallel.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/examples/plot_dataset.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/examples/session_restoring.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/examples/assets/dataset_code.txt
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/src/codeboxapi/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/src/codeboxapi/config.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/src/codeboxapi/errors.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/src/codeboxapi/schema.py
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/src/codeboxapi/utils.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/src/codeboxapi/box/__init__.py
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/src/codeboxapi/box/basebox.py
--rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/src/codeboxapi/box/codebox.py
--rw-r--r--   0        0        0    23178 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/src/codeboxapi/box/localbox.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/tests/general_test.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/tests/run_all_examples.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/LICENSE
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/README.md
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/pyproject.toml
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 codeboxapi-0.1.19/PKG-INFO
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/.env.example
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/mkdocs.yml
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/requirements.lock
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/roadmap.todo
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/.github/workflows/auto-tests.yml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/.github/workflows/code-check.yml
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/.vscode/settings.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/docs/api.md
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/docs/concepts.md
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/docs/examples.md
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/docs/index.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/docs/installation.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/docs/settings.md
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/docs/usage.md
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/examples/async_file_io.py
+-rwxr-xr-x   0        0        0     2180 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/examples/async_plot_dataset.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/examples/file_io.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/examples/parallel.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/examples/plot_dataset.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/examples/session_restoring.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/examples/assets/dataset_code.txt
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/src/codeboxapi/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/src/codeboxapi/config.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/src/codeboxapi/errors.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/src/codeboxapi/schema.py
+-rw-r--r--   0        0        0     6091 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/src/codeboxapi/utils.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/src/codeboxapi/box/__init__.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/src/codeboxapi/box/basebox.py
+-rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/src/codeboxapi/box/codebox.py
+-rw-r--r--   0        0        0    23178 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/src/codeboxapi/box/localbox.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/tests/general_test.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/tests/run_all_examples.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/LICENSE
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/README.md
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/pyproject.toml
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 codeboxapi-0.1.20/PKG-INFO
```

### Comparing `codeboxapi-0.1.19/.pre-commit-config.yaml` & `codeboxapi-0.1.20/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/mkdocs.yml` & `codeboxapi-0.1.20/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/.github/workflows/code-check.yml` & `codeboxapi-0.1.20/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/.github/workflows/docs.yml` & `codeboxapi-0.1.20/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/.github/workflows/python-publish.yml` & `codeboxapi-0.1.20/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/docs/concepts.md` & `codeboxapi-0.1.20/docs/concepts.md`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/docs/examples.md` & `codeboxapi-0.1.20/docs/examples.md`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/docs/index.md` & `codeboxapi-0.1.20/docs/index.md`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/docs/settings.md` & `codeboxapi-0.1.20/docs/settings.md`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/docs/usage.md` & `codeboxapi-0.1.20/docs/usage.md`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/examples/async_file_io.py` & `codeboxapi-0.1.20/examples/async_file_io.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/examples/async_plot_dataset.py` & `codeboxapi-0.1.20/examples/async_plot_dataset.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/examples/file_io.py` & `codeboxapi-0.1.20/examples/file_io.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/examples/plot_dataset.py` & `codeboxapi-0.1.20/examples/plot_dataset.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/src/codeboxapi/config.py` & `codeboxapi-0.1.20/src/codeboxapi/config.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/src/codeboxapi/errors.py` & `codeboxapi-0.1.20/src/codeboxapi/errors.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/src/codeboxapi/schema.py` & `codeboxapi-0.1.20/src/codeboxapi/schema.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/src/codeboxapi/box/basebox.py` & `codeboxapi-0.1.20/src/codeboxapi/box/basebox.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/src/codeboxapi/box/codebox.py` & `codeboxapi-0.1.20/src/codeboxapi/box/codebox.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/src/codeboxapi/box/localbox.py` & `codeboxapi-0.1.20/src/codeboxapi/box/localbox.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/tests/general_test.py` & `codeboxapi-0.1.20/tests/general_test.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/tests/run_all_examples.py` & `codeboxapi-0.1.20/tests/run_all_examples.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/LICENSE` & `codeboxapi-0.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/README.md` & `codeboxapi-0.1.20/README.md`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.1.19/pyproject.toml` & `codeboxapi-0.1.20/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "codeboxapi"
-version = "0.1.19"
+version = "0.1.20"
 description = "CodeBox gives you an easy scalable and isolated python interpreter for your LLM Agents."
 keywords = [
     "codebox",
     "api",
     "python-interpreter",
     "cloud-infra",
     "llm",
```

### Comparing `codeboxapi-0.1.19/PKG-INFO` & `codeboxapi-0.1.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: codeboxapi
-Version: 0.1.19
+Version: 0.1.20
 Summary: CodeBox gives you an easy scalable and isolated python interpreter for your LLM Agents.
 Project-URL: repository, https://github.com/shroominic/codebox-api
 Project-URL: api-reference, https://codeboxapi.com/docs
 Project-URL: docs, https://codeboxapi.com/docs
 Author-email: Shroominic <contact@shroominic.com>
 License: MIT
 License-File: LICENSE
```

