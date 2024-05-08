# Comparing `tmp/disrepair-0.3.1.tar.gz` & `tmp/disrepair-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disrepair-0.3.1.tar", max compression
+gzip compressed data, was "disrepair-1.0.0.tar", max compression
```

## Comparing `disrepair-0.3.1.tar` & `disrepair-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-05-18 16:01:10.205656 disrepair-0.3.1/LICENSE
--rw-r--r--   0        0        0      748 2023-05-18 16:01:10.205656 disrepair-0.3.1/README.md
--rw-r--r--   0        0        0       48 2023-05-18 16:01:10.205656 disrepair-0.3.1/disrepair/__init__.py
--rw-r--r--   0        0        0       29 2023-05-18 16:01:10.205656 disrepair-0.3.1/disrepair/__main__.py
--rwxr-xr-x   0        0        0    11619 2023-05-18 17:14:12.895684 disrepair-0.3.1/disrepair/check.py
--rw-r--r--   0        0        0      855 2023-05-18 17:14:52.599187 disrepair-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1881 1970-01-01 00:00:00.000000 disrepair-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-18 16:01:10.205656 disrepair-1.0.0/LICENSE
+-rw-r--r--   0        0        0      748 2023-05-18 16:01:10.205656 disrepair-1.0.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-08 11:02:02.678094 disrepair-1.0.0/disrepair/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-08 11:02:02.678094 disrepair-1.0.0/disrepair/__main__.py
+-rwxr-xr-x   0        0        0    12814 2024-05-08 11:02:02.678094 disrepair-1.0.0/disrepair/check.py
+-rw-r--r--   0        0        0     2081 2024-05-08 11:02:02.678094 disrepair-1.0.0/disrepair/cmd.py
+-rwxr-xr-x   0        0        0      369 2024-05-08 11:02:02.678094 disrepair-1.0.0/disrepair/options.py
+-rwxr-xr-x   0        0        0     3902 2024-05-08 11:02:02.678094 disrepair-1.0.0/disrepair/reqfile.py
+-rw-r--r--   0        0        0      863 2024-05-08 11:02:02.678094 disrepair-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1888 1970-01-01 00:00:00.000000 disrepair-1.0.0/PKG-INFO
```

### Comparing `disrepair-0.3.1/LICENSE` & `disrepair-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `disrepair-0.3.1/README.md` & `disrepair-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `disrepair-0.3.1/disrepair/check.py` & `disrepair-1.0.0/disrepair/check.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,43 @@
-#!/usr/bin/env python
-
-import os.path
-
-import click
 import requests
 from packaging.version import InvalidVersion, Version
-from pypi_simple import PyPISimple, UnsupportedContentTypeError, UnsupportedRepoVersionError, NoSuchProjectError
-from requirements.requirement import Requirement
+from pypi_simple import NoSuchProjectError, PyPISimple, UnsupportedContentTypeError, UnsupportedRepoVersionError
+from rich import box, progress
 from rich.console import Console
+from rich.prompt import Confirm
+from rich.table import Table
+
+from .options import Options
+from .reqfile import Line, LineType, ReqFile, UpdateStatus
 
-JSON_REPO = 'https://pypi.org/pypi'
-SIMPLE_REPO = "https://pypi.org/simple"
+
+TIMEOUT = 5
 
 
 class CheckFailed(Exception):
     pass
 
 
 class Disrepair:
-    errors = []
-    updates = []
-    pins = []
-    skip = []
-    up2date = []
-
-    def __init__(self, info, verbose, boring, json_repo, simple_repo, simple_only, json_only, pin_warn):
-        if not boring:
-            self.console = Console()
-        self.opt_verbose = verbose
-        self.opt_info = info
-        self.opt_boring = boring
-        self.opt_json_only = json_only
-        self.opt_simple_only = simple_only
-        self.opt_pin_warn = pin_warn
-        self.repo_json = json_repo.rstrip('/')
-        self.repo_simple = simple_repo.rstrip('/')
-
-    def error(self, name, err):
-        self.errors.append(f"⛔ {name}: {err}")
-
-    def unpinned(self, name, version):
-        self.pins.append(f"🟨 {name} ➔ {version}")
-
-    def skipped(self, name, reason):
-        if self.opt_verbose:
-            self.skip.append(f"⬜ {name}: {reason}")
-
-    def update(self, name, spec, latest, url):
-        output = f"🔼 {name} {spec} ➔ {latest}"
-        if url and self.opt_info:
-            output = f"{output}\n   {url}"
-        self.updates.append(output)
-
-    def ok(self, name, version):
-        if self.opt_verbose:
-            self.up2date.append(f"✅ {name} {version}")
-
-    def header(self, message):
-        if self.opt_boring:
-            print(f":: {message}")
-        else:
-            self.console.rule(f"[bold]{message}", align='left')
-
-    def print(self):
-        if self.updates:
-            if self.pins or (self.skip and self.opt_verbose) or (self.up2date and self.opt_verbose) or self.errors:
-                self.header("Updates")
-            for line in self.updates:
-                print(line)
-
-        if self.pins:
-            self.header("Unpinned")
-            for line in self.pins:
-                print(line)
-
-        if self.opt_verbose:
-            if self.skip:
-                self.header("Skipped")
-                for line in self.skip:
-                    print(line)
-
-            if self.up2date:
-                self.header("Up-to-date")
-                for line in self.up2date:
-                    print(line)
-
-        if self.errors:
-            self.header("Errors")
-            for line in self.errors:
-                print(line)
+    requirements_files: list[ReqFile] = []
+    updates: list[Line] = []
+    unpinned: list[Line] = []
+    up2date: list[Line] = []
+    errors: list[Line] = []
+    unsupported: list[Line] = []
+
+    def __init__(self, opt: Options):
+        self.console = Console()
+        opt.json_repo = opt.json_repo.rstrip('/')
+        opt.simple_repo = opt.simple_repo.rstrip('/')
+        self.opt = opt
 
-    def get_pypi_version(self, name: str):
+    def get_pypi_version(self, name: str) -> tuple[str | None, str | None]:
         try:
-            r = requests.get(f"{self.repo_json}/{name}/json", timeout=3)
+            r = requests.get(f"{self.opt.json_repo}/{name}/json", timeout=TIMEOUT)
         except requests.Timeout:
             raise CheckFailed("Timeout exceeded when connecting to PyPI")
         except requests.ConnectionError:
             raise CheckFailed("Unable to connect to PyPI")
 
         if r.status_code == 404:
             return None, None
@@ -133,20 +74,20 @@
                 if data['info']['home_page']:
                     return ver, data['info']['home_page']
 
             if 'package_url' in data['info']:
                 if data['info']['package_url']:
                     return ver, data['info']['package_url']
 
-        return ver, ''
+        return ver, None
 
-    def get_pypi_simple_version(self, name):
-        with PyPISimple(endpoint=self.repo_simple) as client:
+    def get_pypi_simple_version(self, name: str) -> tuple[str | None, str | None]:
+        with PyPISimple(endpoint=self.opt.simple_repo) as client:
             try:
-                page = client.get_project_page(name, timeout=5)
+                page = client.get_project_page(name, timeout=TIMEOUT)
             except requests.RequestException:
                 raise CheckFailed("Connection error")
             except UnsupportedRepoVersionError:
                 raise CheckFailed("Unsupported repo version")
             except UnsupportedContentTypeError:
                 raise CheckFailed("Unsupported content type")
             except NoSuchProjectError:
@@ -156,15 +97,15 @@
 
             if page is None:
                 raise CheckFailed("Package not found")
 
             if not page.packages:
                 raise CheckFailed("Package not found")
 
-            # There is not a guarantee that versions are listed in order.
+            # There is no guarantee that versions are listed in order.
             # We must thus check every version and pick the latest stable version.
 
             chosen_version = None
             for pkg in page.packages:
                 if pkg.version is None:
                     continue
                 try:
@@ -186,133 +127,207 @@
                             chosen_version = pkg.version
                             chosen_version_obj = pkg_version_obj
 
             if chosen_version is None:
                 raise CheckFailed("Could not find a suitable version")
 
             # The simple api offers no url :(
-            return chosen_version, ''
+            return chosen_version, None
 
-    def get_version(self, name):
+    def get_version(self, name: str) -> tuple[str | None, str | None]:
         latest = None
-        if not self.opt_simple_only:
+        if not self.opt.simple_only:
             try:
                 latest, url = self.get_pypi_version(name)
             except CheckFailed:
-                if self.opt_json_only:
+                if self.opt.json_only:
                     raise
 
-        if not self.opt_json_only:
+        if not self.opt.json_only:
             if latest is None:
                 latest, url = self.get_pypi_simple_version(name)
 
         if latest is None:
             raise CheckFailed("Package not found")
 
         return latest, url
 
-    def check_file(self, filepath, recursed=False):
-        filename = os.path.basename(filepath)
-        lineno = 0
-
-        with open(filepath, 'r') as fh:
-            for line in fh.readlines():
-                lineno += 1
-
-                if line.strip() == '':
-                    continue
-
-                elif not line or line.startswith('#'):
-                    continue
-
-                elif line.startswith('-r') or line.startswith('--requirement'):
-                    if recursed:
-                        self.error(f"{filename}:{lineno}", 'Will only recurse into files once')
-                        continue
-
-                    _, new_filename = line.split()
-                    new_file = os.path.join(os.path.dirname(filepath or '.'), new_filename)
-                    if not os.path.exists(new_file):
-                        self.error(new_file, 'File does not exist')
-                    else:
-                        self.check_file(new_file, recursed=True)
-
-                elif line.startswith('-'):
-                    # Don't support any other options.
-                    continue
-
-                else:
-                    try:
-                        req = Requirement.parse(line)
-                    except Exception as ex:
-                        self.error(f"{filename}:{lineno}", f"Could not parse line ({ex})")
-                        continue
-
-                    if len(req.specs) == 0:
-                        if self.opt_pin_warn:
-                            try:
-                                latest, url = self.get_version(req.name)
-                            except CheckFailed as ex:
-                                self.error(req.name, ex)
-                                continue
-                            self.unpinned(req.name, latest)
+    def _parse_file(self, filename: str) -> None:
+        rf = ReqFile(filename)
+        self.requirements_files.append(rf)
+
+        for fp in rf.other_files:
+            self._parse_file(fp)
+
+    def _fetch_metadata(self) -> None:
+        lines: list[Line] = []
+        for reqfile in self.requirements_files:
+            lines.extend(reqfile.lines)
+
+        with progress.Progress(
+            progress.SpinnerColumn(),
+            progress.TextColumn("[progress.description]{task.description}"),
+            progress.BarColumn(),
+            progress.TaskProgressColumn(),
+            progress.MofNCompleteColumn(),
+            console=self.console,
+            transient=True,
+        ) as status:
+            task = status.add_task("[bold]Checking", total=len(lines))
+            for line in lines:
+                if line.ltype == LineType.requirement:
+                    if line.pkgname:
+                        try:
+                            line.latest, line.url = self.get_version(line.pkgname)
+                        except CheckFailed as ex:
+                            line.error = str(ex)
+                            self.errors.append(line)
                         else:
-                            self.skipped(req.name, "Version not pinned")
-                        continue
-
-                    if len(req.specs) != 1:
-                        self.skipped(req.name, 'Unsupported requirement spec')
-                        continue
-                    if req.specs[0][0] not in ['==', '>=']:
-                        self.skipped(req.name, 'Unsupported requirement spec')
-                        continue
-                    spec = req.specs[0][1]
-
-                    try:
-                        latest, url = self.get_version(req.name)
-                    except CheckFailed as ex:
-                        self.error(req.name, ex)
-                        continue
-
-                    ver_latest = Version(latest)
-                    ver_spec = Version(spec)
-                    if ver_latest > ver_spec:
-                        self.update(req.name, spec, latest, url)
-
-                    elif ver_latest == ver_spec:
-                        self.ok(req.name, latest)
-                    elif ver_latest < ver_spec:
-                        self.error(
-                            req.name,
-                            f"Specified version ({spec}) is greater than the latest available ({latest})"
-                        )
-
-    def check(self, filepath):
-        if self.opt_boring:
-            self.check_file(filepath)
-        else:
-            with self.console.status("[bold]Checking requirements..."):
-                self.check_file(filepath)
-        self.print()
-
-
-@click.command()
-@click.argument('filename')
-@click.option('--verbose', '-v', is_flag=True, help='Show all package statuses')
-@click.option('--info', '-i', is_flag=True, help='Show likely package changelog/info links')
-@click.option('--boring', '-b', is_flag=True, help='Disable the rich text formatting')
-@click.option('--json-repo', '-j', default=JSON_REPO, help='Repository URL for the JSON API')
-@click.option('--simple-repo', '-s', default=SIMPLE_REPO, help='Repository URL for the Simple API')
-@click.option('--simple-only', '-S', is_flag=True, help='Only use the Simple API to lookup versions')
-@click.option('--json-only', '-J', is_flag=True, help='Only use the JSON API to lookup versions')
-@click.option('--pin-warn', '-p', is_flag=True, help='Warn when a package version is not pinned')
-@click.pass_context
-def check(ctx, filename, info, verbose, boring, json_repo, simple_repo, simple_only, json_only, pin_warn):
-    if simple_only and json_only:
-        ctx.fail("--simple-only and --json-only cannot both be set")
-
-    t = Disrepair(info, verbose, boring, json_repo, simple_repo, simple_only, json_only, pin_warn)
-    t.check(filename)
-
-
-if __name__ == '__main__':
-    check()
+                            if line.spec is None:
+                                line.status = UpdateStatus.unpinned
+                                self.unpinned.append(line)
+                            else:
+                                if line.latest:
+                                    ver_latest = Version(line.latest)
+                                    ver_spec = Version(line.spec)
+                                    if ver_latest > ver_spec:
+                                        line.status = UpdateStatus.behind
+                                        self.updates.append(line)
+
+                                    elif ver_latest == ver_spec:
+                                        line.status = UpdateStatus.ok
+                                        self.up2date.append(line)
+
+                                    elif ver_latest < ver_spec:
+                                        line.error = (
+                                            "Specified version "
+                                            f"({line.spec}) is greater than the "
+                                            f"latest published version ({line.latest})"
+                                        )
+                                        self.errors.append(line)
+
+                elif line.ltype == LineType.error:
+                    self.errors.append(line)
+                elif line.ltype == LineType.unsupported:
+                    self.unsupported.append(line)
+
+                status.update(task, advance=1)
+
+    def _print_reqs(self) -> None:
+        table = Table(box=box.SIMPLE_HEAVY)
+        table.add_column("Package", no_wrap=True)
+        if len(self.requirements_files) > 1:
+            table.add_column("Location", no_wrap=True)
+        table.add_column("Spec", no_wrap=True)
+        table.add_column("Latest", no_wrap=True)
+        if self.opt.info:
+            table.add_column("URL")
+
+        if self.opt.verbose:
+            for line in self.up2date:
+                row = [line.pkgname]
+                if len(self.requirements_files) > 1:
+                    row.append(line.location)
+                row.extend([line.spec, '✅ Up to date'])
+                if self.opt.info:
+                    row.append(line.url)
+                table.add_row(*row)
+
+        for line in self.updates:
+            row = [line.pkgname]
+            if len(self.requirements_files) > 1:
+                row.append(line.location)
+            row.extend([line.spec, line.latest])
+            if self.opt.info:
+                row.append(line.url)
+            table.add_row(*row)
+
+        if self.opt.unpinned:
+            for line in self.unpinned:
+                row = [line.pkgname]
+                if len(self.requirements_files) > 1:
+                    row.append(line.location)
+                row.extend(['⚠️  Unpinned', line.latest])
+                if self.opt.info:
+                    row.append(line.url)
+                table.add_row(*row)
+
+        if table.rows:
+            self.console.print(table)
+
+    def _print_errors_unsupported(self) -> None:
+        table = Table(box=box.SIMPLE_HEAVY)
+        table.add_column("Line")
+        table.add_column("Package")
+        table.add_column("Error")
+
+        for line in self.errors:
+            loc = str(line.lineno)
+            if len(self.requirements_files) > 1:
+                loc = line.location
+            table.add_row(loc, line.pkgname or '', line.error)
+
+        if self.opt.verbose:
+            for line in self.unsupported:
+                loc = str(line.lineno)
+                if len(self.requirements_files) > 1:
+                    loc = line.location
+                table.add_row(loc, line.pkgname or '', line.error)
+
+        if table.rows:
+            self.console.print(table)
+
+    def cmd_update(self, filename: str) -> None:
+        self._parse_file(filename)
+        self._fetch_metadata()
+
+        printed = False
+        multiple = len(self.requirements_files) > 1
+
+        for reqfile in self.requirements_files:
+            num_updated = 0
+
+            for line in reqfile.lines:
+                if line.ltype == LineType.requirement:
+                    if line.status == UpdateStatus.behind or line.status == UpdateStatus.unpinned:
+                        if self.opt.auto_update:
+                            do_update = True
+                        else:
+                            if printed:
+                                self.console.print('')
+                            printed = True
+                            if multiple:
+                                self.console.print(f'[bold]{line.pkgname}[/bold] {reqfile.filename}')
+                            else:
+                                self.console.print(f'[bold]{line.pkgname}')
+                            if self.opt.info:
+                                if line.url is not None:
+                                    self.console.print(line.url)
+                            self.console.print(f'Current: {line.spec or "Unpinned"}')
+                            self.console.print(f'Latest: {line.latest}')
+                            do_update = Confirm.ask("Do you want to update?", default=True)
+
+                        if do_update:
+                            num_updated += 1
+                            line.line = f'{line.pkgname}=={line.latest}'
+
+        for reqfile in self.requirements_files:
+            if num_updated:
+                with open(reqfile.filepath, mode='w') as fp:
+                    for line in reqfile.lines:
+                        if line.line is not None:
+                            fp.write(line.line)
+                            if not line.line.endswith('\n'):
+                                fp.write('\n')
+
+                if self.opt.auto_update or self.errors:
+                    self.console.print(
+                        f"{reqfile.filename}: {num_updated} package{'s' if num_updated > 1 else ''} updated"
+                    )
+
+        self._print_errors_unsupported()
+
+    def cmd_check(self, filename: str) -> None:
+        self._parse_file(filename)
+        self._fetch_metadata()
+        self._print_reqs()
+        self._print_errors_unsupported()
```

### Comparing `disrepair-0.3.1/pyproject.toml` & `disrepair-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "disrepair"
-version = "0.3.1"
-description = "Checks for out-of-date Python packages in requirements files"
+version = "1.0.0"
+description = "Check and update out-of-date Python packages in requirements files"
 authors = ["David Bell <dave@evad.io>"]
 
 license = "GPL3"
 readme = "README.md"
 homepage = "https://github.com/divad/disrepair"
 repository = "https://github.com/divad/disrepair"
 classifiers = [
@@ -15,22 +15,22 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 click = ">=8.0"
 requests = ">=2.0"
 packaging = ">=21.0"
-pypi-simple = ">=0.8.0"
-requirements-parser = ">=0.5.0"
+pypi-simple = ">=1.5.0"
+requirements-parser = ">=0.9.0"
 rich = ">=12.0"
 setuptools = ">=60"
 
 [tool.poetry.scripts]
-disrepair = 'disrepair:check'
+disrepair = 'disrepair:cmd.cli'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `disrepair-0.3.1/PKG-INFO` & `disrepair-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: disrepair
-Version: 0.3.1
-Summary: Checks for out-of-date Python packages in requirements files
+Version: 1.0.0
+Summary: Check and update out-of-date Python packages in requirements files
 Home-page: https://github.com/divad/disrepair
 License: GPL3
 Author: David Bell
 Author-email: dave@evad.io
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Dist: click (>=8.0)
 Requires-Dist: packaging (>=21.0)
-Requires-Dist: pypi-simple (>=0.8.0)
+Requires-Dist: pypi-simple (>=1.5.0)
 Requires-Dist: requests (>=2.0)
-Requires-Dist: requirements-parser (>=0.5.0)
+Requires-Dist: requirements-parser (>=0.9.0)
 Requires-Dist: rich (>=12.0)
 Requires-Dist: setuptools (>=60)
 Project-URL: Repository, https://github.com/divad/disrepair
 Description-Content-Type: text/markdown
 
 # disrepair
 Checks for out-of-date Python packages in requirements files
```

