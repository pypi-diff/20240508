# Comparing `tmp/django_q_registry-0.2.1.tar.gz` & `tmp/django_q_registry-0.3.0.tar.gz`

## Comparing `django_q_registry-0.2.1.tar` & `django_q_registry-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,32 @@
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/RELEASING.md
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/noxfile.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/.vscode/extensions.json
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/.vscode/settings.json.example
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/docs/conf.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/docs/index.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/docs/requirements.in
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/docs/development/just.md
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/src/django_q_registry/__init__.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/src/django_q_registry/apps.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/src/django_q_registry/conf.py
--rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/src/django_q_registry/models.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/src/django_q_registry/registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/src/django_q_registry/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/src/django_q_registry/management/commands/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/src/django_q_registry/management/commands/setup_periodic_tasks.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/src/django_q_registry/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/src/django_q_registry/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/tests/settings.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/tests/test_conf.py
--rw-r--r--   0        0        0     9855 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/tests/test_models.py
--rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/tests/test_registry.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/tests/test_setup_periodic_tasks.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/tests/test_version.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/.gitignore
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/AUTHORS.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/LICENSE
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/README.md
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 django_q_registry-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/RELEASING.md
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/noxfile.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/docs/index.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/docs/development/just.md
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/__init__.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/apps.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/conf.py
+-rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/models.py
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/management/commands/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/management/commands/setup_periodic_tasks.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/settings.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/test_conf.py
+-rw-r--r--   0        0        0     9855 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/test_models.py
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/test_registry.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/test_setup_periodic_tasks.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/test_version.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/.gitignore
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/AUTHORS.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/README.md
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/PKG-INFO
```

### Comparing `django_q_registry-0.2.1/CHANGELOG.md` & `django_q_registry-0.3.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,63 +11,75 @@
 ### Changed - for changes in existing functionality
 ### Deprecated - for soon-to-be removed features
 ### Removed - for now removed features
 ### Fixed - for any bug fixes
 ### Security - in case of vulnerabilities
 [${version}]: https://github.com/westerveltco/django-q-registry/releases/tag/v${version}
 -->
+
 ## [Unreleased]
 
+## [0.3.0]
+
+### Changed
+
+-   Now using v2024.18 of `django-twc-package`.
+
+### Removed
+
+-   Dropped support for Django 3.2.
+
 ## [0.2.1]
 
 ### Added
 
-- Added a `TaskRegistry.created_tasks` attribute to store the `Task` instances created by the `TaskRegistry`.
+-   Added a `TaskRegistry.created_tasks` attribute to store the `Task` instances created by the `TaskRegistry`.
 
 ### Changed
 
-- Now using v2024.12 of `django-twc-package`.
+-   Now using v2024.12 of `django-twc-package`.
 
 ### Fixed
 
-- Fixed a bug in the `setup_periodic_tasks` management command where newly created tasks via `Task.objects.create_from_registry` were immediately deleted via `Task.objects.delete_dangling_objects`. Newly created tasks are now added to the `TaskRegistry.created_tasks` attribute and are only deleted if they are not in the `TaskRegistry.created_tasks` attribute.
+-   Fixed a bug in the `setup_periodic_tasks` management command where newly created tasks via `Task.objects.create_from_registry` were immediately deleted via `Task.objects.delete_dangling_objects`. Newly created tasks are now added to the `TaskRegistry.created_tasks` attribute and are only deleted if they are not in the `TaskRegistry.created_tasks` attribute.
 
 ## [0.2.0]
 
 ### Added
 
-- Refactored the `django_q_registry.registry.Task` dataclass into a `django_q_registry.models.Task` Django model. This should make it more flexible and robust for registering tasks and the associated `django_q.models.Schedule` instances.
+-   Refactored the `django_q_registry.registry.Task` dataclass into a `django_q_registry.models.Task` Django model. This should make it more flexible and robust for registering tasks and the associated `django_q.models.Schedule` instances.
 
 ### Changed
 
-- Now using [`django-twc-package`](https://github.com/westerveltco/django-twc-package) template for repository and package structure.
-- The default for the `Q_REGISTRY["PERIOIDIC_TASK_SUFFIX"]` app setting has been changed from `"- CRON"` to `"- QREGISTRY"`.
-- All database logic has been moved from the `TaskRegistry` to the `setup_periodic_tasks` management command.
-- GitHub Actions `test` workflow now uses the output of `nox -l --json` to dynamically generate the test matrix.
+-   Now using [`django-twc-package`](https://github.com/westerveltco/django-twc-package) template for repository and package structure.
+-   The default for the `Q_REGISTRY["PERIOIDIC_TASK_SUFFIX"]` app setting has been changed from `"- CRON"` to `"- QREGISTRY"`.
+-   All database logic has been moved from the `TaskRegistry` to the `setup_periodic_tasks` management command.
+-   GitHub Actions `test` workflow now uses the output of `nox -l --json` to dynamically generate the test matrix.
 
 ### Fixed
 
-- Fixed a bug in the hashing of a `Task` where the `hash` function was passed unhashable values (e.g. a `dict`). Thanks to [@Tobi-De](https://github.com/Tobi-De) for the bug report ([#6](https://github.com/westerveltco/django-q-registry/issues/6)).
+-   Fixed a bug in the hashing of a `Task` where the `hash` function was passed unhashable values (e.g. a `dict`). Thanks to [@Tobi-De](https://github.com/Tobi-De) for the bug report ([#6](https://github.com/westerveltco/django-q-registry/issues/6)).
 
 ## [0.1.0]
 
 Initial release!
 
 ### Added
 
-- Initial documentation.
-- Initial tests.
-- Initial CI/CD (GitHub Actions).
-- A registry for Django Q2 periodic tasks.
-  - `registry.register` function for registering periodic tasks with a convenience decorator `register_task`.
-  - A `TASKS` setting for registering periodic tasks from Django settings.
-- Autodiscovery of periodic tasks from a Django project's `tasks.py` files.
-- A `setup_periodic_tasks` management command for setting up periodic tasks in the Django Q2 broker.
+-   Initial documentation.
+-   Initial tests.
+-   Initial CI/CD (GitHub Actions).
+-   A registry for Django Q2 periodic tasks.
+    -   `registry.register` function for registering periodic tasks with a convenience decorator `register_task`.
+    -   A `TASKS` setting for registering periodic tasks from Django settings.
+-   Autodiscovery of periodic tasks from a Django project's `tasks.py` files.
+-   A `setup_periodic_tasks` management command for setting up periodic tasks in the Django Q2 broker.
 
 ### New Contributors
 
-- Josh Thomas <josh@joshthomas.dev> (maintainer)
+-   Josh Thomas <josh@joshthomas.dev> (maintainer)
 
-[unreleased]: https://github.com/westerveltco/django-q-registry/compare/v0.2.1...HEAD
+[unreleased]: https://github.com/westerveltco/django-q-registry/compare/v0.3.0...HEAD
 [0.1.0]: https://github.com/westerveltco/django-q-registry/releases/tag/v0.1.0
 [0.2.0]: https://github.com/westerveltco/django-q-registry/releases/tag/v0.2.0
 [0.2.1]: https://github.com/westerveltco/django-q-registry/releases/tag/v0.2.1
+[0.3.0]: https://github.com/westerveltco/django-q-registry/releases/tag/v0.3.0
```

### Comparing `django_q_registry-0.2.1/CONTRIBUTING.md` & `django_q_registry-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/RELEASING.md` & `django_q_registry-0.3.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/noxfile.py` & `django_q_registry-0.3.0/noxfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from __future__ import annotations
 
 import os
 from pathlib import Path
 
 import nox
 
+nox.options.default_venv_backend = "uv|virtualenv"
+nox.options.reuse_existing_virtualenvs = True
+
 PY38 = "3.8"
 PY39 = "3.9"
 PY310 = "3.10"
 PY311 = "3.11"
 PY312 = "3.12"
 PY_VERSIONS = [PY38, PY39, PY310, PY311, PY312]
 PY_DEFAULT = PY_VERSIONS[0]
 PY_LATEST = PY_VERSIONS[-1]
 
-DJ32 = "3.2"
 DJ42 = "4.2"
 DJ50 = "5.0"
 DJMAIN = "main"
 DJMAIN_MIN_PY = PY310
-DJ_VERSIONS = [DJ32, DJ42, DJ50, DJMAIN]
-DJ_LTS = [DJ32, DJ42]
+DJ_VERSIONS = [DJ42, DJ50, DJMAIN]
+DJ_LTS = [DJ42]
 DJ_DEFAULT = DJ_LTS[0]
 DJ_LATEST = DJ_VERSIONS[-2]
 
 
 def version(ver: str) -> tuple[int, ...]:
     """Convert a string version to a tuple of ints, e.g. "3.10" -> (3, 10)"""
     return tuple(map(int, ver.split(".")))
@@ -33,18 +35,14 @@
 def should_skip(python: str, django: str) -> bool:
     """Return True if the test should be skipped"""
 
     if django == DJMAIN and version(python) < version(DJMAIN_MIN_PY):
         # Django main requires Python 3.10+
         return True
 
-    if django == DJ32 and version(python) >= version(PY312):
-        # Django 3.2 requires Python < 3.12
-        return True
-
     if django == DJ50 and version(python) < version(PY310):
         # Django 5.0 requires Python 3.10+
         return True
 
     return False
 
 
@@ -60,27 +58,32 @@
         (python, django)
         for python in PY_VERSIONS
         for django in DJ_VERSIONS
         if not should_skip(python, django)
     ],
 )
 def tests(session, django):
-    session.install(".[dev]")
+    session.install("django-q-registry[dev] @ .")
 
     if django == DJMAIN:
-        session.install("https://github.com/django/django/archive/refs/heads/main.zip")
+        session.install(
+            "django @ https://github.com/django/django/archive/refs/heads/main.zip"
+        )
     else:
         session.install(f"django=={django}")
 
-    session.run("python", "-m", "pytest", *session.posargs if session.posargs else "")
+    if session.posargs:
+        session.run("python", "-m", "pytest", *session.posargs)
+    else:
+        session.run("python", "-m", "pytest")
 
 
 @nox.session
 def coverage(session):
-    session.install(".[dev]")
+    session.install("django-q-registry[dev] @ .")
     session.run("python", "-m", "pytest", "--cov=django_q_registry")
 
     try:
         summary = os.environ["GITHUB_STEP_SUMMARY"]
         with Path(summary).open("a") as output_buffer:
             output_buffer.write("")
             output_buffer.write("### Coverage\n\n")
@@ -101,15 +104,15 @@
         )
 
     session.run("python", "-m", "coverage", "report")
 
 
 @nox.session
 def lint(session):
-    session.install(".[lint]")
+    session.install("django-q-registry[lint] @ .")
     session.run("python", "-m", "pre_commit", "run", "--all-files")
 
 
 @nox.session
 def mypy(session):
-    session.install(".[dev]")
+    session.install("django-q-registry[dev] @ .")
     session.run("python", "-m", "mypy", ".")
```

### Comparing `django_q_registry-0.2.1/docs/conf.py` & `django_q_registry-0.3.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,18 @@
 html_theme = "furo"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
+html_css_files = [
+    "css/custom.css",
+]
+
 html_title = project
 
 html_theme_options = {
     "footer_icons": [
         {
             "name": "GitHub",
             "url": "https://github.com/westerveltco/django-q-registry",
```

### Comparing `django_q_registry-0.2.1/docs/development/just.md` & `django_q_registry-0.3.0/docs/development/just.md`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/src/django_q_registry/conf.py` & `django_q_registry-0.3.0/src/django_q_registry/conf.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/src/django_q_registry/models.py` & `django_q_registry-0.3.0/src/django_q_registry/models.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/src/django_q_registry/registry.py` & `django_q_registry-0.3.0/src/django_q_registry/registry.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/src/django_q_registry/management/commands/setup_periodic_tasks.py` & `django_q_registry-0.3.0/src/django_q_registry/management/commands/setup_periodic_tasks.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/src/django_q_registry/migrations/0001_initial.py` & `django_q_registry-0.3.0/src/django_q_registry/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/tests/conftest.py` & `django_q_registry-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/tests/settings.py` & `django_q_registry-0.3.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/tests/test_conf.py` & `django_q_registry-0.3.0/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/tests/test_models.py` & `django_q_registry-0.3.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/tests/test_registry.py` & `django_q_registry-0.3.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/tests/test_setup_periodic_tasks.py` & `django_q_registry-0.3.0/tests/test_setup_periodic_tasks.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/.gitignore` & `django_q_registry-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/LICENSE` & `django_q_registry-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.2.1/README.md` & `django_q_registry-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # django-q-registry
 
 [![PyPI](https://img.shields.io/pypi/v/django-q-registry)](https://pypi.org/project/django-q-registry/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-q-registry)
-![Django Version](https://img.shields.io/badge/django-3.2%20%7C%204.2%20%7C%205.0-%2344B78B?labelColor=%23092E20)
+![Django Version](https://img.shields.io/badge/django-4.2%20%7C%205.0-%2344B78B?labelColor=%23092E20)
 <!-- https://shields.io/badges -->
-<!-- django-3.2 | 4.2 | 5.0-#44B78B -->
+<!-- django-4.2 | 5.0-#44B78B -->
 <!-- labelColor=%23092E20 -->
 
 A Django app to register periodic Django Q tasks.
 
 ## Requirements
 
 - Python 3.8, 3.9, 3.10, 3.11, 3.12
-- Django 3.2, 4.2, 5.0
+- Django 4.2, 5.0
 - Django Q2 1.4.3+
   - This package has only been tested with the Django ORM broker.
 
 ## Getting Started
 
 1. Install the package from PyPI:
```

### Comparing `django_q_registry-0.2.1/pyproject.toml` & `django_q_registry-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 requires = ["hatchling"]
 
 [project]
 authors = [{name = "Josh Thomas", email = "josh@joshthomas.dev"}]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: Django",
-  "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.2",
   "Framework :: Django :: 5.0",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython"
 ]
-dependencies = ["django>=3.2", "django_q2>=1.4.3"]
+dependencies = ["django>=4.2", "django_q2>=1.4.3"]
 description = "A Django app to register periodic Django Q tasks."
 dynamic = ["version"]
 keywords = []
 license = {file = "LICENSE"}
 name = "django-q-registry"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -39,15 +38,15 @@
   "coverage[toml]",
   "django-stubs",
   "django-stubs-ext",
   "faker",
   "hatch",
   "mypy",
   "model-bakery",
-  "nox",
+  "nox[uv]",
   "pytest",
   "pytest-cov",
   "pytest-django",
   "pytest-randomly",
   "pytest-reverse",
   "pytest-xdist"
 ]
@@ -66,15 +65,15 @@
 Documentation = "https://django-q-registry.westervelt.dev/"
 Issues = "https://github.com/westerveltco/django-q-registry/issues"
 Source = "https://github.com/westerveltco/django-q-registry"
 
 [tool.bumpver]
 commit = true
 commit_message = ":bookmark: bump version {old_version} -> {new_version}"
-current_version = "0.2.1"
+current_version = "0.3.0"
 push = false  # set to false for CI
 tag = false
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 
 [tool.bumpver.file_patterns]
 ".copier/package.yml" = ['current_version: {version}']
 "src/django_q_registry/__init__.py" = ['__version__ = "{version}"']
@@ -137,16 +136,14 @@
 django_find_project = false
 norecursedirs = ".* bin build dist *.egg htmlcov logs node_modules templates venv"
 python_files = "tests.py test_*.py *_tests.py"
 pythonpath = "src"
 testpaths = ["tests"]
 
 [tool.ruff]
-# Allow unused variables when underscore-prefixed.
-dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 # Exclude a variety of commonly ignored directories.
 exclude = [
   ".bzr",
   ".direnv",
   ".eggs",
   ".git",
   ".github",
@@ -161,44 +158,48 @@
   "build",
   "dist",
   "migrations",
   "node_modules",
   "venv"
 ]
 extend-include = ["*.pyi?"]
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["A", "B", "C", "D", "E", "F", "I"]
-ignore = ["E501", "E741"]  # temporary
 indent-width = 4
 # Same as Black.
 line-length = 88
-select = [
-  "B",  # flake8-bugbear
-  "E",  # Pycodestyle
-  "F",  # Pyflakes
-  "I",  # isort
-  "UP"  # pyupgrade
-]
-# Assume Python >3.8.
+# Assume Python >3.8
 target-version = "py38"
-unfixable = []
 
 [tool.ruff.format]
 # Like Black, indent with spaces, rather than tabs.
 indent-style = "space"
 # Like Black, automatically detect the appropriate line ending.
 line-ending = "auto"
 # Like Black, use double quotes for strings.
 quote-style = "double"
 
-[tool.ruff.isort]
+[tool.ruff.lint]
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = ["A", "B", "C", "D", "E", "F", "I"]
+ignore = ["E501", "E741"]  # temporary
+select = [
+  "B",  # flake8-bugbear
+  "E",  # Pycodestyle
+  "F",  # Pyflakes
+  "I",  # isort
+  "UP"  # pyupgrade
+]
+unfixable = []
+
+[tool.ruff.lint.isort]
 force-single-line = true
 known-first-party = ["django_q_registry"]
 required-imports = ["from __future__ import annotations"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
-[tool.ruff.pyupgrade]
+[tool.ruff.lint.pyupgrade]
 # Preserve types, even if a file imports `from __future__ import annotations`.
 keep-runtime-typing = true
```

### Comparing `django_q_registry-0.2.1/PKG-INFO` & `django_q_registry-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: django-q-registry
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Django app to register periodic Django Q tasks.
 Project-URL: Documentation, https://django-q-registry.westervelt.dev/
 Project-URL: Issues, https://github.com/westerveltco/django-q-registry/issues
 Project-URL: Source, https://github.com/westerveltco/django-q-registry
 Author-email: Josh Thomas <josh@joshthomas.dev>
 License: MIT License
         
@@ -15,15 +15,14 @@
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 License-File: AUTHORS.md
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -31,27 +30,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Requires-Dist: django-q2>=1.4.3
-Requires-Dist: django>=3.2
+Requires-Dist: django>=4.2
 Provides-Extra: dev
 Requires-Dist: bumpver; extra == 'dev'
 Requires-Dist: copier; extra == 'dev'
 Requires-Dist: copier-templates-extensions; extra == 'dev'
 Requires-Dist: coverage[toml]; extra == 'dev'
 Requires-Dist: django-stubs; extra == 'dev'
 Requires-Dist: django-stubs-ext; extra == 'dev'
 Requires-Dist: faker; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: model-bakery; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
-Requires-Dist: nox; extra == 'dev'
+Requires-Dist: nox[uv]; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-django; extra == 'dev'
 Requires-Dist: pytest-randomly; extra == 'dev'
 Requires-Dist: pytest-reverse; extra == 'dev'
 Requires-Dist: pytest-xdist; extra == 'dev'
 Provides-Extra: docs
@@ -66,25 +65,25 @@
 Requires-Dist: pre-commit; extra == 'lint'
 Description-Content-Type: text/markdown
 
 # django-q-registry
 
 [![PyPI](https://img.shields.io/pypi/v/django-q-registry)](https://pypi.org/project/django-q-registry/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-q-registry)
-![Django Version](https://img.shields.io/badge/django-3.2%20%7C%204.2%20%7C%205.0-%2344B78B?labelColor=%23092E20)
+![Django Version](https://img.shields.io/badge/django-4.2%20%7C%205.0-%2344B78B?labelColor=%23092E20)
 <!-- https://shields.io/badges -->
-<!-- django-3.2 | 4.2 | 5.0-#44B78B -->
+<!-- django-4.2 | 5.0-#44B78B -->
 <!-- labelColor=%23092E20 -->
 
 A Django app to register periodic Django Q tasks.
 
 ## Requirements
 
 - Python 3.8, 3.9, 3.10, 3.11, 3.12
-- Django 3.2, 4.2, 5.0
+- Django 4.2, 5.0
 - Django Q2 1.4.3+
   - This package has only been tested with the Django ORM broker.
 
 ## Getting Started
 
 1. Install the package from PyPI:
```

