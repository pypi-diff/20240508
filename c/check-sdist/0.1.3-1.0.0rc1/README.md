# Comparing `tmp/check_sdist-0.1.3.tar.gz` & `tmp/check_sdist-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Oct  3 16:23:46 2023, max compression
+gzip compressed data, last modified: Tue May  7 21:35:39 2024, max compression
```

## Comparing `check_sdist-0.1.3.tar` & `check_sdist-1.0.0rc1.tar`

### file list

```diff
@@ -1,30 +1,34 @@
--rw-r--r--   0        0        0     2098 2023-10-03 16:23:46.000000 check_sdist-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      468 2023-10-03 16:23:46.000000 check_sdist-0.1.3/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0     1111 2023-10-03 16:23:46.000000 check_sdist-0.1.3/noxfile.py
--rw-r--r--   0        0        0     2246 2023-10-03 16:23:46.000000 check_sdist-0.1.3/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      163 2023-10-03 16:23:46.000000 check_sdist-0.1.3/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-10-03 16:23:46.000000 check_sdist-0.1.3/.github/matchers/pylint.json
--rw-r--r--   0        0        0      669 2023-10-03 16:23:46.000000 check_sdist-0.1.3/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1496 2023-10-03 16:23:46.000000 check_sdist-0.1.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      205 2023-10-03 16:23:46.000000 check_sdist-0.1.3/src/check_sdist/__init__.py
--rw-r--r--   0        0        0     3657 2023-10-03 16:23:46.000000 check_sdist-0.1.3/src/check_sdist/__main__.py
--rw-r--r--   0        0        0      539 2023-10-03 16:23:46.000000 check_sdist-0.1.3/src/check_sdist/git.py
--rw-r--r--   0        0        0     1898 2023-10-03 16:23:46.000000 check_sdist-0.1.3/src/check_sdist/inject.py
--rw-r--r--   0        0        0        0 2023-10-03 16:23:46.000000 check_sdist-0.1.3/src/check_sdist/py.typed
--rw-r--r--   0        0        0     1108 2023-10-03 16:23:46.000000 check_sdist-0.1.3/src/check_sdist/sdist.py
--rw-r--r--   0        0        0        0 2023-10-03 16:23:46.000000 check_sdist-0.1.3/src/check_sdist/_compat/__init__.py
--rw-r--r--   0        0        0      238 2023-10-03 16:23:46.000000 check_sdist-0.1.3/src/check_sdist/_compat/importlib.py
--rw-r--r--   0        0        0      161 2023-10-03 16:23:46.000000 check_sdist-0.1.3/src/check_sdist/_compat/tomllib.py
--rw-r--r--   0        0        0      169 2023-10-03 16:23:46.000000 check_sdist-0.1.3/src/check_sdist/resources/__init__.py
--rw-r--r--   0        0        0       94 2023-10-03 16:23:46.000000 check_sdist-0.1.3/src/check_sdist/resources/default-ignore.txt
--rw-r--r--   0        0        0      272 2023-10-03 16:23:46.000000 check_sdist-0.1.3/src/check_sdist/resources/junk-paths.txt
--rw-r--r--   0        0        0      408 2023-10-03 16:23:46.000000 check_sdist-0.1.3/tests/downstream.toml
--rw-r--r--   0        0        0      321 2023-10-03 16:23:46.000000 check_sdist-0.1.3/tests/test_cli.py
--rw-r--r--   0        0        0      738 2023-10-03 16:23:46.000000 check_sdist-0.1.3/tests/test_downstream.py
--rw-r--r--   0        0        0     1418 2023-10-03 16:23:46.000000 check_sdist-0.1.3/tests/test_inject.py
--rw-r--r--   0        0        0      758 2023-10-03 16:23:46.000000 check_sdist-0.1.3/tests/test_package.py
--rw-r--r--   0        0        0     2217 2023-10-03 16:23:46.000000 check_sdist-0.1.3/.gitignore
--rw-r--r--   0        0        0     1526 2023-10-03 16:23:46.000000 check_sdist-0.1.3/LICENSE
--rw-r--r--   0        0        0     3065 2023-10-03 16:23:46.000000 check_sdist-0.1.3/README.md
--rw-r--r--   0        0        0     3453 2023-10-03 16:23:46.000000 check_sdist-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4532 2023-10-03 16:23:46.000000 check_sdist-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2366 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      500 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0     1576 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/noxfile.py
+-rw-r--r--   0        0        0     2246 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      669 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1586 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.github/workflows/ci.yml
+-rwxr-xr-x   0        0        0     1005 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/scripts/generate_schema.py
+-rw-r--r--   0        0        0      207 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/__init__.py
+-rw-r--r--   0        0        0     5182 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/__main__.py
+-rw-r--r--   0        0        0      642 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/git.py
+-rw-r--r--   0        0        0     1898 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/inject.py
+-rw-r--r--   0        0        0        0 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/py.typed
+-rw-r--r--   0        0        0      452 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/schema.py
+-rw-r--r--   0        0        0     1326 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/sdist.py
+-rw-r--r--   0        0        0        0 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/_compat/__init__.py
+-rw-r--r--   0        0        0      238 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/_compat/importlib.py
+-rw-r--r--   0        0        0      161 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/_compat/tomllib.py
+-rw-r--r--   0        0        0      169 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/resources/__init__.py
+-rw-r--r--   0        0        0     1008 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/resources/check-sdist.schema.json
+-rw-r--r--   0        0        0      100 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/resources/default-ignore.txt
+-rw-r--r--   0        0        0      272 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/src/check_sdist/resources/junk-paths.txt
+-rw-r--r--   0        0        0      471 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/tests/downstream.toml
+-rw-r--r--   0        0        0      321 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/tests/test_cli.py
+-rw-r--r--   0        0        0      817 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/tests/test_downstream.py
+-rw-r--r--   0        0        0     1418 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/tests/test_inject.py
+-rw-r--r--   0        0        0      758 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/tests/test_package.py
+-rw-r--r--   0        0        0     1131 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/tests/test_validate_pyproject.py
+-rw-r--r--   0        0        0     2217 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/.gitignore
+-rw-r--r--   0        0        0     1526 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     3635 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/README.md
+-rw-r--r--   0        0        0     3600 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5181 2024-05-07 21:35:39.000000 check_sdist-1.0.0rc1/PKG-INFO
```

### Comparing `check_sdist-0.1.3/.pre-commit-config.yaml` & `check_sdist-1.0.0rc1/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
-  - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: "23.9.1"
-    hooks:
-      - id: black-jupyter
-
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.4.0"
+    rev: "v4.6.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
@@ -28,53 +23,68 @@
     rev: "v1.10.0"
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.3"
+    rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.292
+    rev: v0.4.3
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
+      - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.5.1"
+    rev: "v1.10.0"
     hooks:
       - id: mypy
         files: src|tests
         args: []
         additional_dependencies:
-          ["tomli", "pathspec", "importlib-resources", "pytest"]
+          [
+            "tomli",
+            "pathspec",
+            "importlib-resources",
+            "pytest",
+            "validate-pyproject",
+          ]
 
   - repo: https://github.com/henryiii/check-sdist
-    rev: "v0.1.2"
+    rev: "v0.1.3"
     hooks:
       - id: check-sdist
         args: [--inject-junk]
         additional_dependencies:
           - hatchling
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
       - id: codespell
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: "v0.9.0.6"
+    rev: "v0.10.0.1"
     hooks:
       - id: shellcheck
 
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
         language: pygrep
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest
         exclude: .pre-commit-config.yaml
+
+  - repo: https://github.com/python-jsonschema/check-jsonschema
+    rev: 0.28.2
+    hooks:
+      - id: check-dependabot
+      - id: check-github-workflows
+      - id: check-metaschema
+        files: "^src/check_sdist/resources/check-sdist.schema.json$"
```

### Comparing `check_sdist-0.1.3/.github/CONTRIBUTING.md` & `check_sdist-1.0.0rc1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.3/.github/matchers/pylint.json` & `check_sdist-1.0.0rc1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.3/.github/workflows/cd.yml` & `check_sdist-1.0.0rc1/.github/workflows/cd.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,24 @@
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
-      - uses: hynek/build-and-inspect-python-package@v1
+      - uses: hynek/build-and-inspect-python-package@v2
 
   publish:
     name: Publish
     needs: [dist]
     environment: pypi
     permissions:
       id-token: write
     runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
           name: Packages
           path: dist
 
       - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `check_sdist-0.1.3/.github/workflows/ci.yml` & `check_sdist-1.0.0rc1/.github/workflows/ci.yml`

 * *Files 24% similar despite different names*

```diff
@@ -30,41 +30,45 @@
   checks:
     name: Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}
     runs-on: ${{ matrix.runs-on }}
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.8", "3.12"]
-        runs-on: [ubuntu-latest, macos-latest, windows-latest]
+        runs-on: [ubuntu-latest, macos-14, windows-latest]
 
         include:
           - python-version: pypy-3.8
             runs-on: ubuntu-latest
+          - python-version: "3.10"
+            runs-on: macos-13
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
+      - uses: yezz123/setup-uv@v4
+
       - name: Install package
-        run: python -m pip install .[test]
+        run: uv pip install -e.[test] --system
 
       - name: Test package
-        run: python -m pytest -ra --cov=check-sdist
+        run: pytest -ra --cov=check-sdist
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
 
   dist:
     name: Distribution build
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
-      - uses: hynek/build-and-inspect-python-package@v1
+      - uses: hynek/build-and-inspect-python-package@v2
```

### Comparing `check_sdist-0.1.3/src/check_sdist/__main__.py` & `check_sdist-1.0.0rc1/src/check_sdist/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,92 @@
 from __future__ import annotations
 
 import argparse
 import contextlib
+import importlib.util
+import shutil
 from collections.abc import Sequence
 from pathlib import Path
+from typing import Literal
 
 import pathspec
 
 from . import __version__
 from ._compat import tomllib
 from .git import git_files
 from .inject import inject_junk_files
 from .resources import resources
 from .sdist import sdist_files
 
 
-def compare(source_dir: Path, *, isolated: bool, verbose: bool = False) -> int:
+def select_installer(
+    installer: Literal["pip", "uv", "uv|pip"],  # type: ignore[name-defined]
+) -> Literal["uv", "pip"]:
+    """
+    Select uv, pip, or uv if available, then pip ("uv|pip"). Returns uv, pip,
+    or throws an error if uv was required and not available.
+    """
+    if "uv" in installer:
+        if importlib.util.find_spec("uv") is not None:
+            return "uv"
+
+        if shutil.which("uv") is not None:
+            return "uv"
+
+        if installer == "uv":
+            msg = "Can't find uv"
+            raise ImportError(msg)
+
+    return "pip"
+
+
+def compare(
+    source_dir: Path,
+    *,
+    isolated: bool,
+    verbose: bool = False,
+    installer: Literal["uv", "pip", "uv|pip"] = "uv|pip",  # type: ignore[name-defined]
+) -> int:
     """
     Compare the files in the SDist with the files tracked by git.
 
     Takes the source directory and a flag indicating whether the SDist should
     be built in an isolated environment.
 
     Return 0 if they match, 1 if the SDist has files that are not tracked by
     git, 2 if the SDist is missing files that are tracked by git, and 3 if both
     conditions are true.
     """
 
-    sdist = sdist_files(source_dir, isolated) - {"PKG-INFO"}
-    git = git_files(source_dir)
+    installer = select_installer(installer)
 
     config = {}
     pyproject_toml = source_dir.joinpath("pyproject.toml")
     with contextlib.suppress(FileNotFoundError), pyproject_toml.open("rb") as f:
         pyproject = tomllib.load(f)
         config = pyproject.get("tool", {}).get("check-sdist", {})
 
     sdist_only_patterns = config.get("sdist-only", [])
     git_only_patterns = config.get("git-only", [])
     default_ignore = config.get("default-ignore", True)
+    recurse_submodules = config.get("recurse-submodules", True)
+    mode = config.get("mode", "git")
+
+    sdist = sdist_files(source_dir, isolated=isolated, installer=installer) - {
+        "PKG-INFO"
+    }
+    if mode == "git":
+        git = git_files(source_dir, recurse_submodules=recurse_submodules)
+    elif mode == "all":
+        git = frozenset(
+            str(p.relative_to(source_dir)) for p in source_dir.rglob("*") if p.is_file()
+        )
+    else:
+        msg = "Only 'all' and 'git' supported for 'mode'"
+        raise ValueError(msg)
 
     if default_ignore:
         with resources.joinpath("default-ignore.txt").open("r", encoding="utf-8") as f:
             git_only_patterns.extend(f.read().splitlines())
         sdist_only_patterns.extend("*.dist-info")
 
     sdist_spec = pathspec.GitIgnoreSpec.from_lines(sdist_only_patterns)
@@ -95,20 +139,31 @@
     )
     parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         help="Print out SDist contents too",
     )
+    parser.add_argument(
+        "--installer",
+        choices={"uv", "pip", "uv|pip"},
+        default="uv|pip",
+        help="Tool to use when installing packages for making the SDist",
+    )
     args = parser.parse_args(sys_args)
 
     with contextlib.ExitStack() as stack:
         if args.inject_junk:
             stack.enter_context(inject_junk_files(args.source_dir))
 
     raise SystemExit(
-        compare(args.source_dir, isolated=not args.no_isolation, verbose=args.verbose)
+        compare(
+            args.source_dir,
+            isolated=not args.no_isolation,
+            verbose=args.verbose,
+            installer=args.installer,
+        )
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `check_sdist-0.1.3/src/check_sdist/git.py` & `check_sdist-1.0.0rc1/src/check_sdist/git.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import subprocess
 from pathlib import Path
 
 
-def git_files(source_dir: Path) -> frozenset[str]:
+def git_files(source_dir: Path, recurse_submodules: bool = True) -> frozenset[str]:
     """Return the files that are tracked by git in the source directory."""
 
     cmd = ["git", "ls-files", "--cached"]
+    if recurse_submodules:
+        cmd.append("--recurse-submodules")
     return frozenset(
         subprocess.run(
             cmd,
             cwd=source_dir,
             text=True,
             capture_output=True,
             check=True,
```

### Comparing `check_sdist-0.1.3/src/check_sdist/inject.py` & `check_sdist-1.0.0rc1/src/check_sdist/inject.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.3/src/check_sdist/sdist.py` & `check_sdist-1.0.0rc1/src/check_sdist/sdist.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 from __future__ import annotations
 
 import subprocess
 import sys
 import tarfile
 import tempfile
 from pathlib import Path
+from typing import Literal
 
 
-def sdist_files(source_dir: Path, isolated: bool) -> frozenset[str]:
+def sdist_files(
+    source_dir: Path, *, isolated: bool, installer: Literal["uv", "pip"]
+) -> frozenset[str]:
     """Return the files that would be (are) placed in the SDist."""
 
     with tempfile.TemporaryDirectory() as outdir:
-        cmd = [sys.executable, "-m", "build", "--sdist", "--outdir", outdir]
+        cmd = [
+            sys.executable,
+            "-m",
+            "build",
+            "--sdist",
+            "--outdir",
+            outdir,
+            f"--installer={installer}",
+        ]
         if not isolated:
             cmd.append("--no-isolation")
         subprocess.run(cmd, check=True, cwd=source_dir)
 
         (outpath,) = Path(outdir).glob("*.tar.gz")
 
         with tarfile.open(outpath) as tar:
@@ -27,8 +38,8 @@
                 t.name.split("/", maxsplit=1)[1]
                 for t in tar.getmembers()
                 if t.isfile() or t.issym()
             )
 
 
 if __name__ == "__main__":
-    print(*sorted(sdist_files(Path.cwd(), True)), sep="\n")
+    print(*sorted(sdist_files(Path.cwd(), isolated=True, installer="pip")), sep="\n")
```

### Comparing `check_sdist-0.1.3/tests/test_inject.py` & `check_sdist-1.0.0rc1/tests/test_inject.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.3/tests/test_package.py` & `check_sdist-1.0.0rc1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.3/.gitignore` & `check_sdist-1.0.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.3/LICENSE` & `check_sdist-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `check_sdist-0.1.3/README.md` & `check_sdist-1.0.0rc1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -27,21 +27,23 @@
 files.
 
 ### Quick start
 
 To run:
 
 ```console
-$ pipx run check-sdist
+$ pipx run check-sdist[uv]
 ```
 
 You can add `--no-isolation` to disable build isolation (faster, but must
 preinstall build dependencies), `--source-dir` to select a different source
 directory to check, and `--inject-junk` to temporarily inject some common junk
-files while running.
+files while running. You can select an installer for build to use with
+`--installer=`, choices are `uv`, `pip`, or `uv|pip`, which will use uv if
+available (the default).
 
 If you need the latest development version:
 
 ```console
 $ pipx run --spec git+https://github.com/henryiii/check-sdist check-sdist
 ```
 
@@ -76,19 +78,29 @@
 To configure, these options are supported in your `pyproject.toml` file:
 
 ```toml
 [tool.check-sdist]
 sdist-only = []
 git-only = []
 default-ignore = true
+recurse-submodules = true
+mode = "git"
 ```
 
 You can add `.gitignore` style lines here, and you can turn off the default
 ignore list, which adds some default git-only files.
 
+By default, check-sdist recursively scans the contents of Git submodules, but
+you can disable this behavior (e.g. to support older Git versions that don't
+have this capability).
+
+You can also select `mode = "all"`, which will instead check every file on your
+system. Be prepared to ignore lots of things manually, like `*.pyc` files, if
+you use this.
+
 ### See also
 
 - [check-manifest](https://github.com/mgedmin/check-manifest): A (currently)
   setuptools specific checker that can suggest possible ways to include/exclude
   files.
-- [scikit-hep developer pages](https://scikit-hep.org/developer): Guidelines on
-  which this package was designed.
+- [Scientific Python Development Guide](https://learn.scientific-python.org/development/):
+  Guidelines on which this package was designed.
```

### Comparing `check_sdist-0.1.3/pyproject.toml` & `check_sdist-1.0.0rc1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [
   { name = "Henry Schreiner", email = "henryschreineriii@gmail.com" },
 ]
 description = "Check the contents of an SDist vs. git"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
-  "Development Status :: 4 - Beta",
+  "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
@@ -23,45 +23,47 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
-  "build",
+  "build >=1.2",
+  "importlib-resources; python_version<'3.9'",
   "pathspec",
   "tomli; python_version<'3.11'",
-  "importlib-resources; python_version<'3.9'",
 ]
 keywords = ["sdist", "packaging", "lint"]
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
   "pytest-cov >=3",
+  "pyproject-hooks !=1.1.0",
+  "validate-pyproject >=0.16",
 ]
-dev = [
-  "pytest >=6",
-  "pytest-cov >=3",
+uv = [
+  "uv",
 ]
 
 [project.urls]
 Homepage = "https://github.com/henryiii/check-sdist"
 "Bug Tracker" = "https://github.com/henryiii/check-sdist/issues"
 Changelog = "https://github.com/henryiii/check-sdist/releases"
 
 [project.scripts]
 check-sdist = "check_sdist.__main__:main"
 
+[project.entry-points."validate_pyproject.tool_schema"]
+check-sdist = "check_sdist.schema:get_schema"
+
 [tool.hatch]
 version.path = "src/check_sdist/__init__.py"
-envs.default.dependencies = [
-  "pytest",
-  "pytest-cov",
-]
+envs.default.features = ["test"]
+envs.hatch-test.features = ["test", "cli"]
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = ["-ra", "--showlocals", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = ["error"]
@@ -85,16 +87,18 @@
 [[tool.mypy.overrides]]
 module = "check_sdist.*"
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 
 
 [tool.ruff]
-select = [
-  "E", "F", "W", # flake8
+src = ["src"]
+
+[tool.ruff.lint]
+extend-select = [
   "B",           # flake8-bugbear
   "I",           # isort
   "ARG",         # flake8-unused-arguments
   "C4",          # flake8-comprehensions
   "EM",          # flake8-errmsg
   "ICN",         # flake8-import-conventions
   "ISC",         # flake8-implicit-str-concat
@@ -107,21 +111,18 @@
   "RET",         # flake8-return
   "RUF",         # Ruff-specific
   "SIM",         # flake8-simplify
   "UP",          # pyupgrade
   "YTT",         # flake8-2020
   "EXE",         # flake8-executable
 ]
-extend-ignore = [
-  "PLR",    # Design related pylint codes
+ignore = [
+  "PLR09",  # Design related pylint codes
   "E501",   # Line too long
-]
-src = ["src"]
-unfixable = [
-  "F841", # Removes unused variables
+  "ISC001", # Conflicts with formatter
 ]
 flake8-unused-arguments.ignore-variadic-names = true
 isort.required-imports = ["from __future__ import annotations"]
 
 
 [tool.pylint]
 py-version = "3.8"
```

### Comparing `check_sdist-0.1.3/PKG-INFO` & `check_sdist-1.0.0rc1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: check-sdist
-Version: 0.1.3
+Version: 1.0.0rc1
 Summary: Check the contents of an SDist vs. git
 Project-URL: Homepage, https://github.com/henryiii/check-sdist
 Project-URL: Bug Tracker, https://github.com/henryiii/check-sdist/issues
 Project-URL: Changelog, https://github.com/henryiii/check-sdist/releases
 Author-email: Henry Schreiner <henryschreineriii@gmail.com>
 License-File: LICENSE
 Keywords: lint,packaging,sdist
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: build
+Requires-Dist: build>=1.2
 Requires-Dist: importlib-resources; python_version < '3.9'
 Requires-Dist: pathspec
 Requires-Dist: tomli; python_version < '3.11'
-Provides-Extra: dev
-Requires-Dist: pytest-cov>=3; extra == 'dev'
-Requires-Dist: pytest>=6; extra == 'dev'
 Provides-Extra: test
+Requires-Dist: pyproject-hooks!=1.1.0; extra == 'test'
 Requires-Dist: pytest-cov>=3; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
+Requires-Dist: validate-pyproject>=0.16; extra == 'test'
+Provides-Extra: uv
+Requires-Dist: uv; extra == 'uv'
 Description-Content-Type: text/markdown
 
 # check-sdist
 
 [![Actions Status][actions-badge]][actions-link]
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
@@ -63,21 +64,23 @@
 files.
 
 ### Quick start
 
 To run:
 
 ```console
-$ pipx run check-sdist
+$ pipx run check-sdist[uv]
 ```
 
 You can add `--no-isolation` to disable build isolation (faster, but must
 preinstall build dependencies), `--source-dir` to select a different source
 directory to check, and `--inject-junk` to temporarily inject some common junk
-files while running.
+files while running. You can select an installer for build to use with
+`--installer=`, choices are `uv`, `pip`, or `uv|pip`, which will use uv if
+available (the default).
 
 If you need the latest development version:
 
 ```console
 $ pipx run --spec git+https://github.com/henryiii/check-sdist check-sdist
 ```
 
@@ -112,19 +115,29 @@
 To configure, these options are supported in your `pyproject.toml` file:
 
 ```toml
 [tool.check-sdist]
 sdist-only = []
 git-only = []
 default-ignore = true
+recurse-submodules = true
+mode = "git"
 ```
 
 You can add `.gitignore` style lines here, and you can turn off the default
 ignore list, which adds some default git-only files.
 
+By default, check-sdist recursively scans the contents of Git submodules, but
+you can disable this behavior (e.g. to support older Git versions that don't
+have this capability).
+
+You can also select `mode = "all"`, which will instead check every file on your
+system. Be prepared to ignore lots of things manually, like `*.pyc` files, if
+you use this.
+
 ### See also
 
 - [check-manifest](https://github.com/mgedmin/check-manifest): A (currently)
   setuptools specific checker that can suggest possible ways to include/exclude
   files.
-- [scikit-hep developer pages](https://scikit-hep.org/developer): Guidelines on
-  which this package was designed.
+- [Scientific Python Development Guide](https://learn.scientific-python.org/development/):
+  Guidelines on which this package was designed.
```

