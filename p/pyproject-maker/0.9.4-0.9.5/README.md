# Comparing `tmp/pyproject_maker-0.9.4.tar.gz` & `tmp/pyproject_maker-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_maker-0.9.4.tar", max compression
+gzip compressed data, was "pyproject_maker-0.9.5.tar", max compression
```

## Comparing `pyproject_maker-0.9.4.tar` & `pyproject_maker-0.9.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1069 2023-06-30 11:14:30.586362 pyproject_maker-0.9.4/LICENSE.txt
--rw-r--r--   0        0        0     8142 2023-10-29 18:06:17.569529 pyproject_maker-0.9.4/README.md
--rw-r--r--   0        0        0      196 2023-06-30 11:14:30.586362 pyproject_maker-0.9.4/py_maker/__init__.py
--rw-r--r--   0        0        0       13 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/commands/__init__.py
--rw-r--r--   0        0        0      738 2023-10-10 11:31:20.017462 pyproject_maker-0.9.4/py_maker/commands/config.py
--rw-r--r--   0        0        0     2706 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/commands/new.py
--rw-r--r--   0        0        0     5605 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/commands/template.py
--rw-r--r--   0        0        0       78 2023-10-10 11:31:20.017462 pyproject_maker-0.9.4/py_maker/config/__init__.py
--rw-r--r--   0        0        0     5016 2023-11-04 17:04:58.877871 pyproject_maker-0.9.4/py_maker/config/settings.py
--rw-r--r--   0        0        0     1970 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/constants.py
--rw-r--r--   0        0        0      153 2023-10-04 18:08:22.439406 pyproject_maker-0.9.4/py_maker/github_ctrl/__init__.py
--rw-r--r--   0        0        0     2824 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/github_ctrl/main.py
--rw-r--r--   0        0        0     4986 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/helpers.py
--rw-r--r--   0        0        0      555 2023-07-26 09:30:08.132829 pyproject_maker-0.9.4/py_maker/licenses/Apache2.jinja
--rw-r--r--   0        0        0     1273 2023-07-26 09:30:08.132829 pyproject_maker-0.9.4/py_maker/licenses/BSD2.jinja
--rw-r--r--   0        0        0     1466 2023-07-26 09:30:08.132829 pyproject_maker-0.9.4/py_maker/licenses/BSD3.jinja
--rw-r--r--   0        0        0    16380 2023-07-26 09:30:08.136829 pyproject_maker-0.9.4/py_maker/licenses/CDDL.jinja
--rw-r--r--   0        0        0    14197 2023-07-26 09:30:08.136829 pyproject_maker-0.9.4/py_maker/licenses/EPL2.jinja
--rw-r--r--   0        0        0    18092 2023-07-26 09:30:08.136829 pyproject_maker-0.9.4/py_maker/licenses/GPL2.jinja
--rw-r--r--   0        0        0    35149 2023-07-26 09:30:08.136829 pyproject_maker-0.9.4/py_maker/licenses/GPL3.jinja
--rw-r--r--   0        0        0     7652 2023-07-26 09:30:08.136829 pyproject_maker-0.9.4/py_maker/licenses/LGPL.jinja
--rw-r--r--   0        0        0     1079 2023-07-26 09:30:08.136829 pyproject_maker-0.9.4/py_maker/licenses/MIT.jinja
--rw-r--r--   0        0        0    16725 2023-07-26 09:30:08.136829 pyproject_maker-0.9.4/py_maker/licenses/MPL2.jinja
--rw-r--r--   0        0        0      126 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/licenses/__init__.py
--rw-r--r--   0        0        0     1121 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/main.py
--rw-r--r--   0        0        0      162 2023-08-10 16:04:17.271047 pyproject_maker-0.9.4/py_maker/prompt/__init__.py
--rw-r--r--   0        0        0     2332 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/prompt/prompt.py
--rw-r--r--   0        0        0    21018 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/pymaker.py
--rw-r--r--   0        0        0      645 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/schema.py
--rw-r--r--   0        0        0      637 2023-09-13 18:19:56.541956 pyproject_maker-0.9.4/py_maker/template/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2023-09-13 18:19:56.541956 pyproject_maker-0.9.4/py_maker/template/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      275 2023-09-13 18:19:56.541956 pyproject_maker-0.9.4/py_maker/template/.github/dependabot.yml
--rw-r--r--   0        0        0      165 2023-10-29 18:16:26.244520 pyproject_maker-0.9.4/py_maker/template/.github/workflows/linting.yml
--rw-r--r--   0        0        0     4478 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/template/.gitignore
--rw-r--r--   0        0        0       39 2023-07-04 16:47:59.617003 pyproject_maker-0.9.4/py_maker/template/.markdownlint.json
--rw-r--r--   0        0        0     1024 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/template/.pre-commit-config.yaml
--rw-r--r--   0        0        0       66 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/template/CHANGELOG.md
--rw-r--r--   0        0        0     5479 2023-09-13 18:30:41.087988 pyproject_maker-0.9.4/py_maker/template/CODE_OF_CONDUCT.md.jinja
--rw-r--r--   0        0        0      101 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/template/CONTRIBUTING.md
--rw-r--r--   0        0        0     2675 2023-09-23 10:34:58.038760 pyproject_maker-0.9.4/py_maker/template/README.md.jinja
--rw-r--r--   0        0        0      108 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/template/TODO.md
--rw-r--r--   0        0        0      193 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/template/__init__.py
--rw-r--r--   0        0        0      139 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/template/app/__init__.py
--rw-r--r--   0        0        0      634 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/template/app/main.py.jinja
--rw-r--r--   0        0        0     4722 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/template/pyproject.toml.jinja
--rw-r--r--   0        0        0       29 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/template/tests/__init__.py
--rw-r--r--   0        0        0      110 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/tree/__init__.py
--rw-r--r--   0        0        0     2989 2023-10-29 18:06:17.573529 pyproject_maker-0.9.4/py_maker/tree/tree.py
--rw-r--r--   0        0        0     5309 2023-12-11 19:17:26.850102 pyproject_maker-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     9819 1970-01-01 00:00:00.000000 pyproject_maker-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-30 11:14:30.586362 pyproject_maker-0.9.5/LICENSE.txt
+-rw-r--r--   0        0        0     8142 2023-10-29 18:06:17.569529 pyproject_maker-0.9.5/README.md
+-rw-r--r--   0        0        0      196 2023-06-30 11:14:30.586362 pyproject_maker-0.9.5/py_maker/__init__.py
+-rw-r--r--   0        0        0       13 2023-10-29 18:06:17.573529 pyproject_maker-0.9.5/py_maker/commands/__init__.py
+-rw-r--r--   0        0        0      731 2024-03-04 11:45:43.564791 pyproject_maker-0.9.5/py_maker/commands/config.py
+-rw-r--r--   0        0        0     2707 2024-03-04 11:45:40.204812 pyproject_maker-0.9.5/py_maker/commands/new.py
+-rw-r--r--   0        0        0     5606 2024-03-04 11:45:40.204812 pyproject_maker-0.9.5/py_maker/commands/template.py
+-rw-r--r--   0        0        0       79 2024-03-04 11:45:40.204812 pyproject_maker-0.9.5/py_maker/config/__init__.py
+-rw-r--r--   0        0        0     4989 2024-03-04 11:45:43.564791 pyproject_maker-0.9.5/py_maker/config/settings.py
+-rw-r--r--   0        0        0     1990 2024-03-04 11:45:40.204812 pyproject_maker-0.9.5/py_maker/constants.py
+-rw-r--r--   0        0        0      154 2024-03-04 11:45:40.204812 pyproject_maker-0.9.5/py_maker/github_ctrl/__init__.py
+-rw-r--r--   0        0        0     2825 2024-03-04 11:45:40.204812 pyproject_maker-0.9.5/py_maker/github_ctrl/main.py
+-rw-r--r--   0        0        0     5334 2024-03-04 11:45:40.204812 pyproject_maker-0.9.5/py_maker/helpers.py
+-rw-r--r--   0        0        0      555 2023-07-26 09:30:08.132829 pyproject_maker-0.9.5/py_maker/licenses/Apache2.jinja
+-rw-r--r--   0        0        0     1273 2023-07-26 09:30:08.132829 pyproject_maker-0.9.5/py_maker/licenses/BSD2.jinja
+-rw-r--r--   0        0        0     1466 2023-07-26 09:30:08.132829 pyproject_maker-0.9.5/py_maker/licenses/BSD3.jinja
+-rw-r--r--   0        0        0    16380 2023-07-26 09:30:08.136829 pyproject_maker-0.9.5/py_maker/licenses/CDDL.jinja
+-rw-r--r--   0        0        0    14197 2023-07-26 09:30:08.136829 pyproject_maker-0.9.5/py_maker/licenses/EPL2.jinja
+-rw-r--r--   0        0        0    18092 2023-07-26 09:30:08.136829 pyproject_maker-0.9.5/py_maker/licenses/GPL2.jinja
+-rw-r--r--   0        0        0    35149 2023-07-26 09:30:08.136829 pyproject_maker-0.9.5/py_maker/licenses/GPL3.jinja
+-rw-r--r--   0        0        0     7652 2023-07-26 09:30:08.136829 pyproject_maker-0.9.5/py_maker/licenses/LGPL.jinja
+-rw-r--r--   0        0        0     1079 2023-07-26 09:30:08.136829 pyproject_maker-0.9.5/py_maker/licenses/MIT.jinja
+-rw-r--r--   0        0        0    16725 2023-07-26 09:30:08.136829 pyproject_maker-0.9.5/py_maker/licenses/MPL2.jinja
+-rw-r--r--   0        0        0      126 2023-10-29 18:06:17.573529 pyproject_maker-0.9.5/py_maker/licenses/__init__.py
+-rw-r--r--   0        0        0     1247 2024-03-04 11:45:43.564791 pyproject_maker-0.9.5/py_maker/main.py
+-rw-r--r--   0        0        0      163 2024-03-04 11:45:40.204812 pyproject_maker-0.9.5/py_maker/prompt/__init__.py
+-rw-r--r--   0        0        0     2353 2024-03-04 11:45:40.204812 pyproject_maker-0.9.5/py_maker/prompt/prompt.py
+-rw-r--r--   0        0        0    21342 2024-03-04 13:45:11.631341 pyproject_maker-0.9.5/py_maker/pymaker.py
+-rw-r--r--   0        0        0      646 2024-03-04 11:45:40.204812 pyproject_maker-0.9.5/py_maker/schema.py
+-rw-r--r--   0        0        0      637 2023-09-13 18:19:56.541956 pyproject_maker-0.9.5/py_maker/template/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2023-09-13 18:19:56.541956 pyproject_maker-0.9.5/py_maker/template/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      275 2023-09-13 18:19:56.541956 pyproject_maker-0.9.5/py_maker/template/.github/dependabot.yml
+-rw-r--r--   0        0        0      165 2023-10-29 18:16:26.244520 pyproject_maker-0.9.5/py_maker/template/.github/workflows/linting.yml
+-rw-r--r--   0        0        0     4478 2023-10-29 18:06:17.573529 pyproject_maker-0.9.5/py_maker/template/.gitignore
+-rw-r--r--   0        0        0       39 2023-07-04 16:47:59.617003 pyproject_maker-0.9.5/py_maker/template/.markdownlint.json
+-rw-r--r--   0        0        0     1641 2024-03-04 13:32:55.207849 pyproject_maker-0.9.5/py_maker/template/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       66 2023-10-29 18:06:17.573529 pyproject_maker-0.9.5/py_maker/template/CHANGELOG.md
+-rw-r--r--   0        0        0     5479 2023-09-13 18:30:41.087988 pyproject_maker-0.9.5/py_maker/template/CODE_OF_CONDUCT.md.jinja
+-rw-r--r--   0        0        0      101 2023-10-29 18:06:17.573529 pyproject_maker-0.9.5/py_maker/template/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2675 2023-09-23 10:34:58.038760 pyproject_maker-0.9.5/py_maker/template/README.md.jinja
+-rw-r--r--   0        0        0      108 2023-10-29 18:06:17.573529 pyproject_maker-0.9.5/py_maker/template/TODO.md
+-rw-r--r--   0        0        0      193 2023-10-29 18:06:17.573529 pyproject_maker-0.9.5/py_maker/template/__init__.py
+-rw-r--r--   0        0        0      139 2023-10-29 18:06:17.573529 pyproject_maker-0.9.5/py_maker/template/app/__init__.py
+-rw-r--r--   0        0        0      634 2023-10-29 18:06:17.573529 pyproject_maker-0.9.5/py_maker/template/app/main.py.jinja
+-rw-r--r--   0        0        0     5098 2024-03-04 13:32:55.207849 pyproject_maker-0.9.5/py_maker/template/pyproject.toml.jinja
+-rw-r--r--   0        0        0       29 2023-10-29 18:06:17.573529 pyproject_maker-0.9.5/py_maker/template/tests/__init__.py
+-rw-r--r--   0        0        0      111 2024-03-04 11:45:40.204812 pyproject_maker-0.9.5/py_maker/tree/__init__.py
+-rw-r--r--   0        0        0     2990 2024-03-04 11:45:40.204812 pyproject_maker-0.9.5/py_maker/tree/tree.py
+-rw-r--r--   0        0        0     5427 2024-03-04 13:52:00.668838 pyproject_maker-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     9771 1970-01-01 00:00:00.000000 pyproject_maker-0.9.5/PKG-INFO
```

### Comparing `pyproject_maker-0.9.4/LICENSE.txt` & `pyproject_maker-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/README.md` & `pyproject_maker-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/commands/config.py` & `pyproject_maker-0.9.5/py_maker/commands/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Show or change the Configuration."""
+
 import typer
 
 from py_maker.config import settings
 from py_maker.helpers import header, show_table
 
 app = typer.Typer(no_args_is_help=True)
 
@@ -19,15 +20,15 @@
     """Change the current configuration."""
     header()
     settings.change_settings()
 
 
 @app.command()
 def token() -> None:
-    """Change the current configuration."""
+    """Change the current token."""
     header()
     settings.change_token()
 
 
 @app.command(name="edit")
 def edit_config() -> None:
     """Open the Configuration file in the default editor."""
```

### Comparing `pyproject_maker-0.9.4/py_maker/commands/new.py` & `pyproject_maker-0.9.5/py_maker/commands/new.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Create a new project."""
+
 from typing import Annotated, Optional, Union
 
 import typer
 from rich import print  # pylint: disable=W0622
 
 from py_maker.config import settings
 from py_maker.constants import ExitErrors
```

### Comparing `pyproject_maker-0.9.4/py_maker/commands/template.py` & `pyproject_maker-0.9.5/py_maker/commands/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deal with template files."""
+
 import importlib.resources as pkg_resources
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import typer
 from rich import print  # pylint: disable=redefined-builtin
```

### Comparing `pyproject_maker-0.9.4/py_maker/config/settings.py` & `pyproject_maker-0.9.5/py_maker/config/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Control the settings of the project.
 
 Allows reading from a settings file and writing to it.
 """
+
 import os
 import platform
 import subprocess  # nosec
 from typing import Literal, Optional
 
 from rich import print  # pylint: disable=redefined-builtin
 from simple_toml_settings import TOMLSettings
@@ -69,15 +70,15 @@
             default=git_author if missing else self.author_name,
         )
         self.author_email = Prompt.ask(
             "Author Email?",
             default=git_email if missing else self.author_email,
         )
         self.github_username = Prompt.ask(
-            "Github Username? \[optional]",  # noqa: W605 # type: ignore
+            r"Github Username? \[optional]",
             default="" if missing else self.github_username,
         )
         self.default_license = Prompt.ask(
             "Application License?",
             choices=license_names,
             default="MIT" if missing else self.default_license,
         )
```

### Comparing `pyproject_maker-0.9.4/py_maker/constants.py` & `pyproject_maker-0.9.5/py_maker/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Some constants needed for the rest of the App."""
+
 from enum import IntEnum
 
 LICENCES: list[dict[str, str]] = [
     {"name": "None", "url": ""},
     {"name": "Apache2", "url": "https://opensource.org/licenses/Apache-2.0"},
     {"name": "BSD3", "url": "https://opensource.org/licenses/BSD-3-Clause"},
     {"name": "BSD2", "url": "https://opensource.org/licenses/BSD-2-Clause"},
@@ -28,14 +29,15 @@
     DIRECTORY_EXISTS = 2
     GIT_ERROR = 3
     FOLDER_NOT_EMPTY = 4
     PERMISSION_DENIED = 5
     USER_ABORT = 6
     OS_ERROR = 7
     INVALID_ACTION = 8
+    TOML_ERROR = 9
 
 
 MKDOCS_CONFIG = """
 site_name: {name}
 
 # default to using the material theme
 theme:
```

### Comparing `pyproject_maker-0.9.4/py_maker/github_ctrl/main.py` & `pyproject_maker-0.9.5/py_maker/github_ctrl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Define the GitHub class.
 
 This is a class to encapsulate the GitHub API and is responsible for
 authenticating with GitHub and performing the necessary operations.
 """
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional, Union
 
 from github import Auth, Github
 from github.GithubException import GithubException
 from rich import print  # pylint: disable=redefined-builtin
```

### Comparing `pyproject_maker-0.9.4/py_maker/helpers.py` & `pyproject_maker-0.9.5/py_maker/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helpers for the config module."""
+
 from __future__ import annotations
 
 import datetime
 import re
 import shutil
 import sys
 from importlib import metadata, resources
@@ -24,18 +25,25 @@
 SUCCESS_RESPONSE = 200
 
 
 def get_author_and_email_from_git() -> tuple[str, str]:
     """Get the author name and email from git."""
     config = GitConfigParser()
 
-    return (
-        str(config.get_value("user", "name", "")),
-        str(config.get_value("user", "email", "")),
-    )
+    try:
+        author_name = str(config.get_value("user", "name", ""))
+    except KeyError:
+        author_name = ""
+
+    try:
+        author_email = str(config.get_value("user", "email", ""))
+    except KeyError:
+        author_email = ""
+
+    return author_name, author_email
 
 
 def get_file_list(template_dir: Union[Traversable, Path]) -> list[Path]:
     """Return a list of files to be copied to the project directory.
 
     The root __init__.py file is excluded from the list, as it is only there so
     that the template directory can be treated as a package.
@@ -108,15 +116,15 @@
 
     Return True if the package name already exists on PyPI, False otherwise.
     Timeout after 5 seconds, which also returns False.
     """
     url = f"https://pypi.org/pypi/{package_name}/json"
     try:
         response = requests.get(url, timeout=5)
-    except requests.exceptions.Timeout:
+    except (requests.exceptions.Timeout, requests.exceptions.ConnectionError):
         return False
     return response.status_code == SUCCESS_RESPONSE
 
 
 def get_toml_path() -> Path:
     """Return the full path of the pyproject.toml.
 
@@ -141,14 +149,17 @@
         # we are locally developing the package
         try:
             config = rtoml.load(toml_path)
             version: str = config["tool"]["poetry"]["version"]
         except (KeyError, OSError) as exc:
             print(f"Problem getting the Version : {exc}")
             sys.exit(ExitErrors.OS_ERROR)
+        except rtoml.TomlParsingError as exc:
+            print(f"Invalid 'pyproject.toml' file : {exc}")
+            sys.exit(ExitErrors.TOML_ERROR)
         else:
             return version
     else:
         # if we are here then the package must be installed not local dev
         try:
             return metadata.version("pyproject_maker")
         except metadata.PackageNotFoundError as exc:
```

### Comparing `pyproject_maker-0.9.4/py_maker/licenses/Apache2.jinja` & `pyproject_maker-0.9.5/py_maker/licenses/Apache2.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/licenses/BSD2.jinja` & `pyproject_maker-0.9.5/py_maker/licenses/BSD2.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/licenses/BSD3.jinja` & `pyproject_maker-0.9.5/py_maker/licenses/BSD3.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/licenses/CDDL.jinja` & `pyproject_maker-0.9.5/py_maker/licenses/CDDL.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/licenses/EPL2.jinja` & `pyproject_maker-0.9.5/py_maker/licenses/EPL2.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/licenses/GPL2.jinja` & `pyproject_maker-0.9.5/py_maker/licenses/GPL2.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/licenses/GPL3.jinja` & `pyproject_maker-0.9.5/py_maker/licenses/GPL3.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/licenses/LGPL.jinja` & `pyproject_maker-0.9.5/py_maker/licenses/LGPL.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/licenses/MIT.jinja` & `pyproject_maker-0.9.5/py_maker/licenses/MIT.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/licenses/MPL2.jinja` & `pyproject_maker-0.9.5/py_maker/licenses/MPL2.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/main.py` & `pyproject_maker-0.9.5/py_maker/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Main application entry point."""
+
 from typing import Optional
 
 import typer
 from rich import print  # pylint: disable=redefined-builtin
 
 from py_maker.commands import config, new, template
 from py_maker.helpers import get_app_version
@@ -35,9 +36,18 @@
 app.add_typer(
     config.app, name="config", help="Show or change the Configuration."
 )
 app.add_typer(
     template.app, name="template", help="Utilities for handling template files."
 )
 
-if __name__ == "__main__":
+
+def run_app() -> None:
+    """Run the main application.
+
+    Breaking it out like this for testing.
+    """
     app()
+
+
+if __name__ == "__main__":
+    run_app()
```

### Comparing `pyproject_maker-0.9.4/py_maker/prompt/prompt.py` & `pyproject_maker-0.9.5/py_maker/prompt/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Subclass the Prompt class from Rich to add a few features.
 
 I have a PR open to add these features to Rich, but until it is merged (if it is
 merged) I will use this subclass.
 
 Currently only makes the choices case-insensitive.
 """
+
 from typing import Any
 
 from rich.prompt import Confirm as RichConfirm
 from rich.prompt import InvalidResponse, PromptType
 from rich.prompt import Prompt as RichPrompt
 
 
@@ -51,15 +52,15 @@
 
         Returns:
             PromptType: The value to be returned from ask method.
         """
         value = value.strip()
         try:
             return_value: PromptType = self.response_type(value)  # type: ignore
-        except ValueError as exc:
+        except ValueError as exc:  # pragma: no cover
             raise InvalidResponse(self.validate_error_message) from exc
 
         if self.choices is not None:
             if not self.check_choice(value):
                 raise InvalidResponse(self.illegal_choice_message)
 
             # return the original choice, not the lower case version
```

### Comparing `pyproject_maker-0.9.4/py_maker/pymaker.py` & `pyproject_maker-0.9.5/py_maker/pymaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class to encapsulate the application."""
+
 from __future__ import annotations
 
 import importlib.resources as pkg_resources
 import os
 import re
 import shutil
 import subprocess  # nosec
@@ -216,27 +217,33 @@
         """Display steps to be carried out after the project is created.
 
         Currently just prints messages on what to do next.
         """
         proj_loc = (
             self.location if self.location != "." else self.choices.project_dir
         )
+        run_cmd = (
+            f"{self.location}"
+            if not self.choices.standalone
+            else "python main.py"
+        )
+
         output = f"""
 --> [green]Project created successfully.[/green]
 
 [bold]Next steps:[/bold]
 
     1) Change to the project directory:
         'cd {proj_loc}'
     2) Install the dependencies if not done (creates a virtual environment):
         'poetry install'
     3) Activate the virtual environment:
         'poetry shell'
     4) Run the application:
-        '{self.location}'
+        '{run_cmd}'
     5) Code!
 
 See the [bold][green]README.md[/green][/bold] file for more information.
         """
         print(output)
 
     # ------------------------------------------------------------------------ #
@@ -303,26 +310,32 @@
 
         # if this is not a standalone script, ask for more details, useful
         # for PypI uploads.
         if not self.choices.standalone:
             self.choices.package_name = self.get_sanitized_package_name(pk_name)
             self.choices.homepage = Prompt.ask("Homepage URL?", default="")
 
-            github_username = (
-                self.settings.github_username
-                if self.settings.github_username
-                else "<your GitHub username>"
-            )
-            self.choices.repository = Prompt.ask(
-                "Repository URL?",
-                default=(
-                    f"https://github.com/{github_username}/"
-                    f"{re.sub(r'[_.]+', '-', self.choices.package_name)}"
-                ),
-            )
+        # offer to create a repo on GitHub, for both type of projects.
+        github_username = (
+            self.settings.github_username
+            if self.settings.github_username
+            else "<your GitHub username>"
+        )
+        repo_name = (
+            sanitize(self.choices.project_dir.name)
+            if self.choices.package_name == "-"
+            else self.choices.package_name
+        )
+        self.choices.repository = Prompt.ask(
+            "Repository URL?",
+            default=(
+                f"https://github.com/{github_username}/"
+                f"{re.sub(r'[_.]+', '-', repo_name.lower())}"
+            ),
+        )
 
         self.choices.description = Prompt.ask(
             "Description of the Application?",
         )
         self.choices.author = Prompt.ask(
             "Author Name?", default=self.settings.author_name
         )
```

### Comparing `pyproject_maker-0.9.4/py_maker/schema.py` & `pyproject_maker-0.9.5/py_maker/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define some Pydantic schemas for the application."""
+
 from pathlib import Path
 from typing import Optional
 
 from pydantic import BaseModel
 
 
 class ProjectSettings(BaseModel):
```

### Comparing `pyproject_maker-0.9.4/py_maker/template/.github/ISSUE_TEMPLATE/bug_report.md` & `pyproject_maker-0.9.5/py_maker/template/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/template/.github/ISSUE_TEMPLATE/feature_request.md` & `pyproject_maker-0.9.5/py_maker/template/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/template/.gitignore` & `pyproject_maker-0.9.5/py_maker/template/.gitignore`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/template/.pre-commit-config.yaml` & `pyproject_maker-0.9.5/py_maker/template/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -8,35 +8,60 @@
         args: [--unsafe]
       - id: trailing-whitespace
       - id: check-toml
       - id: check-merge-conflict
       - id: end-of-file-fixer
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.2
+    rev: v0.3.0
     hooks:
       - id: ruff
       - id: ruff-format
 
   - repo: https://github.com/jackdewinter/pymarkdown
-    rev: v0.9.13.4
+    rev: v0.9.17
     hooks:
       - id: pymarkdown
         exclude: .github/|CHANGELOG
         args: [-d, "MD046", scan]
 
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: "v1.8.0"
+    hooks:
+      - id: mypy
+        name: "run mypy"
+        additional_dependencies:
+          - "types-requests"
+
   - repo: https://github.com/python-poetry/poetry
-    rev: "1.6.1"
+    rev: "1.8.0"
     hooks:
       - id: poetry-check
       # - id: poetry-lock
+
+  - repo: https://github.com/python-poetry/poetry-plugin-export
+    rev: "1.6.0"
+    hooks:
       - id: poetry-export
+        name: "export production dependencies"
         args:
           [
             "--without-hashes",
             "-f",
             "requirements.txt",
             "-o",
             "requirements.txt",
+            "--without",
+            "dev",
+          ]
+      - id: poetry-export
+        name: "export development dependencies"
+        args:
+          [
+            "--without-hashes",
+            "-f",
+            "requirements.txt",
+            "-o",
+            "requirements-dev.txt",
             "--with",
             "dev",
           ]
```

### Comparing `pyproject_maker-0.9.4/py_maker/template/CODE_OF_CONDUCT.md.jinja` & `pyproject_maker-0.9.5/py_maker/template/CODE_OF_CONDUCT.md.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/template/README.md.jinja` & `pyproject_maker-0.9.5/py_maker/template/README.md.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/template/app/main.py.jinja` & `pyproject_maker-0.9.5/py_maker/template/app/main.py.jinja`

 * *Files identical despite different names*

### Comparing `pyproject_maker-0.9.4/py_maker/template/pyproject.toml.jinja` & `pyproject_maker-0.9.5/py_maker/template/pyproject.toml.jinja`

 * *Files 17% similar despite different names*

```diff
@@ -19,151 +19,180 @@
 "Bug Tracker" = "{{ repository }}/issues"
 "Changelog" = "{{ repository }}/blob/main/CHANGELOG.md"
 
 [tool.poetry.scripts]
 # rename "{{ slug }}" below to change the executable name. You can also
 # add more scripts if your package offers multiple commands.
 {{ slug }} = "{{ package_name }}.main:app"
+
+{% else%}
+package-mode = false
+
 {% endif %}
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Configure dev dependencies you can add or remove as needed
 [tool.poetry.group.dev.dependencies]
 {% if options.lint %}
 # linting, type-checking and security checks
-mypy = "^1.4.1"
-pre-commit = "^3.3.3"
+mypy = "^1.8.0"
+pre-commit = "^3.6.2"
 pymarkdownlnt = "^0.9.12"
-ruff = "^0.1.3"
+ruff = "^0.3.0"
 {% endif %}
 
 # task runner
-poethepoet = "^0.24.0"
+poethepoet = "^0.25.0"
 
 {% if options.test %}
 # testing
-pytest = "^7.4.0"
-pytest-cov = "^4.0.0"
-pytest-xdist = "^3.2.1"
-pytest-sugar = "^0.9.7"
-pytest-randomly = "^3.13.0"
+pytest = "^8.1.0"
+pytest-cov = "^4.1.0"
+pytest-xdist = "^3.5.0"
+pytest-sugar = ">=1.0.0"
+pytest-randomly = "^3.15.0"
 pytest-reverse = "^1.7.0"
-pytest-asyncio = "^0.21.1"
-pytest-mock = "^3.11.1"
+pytest-mock = "^3.12.0"
 mock = "^5.1.0"
-faker = "^19.2.0"
-pyfakefs = "^5.2.4"
+faker = ">=23.3.0"
+pyfakefs = "^5.3.5"
 {% endif %}
 
 {% if options.docs %}
 # documentation
-github-changelog-md = "^0.3.0"
-mkdocs = "^1.4.3"
-mkdocs-autorefs = "^0.5.0"
-mkdocs-material = "^9.1.19"
-mkdocs-minify-plugin = "^0.7.0"
-mkdocstrings = ">=0.22,<0.24"
-pymdown-extensions = "^10.1"
-pygments = "^2.15.1"
+github-changelog-md = "^0.9.1"
+mkdocs = "^1.5.3"
+mkdocs-autorefs = ">=1.0.1"
+mkdocs-material = "^9.5.12"
+mkdocs-git-revision-date-localized-plugin = "^1.2.4"
+mkdocs-latest-git-tag-plugin = "^0.1.2"
+mkdocs-minify-plugin = ">=0.8.0"
+mkdocstrings = ">=0.24.1"
+pymdown-extensions = "^10.7"
+pygments = "^2.17.2"
 {% endif %}
 
 # setup PoeThePoet tasks
 [tool.poe.tasks]
 pre.cmd = "pre-commit run --all-files"
 pre.help = "Run pre-commit checks"
 {% if options.lint %}
 mypy.cmd = "mypy py_maker/**/*.py tests/**/*.py --strict"
 mypy.help = "Run mypy checks"
 format.cmd = "ruff format ."
 format.help = "Format code with Ruff"
 ruff.cmd = "ruff check ."
 ruff.help = "Run Ruff checks"
-markdown.cmd = "pymarkdown scan  -r py_maker/**/[!CHANGELOG]*.md docs/**/*.md"
+markdown.cmd = "pymarkdown scan  -r py_maker/**/[!CHANGELOG,!.github/]*.md docs/**/*.md"
 markdown.help = "Run markdown checks"
 
 # run all linting checks in sequence. we want to run them all, even if one fails
 lint.ignore_fail = "return_non_zero"
 lint.sequence = ["format", "ruff", "mypy", "markdown"]
 lint.help = "Run all linting checks"
 {% endif %}
 
+{% if options.test %}
+test.cmd = "pytest"
+test.help = "Run all tests (pytest)"
+{% endif %}
+
 {% if options.docs %}
 "docs:publish".cmd = "mkdocs gh-deploy"
 "docs:publish".help = "Publish documentation to GitHub Pages"
 "docs:build".cmd = "mkdocs build"
 "docs:build".help = "Build documentation locally to './site' folder"
 "docs:serve".cmd = "mkdocs serve -w TODO.md -w CHANGELOG.md -w CONTRIBUTING.md"
 "docs:serve".help = "Serve documentation locally"
 "docs:serve:all".cmd = "mkdocs serve -w TODO.md -w CHANGELOG.md -w CONTRIBUTING.md -a 0.0.0.0:9000"
 "docs:serve:all".help = "Serve documentation locally on all interfaces"
 {% endif %}
 
 # generate a CHANGELOG.md file from GitHub releases
-changelog.cmd = "github-changelog-md -r py-maker"
+changelog.cmd = "github-changelog-md"
 changelog.help = "Generate a CHANGELOG.md file"
 
 {% if options.lint %}
 # configure assorted tools and linters
 [tool.pymarkdown]
 plugins.md014.enabled = false
 plugins.md046.enabled = false
 
 [tool.ruff]
 line-length = 80
-select = ["ALL"] # we are being very strict!
-ignore = [
+lint.select = ["ALL"] # we are being very strict!
+lint.ignore = [
   "ANN101",
   "PGH003",
   "FBT002",
   "FBT003",
   "B006",
 ] # These rules are too strict even for us 😝
-extend-ignore = ["COM812", "ISC001"] # these are ignored for ruff formatting
+lint.extend-ignore = [
+  "COM812",
+  "ISC001",
+] # these are ignored for ruff formatting
 
 src = ["py_maker"]
 target-version = "py39" # minimum python version supported
 
 [tool.ruff.format]
 indent-style = "space"
 quote-style = "double"
 
-[tool.ruff.pep8-naming]
+[tool.ruff.lint.pep8-naming]
 classmethod-decorators = ["pydantic.validator", "pydantic.root_validator"]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.extend-per-file-ignores]
+[tool.ruff.lint.extend-per-file-ignores]
 "tests/**/*.py" = [
   "S101",   # we can (and MUST!) use 'assert' in test files.
   "ANN001", # annotations for fixtures are sometimes a pain for test files
 ]
-"py_maker/main.py" = ["UP007", "PLR0913"] # These cause issues in Typer Apps
-"py_maker/commands/*.py" = ["UP007", "PLR0913"] # Same as above
 
-[tool.ruff.isort]
-known-first-party = ["py_maker"]
+[tool.ruff.lint.isort]
+known-first-party = []
 
-[tool.ruff.pyupgrade]
+[tool.ruff.lint.pyupgrade]
 keep-runtime-typing = true
 
 [[tool.mypy.overrides]]
 disable_error_code = ["method-assign", "no-untyped-def", "attr-defined"]
 module = "tests.*"
 {% endif %}
 
 {% if options.test %}
+# Options for pytest and coverage
 [tool.pytest.ini_options]
-addopts = ["--cov", "--cov-report", "term-missing", "--cov-report", "html"]
+addopts = [
+  "-m",
+  "not rewrite",
+  "--cov",
+  "--cov-report",
+  "term-missing",
+  "--cov-report",
+  "html"
+]
 filterwarnings = []
 mock_use_standalone_module = true
+markers = [
+  "unit: Unit tests",
+  "integration: Integration tests",
+  "rewrite: Tests need Rewriting", # will be skipped automatically
+]
 
 [tool.coverage.run]
 # source = []
 omit = ["*/tests/*"]
+concurrency = ["thread", "greenlet"]
+
+[tool.coverage.report]
+show_missing = true
 {% endif %}
```

### Comparing `pyproject_maker-0.9.4/py_maker/tree/tree.py` & `pyproject_maker-0.9.5/py_maker/tree/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """WIP Class to display a directory tree using Rich to the console.
 
 Heavily influenced by the example in Rich.tree documentation.
 """
+
 from __future__ import annotations
 
 import os
 import pathlib
 
 from rich import print  # pylint: disable=redefined-builtin
 from rich.filesize import decimal
```

### Comparing `pyproject_maker-0.9.4/pyproject.toml` & `pyproject_maker-0.9.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyproject-maker"
-version = "0.9.4"
+version = "0.9.5"
 description = "A command line app to create a Python project skeleton."
 authors = ["Grant Ramsay <seapagan@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 repository = "https://github.com/seapagan/py-maker"
 homepage = "https://py-maker.seapagan.net"
@@ -34,66 +34,64 @@
 
 [tool.poetry.scripts]
 pymaker = "py_maker.main:app"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 typer = { extras = ["all"], version = "^0.9.0" }
-jinja2 = "^3.1.2"
-gitpython = "^3.1.32"
-pydantic = "^2.4"
-rich = "^13.4.2"
+jinja2 = "^3.1.3"
+gitpython = "^3.1.42"
+pydantic = "^2.6.3"
+rich = "^13.7.1"
 rtoml = "^0.9.0"
 requests = "^2.31.0"
-pygithub = "^2.1.1"
-simple-toml-settings = "^0.3"
-github-changelog-md = "^0.8.0"
+pygithub = "^2.2.0"
+simple-toml-settings = "^0.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Configure dev dependencies
 [tool.poetry.group.dev.dependencies]
 # linting, type-checking and security checks
-mypy = "^1.4.1"
-pre-commit = "^3.3.3"
+mypy = "^1.8.0"
+pre-commit = "^3.6.2"
 pymarkdownlnt = "^0.9.12"
-ruff = "^0.1.3"
+ruff = "^0.3.0"
 
 # testing
-pytest = "^7.4.0"
-pytest-cov = "^4.0.0"
-pytest-xdist = "^3.2.1"
-pytest-sugar = "^0.9.7"
-pytest-randomly = "^3.13.0"
+pytest = "^8.1.0"
+pytest-cov = "^4.1.0"
+pytest-xdist = "^3.5.0"
+pytest-sugar = ">=1.0.0"
+pytest-randomly = "^3.15.0"
 pytest-reverse = "^1.7.0"
-pytest-asyncio = "^0.21.1"
-pytest-mock = "^3.11.1"
+pytest-mock = "^3.12.0"
 mock = "^5.1.0"
-faker = ">=19.2,<21.0"
-pyfakefs = "^5.2.4"
+faker = ">=23.3.0"
+pyfakefs = "^5.3.5"
 
 # documentation
-github-changelog-md = ">=0.7.2"
-mkdocs = "^1.4.3"
-mkdocs-autorefs = "^0.5.0"
-mkdocs-material = "^9.1.19"
-mkdocs-git-revision-date-localized-plugin = "^1.2.0"
+github-changelog-md = "^0.9.1"
+mkdocs = "^1.5.3"
+mkdocs-autorefs = ">=1.0.1"
+mkdocs-material = "^9.5.12"
+mkdocs-git-revision-date-localized-plugin = "^1.2.4"
 mkdocs-latest-git-tag-plugin = "^0.1.2"
-mkdocs-minify-plugin = "^0.7.0"
-mkdocstrings = ">=0.22,<0.25"
-pymdown-extensions = "^10.1"
-pygments = "^2.15.1"
+mkdocs-minify-plugin = ">=0.8.0"
+mkdocstrings = ">=0.24.1"
+pymdown-extensions = "^10.7"
+pygments = "^2.17.2"
 
 # typing stubs
-types-requests = "^2.31.0.2"
+types-requests = "^2.31.0.20240218"
 
 # assorted utilities
-poethepoet = "^0.24.0"
+poethepoet = ">=0.25.0"
 
 [tool.poe.tasks]
 # setup 'PoeThePoet' tasks
 pre.cmd = "pre-commit run --all-files"
 pre.help = "Run pre-commit checks"
 mypy.cmd = "mypy py_maker/**/*.py tests/**/*.py --strict"
 mypy.help = "Run mypy checks"
@@ -130,57 +128,64 @@
 # configure assorted tools and linters
 [tool.pymarkdown]
 plugins.md014.enabled = false
 plugins.md046.enabled = false
 
 [tool.ruff]
 line-length = 80
-select = ["ALL"] # we are being very strict!
-ignore = [
+lint.select = ["ALL"] # we are being very strict!
+lint.ignore = [
   "ANN101",
   "PGH003",
   "FBT002",
   "FBT003",
   "B006",
 ] # These rules are too strict even for us 😝
-extend-ignore = ["COM812", "ISC001"] # these are ignored for ruff formatting
+lint.extend-ignore = [
+  "COM812",
+  "ISC001",
+] # these are ignored for ruff formatting
 
 src = ["py_maker"]
 target-version = "py39" # minimum python version supported
 
 [tool.ruff.format]
 indent-style = "space"
 quote-style = "double"
 
-[tool.ruff.pep8-naming]
+[tool.ruff.lint.pep8-naming]
 classmethod-decorators = ["pydantic.validator", "pydantic.root_validator"]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.extend-per-file-ignores]
+[tool.ruff.lint.extend-per-file-ignores]
 "tests/**/*.py" = [
   "S101",   # we can (and MUST!) use 'assert' in test files.
   "ANN001", # annotations for fixtures are sometimes a pain for test files
 ]
 "py_maker/main.py" = ["UP007", "PLR0913"] # These cause issues in Typer Apps
 "py_maker/commands/*.py" = ["UP007", "PLR0913"] # Same as above
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["py_maker"]
 
-[tool.ruff.pyupgrade]
+[tool.ruff.lint.pyupgrade]
 keep-runtime-typing = true
 
 [[tool.mypy.overrides]]
 disable_error_code = ["method-assign", "no-untyped-def", "attr-defined"]
 module = "tests.*"
 
 # Options for pytest and coverage
 [tool.pytest.ini_options]
 addopts = ["--cov", "--cov-report", "term-missing", "--cov-report", "html"]
 filterwarnings = []
 mock_use_standalone_module = true
+markers = ["e2e: mark a test as an end-to-end test."]
 
 [tool.coverage.run]
-# source = []
-omit = ["*/tests/*"]
+omit = ["*/tests/*", "py_maker/tree/*"]
+source = ["py_maker"]
+
+[tool.coverage.report]
+show_missing = true
```

### Comparing `pyproject_maker-0.9.4/PKG-INFO` & `pyproject_maker-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-maker
-Version: 0.9.4
+Version: 0.9.5
 Summary: A command line app to create a Python project skeleton.
 Home-page: https://py-maker.seapagan.net
 License: MIT
 Author: Grant Ramsay
 Author-email: seapagan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -16,23 +16,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Utilities
-Requires-Dist: github-changelog-md (>=0.8.0,<0.9.0)
-Requires-Dist: gitpython (>=3.1.32,<4.0.0)
-Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: pydantic (>=2.4,<3.0)
-Requires-Dist: pygithub (>=2.1.1,<3.0.0)
+Requires-Dist: gitpython (>=3.1.42,<4.0.0)
+Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: pydantic (>=2.6.3,<3.0.0)
+Requires-Dist: pygithub (>=2.2.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: rtoml (>=0.9.0,<0.10.0)
-Requires-Dist: simple-toml-settings (>=0.3,<0.4)
+Requires-Dist: simple-toml-settings (>=0.4,<0.5)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/seapagan/py-maker/issues
 Project-URL: Changelog, https://github.com/seapagan/py-maker/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://py-maker.seapagan.net
 Project-URL: Pull Requests, https://github.com/seapagan/py-maker/pulls
 Project-URL: Repository, https://github.com/seapagan/py-maker
 Description-Content-Type: text/markdown
```

