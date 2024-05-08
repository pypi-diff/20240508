# Comparing `tmp/scikit_build_core_conan-0.1.0.tar.gz` & `tmp/scikit_build_core_conan-0.2.0.tar.gz`

## Comparing `scikit_build_core_conan-0.1.0.tar` & `scikit_build_core_conan-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.1.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.1.0/src/scikit_build_core_conan/__init__.py
--rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.1.0/src/scikit_build_core_conan/build/__init__.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.1.0/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.1.0/LICENSE
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.1.0/README.md
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.2.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.2.0/src/scikit_build_core_conan/__init__.py
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.2.0/src/scikit_build_core_conan/build/__init__.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.2.0/README.md
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 scikit_build_core_conan-0.2.0/PKG-INFO
```

### Comparing `scikit_build_core_conan-0.1.0/.github/workflows/cd.yml` & `scikit_build_core_conan-0.2.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core_conan-0.1.0/src/scikit_build_core_conan/build/__init__.py` & `scikit_build_core_conan-0.2.0/src/scikit_build_core_conan/build/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import copy
 import dataclasses
 import io
 import json
 import os
 import shutil
+import sys
 import tempfile
-import tomllib
 from contextlib import redirect_stdout
 from pathlib import Path
 from typing import List, Optional
 
+if sys.version_info < (3, 11):
+    import tomli as tomllib
+else:
+    import tomllib
+
 import scikit_build_core.build
 from conan.api.conan_api import ConanAPI
 from conan.cli.cli import Cli as ConanCli
 from scikit_build_core.build import (
     build_sdist,
     get_requires_for_build_editable,
     get_requires_for_build_sdist,
@@ -34,23 +39,57 @@
     "prepare_metadata_for_build_wheel",
 ]
 
 from scikit_build_core.settings.sources import SourceChain, TOMLSource
 
 
 @dataclasses.dataclass
+class ConanLocalRecipesSettings:
+    path: str = "."
+    name: Optional[str] = None
+    version: Optional[str] = None
+
+
+@dataclasses.dataclass
 class ConanSettings:
     path: str = "."
     build: str = "missing"
     profile: Optional[str] = None
     options: List[str] = dataclasses.field(default_factory=list)
     settings: List[str] = dataclasses.field(default_factory=list)
     config: List[str] = dataclasses.field(default_factory=list)
     generator: Optional[str] = None
     output_folder: Optional[str] = None
+    local_recipes: List[ConanLocalRecipesSettings] = dataclasses.field(default_factory=list)
+
+
+def detect_profile():
+    f = io.StringIO()
+    conan_api = ConanAPI()
+    conan_cli = ConanCli(conan_api)
+    with redirect_stdout(f):
+        conan_cli.run(["profile", "list", "--format=json"])
+    profiles: list[str] = json.loads(f.getvalue())
+    if "default" not in profiles:
+        conan_cli.run(["profile", "detect"])
+
+
+def conan_export_local_recipes(settings: ConanLocalRecipesSettings) -> None:
+    path = os.path.abspath(settings.path)
+    cmd = ["export", f"{path}"]
+
+    if settings.name:
+        cmd += ["--name", settings.name]
+
+    if settings.version:
+        cmd += ["--version", settings.version]
+
+    conan_api = ConanAPI()
+    conan_cli = ConanCli(conan_api)
+    conan_cli.run(cmd)
 
 
 def conan_install(settings: ConanSettings, build_type: str) -> dict:
     path = Path(settings.path).absolute()
 
     # Use a tmp folder for conanfile to avoid modifying the existing CMakeUserPresets.json
     with tempfile.TemporaryDirectory() as tmp:
@@ -92,38 +131,47 @@
             conan_cli.run(cmd)
         out = f.getvalue()
         data = json.loads(out)
         return data["graph"]["nodes"]["0"]
 
 
 def _build_wheel_impl(
-        wheel_directory: str,
-        config_settings: dict[str, list[str] | str] | None = None,
-        metadata_directory: str | None = None,
-        *,
-        editable: bool,
+    wheel_directory: str,
+    config_settings: dict[str, list[str] | str] | None = None,
+    metadata_directory: str | None = None,
+    *,
+    editable: bool,
 ) -> str:
     # Load settings for scikit-build
     skbuild_settings = SettingsReader.from_file("pyproject.toml").settings
     build_type = skbuild_settings.cmake.build_type
 
     # Load settings for scikit-build-core-conan
     prefixes = ["tool", "scikit-build-core-conan"]
     with Path("pyproject.toml").open("rb") as f:
         pyproject = tomllib.load(f)
         pyproject = copy.deepcopy(pyproject)
 
-    process_overides(pyproject.get("tool", {}).get("scikit-build-core-conan", {}), "editable" if editable else "wheel",
-                     None)
+    process_overides(
+        pyproject.get("tool", {}).get("scikit-build-core-conan", {}), "editable" if editable else "wheel", None
+    )
     # noinspection PyTypeChecker
     conan_settings = SourceChain(
         TOMLSource(*prefixes, settings=pyproject),
         prefixes=prefixes,
     ).convert_target(ConanSettings)
 
+    # Detect conan profile if one is not specified
+    if not conan_settings.profile:
+        detect_profile()
+
+    # Export local dependencies
+    for recipe in conan_settings.local_recipes:
+        conan_export_local_recipes(recipe)
+
     # Use a tmp folder for the toolchain file
     with tempfile.TemporaryDirectory() as tmp:
         if conan_settings.output_folder is None:
             conan_settings.output_folder = tmp
 
         # Install the C++ dependencies
         result = conan_install(conan_settings, build_type)
@@ -147,20 +195,20 @@
         if not editable:
             return scikit_build_core.build.build_wheel(wheel_directory, config_settings, metadata_directory)
         else:
             return scikit_build_core.build.build_editable(wheel_directory, config_settings, metadata_directory)
 
 
 def build_wheel(
-        wheel_directory: str,
-        config_settings: dict[str, list[str] | str] | None = None,
-        metadata_directory: str | None = None,
+    wheel_directory: str,
+    config_settings: dict[str, list[str] | str] | None = None,
+    metadata_directory: str | None = None,
 ) -> str:
     return _build_wheel_impl(wheel_directory, config_settings, metadata_directory, editable=False)
 
 
 def build_editable(
-        wheel_directory: str,
-        config_settings: dict[str, list[str] | str] | None = None,
-        metadata_directory: str | None = None,
+    wheel_directory: str,
+    config_settings: dict[str, list[str] | str] | None = None,
+    metadata_directory: str | None = None,
 ) -> str:
     return _build_wheel_impl(wheel_directory, config_settings, metadata_directory, editable=True)
```

### Comparing `scikit_build_core_conan-0.1.0/.gitignore` & `scikit_build_core_conan-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_build_core_conan-0.1.0/LICENSE` & `scikit_build_core_conan-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core_conan-0.1.0/README.md` & `scikit_build_core_conan-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -36,22 +36,32 @@
 the `pyproject.toml` file. They can also be passed via `-C/--config-setting` in build or `-C/--config-settings`
 in `pip`. Below are the supported configuration options:
 
 ```toml
 [tool.scikit-build-core-conan]
 path = "."
 build = "missing"
-profile = "/path/to/profile"
+profile = "default"
 options = []
 settings = []
 config = []
 generator = "Ninja"
 output_folder = "build"
 ```
 
+### Local recipes
+
+Sometimes you may want to consume a local recipe rather than from the conan centre index. You can do this like this:
+```toml
+[[tool.scikit-build-core-conan.local-recipes]]
+path = "path/to/recipe"
+name = "recipe"   # optional: package name if not specified in conanfile
+version = "0.0.1" # optional: package version if not specified in conanfile
+```
+
 ### Overrides
 
 `scikit-build-core-conan` uses the same override system as `scikit-build-core`. For more details, check out the
 [documentation](https://scikit-build-core.readthedocs.io/en/latest/configuration.html#overrides) of `scikit-build-core`.
 
 For example:
```

### Comparing `scikit_build_core_conan-0.1.0/pyproject.toml` & `scikit_build_core_conan-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scikit-build-core-conan"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name = "Zhengyu Wu", email = "zhengyu.wu21@imperial.ac.uk" },
 ]
 description = "A conan plugin for scikit-build-core"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -29,13 +29,14 @@
     "Programming Language :: Python :: 3.12",
     "Development Status :: 3 - Alpha",
     "Typing :: Typed",
 ]
 
 dependencies = [
     "scikit-build-core >= 0.9.0",
-    "conan >= 2.0.0"
+    "conan >= 2.0.0",
+    "tomli; python_version < '3.11'",
 ]
 
 [project.urls]
 Homepage = "https://github.com/wu-vincent/scikit-build-core-conan"
 Issues = "https://github.com/wu-vincent/scikit-build-core-conan/issues"
```

### Comparing `scikit_build_core_conan-0.1.0/PKG-INFO` & `scikit_build_core_conan-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scikit-build-core-conan
-Version: 0.1.0
+Version: 0.2.0
 Summary: A conan plugin for scikit-build-core
 Project-URL: Homepage, https://github.com/wu-vincent/scikit-build-core-conan
 Project-URL: Issues, https://github.com/wu-vincent/scikit-build-core-conan/issues
 Author-email: Zhengyu Wu <zhengyu.wu21@imperial.ac.uk>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: conan>=2.0.0
 Requires-Dist: scikit-build-core>=0.9.0
+Requires-Dist: tomli; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # scikit-build-core-conan
 
 A conan plugin for scikit-build-core
 
 > [!NOTE]
@@ -66,22 +67,32 @@
 the `pyproject.toml` file. They can also be passed via `-C/--config-setting` in build or `-C/--config-settings`
 in `pip`. Below are the supported configuration options:
 
 ```toml
 [tool.scikit-build-core-conan]
 path = "."
 build = "missing"
-profile = "/path/to/profile"
+profile = "default"
 options = []
 settings = []
 config = []
 generator = "Ninja"
 output_folder = "build"
 ```
 
+### Local recipes
+
+Sometimes you may want to consume a local recipe rather than from the conan centre index. You can do this like this:
+```toml
+[[tool.scikit-build-core-conan.local-recipes]]
+path = "path/to/recipe"
+name = "recipe"   # optional: package name if not specified in conanfile
+version = "0.0.1" # optional: package version if not specified in conanfile
+```
+
 ### Overrides
 
 `scikit-build-core-conan` uses the same override system as `scikit-build-core`. For more details, check out the
 [documentation](https://scikit-build-core.readthedocs.io/en/latest/configuration.html#overrides) of `scikit-build-core`.
 
 For example:
```

