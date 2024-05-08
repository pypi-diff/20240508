# Comparing `tmp/spiceai-0.3.2.tar.gz` & `tmp/spiceai-0.3.3.tar.gz`

## Comparing `spiceai-0.3.2.tar` & `spiceai-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 spiceai-0.3.2/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.2/scripts/mytoml.toml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.2/scripts/prompt.txt
--rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 spiceai-0.3.2/scripts/run.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spiceai-0.3.2/spice/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.2/spice/errors.py
--rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 spiceai-0.3.2/spice/models.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 spiceai-0.3.2/spice/providers.py
--rw-r--r--   0        0        0    34718 2020-02-02 00:00:00.000000 spiceai-0.3.2/spice/spice.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.2/spice/spice_message.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 spiceai-0.3.2/spice/utils.py
--rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.2/spice/wrapped_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spiceai-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 spiceai-0.3.2/tests/conftest.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 spiceai-0.3.2/tests/test_spice.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.2/LICENSE
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.2/README.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 spiceai-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 spiceai-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    28615 2020-02-02 00:00:00.000000 spiceai-0.3.3/tags
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 spiceai-0.3.3/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 spiceai-0.3.3/.ropeproject/globalnames
+-rw-r--r--   0        0        0    89341 2020-02-02 00:00:00.000000 spiceai-0.3.3/.ropeproject/history
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.3/scripts/mytoml.toml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.3/scripts/prompt.txt
+-rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 spiceai-0.3.3/scripts/run.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spiceai-0.3.3/spice/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.3/spice/errors.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 spiceai-0.3.3/spice/models.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 spiceai-0.3.3/spice/providers.py
+-rw-r--r--   0        0        0    34756 2020-02-02 00:00:00.000000 spiceai-0.3.3/spice/spice.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.3/spice/spice_message.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 spiceai-0.3.3/spice/utils.py
+-rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.3/spice/wrapped_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spiceai-0.3.3/tests/__init__.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 spiceai-0.3.3/tests/conftest.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 spiceai-0.3.3/tests/test_spice.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.3/LICENSE
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.3/README.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 spiceai-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 spiceai-0.3.3/PKG-INFO
```

### Comparing `spiceai-0.3.2/.github/workflows/ruff.yml` & `spiceai-0.3.3/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.2/scripts/run.py` & `spiceai-0.3.3/scripts/run.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.2/spice/errors.py` & `spiceai-0.3.3/spice/errors.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.2/spice/models.py` & `spiceai-0.3.3/spice/models.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.2/spice/providers.py` & `spiceai-0.3.3/spice/providers.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.2/spice/spice.py` & `spiceai-0.3.3/spice/spice.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,26 +263,26 @@
             logging_dir.mkdir(exist_ok=True, parents=True)
             with open(logging_dir / "prompts.json", "w") as file:
                 json.dump(self._prompts, file)
 
     def _log_response(self, response: SpiceResponse, name: Optional[str] = None):
         if self.logging_dir is not None:
             response_dict = dataclasses.asdict(response)
-            if name is None:
-                name = "spice"
-            if self._cur_logged_names[name] != 0 or name == "prompts":
-                name += f"_{self._cur_logged_names[name]}"
-            self._cur_logged_names[name] += 1
-            name += ".json"
+            base_name = "spice" if name is None else name
+            if base_name == "prompts":
+                full_name = "prompts.json"
+            else:
+                full_name = f"{base_name}_{self._cur_logged_names[base_name]}.json"
+                self._cur_logged_names[base_name] += 1
 
             response_json = json.dumps(response_dict, cls=MessagesEncoder)
 
             logging_dir = self.logging_dir / self._cur_run
             logging_dir.mkdir(exist_ok=True, parents=True)
-            with (logging_dir / name).open("w") as file:
+            with (logging_dir / full_name).open("w") as file:
                 file.write(f"{response_json}\n")
 
     @property
     def total_cost(self) -> float:
         """The total cost in cents of all api calls made through this Spice client."""
         return self._total_cost
```

### Comparing `spiceai-0.3.2/spice/spice_message.py` & `spiceai-0.3.3/spice/spice_message.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.2/spice/utils.py` & `spiceai-0.3.3/spice/utils.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.2/spice/wrapped_clients.py` & `spiceai-0.3.3/spice/wrapped_clients.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.2/tests/conftest.py` & `spiceai-0.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.2/tests/test_spice.py` & `spiceai-0.3.3/tests/test_spice.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.2/LICENSE` & `spiceai-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.2/README.md` & `spiceai-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.2/pyproject.toml` & `spiceai-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch]
 
 [tool.hatch.build.targets.wheel]
 packages=["spice"]
 
 [project]
 name = "spiceai"
-version = "0.3.2"
+version = "0.3.3"
 license = {text = "Apache-2.0"}
 description = "A Python library for building AI-powered applications."
 readme = "README.md"
 dependencies = [
     "python-dotenv",
     "openai",
     "anthropic",
```

### Comparing `spiceai-0.3.2/PKG-INFO` & `spiceai-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: spiceai
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python library for building AI-powered applications.
 License: Apache-2.0
 License-File: LICENSE
 Requires-Dist: anthropic
 Requires-Dist: httpx
 Requires-Dist: jinja2
 Requires-Dist: openai
```

