# Comparing `tmp/nens-meta-0.5.tar.gz` & `tmp/nens-meta-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nens-meta-0.5.tar", last modified: Mon Apr  8 09:53:03 2024, max compression
+gzip compressed data, was "nens-meta-0.6.tar", last modified: Tue May  7 13:28:19 2024, max compression
```

## Comparing `nens-meta-0.5.tar` & `nens-meta-0.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-04-08 09:53:03.860541 nens-meta-0.5/
--rw-r--r--   0 reinout    (501) staff       (20)     2680 2024-04-08 09:53:03.000000 nens-meta-0.5/CHANGES.md
--rw-r--r--   0 reinout    (501) staff       (20)     1766 2024-04-08 09:53:03.000000 nens-meta-0.5/DEVELOPMENT.md
--rw-r--r--   0 reinout    (501) staff       (20)     1075 2024-04-08 09:53:03.000000 nens-meta-0.5/LICENSE
--rw-r--r--   0 reinout    (501) staff       (20)      153 2024-04-08 09:53:03.000000 nens-meta-0.5/MANIFEST.in
--rw-r--r--   0 reinout    (501) staff       (20)     2356 2024-04-08 09:53:03.860343 nens-meta-0.5/PKG-INFO
--rw-r--r--   0 reinout    (501) staff       (20)     1666 2024-04-08 09:53:03.000000 nens-meta-0.5/README.md
--rw-r--r--   0 reinout    (501) staff       (20)     1002 2024-04-08 09:53:03.000000 nens-meta-0.5/USAGE.md
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-04-08 09:53:03.857248 nens-meta-0.5/nens_meta/
--rw-r--r--   0 reinout    (501) staff       (20)       20 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/__init__.py
--rw-r--r--   0 reinout    (501) staff       (20)     6386 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/nens_toml.py
--rw-r--r--   0 reinout    (501) staff       (20)     8601 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/pyproject_toml.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-04-08 09:53:03.858274 nens-meta-0.5/nens_meta/templates/
--rw-r--r--   0 reinout    (501) staff       (20)       75 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/templates/README.md
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-04-08 09:53:03.859071 nens-meta-0.5/nens_meta/templates/default/
--rw-r--r--   0 reinout    (501) staff       (20)      120 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/templates/default/dependabot.yml.j2
--rw-r--r--   0 reinout    (501) staff       (20)      345 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/templates/default/editorconfig.j2
--rw-r--r--   0 reinout    (501) staff       (20)      452 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/templates/default/gitignore.j2
--rw-r--r--   0 reinout    (501) staff       (20)     1013 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/templates/default/meta_workflow.yml.j2
--rw-r--r--   0 reinout    (501) staff       (20)      732 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/templates/default/pre-commit-config.yaml.j2
--rw-r--r--   0 reinout    (501) staff       (20)      278 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/templates/default/requirements.yml.j2
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-04-08 09:53:03.859738 nens-meta-0.5/nens_meta/tests/
--rw-r--r--   0 reinout    (501) staff       (20)        0 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/tests/__init__.py
--rw-r--r--   0 reinout    (501) staff       (20)     4522 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/tests/test_nens_toml.py
--rw-r--r--   0 reinout    (501) staff       (20)     6072 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/tests/test_pyproject_toml.py
--rw-r--r--   0 reinout    (501) staff       (20)     3197 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/tests/test_update_project.py
--rw-r--r--   0 reinout    (501) staff       (20)     2429 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/tests/test_utils.py
--rw-r--r--   0 reinout    (501) staff       (20)     8375 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/update_project.py
--rw-r--r--   0 reinout    (501) staff       (20)     2709 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta/utils.py
-drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-04-08 09:53:03.859927 nens-meta-0.5/nens_meta.egg-info/
--rw-r--r--   0 reinout    (501) staff       (20)     2356 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta.egg-info/PKG-INFO
--rw-r--r--   0 reinout    (501) staff       (20)      881 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta.egg-info/SOURCES.txt
--rw-r--r--   0 reinout    (501) staff       (20)        1 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta.egg-info/dependency_links.txt
--rw-r--r--   0 reinout    (501) staff       (20)       70 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta.egg-info/entry_points.txt
--rw-r--r--   0 reinout    (501) staff       (20)       66 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta.egg-info/requires.txt
--rw-r--r--   0 reinout    (501) staff       (20)       10 2024-04-08 09:53:03.000000 nens-meta-0.5/nens_meta.egg-info/top_level.txt
--rw-r--r--   0 reinout    (501) staff       (20)     1583 2024-04-08 09:53:03.000000 nens-meta-0.5/pyproject.toml
--rw-r--r--   0 reinout    (501) staff       (20)       38 2024-04-08 09:53:03.860578 nens-meta-0.5/setup.cfg
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-05-07 13:28:19.659325 nens-meta-0.6/
+-rw-r--r--   0 reinout    (501) staff       (20)     3017 2024-05-07 13:28:19.000000 nens-meta-0.6/CHANGES.md
+-rw-r--r--   0 reinout    (501) staff       (20)     1766 2024-05-07 13:28:19.000000 nens-meta-0.6/DEVELOPMENT.md
+-rw-r--r--   0 reinout    (501) staff       (20)     1075 2024-05-07 13:28:19.000000 nens-meta-0.6/LICENSE
+-rw-r--r--   0 reinout    (501) staff       (20)      153 2024-05-07 13:28:19.000000 nens-meta-0.6/MANIFEST.in
+-rw-r--r--   0 reinout    (501) staff       (20)     2356 2024-05-07 13:28:19.659105 nens-meta-0.6/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)     1666 2024-05-07 13:28:19.000000 nens-meta-0.6/README.md
+-rw-r--r--   0 reinout    (501) staff       (20)     1002 2024-05-07 13:28:19.000000 nens-meta-0.6/USAGE.md
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-05-07 13:28:19.656206 nens-meta-0.6/nens_meta/
+-rw-r--r--   0 reinout    (501) staff       (20)       20 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)     5446 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/nens_toml.py
+-rw-r--r--   0 reinout    (501) staff       (20)     4716 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/pyproject_toml.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-05-07 13:28:19.657047 nens-meta-0.6/nens_meta/templates/
+-rw-r--r--   0 reinout    (501) staff       (20)       75 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/templates/README.md
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-05-07 13:28:19.657825 nens-meta-0.6/nens_meta/templates/default/
+-rw-r--r--   0 reinout    (501) staff       (20)      120 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/templates/default/dependabot.yml.j2
+-rw-r--r--   0 reinout    (501) staff       (20)      345 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/templates/default/editorconfig.j2
+-rw-r--r--   0 reinout    (501) staff       (20)      452 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/templates/default/gitignore.j2
+-rw-r--r--   0 reinout    (501) staff       (20)      571 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/templates/default/meta_workflow.yml.j2
+-rw-r--r--   0 reinout    (501) staff       (20)      726 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/templates/default/pre-commit-config.yaml.j2
+-rw-r--r--   0 reinout    (501) staff       (20)      278 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/templates/default/requirements.yml.j2
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-05-07 13:28:19.658454 nens-meta-0.6/nens_meta/tests/
+-rw-r--r--   0 reinout    (501) staff       (20)        0 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/tests/__init__.py
+-rw-r--r--   0 reinout    (501) staff       (20)     3893 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/tests/test_nens_toml.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2113 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/tests/test_pyproject_toml.py
+-rw-r--r--   0 reinout    (501) staff       (20)     3197 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/tests/test_update_project.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2405 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/tests/test_utils.py
+-rw-r--r--   0 reinout    (501) staff       (20)     7598 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/update_project.py
+-rw-r--r--   0 reinout    (501) staff       (20)     2606 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta/utils.py
+drwxr-xr-x   0 reinout    (501) staff       (20)        0 2024-05-07 13:28:19.658641 nens-meta-0.6/nens_meta.egg-info/
+-rw-r--r--   0 reinout    (501) staff       (20)     2356 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta.egg-info/PKG-INFO
+-rw-r--r--   0 reinout    (501) staff       (20)      881 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta.egg-info/SOURCES.txt
+-rw-r--r--   0 reinout    (501) staff       (20)        1 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta.egg-info/dependency_links.txt
+-rw-r--r--   0 reinout    (501) staff       (20)       70 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta.egg-info/entry_points.txt
+-rw-r--r--   0 reinout    (501) staff       (20)       66 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta.egg-info/requires.txt
+-rw-r--r--   0 reinout    (501) staff       (20)       10 2024-05-07 13:28:19.000000 nens-meta-0.6/nens_meta.egg-info/top_level.txt
+-rw-r--r--   0 reinout    (501) staff       (20)     1583 2024-05-07 13:28:19.000000 nens-meta-0.6/pyproject.toml
+-rw-r--r--   0 reinout    (501) staff       (20)       38 2024-05-07 13:28:19.659362 nens-meta-0.6/setup.cfg
```

### Comparing `nens-meta-0.5/CHANGES.md` & `nens-meta-0.6/CHANGES.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # Changelog of nens-meta
 
 
+## 0.6 (2024-05-07)
+
+
+- Removed most of the python library/packaging/testing stuff, leaving basically only the ruff/precommit parts. This simplifies it a lot.
+- The `is_python_project` config variable is now `uses_python`.
+- The `nens-update-project` command no longer requires a path argument, but just works in the current directory.
+
 ## 0.5 (2024-04-08)
 
 - Simplified everything by removing tox for now.
 - Suggesting initial `requirements.yml` for ansible projects as ansible-lint almost always needs it.
 - Allow additional directories (`extra_package_names`) with python code next to the "main" one (`package_name`). Some projects use more than one directory. This has effect on the test runner, coverage reports, etc.
```

### Comparing `nens-meta-0.5/DEVELOPMENT.md` & `nens-meta-0.6/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `nens-meta-0.5/LICENSE` & `nens-meta-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nens-meta-0.5/PKG-INFO` & `nens-meta-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nens-meta
-Version: 0.5
+Version: 0.6
 Summary: Basic project automation and update tool
 Author-email: Reinout van Rees <reinout.vanrees@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Documentation, https://nens-meta.readthedocs.io/
 Project-URL: Repository, https://github.com/nens/nens-meta
 Project-URL: Changelog, https://github.com/nens/nens-meta/blob/main/CHANGES.md
 Requires-Python: >=3.11
```

### Comparing `nens-meta-0.5/README.md` & `nens-meta-0.6/README.md`

 * *Files identical despite different names*

### Comparing `nens-meta-0.5/USAGE.md` & `nens-meta-0.6/USAGE.md`

 * *Files identical despite different names*

### Comparing `nens-meta-0.5/nens_meta/nens_toml.py` & `nens-meta-0.6/nens_meta/nens_toml.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,72 +14,60 @@
 
 @dataclass
 class Option:
     key: str
     description: str
     value_type: type = str
     default: Any = ""
-    default_if_python: Any = ""
 
 
 META_FILENAME = ".nens.toml"
 KNOWN_SECTIONS: dict[str, list[Option]] = {}
 # First key is the section name, the second key/value pair is the variable name and the
 # explanation. If the second key ends with "_TRUE"/"_FALSE", this is stripped and will
 # be used to treat the value as a boolean with the indicated default.
 KNOWN_SECTIONS["meta"] = [
     Option(key="meta_version", description="Version used to generate the config"),
     Option(
         key="project_name",
         description="Project name (normally the name of the directory)",
     ),
     Option(
-        key="is_python_project",
-        description="Whether we are a python project",
+        key="uses_python",
+        description="Whether we use python",
         default=False,
         value_type=bool,
     ),
     Option(
         key="uses_ansible",
         description="Whether we have an ansible dir",
         default=False,
         value_type=bool,
     ),
-    Option(key="package_name", description="Name of the main python package"),
-    Option(
-        key="extra_package_names",
-        description="Extra dirs with packages, in addition to package_name",
-        default=[],
-        value_type=list,
-    ),
-    Option(key="minimum_coverage", description="Minimum code coverage percentage"),
 ]
 KNOWN_SECTIONS["pyprojecttoml"] = []
 KNOWN_SECTIONS["meta_workflow"] = [
     Option(
         key="main_python_version",
         description="Python version to use for linting and so",
-        default="3.11",
+        default="3.12",
     ),
 ]
 
 logger = logging.getLogger(__name__)
 
 
 def write_documentation():
     target = Path(__file__).parent.parent / "doc" / "nens_toml_example.toml"
     lines = []
     for section in KNOWN_SECTIONS:
         lines.append(f"[{section}]")
         for option in KNOWN_SECTIONS[section]:
             lines.append(f"# {option.description}")
             lines.append(f"{option.key} = {repr(option.default)}")
-            if option.default_if_python:
-                lines.append("# In case of a python project:")
-                lines.append(f"# {option.key} = {option.default_if_python}")
         lines.append("")
 
     content = "\n".join(lines)
     content = content.replace(" False", " false")  # Toml syntax hack
     target.write_text(content)
 
 
@@ -95,21 +83,19 @@
     our_config.update_meta_options()
     our_config.write()
 
 
 def detected_meta_values(project: Path) -> dict[str, str | bool | list]:
     """Return values we can detect about the project, normally set in [meta]"""
     detected: dict[str, str | bool | list] = {}
-    detected["is_python_project"] = utils.is_python_project(project)
+    detected["uses_python"] = utils.uses_python(project)
     detected["uses_ansible"] = utils.uses_ansible(project)
     detected["meta_version"] = __version__
     name = project.resolve().name
     detected["project_name"] = name
-    if detected["is_python_project"]:
-        detected["package_name"] = name.replace("-", "_")
     return detected
 
 
 class MissingDocumentationError(Exception):
     pass
 
 
@@ -164,22 +150,15 @@
                 f"Section {section_name} not documented in nens-meta"
             )
         section = self._contents.get(section_name)
         if section is None:
             section = {}
         options: dict[str, str | bool | list] = {}
         for option in KNOWN_SECTIONS[section_name]:
-            if (
-                self._contents.get("meta")
-                and self._contents.get("meta")["is_python_project"]
-            ):
-                default = option.default_if_python or option.default
-            else:
-                default = option.default
-            value = section.get(option.key, copy.deepcopy(default))
+            value = section.get(option.key, copy.deepcopy(option.default))
             if not isinstance(value, option.value_type):
                 raise ValueError(
                     f"{option.key} should be of type {option.value_type}, not {type(value)}"
                 )
             options[option.key] = value
         logger.debug(f"Contents of section {section_name}: {options}")
         return options
```

### Comparing `nens-meta-0.5/nens_meta/templates/default/pre-commit-config.yaml.j2` & `nens-meta-0.6/nens_meta/templates/default/pre-commit-config.yaml.j2`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
         args: [--allow-multiple-documents]
       - id: check-toml
       - id: check-added-large-files
-{% if is_python_project %}
+{% if uses_python %}
   - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
     rev: v0.1.13
     hooks:
       # Run the linter.
       - id: ruff
         args: ["--fix"]
```

### Comparing `nens-meta-0.5/nens_meta/tests/test_nens_toml.py` & `nens-meta-0.6/nens_meta/tests/test_nens_toml.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,44 +67,44 @@
 
 
 def test_section_options_boolean1(tmp_path: Path):
     # Handle boolean values (those have _TRUE or _FALSE prepended)
     nens_toml.nens_toml_file(tmp_path).write_text(
         """
     [meta]
-    is_python_project = true
+    uses_python = true
     """
     )
     config = nens_toml.OurConfig(tmp_path)
-    assert config.section_options("meta")["is_python_project"] is True
+    assert config.section_options("meta")["uses_python"] is True
 
 
 def test_section_options_boolean2(tmp_path: Path):
     # Handle default for boolean values
     nens_toml.nens_toml_file(tmp_path).write_text(
         """
     [meta]
-    # is_python_project has a default of false
+    # uses_python has a default of false
     """
     )
     config = nens_toml.OurConfig(tmp_path)
-    assert config.section_options("meta")["is_python_project"] is False
+    assert config.section_options("meta")["uses_python"] is False
 
 
 def test_section_options_boolean3(tmp_path: Path):
     # Complain if a boolean value has a non-boolean value.
     nens_toml.nens_toml_file(tmp_path).write_text(
         """
     [meta]
-    is_python_project = "1972"
+    uses_python = "1972"
     """
     )
     config = nens_toml.OurConfig(tmp_path)
     with pytest.raises(ValueError):
-        config.section_options("meta")["is_python_project"]
+        config.section_options("meta")["uses_python"]
 
 
 def test_update_meta_options1(tmp_path: Path):
     # Create a new "meta" section if it is missing.
     nens_toml.nens_toml_file(tmp_path).write_text("")
     config = nens_toml.OurConfig(tmp_path)
     # the init automatically calls config.update_meta_options()
@@ -117,28 +117,14 @@
     config = nens_toml.OurConfig(tmp_path)
     # the init automatically calls config.update_meta_options()
     meta_section = config.section_options("meta")
     assert "meta_version" in meta_section
     assert "project_name" in meta_section
 
 
-def test_update_meta_options3(tmp_path: Path):
-    # package_name is updated/guessed for python packages.
-    project_dir = tmp_path / "my-project"
-    project_dir.mkdir()
-    python_indicator = project_dir / "pyproject.toml"
-    python_indicator.write_text("")
-    nens_toml.nens_toml_file(project_dir).write_text("")
-    config = nens_toml.OurConfig(project_dir)
-    # the init automatically calls config.update_meta_options()
-    meta_section = config.section_options("meta")
-    assert meta_section["project_name"] == "my-project"
-    assert meta_section["package_name"] == "my_project"
-
-
 def test_update_meta_options4(tmp_path: Path):
     # The version should always be updated.
     nens_toml.nens_toml_file(tmp_path).write_text(
         """
     [meta]
     meta_version = "1972"
     """
```

### Comparing `nens-meta-0.5/nens_meta/tests/test_update_project.py` & `nens-meta-0.6/nens_meta/tests/test_update_project.py`

 * *Files identical despite different names*

### Comparing `nens-meta-0.5/nens_meta/tests/test_utils.py` & `nens-meta-0.6/nens_meta/tests/test_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -55,23 +55,23 @@
     f.write_text("bla bla\n# NENS_META_LEAVE_ALONE\n")
     utils.write_if_changed(f, "test")
     content = f.read_text()
     assert content.startswith("bla bla")
     assert (tmp_path / "sample.txt.suggestion").exists()
 
 
-def test_is_python_project1():
+def test_uses_python1():
     # We ourselves are a python project.
     ourselves = Path(__file__).parent.parent.parent
-    assert utils.is_python_project(ourselves)
+    assert utils.uses_python(ourselves)
 
 
-def test_is_python_project2(tmp_path: Path):
+def test_uses_python2(tmp_path: Path):
     # An empty dir is not a python project
-    assert not utils.is_python_project(tmp_path)
+    assert not utils.uses_python(tmp_path)
 
 
 def test_uses_ansible1():
     # We ourselves have no ansible/ dir.
     ourselves = Path(__file__).parent.parent.parent
     assert not utils.uses_ansible(ourselves)
```

### Comparing `nens-meta-0.5/nens_meta/update_project.py` & `nens-meta-0.6/nens_meta/update_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,65 +174,48 @@
         nens_toml.create_if_missing(project_dir)
         logger.warning("No .nens.toml found, created one. Re-run after checking.")
         sys.exit(1)
 
 
 def do_some_python_checks(project_dir: Path):
     """Run some checks to help identify issues and things you still need to do"""
-    requirementstxt = project_dir / "requirements.txt"
-    if not requirementstxt.exists():
-        logger.warning(f"There is no {requirementstxt}")
-    else:
-        dev_indicator1 = "-e "
-        dev_indicator2 = "[test]"
-        if not (
-            dev_indicator1 in requirementstxt.read_text()
-            and dev_indicator2 in requirementstxt.read_text()
-        ):
-            logger.warning(
-                f"The text '{dev_indicator1}' and '{dev_indicator2}' are "
-                f"not both found in {requirementstxt}"
-            )
-        if "coverage" not in requirementstxt.read_text():
-            logger.warning("You might want to add 'coverage' to requirements.txt")
     for file_to_check in project_dir.glob("*.outdated"):
         logger.warning(
             f"Check the old {file_to_check}: move settings to pyproject.toml, perhaps?"
         )
     website = "https://nens-meta.readthedocs.io"
     readme = Path("README.md")
     if readme.exists():
         if website not in readme.read_text():
             logger.warning(
                 f"{website} is not mentioned in the readme as an instruction"
             )
 
 
 def update_project(
-    project_dir: Annotated[Path, typer.Argument(exists=True)],
     verbose: Annotated[bool, typer.Option(help="Verbose logging")] = False,
 ):  # pragma: no cover
+    project_dir = Path(".")
     log_level = logging.DEBUG if verbose else logging.INFO
     logging.basicConfig(level=log_level, format="%(levelname)-7s: %(message)s")
     check_prerequisites(project_dir)
     our_config = nens_toml.OurConfig(project_dir)
     our_config.write()
 
-    if our_config.section_options("meta")["is_python_project"]:
+    if our_config.section_options("meta")["uses_python"]:
         if not pyproject_toml.pyproject_toml_file(project_dir).exists():
             pyproject_toml.create_if_missing(project_dir)
         options_for_project_config = {}
         options_for_project_config.update(our_config.section_options("meta"))
         options_for_project_config.update(our_config.section_options("pyprojecttoml"))
         project_config = pyproject_toml.PyprojectToml(
             project_dir, options_for_project_config
         )
         project_config.update()
         project_config.write()
-        project_config.move_outdated_files()
 
     # Grab editorconfig table and pass it along. Or rather the whole thing?
     editorconfig = Editorconfig(project_dir, our_config)
     editorconfig.write()
     gitignore = Gitignore(project_dir, our_config)
     gitignore.write()
     precommitconfig = Precommitconfig(project_dir, our_config)
@@ -242,13 +225,13 @@
     meta_workflow_yml = MetaWorkflowYml(project_dir, our_config)
     meta_workflow_yml.write()
 
     if our_config.section_options("meta")["uses_ansible"]:
         requirements_yml = RequirementsYml(project_dir, our_config)
         requirements_yml.write()
 
-    if our_config.section_options("meta")["is_python_project"]:
+    if our_config.section_options("meta")["uses_python"]:
         do_some_python_checks(project_dir)
 
 
 def main():  # pragma: no cover
     typer.run(update_project)
```

### Comparing `nens-meta-0.5/nens_meta/utils.py` & `nens-meta-0.6/nens_meta/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,20 +62,19 @@
         logger.debug(f"Leave-alone marger found in {target}")
         target = target.parent / (target.name + SUGGESTION_SUFFIX)
 
     target.write_text(new_content)
     logger.info(f"Wrote {target}")
 
 
-def is_python_project(project: Path) -> bool:
+def uses_python(project: Path) -> bool:
     """Return whether we detect a python project"""
-    for indicator in ["setup.py", "pyproject.toml", "setup.cfg"]:
-        if (project / indicator).exists():
-            logger.debug(f"{indicator} found, assuming it is a python project")
-            return True
+    if any(project.glob("**/*.py")):
+        logger.debug("*.py found, assuming we use python")
+        return True
     return False
 
 
 def uses_ansible(project: Path) -> bool:
     """Return whether we detect an ansible dir"""
     if (project / "ansible").exists():
         logger.debug("ansible/ dir found, assuming we use ansible")
```

### Comparing `nens-meta-0.5/nens_meta.egg-info/PKG-INFO` & `nens-meta-0.6/nens_meta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nens-meta
-Version: 0.5
+Version: 0.6
 Summary: Basic project automation and update tool
 Author-email: Reinout van Rees <reinout.vanrees@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Documentation, https://nens-meta.readthedocs.io/
 Project-URL: Repository, https://github.com/nens/nens-meta
 Project-URL: Changelog, https://github.com/nens/nens-meta/blob/main/CHANGES.md
 Requires-Python: >=3.11
```

### Comparing `nens-meta-0.5/nens_meta.egg-info/SOURCES.txt` & `nens-meta-0.6/nens_meta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nens-meta-0.5/pyproject.toml` & `nens-meta-0.6/pyproject.toml`

 * *Files identical despite different names*

