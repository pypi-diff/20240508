# Comparing `tmp/exasol_toolbox-0.8.0.tar.gz` & `tmp/exasol_toolbox-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol_toolbox-0.8.0.tar", max compression
+gzip compressed data, was "exasol_toolbox-0.9.0.tar", max compression
```

## Comparing `exasol_toolbox-0.8.0.tar` & `exasol_toolbox-0.9.0.tar`

### file list

```diff
@@ -1,46 +1,59 @@
--rw-r--r--   0        0        0     1063 2024-02-07 07:11:40.384720 exasol_toolbox-0.8.0/LICENSE
--rw-r--r--   0        0        0     1859 2024-02-07 07:11:40.384720 exasol_toolbox-0.8.0/README.rst
--rw-r--r--   0        0        0     2324 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/doc/changelog.rst
--rw-r--r--   0        0        0        0 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/__init__.py
--rw-r--r--   0        0        0     7305 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/metrics.py
--rw-r--r--   0        0        0        0 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/nox/__init__.py
--rw-r--r--   0        0        0     9752 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/nox/tasks.py
--rw-r--r--   0        0        0        0 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/pre_commit_hooks/__init__.py
--rw-r--r--   0        0        0     4217 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/pre_commit_hooks/package_version.py
--rw-r--r--   0        0        0      612 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/project.py
--rw-r--r--   0        0        0        0 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/sphinx/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/sphinx/github.py
--rw-r--r--   0        0        0      976 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/sphinx/multiversion/__init__.py
--rwxr-xr-x   0        0        0       76 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/sphinx/multiversion/__main__.py
--rw-r--r--   0        0        0     4488 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/sphinx/multiversion/git.py
--rw-r--r--   0        0        0    20685 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/sphinx/multiversion/main.py
--rw-r--r--   0        0        0     8369 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/sphinx/multiversion/sphinx.py
--rw-r--r--   0        0        0      402 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/sphinx/multiversion/templates/multiversion-index.html
--rw-r--r--   0        0        0      102 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/blank.md
--rw-r--r--   0        0        0     1884 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0        0        0      865 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      923 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0        0        0      993 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/refactoring.md
--rw-r--r--   0        0        0     1093 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/security.md
--rw-r--r--   0        0        0      461 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0        0        0      694 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/actions/python-environment/action.yml
--rw-r--r--   0        0        0      393 2024-02-07 07:11:40.388721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/dependabot.yml
--rw-r--r--   0        0        0      836 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/workflows/build-and-publish.yml
--rw-r--r--   0        0        0      507 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/workflows/check-release-tag.yml
--rw-r--r--   0        0        0     2703 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/workflows/checks.yml
--rw-r--r--   0        0        0      617 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/workflows/ci-cd.yml
--rw-r--r--   0        0        0      497 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/workflows/ci.yml
--rw-r--r--   0        0        0      651 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      395 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/workflows/pr-merge.yml
--rw-r--r--   0        0        0     1526 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/templates/github/workflows/report.yml
--rw-r--r--   0        0        0      881 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/templates/noxconfig.py
--rw-r--r--   0        0        0      212 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/templates/noxfile.py
--rw-r--r--   0        0        0      784 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/templates/pre-commit-config.yaml
--rw-r--r--   0        0        0        0 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/tools/__init__.py
--rw-r--r--   0        0        0     7488 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/tools/security.py
--rw-r--r--   0        0        0      294 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/tools/tbx.py
--rw-r--r--   0        0        0     5775 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/tools/workflow.py
--rw-r--r--   0        0        0      404 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/exasol/toolbox/version.py
--rw-r--r--   0        0        0     2021 2024-02-07 07:11:40.392721 exasol_toolbox-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3773 1970-01-01 00:00:00.000000 exasol_toolbox-0.8.0/setup.py
--rw-r--r--   0        0        0     3340 1970-01-01 00:00:00.000000 exasol_toolbox-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-08 13:13:15.055326 exasol_toolbox-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1859 2024-05-08 13:13:15.055326 exasol_toolbox-0.9.0/README.rst
+-rw-r--r--   0        0        0        0 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/__init__.py
+-rw-r--r--   0        0        0      329 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/cli.py
+-rw-r--r--   0        0        0       64 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/error.py
+-rw-r--r--   0        0        0      532 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/git.py
+-rw-r--r--   0        0        0     7341 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/metrics.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/nox/__init__.py
+-rw-r--r--   0        0        0     1284 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/nox/_documentation.py
+-rw-r--r--   0        0        0     1128 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/nox/_format.py
+-rw-r--r--   0        0        0     1146 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/nox/_lint.py
+-rw-r--r--   0        0        0     1730 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/nox/_metrics.py
+-rw-r--r--   0        0        0     5022 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/nox/_release.py
+-rw-r--r--   0        0        0     2001 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/nox/_shared.py
+-rw-r--r--   0        0        0     3201 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/nox/_test.py
+-rw-r--r--   0        0        0     1923 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/nox/plugin.py
+-rw-r--r--   0        0        0     1444 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/nox/tasks.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/pre_commit_hooks/__init__.py
+-rw-r--r--   0        0        0     4280 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/pre_commit_hooks/package_version.py
+-rw-r--r--   0        0        0     4246 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/release/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:13:15.059326 exasol_toolbox-0.9.0/exasol/toolbox/sphinx/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/sphinx/github.py
+-rw-r--r--   0        0        0      976 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/sphinx/multiversion/__init__.py
+-rwxr-xr-x   0        0        0       76 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/sphinx/multiversion/__main__.py
+-rw-r--r--   0        0        0     4534 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/sphinx/multiversion/git.py
+-rw-r--r--   0        0        0    20769 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/sphinx/multiversion/main.py
+-rw-r--r--   0        0        0     8387 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/sphinx/multiversion/sphinx.py
+-rw-r--r--   0        0        0      402 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/sphinx/multiversion/templates/multiversion-index.html
+-rw-r--r--   0        0        0      102 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/blank.md
+-rw-r--r--   0        0        0     1884 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0        0        0      865 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      923 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0        0        0      993 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/refactoring.md
+-rw-r--r--   0        0        0     1093 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/security.md
+-rw-r--r--   0        0        0      461 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0        0        0      694 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/actions/python-environment/action.yml
+-rw-r--r--   0        0        0      393 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/dependabot.yml
+-rw-r--r--   0        0        0      836 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/workflows/build-and-publish.yml
+-rw-r--r--   0        0        0      507 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/workflows/check-release-tag.yml
+-rw-r--r--   0        0        0     2725 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/workflows/checks.yml
+-rw-r--r--   0        0        0      514 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0      445 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/workflows/ci.yml
+-rw-r--r--   0        0        0      651 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      317 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/workflows/pr-merge.yml
+-rw-r--r--   0        0        0     1526 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/github/workflows/report.yml
+-rw-r--r--   0        0        0      881 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/noxconfig.py
+-rw-r--r--   0        0        0      212 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/noxfile.py
+-rw-r--r--   0        0        0      784 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/templates/pre-commit-config.yaml
+-rw-r--r--   0        0        0        0 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/tools/__init__.py
+-rw-r--r--   0        0        0     2364 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/tools/issue.py
+-rw-r--r--   0        0        0      922 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/tools/replace_version.py
+-rw-r--r--   0        0        0     7488 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/tools/security.py
+-rw-r--r--   0        0        0      374 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/tools/tbx.py
+-rw-r--r--   0        0        0     5397 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/tools/template.py
+-rw-r--r--   0        0        0     2439 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/tools/workflow.py
+-rw-r--r--   0        0        0      404 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/exasol/toolbox/version.py
+-rw-r--r--   0        0        0     2161 2024-05-08 13:13:15.063326 exasol_toolbox-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 exasol_toolbox-0.9.0/setup.py
+-rw-r--r--   0        0        0     3446 1970-01-01 00:00:00.000000 exasol_toolbox-0.9.0/PKG-INFO
```

### Comparing `exasol_toolbox-0.8.0/LICENSE` & `exasol_toolbox-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.8.0/README.rst` & `exasol_toolbox-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/metrics.py` & `exasol_toolbox-0.9.0/exasol/toolbox/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,25 +84,25 @@
         tmp_dir = Path(tmpdir)
         report = tmp_dir / "coverage.json"
         run(
             ["coverage", "json", f"--data-file={file}", "-o", f"{report}"],
             capture_output=True,
             check=True,
         )
-        with open(report) as r:
+        with open(report, encoding="utf-8") as r:
             data = json.load(r)
             total: float = data["totals"]["percent_covered"]
 
         return total
 
 
 def _static_code_analysis(file: Union[str, Path]) -> Rating:
     def pylint(f: Union[str, Path]) -> Rating:
         expr = re.compile(r"^Your code has been rated at (\d+.\d+)/.*", re.MULTILINE)
-        with open(f) as results:
+        with open(f, encoding="utf-8") as results:
             data = results.read()
 
         matches = expr.search(data)
         if matches:
             groups = matches.groups()
         try:
             group = groups[0]
```

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/pre_commit_hooks/package_version.py` & `exasol_toolbox-0.9.0/exasol/toolbox/pre_commit_hooks/package_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 class CommitHookError(Exception):
     """Indicates that this commit hook encountered an error"""
 
 
 def version_from_python_module(path: Path) -> Version:
     """Retrieve version information from the `version` module"""
-    with open(path) as file:
+    with open(path, encoding="utf-8") as file:
         _locals: Dict[str, Any] = {}
         _globals: Dict[str, Any] = {}
         exec(file.read(), _locals, _globals)
 
         try:
             version = _globals["VERSION"]
         except KeyError as ex:
@@ -62,25 +62,27 @@
 
 
 def version_from_poetry() -> Version:
     poetry = which("poetry")
     if not poetry:
         raise CommitHookError("Couldn't find poetry executable")
 
-    result = subprocess.run([poetry, "version", "--no-ansi"], capture_output=True)
+    result = subprocess.run(
+        [poetry, "version", "--no-ansi"], capture_output=True, check=False
+    )
     version = result.stdout.decode().split()[1]
     return version_from_string(version)
 
 
 def write_version_module(version: Version, path: str, exists_ok: bool = True) -> None:
     version_file = Path(path)
     if version_file.exists() and not exists_ok:
         raise CommitHookError(f"Version file [{version_file}] already exists.")
     version_file.unlink(missing_ok=True)
-    with open(version_file, "w") as f:
+    with open(version_file, "w", encoding="utf-8") as f:
         f.write(
             _VERSION_MODULE_TEMPLATE.format(
                 major=version.major, minor=version.minor, patch=version.patch
             )
         )
```

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/sphinx/multiversion/__init__.py` & `exasol_toolbox-0.9.0/exasol/toolbox/sphinx/multiversion/__init__.py`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/sphinx/multiversion/git.py` & `exasol_toolbox-0.9.0/exasol/toolbox/sphinx/multiversion/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,19 @@
     cmd = (
         "git",
         "cat-file",
         "-e",
         f"{refname}:{filename}",
     )
     proc = subprocess.run(
-        cmd, cwd=gitroot, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
+        cmd,
+        cwd=gitroot,
+        stdout=subprocess.DEVNULL,
+        stderr=subprocess.DEVNULL,
+        check=False,
     )
     return proc.returncode == 0
 
 
 def copy_tree(gitroot, src, dst, reference, sourcepath="."):
     with tempfile.SpooledTemporaryFile() as fp:
         cmd = (
```

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/sphinx/multiversion/main.py` & `exasol_toolbox-0.9.0/exasol/toolbox/sphinx/multiversion/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,15 +367,15 @@
 
         if not metadata:
             logger.error("No matching refs found!")
             return 2
 
         # Write Metadata
         metadata_path = os.path.abspath(os.path.join(tmp, "versions.json"))
-        with open(metadata_path, mode="w") as fp:
+        with open(metadata_path, mode="w", encoding="utf-8") as fp:
             json.dump(metadata, fp, indent=2)
 
         # Run Sphinx
         argv.extend(["-D", f"smv_metadata_path={metadata_path}"])
         for version_name, data in metadata.items():
             os.makedirs(data["outputdir"], exist_ok=True)
 
@@ -564,14 +564,16 @@
                         config.smv_postbuild_export_destination,
                     )
                     export_to_destination(matches, export_dst)
 
         with resources.path(
             "exasol.sphinx_extensions.multiversion.templates", "multiversion-index.html"
         ) as p:
-            with open(p) as f:
+            with open(p, encoding="utf-8") as f:
                 template = Template(f.read())
-            with open(os.path.join(args.outputdir, "index.html"), "w") as f:
+            with open(
+                os.path.join(args.outputdir, "index.html"), "w", encoding="utf-8"
+            ) as f:
                 ref = gitrefs[-1]
                 f.write(template.render(version=ref.name))
 
     return 0
```

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/sphinx/multiversion/sphinx.py` & `exasol_toolbox-0.9.0/exasol/toolbox/sphinx/multiversion/sphinx.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     :param sphinx.application.Sphinx app: Sphinx application object.
     """
 
     if not config.smv_metadata:
         if not config.smv_metadata_path:
             return
 
-        with open(config.smv_metadata_path) as f:
+        with open(config.smv_metadata_path, encoding="utf-8") as f:
             metadata = json.load(f)
 
         config.smv_metadata = metadata
 
     if not config.smv_current_version:
         return
```

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/bug.md` & `exasol_toolbox-0.9.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/documentation.md` & `exasol_toolbox-0.9.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/documentation.md`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/feature.md` & `exasol_toolbox-0.9.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/refactoring.md` & `exasol_toolbox-0.9.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/refactoring.md`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/security.md` & `exasol_toolbox-0.9.0/exasol/toolbox/templates/github/ISSUE_TEMPLATE/security.md`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/templates/github/actions/python-environment/action.yml` & `exasol_toolbox-0.9.0/exasol/toolbox/templates/github/actions/python-environment/action.yml`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/templates/github/workflows/build-and-publish.yml` & `exasol_toolbox-0.9.0/exasol/toolbox/templates/github/workflows/build-and-publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     runs-on: ubuntu-latest
     steps:
 
       - name: SCM Checkout
         uses: actions/checkout@v3
 
       - name: Setup Python & Poetry Environment
-        uses: exasol/python-toolbox/.github/actions/python-environment@0.8.0
+        uses: exasol/python-toolbox/.github/actions/python-environment@0.9.0
 
       - name: Build Artifacts
         run: poetry build
 
       - name: PyPi Release
         env:
           POETRY_HTTP_BASIC_PYPI_USERNAME: "__token__"
```

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/templates/github/workflows/checks.yml` & `exasol_toolbox-0.9.0/exasol/toolbox/templates/github/workflows/checks.yml`

 * *Files 3% similar despite different names*

```diff
@@ -11,34 +11,34 @@
     steps:
       - name: SCM Checkout
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Setup Python & Poetry Environment
-        uses: exasol/python-toolbox/.github/actions/python-environment@0.8.0
+        uses: exasol/python-toolbox/.github/actions/python-environment@0.9.0
 
       - name: Check Version(s)
-        run: poetry run version-check exasol/toolbox/version.py
+        run: poetry run version-check  <<Add path to version.py file>> 
 
   build-documentation-job:
     name: Build Documentation
     needs: [version-check-job]
     runs-on: ubuntu-latest
 
     steps:
-    - name: SCM Checkout
-      uses: actions/checkout@v3
+      - name: SCM Checkout
+        uses: actions/checkout@v3
 
-    - name: Setup Python & Poetry Environment
-      uses: exasol/python-toolbox/.github/actions/python-environment@0.8.0
+      - name: Setup Python & Poetry Environment
+        uses: exasol/python-toolbox/.github/actions/python-environment@0.9.0
 
-    - name: Build Documentation
-      run: |
-        poetry run python -m nox -s build-docs
+      - name: Build Documentation
+        run: |
+          poetry run python -m nox -s build-docs
 
   lint-job:
     name: Linting (Python-${{ matrix.python-version }})
     needs: [version-check-job]
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
@@ -46,15 +46,15 @@
         python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - name: SCM Checkout
         uses: actions/checkout@v3
 
       - name: Setup Python & Poetry Environment
-        uses: exasol/python-toolbox/.github/actions/python-environment@0.8.0
+        uses: exasol/python-toolbox/.github/actions/python-environment@0.9.0
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Run Tests
         run: poetry run nox -s lint
 
   type-check-job:
@@ -67,15 +67,15 @@
         python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - name: SCM Checkout
         uses: actions/checkout@v3
 
       - name: Setup Python & Poetry Environment
-        uses: exasol/python-toolbox/.github/actions/python-environment@0.8.0
+        uses: exasol/python-toolbox/.github/actions/python-environment@0.9.0
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Run Tests
         run: poetry run nox -s type-check
 
   tests-job:
@@ -89,13 +89,13 @@
         exasol-version: ["7.1.9"]
 
     steps:
       - name: SCM Checkout
         uses: actions/checkout@v3
 
       - name: Setup Python & Poetry Environment
-        uses: exasol/python-toolbox/.github/actions/python-environment@0.8.0
+        uses: exasol/python-toolbox/.github/actions/python-environment@0.9.0
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Run Tests
         run: poetry run nox -s coverage -- -- --db-version ${{ matrix.exasol-version }}
```

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/templates/github/workflows/gh-pages.yml` & `exasol_toolbox-0.9.0/exasol/toolbox/templates/github/workflows/gh-pages.yml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     runs-on: ubuntu-latest
 
     steps:
       - name: SCM Checkout
         uses: actions/checkout@v3
 
       - name: Setup Python & Poetry Environment
-        uses: exasol/python-toolbox/.github/actions/python-environment@0.8.0
+        uses: exasol/python-toolbox/.github/actions/python-environment@0.9.0
 
       - name: Build Documentation
         run: |
           poetry run python -m nox -s build-docs
 
       - name: Deploy
         uses: JamesIves/github-pages-deploy-action@v4.4.1
```

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/templates/github/workflows/report.yml` & `exasol_toolbox-0.9.0/exasol/toolbox/templates/github/workflows/report.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     steps:
       - name: SCM Checkout
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Setup Python & Poetry Environment
-        uses: exasol/python-toolbox/.github/actions/python-environment@0.8.0
+        uses: exasol/python-toolbox/.github/actions/python-environment@0.9.0
 
       - name: Download Artifacts
         uses: actions/download-artifact@v3
         with:
           path: ./artifacts
 
       - name: Copy Artifacts into Root Folder
@@ -34,15 +34,15 @@
           cp .coverage/.coverage ../
           cp .lint.txt/.lint.txt ../
 
       - name: Generate Report
         run: poetry run nox -s report -- -- --format json | tee metrics.json
 
       - name: Upload Artifacts
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: metrics.json
           path: metrics.json
 
       - name: Generate GitHub Summary
         run: |
           echo -e "# Summary\n" >> $GITHUB_STEP_SUMMARY
```

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/templates/noxconfig.py` & `exasol_toolbox-0.9.0/exasol/toolbox/templates/noxconfig.py`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/templates/pre-commit-config.yaml` & `exasol_toolbox-0.9.0/exasol/toolbox/templates/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.8.0/exasol/toolbox/tools/security.py` & `exasol_toolbox-0.9.0/exasol/toolbox/tools/security.py`

 * *Files identical despite different names*

### Comparing `exasol_toolbox-0.8.0/pyproject.toml` & `exasol_toolbox-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "exasol-toolbox"
 packages = [
     { include = "exasol" },
 ]
-version = "0.8.0"
+version = "0.9.0"
 description = ""
 authors = [
     "Nicola Coretti <nicola.coretti@exasol.com>"
 ]
 license = "MIT"
 readme = "README.rst"
 include = [
@@ -44,18 +44,23 @@
 pyupgrade = ">=2.38.2,<4.0.0"
 black = "^23.1.0"
 isort = "^5.12.0"
 pre-commit = "^3.1.1"
 coverage = ">=6.4.4,<8.0.0"
 pylint = ">=2.15.4"
 typer = {extras = ["all"], version = ">=0.7.0"}
-prysk = ">=0.15.1"
+prysk = {extras = ["pytest-plugin"], version = "^0.17.0"}
 importlib-resources = ">=5.12.0"
+myst-parser = "^2.0.0"
+pluggy = "^1.5.0"
 
 
+[tool.poetry.group.dev.dependencies]
+autoimport = "^1.4.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry.plugins."console_scripts"]
 "sphinx-multiversion" = "exasol.toolbox.sphinx.multiversion.main:main"
```

### Comparing `exasol_toolbox-0.8.0/setup.py` & `exasol_toolbox-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from setuptools import setup
 
 packages = \
 ['exasol',
  'exasol.toolbox',
  'exasol.toolbox.nox',
  'exasol.toolbox.pre_commit_hooks',
+ 'exasol.toolbox.release',
  'exasol.toolbox.sphinx',
  'exasol.toolbox.sphinx.multiversion',
  'exasol.toolbox.templates',
  'exasol.toolbox.tools']
 
 package_data = \
 {'': ['*'],
@@ -23,17 +24,19 @@
 install_requires = \
 ['black>=23.1.0,<24.0.0',
  'coverage>=6.4.4,<8.0.0',
  'furo>=2022.9.15,<2023.0.0',
  'importlib-resources>=5.12.0',
  'isort>=5.12.0,<6.0.0',
  'mypy>=0.971',
+ 'myst-parser>=2.0.0,<3.0.0',
  'nox>=2022.8.7,<2023.0.0',
+ 'pluggy>=1.5.0,<2.0.0',
  'pre-commit>=3.1.1,<4.0.0',
- 'prysk>=0.15.1',
+ 'prysk[pytest-plugin]>=0.17.0,<0.18.0',
  'pylint>=2.15.4',
  'pytest>=7.2.2,<8.0.0',
  'pyupgrade>=2.38.2,<4.0.0',
  'sphinx-copybutton>=0.5.0,<0.6.0',
  'sphinx>=5.3,<7.0',
  'typer[all]>=0.7.0']
 
@@ -42,15 +45,15 @@
                      'exasol.toolbox.sphinx.multiversion.main:main',
                      'tbx = exasol.toolbox.tools.tbx:CLI',
                      'version-check = '
                      'exasol.toolbox.pre_commit_hooks.package_version:main']}
 
 setup_kwargs = {
     'name': 'exasol-toolbox',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': '',
     'long_description': 'Exasol Toolbox\n#####################\n\n.. image:: https://img.shields.io/pypi/v/exasol-toolbox\n     :target: https://pypi.org/project/exasol-toolbox/\n     :alt: PyPI Version\n\n.. image:: https://img.shields.io/pypi/pyversions/exasol-toolbox\n    :target: https://pypi.org/project/exasol-toolbox\n    :alt: PyPI - Python Version\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n    :alt: Formatter - Black\n\n.. image:: https://img.shields.io/badge/imports-isort-ef8336.svg\n    :target: https://pycqa.github.io/isort/\n    :alt: Formatter - Isort\n\n.. image:: https://img.shields.io/badge/typing-mypy-blue\n    :target: https://github.com/PyCQA/pylint\n    :alt: Pylint\n\n.. image:: https://img.shields.io/badge/pylint-7.8-green\n    :target: https://github.com/PyCQA/pylint\n    :alt: Pylint\n\n.. image:: https://img.shields.io/pypi/l/exasol-bucketfs\n     :target: https://opensource.org/licenses/MIT\n     :alt: License\n\n.. image:: https://img.shields.io/github/last-commit/nicoretti/python-toolbox\n     :target: https://pypi.org/project/exasol-toolbox/\n     :alt: Last Commit\n\n\n🚀 Features\n------------\n\n* Centrally managed standard tasks\n    - code formatting & upgrading\n    - linting\n    - type-checking\n    - unit-tests\n    - integration-tests\n    - coverage\n    - documentation\n\n* Centrally manged core workflows\n    - workspace/project verification\n    - build and publish releases\n    - build and publish documentation\n\n* Configurable & Extensible\n    - Project configuration\n    - Event hooks\n\n🔌️ Prerequisites\n-----------------\n\n- `Python <https://www.python.org/>`_ >= 3.8\n\n💾 Installation\n----------------\n\n.. code-block:: shell\n\n    pip install exasol-toolbox\n\n📚 Documentation\n----------------\n\nThe latest documentation can be found `here <https://exasol.github.io/python-toolbox/>`_\n',
     'author': 'Nicola Coretti',
     'author_email': 'nicola.coretti@exasol.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `exasol_toolbox-0.8.0/PKG-INFO` & `exasol_toolbox-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exasol-toolbox
-Version: 0.8.0
+Version: 0.9.0
 Summary: 
 License: MIT
 Keywords: nox,tooling,ci,cd,exasol,infrastructure
 Author: Nicola Coretti
 Author-email: nicola.coretti@exasol.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,17 +15,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.1.0,<24.0.0)
 Requires-Dist: coverage (>=6.4.4,<8.0.0)
 Requires-Dist: furo (>=2022.9.15,<2023.0.0)
 Requires-Dist: importlib-resources (>=5.12.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: mypy (>=0.971)
+Requires-Dist: myst-parser (>=2.0.0,<3.0.0)
 Requires-Dist: nox (>=2022.8.7,<2023.0.0)
+Requires-Dist: pluggy (>=1.5.0,<2.0.0)
 Requires-Dist: pre-commit (>=3.1.1,<4.0.0)
-Requires-Dist: prysk (>=0.15.1)
+Requires-Dist: prysk[pytest-plugin] (>=0.17.0,<0.18.0)
 Requires-Dist: pylint (>=2.15.4)
 Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Requires-Dist: pyupgrade (>=2.38.2,<4.0.0)
 Requires-Dist: sphinx (>=5.3,<7.0)
 Requires-Dist: sphinx-copybutton (>=0.5.0,<0.6.0)
 Requires-Dist: typer[all] (>=0.7.0)
 Project-URL: Changelog, https://exasol.github.io/python-toolbox/changelog.html
```

