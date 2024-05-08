# Comparing `tmp/changelog_gen-0.9.8.tar.gz` & `tmp/changelog_gen-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelog_gen-0.9.8.tar", max compression
+gzip compressed data, was "changelog_gen-0.9.9.tar", max compression
```

## Comparing `changelog_gen-0.9.8.tar` & `changelog_gen-0.9.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11307 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/LICENSE
--rw-r--r--   0        0        0    12368 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/README.md
--rw-r--r--   0        0        0        0 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/changelog_gen/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/changelog_gen/cli/__init__.py
--rw-r--r--   0        0        0    11459 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/changelog_gen/cli/command.py
--rw-r--r--   0        0        0      551 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/changelog_gen/cli/util.py
--rw-r--r--   0        0        0    12529 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/changelog_gen/config.py
--rw-r--r--   0        0        0      528 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/changelog_gen/errors.py
--rw-r--r--   0        0        0     8569 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/changelog_gen/extractor.py
--rw-r--r--   0        0        0     2898 2024-04-12 14:27:32.183276 changelog_gen-0.9.8/changelog_gen/post_processor.py
--rw-r--r--   0        0        0     6013 2024-04-12 14:27:32.183276 changelog_gen-0.9.8/changelog_gen/vcs.py
--rw-r--r--   0        0        0     4366 2024-04-12 14:27:32.183276 changelog_gen-0.9.8/changelog_gen/version.py
--rw-r--r--   0        0        0     7316 2024-04-12 14:27:32.183276 changelog_gen-0.9.8/changelog_gen/writer.py
--rw-r--r--   0        0        0     2846 2024-04-12 14:27:32.183276 changelog_gen-0.9.8/pyproject.toml
--rw-r--r--   0        0        0    13402 1970-01-01 00:00:00.000000 changelog_gen-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    11307 2024-04-18 14:30:45.273800 changelog_gen-0.9.9/LICENSE
+-rw-r--r--   0        0        0    11532 2024-04-18 14:30:45.273800 changelog_gen-0.9.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 14:30:45.273800 changelog_gen-0.9.9/changelog_gen/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:30:45.273800 changelog_gen-0.9.9/changelog_gen/cli/__init__.py
+-rw-r--r--   0        0        0    11972 2024-04-18 14:30:45.273800 changelog_gen-0.9.9/changelog_gen/cli/command.py
+-rw-r--r--   0        0        0      551 2024-04-18 14:30:45.273800 changelog_gen-0.9.9/changelog_gen/cli/util.py
+-rw-r--r--   0        0        0    12943 2024-04-18 14:30:45.273800 changelog_gen-0.9.9/changelog_gen/config.py
+-rw-r--r--   0        0        0      528 2024-04-18 14:30:45.273800 changelog_gen-0.9.9/changelog_gen/errors.py
+-rw-r--r--   0        0        0     8569 2024-04-18 14:30:45.273800 changelog_gen-0.9.9/changelog_gen/extractor.py
+-rw-r--r--   0        0        0     2898 2024-04-18 14:30:45.273800 changelog_gen-0.9.9/changelog_gen/post_processor.py
+-rw-r--r--   0        0        0     6013 2024-04-18 14:30:45.273800 changelog_gen-0.9.9/changelog_gen/vcs.py
+-rw-r--r--   0        0        0     4366 2024-04-18 14:30:45.273800 changelog_gen-0.9.9/changelog_gen/version.py
+-rw-r--r--   0        0        0     7316 2024-04-18 14:30:45.273800 changelog_gen-0.9.9/changelog_gen/writer.py
+-rw-r--r--   0        0        0     2847 2024-04-18 14:30:45.273800 changelog_gen-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0    12566 1970-01-01 00:00:00.000000 changelog_gen-0.9.9/PKG-INFO
```

### Comparing `changelog_gen-0.9.8/LICENSE` & `changelog_gen-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.8/README.md` & `changelog_gen-0.9.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Changelog Generator - v0.9.8
+# Changelog Generator - v0.9.9
 [![image](https://img.shields.io/pypi/v/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 [![image](https://img.shields.io/pypi/l/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 [![image](https://img.shields.io/pypi/pyversions/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 ![style](https://github.com/NRWLDev/changelog-gen/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/changelog-gen/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/changelog-gen/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/changelog-gen)
 
@@ -277,60 +277,39 @@
   "main",
   "develop",
 ]
 ```
 
 #### `commit_types = `
   _**[optional]**_<br />
-  **default**: { <br />
-      "feat": { <br />
-        "header": "Features and Improvements", <br />
-        "semver": "minor",
-      }<br />
-      "fix": {<br />
-        "header": "Bug fixes", <br />
-        "semver": "patch",<br />
-      },<br />
-      "docs": {<br />
-        "header": "Documentation", <br />
-        "semver": "patch",<br />
-      },<br />
-      "bug": {<br />
-        "header": "Bug fixes", <br />
-        "semver": "patch",<br />
-      },<br />
-      "chore": {<br />
-        "header": "Miscellaneous", <br />
-        "semver": "patch",<br />
-      },<br />
-      "ci": {<br />
-        "header": "Miscellaneous", <br />
-        "semver": "patch",<br />
-      },<br />
-      "perf": {<br />
-        "header": "Miscellaneous", <br />
-        "semver": "patch",<br />
-      },<br />
-      "refactor": {<br />
-        "header": "Miscellaneous", <br />
-        "semver": "patch",<br />
-      },<br />
-      "revert": {<br />
-        "header": "Miscellaneous", <br />
-        "semver": "patch",<br />
-      },<br />
-      "style": {<br />
-        "header": "Miscellaneous", <br />
-        "semver": "patch",<br />
-      },<br />
-      "test": {<br />
-        "header": "Miscellaneous", <br />
-        "semver": "patch",<br />
-      },<br />
-  }
+  **default**:
+  ```toml
+feat.header = "Features and Improvements"
+feat.semver = "minor"
+fix.header = "Bug fixes"
+fix.semver = "patch"
+docs.header = "Documentation"
+docs.semver = "patch"
+bug.header = "Bug fixes"
+bug.semver = "patch"
+chore.header = "Miscellaneous"
+chore.semver = "patch"
+ci.header = "Miscellaneous"
+ci.semver = "patch"
+perf.header = "Miscellaneous"
+perf.semver = "patch"
+refactor.header = "Miscellaneous"
+refactor.semver = "patch"
+revert.header = "Miscellaneous"
+revert.semver = "patch"
+style.header = "Miscellaneous"
+style.semver = "patch"
+test.header = "Miscellaneous"
+test.semver = "patch"
+  ```
 
   Define commit types and which headers and semver in the changelog they should map to, default semver is `patch`.
 
   Example:
 
 ```toml
 [tool.changelog_gen.commit_types]
@@ -341,20 +320,21 @@
 remove.semver = "minor"
 fix.header = "Bugfixes"
 ```
 
 #### `sections =`
   _**[Deprecated]**_<br />
   _**[optional]**_<br />
-  **default**: { <br />
-      "feat": "Features and Improvements", <br />
-      "fix": "Bug fixes", <br />
-      "docs": "Documentation", <br />
-      "misc": "Miscellaneous", <br />
-  }
+  **default**:
+  ```toml
+feat = "Features and Improvements"
+fix = "Bug fixes"
+docs = "Documentation"
+misc = "Miscellaneous"
+  ```
 
   Define custom headers or new sections/headers, new sections will require a
   matching section_mapping configuration.
 
   This configuration has been deprecated, use `commit_types` instead.
 
   Example:
@@ -366,25 +346,26 @@
 remove = "Removals"
 fix = "Bugfixes"
 ```
 
 #### `section_mapping =`
   _**[Deprecated]**_<br />
   _**[optional]**_<br />
-  **default**: { <br />
-      "bug": "fix", <br />
-      "chore": "misc", <br />
-      "ci": "misc", <br />
-      "docs": "docs", <br />
-      "perf": "misc", <br />
-      "refactor": "misc", <br />
-      "revert": "misc", <br />
-      "style": "misc", <br />
-      "test": "misc", <br />
-  }
+  **default**:
+  ```toml
+bug = "fix"
+chore = "misc"
+ci = "misc"
+docs = "docs"
+perf = "misc"
+refactor = "misc"
+revert = "misc"
+style = "misc"
+test = "misc"
+  ```
 
   Configure additional supported commit types to supported changelog sections.
 
   This configuration has been deprecated, use `commit_types` instead.
 
   Example:
```

### Comparing `changelog_gen-0.9.8/changelog_gen/cli/command.py` & `changelog_gen-0.9.9/changelog_gen/cli/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
 
 import contextlib
 import importlib.metadata
 import json
 import logging
 import logging.config
+import platform
 import shlex
 import subprocess
 from datetime import datetime, timezone
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Optional
 from warnings import warn
 
 import click
 import rtoml
 import typer
+from pygments import formatters, highlight, lexers
 from rich.logging import RichHandler
 
 from changelog_gen import (
     config,
     errors,
     extractor,
     writer,
@@ -37,14 +39,15 @@
     1: logging.WARNING,
     2: logging.INFO,
     3: logging.DEBUG,
 }
 
 tempfile_prefix = "_tmp_changelog"
 
+
 def setup_logging(verbose: int = 0) -> None:
     """Configure the logging."""
     logging.basicConfig(
         level=VERBOSITY.get(verbose, logging.DEBUG),
         format="%(message)s",
         datefmt="[%X]",
         handlers=[
@@ -94,32 +97,45 @@
 
     if info["dirty"] and not cfg.allow_dirty:
         logger.error("Working directory is not clean. Use `allow_dirty` configuration to ignore.")
         raise typer.Exit(code=1)
 
     if info["missing_local"] and not cfg.allow_missing:
         logger.error(
-            "Current local branch is missing commits from remote %s. Use `allow_missing` configuration to ignore.",
+            "Current local branch is missing commits from remote %s.\nUse `allow_missing` configuration to ignore.",
             info["branch"],
         )
         raise typer.Exit(code=1)
 
     if info["missing_remote"] and not cfg.allow_missing:
         logger.error(
-            "Current remote branch is missing commits from local %s. Use `allow_missing` configuration to ignore.",
+            "Current remote branch is missing commits from local %s.\nUse `allow_missing` configuration to ignore.",
             info["branch"],
         )
         raise typer.Exit(code=1)
 
     allowed_branches = cfg.allowed_branches
     if allowed_branches and info["branch"] not in allowed_branches:
         logger.error("Current branch not in allowed generation branches.")
         raise typer.Exit(code=1)
 
 
+@app.command("config")
+def display_config() -> None:
+    """Display current configuration."""
+    cfg = config.read()
+    typer.echo(
+        highlight(
+            rtoml.dumps(cfg.to_dict(), pretty=True),
+            lexers.TOMLLexer(),
+            formatters.TerminalFormatter(),
+        ),
+    )
+
+
 @init_app.command("changelog-init")
 @app.command("init")
 def init(
     ctx: typer.Context,
     file_format: writer.Extension = typer.Option("md", help="File format to generate."),
     verbose: int = typer.Option(0, "-v", "--verbose", help="Set output verbosity.", count=True, max=3),
 ) -> None:
@@ -213,14 +229,18 @@
         reject_empty=reject_empty,
         date_format=date_format,
         post_process_url=post_process_url,
         post_process_auth_env=post_process_auth_env,
         verbose=verbose,
     )
 
+    if platform.system() == "Windows" and interactive:
+        logger.debug("Disabling interactive on windows.")
+        interactive = False
+
     try:
         _gen(cfg, version_part, version_tag, dry_run=dry_run, interactive=interactive)
     except errors.ChangelogException as ex:
         logger.error("%s", ex)  # noqa: TRY400
         raise typer.Exit(code=1) from ex
```

### Comparing `changelog_gen-0.9.8/changelog_gen/cli/util.py` & `changelog_gen-0.9.9/changelog_gen/cli/util.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.8/changelog_gen/config.py` & `changelog_gen-0.9.9/changelog_gen/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,17 +209,22 @@
 
     @classmethod
     def from_dict(cls: type[Config], data: dict) -> Config:
         """Convert a dictionary of key value pairs into a Config object."""
         if "commit_types" in data:
             for k, v in data["commit_types"].items():
                 value = json.loads(v) if isinstance(v, str) else v
-                data["commit_types"][k] = CommitType(**value)
+                ct = CommitType(**value) if isinstance(value, dict) else value
+                data["commit_types"][k] = ct
         return cls(**data)
 
+    def to_dict(self: Config) -> dict:
+        """Convert a Config object to a dictionary of key value pairs."""
+        return dataclasses.asdict(self)
+
 
 def _process_overrides(overrides: dict) -> tuple[dict, PostProcessConfig | None]:
     """Process provided overrides.
 
     Remove any unsupplied values (None).
     """
     post_process_url = overrides.pop("post_process_url", "")
@@ -241,14 +246,17 @@
     cfg = {}
     with pyproject.open() as f:
         data = rtoml.load(f)
 
         if "tool" not in data or "changelog_gen" not in data["tool"]:
             return cfg
 
+        commit_types = SUPPORTED_TYPES.copy()
+        commit_types.update(data["tool"]["changelog_gen"].get("commit_types", {}))
+        data["tool"]["changelog_gen"]["commit_types"] = commit_types
         return data["tool"]["changelog_gen"]
 
 
 def _process_setup_cfg(setup: Path) -> dict:
     cfg = {}
     parser = ConfigParser("")
```

### Comparing `changelog_gen-0.9.8/changelog_gen/errors.py` & `changelog_gen-0.9.9/changelog_gen/errors.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.8/changelog_gen/extractor.py` & `changelog_gen-0.9.9/changelog_gen/extractor.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.8/changelog_gen/post_processor.py` & `changelog_gen-0.9.9/changelog_gen/post_processor.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.8/changelog_gen/vcs.py` & `changelog_gen-0.9.9/changelog_gen/vcs.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.8/changelog_gen/version.py` & `changelog_gen-0.9.9/changelog_gen/version.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.8/changelog_gen/writer.py` & `changelog_gen-0.9.9/changelog_gen/writer.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.8/pyproject.toml` & `changelog_gen-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "changelog_gen"
-version = "0.9.8"
+version = "0.9.9"
 description = "Changelog generation tool"
 authors = ["Daniel Edgecombe <edgy.edgemond@gmail.com>"]
 license = "Apache-2.0"
 repository="https://github.com/EdgyEdgemond/changelog-gen/"
 homepage="https://github.com/EdgyEdgemond/changelog-gen/"
 readme = "README.md"
 
@@ -33,15 +33,15 @@
 pytest-git = "^1.7.0"
 
 # Style
 ruff = "^0.3.0"
 pre-commit = "^3.0.2"
 
 [tool.bumpversion]
-current_version = "0.9.8"
+current_version = "0.9.9"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "README.md"
 
 [[tool.bumpversion.files]]
@@ -56,14 +56,15 @@
 allowed_branches = [
     "main",
 ]
 date_format = "- %Y-%m-%d"
 issue_link = "https://github.com/EdgyEdgemond/changelog-gen/issues/::issue_ref::"
 commit_link = "https://github.com/EdgyEdgemond/changelog-gen/commit/::commit_hash::"
 
+
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = [
     "--random-order",
     "-p no:logging",
 ]
 filterwarnings = [
```

### Comparing `changelog_gen-0.9.8/PKG-INFO` & `changelog_gen-0.9.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog_gen
-Version: 0.9.8
+Version: 0.9.9
 Summary: Changelog generation tool
 Home-page: https://github.com/EdgyEdgemond/changelog-gen/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: edgy.edgemond@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,15 +20,15 @@
 Requires-Dist: httpx (>=0.25,<0.26)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: rtoml (>=0.9)
 Requires-Dist: typer (>=0,<1)
 Project-URL: Repository, https://github.com/EdgyEdgemond/changelog-gen/
 Description-Content-Type: text/markdown
 
-# Changelog Generator - v0.9.8
+# Changelog Generator - v0.9.9
 [![image](https://img.shields.io/pypi/v/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 [![image](https://img.shields.io/pypi/l/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 [![image](https://img.shields.io/pypi/pyversions/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 ![style](https://github.com/NRWLDev/changelog-gen/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/changelog-gen/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/changelog-gen/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/changelog-gen)
 
@@ -303,60 +303,39 @@
   "main",
   "develop",
 ]
 ```
 
 #### `commit_types = `
   _**[optional]**_<br />
-  **default**: { <br />
-      "feat": { <br />
-        "header": "Features and Improvements", <br />
-        "semver": "minor",
-      }<br />
-      "fix": {<br />
-        "header": "Bug fixes", <br />
-        "semver": "patch",<br />
-      },<br />
-      "docs": {<br />
-        "header": "Documentation", <br />
-        "semver": "patch",<br />
-      },<br />
-      "bug": {<br />
-        "header": "Bug fixes", <br />
-        "semver": "patch",<br />
-      },<br />
-      "chore": {<br />
-        "header": "Miscellaneous", <br />
-        "semver": "patch",<br />
-      },<br />
-      "ci": {<br />
-        "header": "Miscellaneous", <br />
-        "semver": "patch",<br />
-      },<br />
-      "perf": {<br />
-        "header": "Miscellaneous", <br />
-        "semver": "patch",<br />
-      },<br />
-      "refactor": {<br />
-        "header": "Miscellaneous", <br />
-        "semver": "patch",<br />
-      },<br />
-      "revert": {<br />
-        "header": "Miscellaneous", <br />
-        "semver": "patch",<br />
-      },<br />
-      "style": {<br />
-        "header": "Miscellaneous", <br />
-        "semver": "patch",<br />
-      },<br />
-      "test": {<br />
-        "header": "Miscellaneous", <br />
-        "semver": "patch",<br />
-      },<br />
-  }
+  **default**:
+  ```toml
+feat.header = "Features and Improvements"
+feat.semver = "minor"
+fix.header = "Bug fixes"
+fix.semver = "patch"
+docs.header = "Documentation"
+docs.semver = "patch"
+bug.header = "Bug fixes"
+bug.semver = "patch"
+chore.header = "Miscellaneous"
+chore.semver = "patch"
+ci.header = "Miscellaneous"
+ci.semver = "patch"
+perf.header = "Miscellaneous"
+perf.semver = "patch"
+refactor.header = "Miscellaneous"
+refactor.semver = "patch"
+revert.header = "Miscellaneous"
+revert.semver = "patch"
+style.header = "Miscellaneous"
+style.semver = "patch"
+test.header = "Miscellaneous"
+test.semver = "patch"
+  ```
 
   Define commit types and which headers and semver in the changelog they should map to, default semver is `patch`.
 
   Example:
 
 ```toml
 [tool.changelog_gen.commit_types]
@@ -367,20 +346,21 @@
 remove.semver = "minor"
 fix.header = "Bugfixes"
 ```
 
 #### `sections =`
   _**[Deprecated]**_<br />
   _**[optional]**_<br />
-  **default**: { <br />
-      "feat": "Features and Improvements", <br />
-      "fix": "Bug fixes", <br />
-      "docs": "Documentation", <br />
-      "misc": "Miscellaneous", <br />
-  }
+  **default**:
+  ```toml
+feat = "Features and Improvements"
+fix = "Bug fixes"
+docs = "Documentation"
+misc = "Miscellaneous"
+  ```
 
   Define custom headers or new sections/headers, new sections will require a
   matching section_mapping configuration.
 
   This configuration has been deprecated, use `commit_types` instead.
 
   Example:
@@ -392,25 +372,26 @@
 remove = "Removals"
 fix = "Bugfixes"
 ```
 
 #### `section_mapping =`
   _**[Deprecated]**_<br />
   _**[optional]**_<br />
-  **default**: { <br />
-      "bug": "fix", <br />
-      "chore": "misc", <br />
-      "ci": "misc", <br />
-      "docs": "docs", <br />
-      "perf": "misc", <br />
-      "refactor": "misc", <br />
-      "revert": "misc", <br />
-      "style": "misc", <br />
-      "test": "misc", <br />
-  }
+  **default**:
+  ```toml
+bug = "fix"
+chore = "misc"
+ci = "misc"
+docs = "docs"
+perf = "misc"
+refactor = "misc"
+revert = "misc"
+style = "misc"
+test = "misc"
+  ```
 
   Configure additional supported commit types to supported changelog sections.
 
   This configuration has been deprecated, use `commit_types` instead.
 
   Example:
```

