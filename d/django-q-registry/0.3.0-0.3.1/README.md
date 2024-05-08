# Comparing `tmp/django_q_registry-0.3.0.tar.gz` & `tmp/django_q_registry-0.3.1.tar.gz`

## Comparing `django_q_registry-0.3.0.tar` & `django_q_registry-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/RELEASING.md
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/noxfile.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/docs/conf.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/docs/index.md
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/docs/_static/css/custom.css
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/docs/development/just.md
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/__init__.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/apps.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/conf.py
--rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/models.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/management/commands/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/management/commands/setup_periodic_tasks.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/src/django_q_registry/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/settings.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/test_conf.py
--rw-r--r--   0        0        0     9855 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/test_models.py
--rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/test_registry.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/test_setup_periodic_tasks.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/tests/test_version.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/.gitignore
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/AUTHORS.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/LICENSE
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/README.md
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 django_q_registry-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/RELEASING.md
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/noxfile.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/docs/conf.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/docs/index.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/docs/development/just.md
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/src/django_q_registry/__init__.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/src/django_q_registry/apps.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/src/django_q_registry/conf.py
+-rw-r--r--   0        0        0     9814 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/src/django_q_registry/models.py
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/src/django_q_registry/registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/src/django_q_registry/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/src/django_q_registry/management/commands/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/src/django_q_registry/management/commands/setup_periodic_tasks.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/src/django_q_registry/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/src/django_q_registry/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/tests/settings.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/tests/test_conf.py
+-rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/tests/test_models.py
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/tests/test_registry.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/tests/test_setup_periodic_tasks.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/tests/test_version.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/.gitignore
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/AUTHORS.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/README.md
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 django_q_registry-0.3.1/PKG-INFO
```

### Comparing `django_q_registry-0.3.0/CHANGELOG.md` & `django_q_registry-0.3.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 ### Fixed - for any bug fixes
 ### Security - in case of vulnerabilities
 [${version}]: https://github.com/westerveltco/django-q-registry/releases/tag/v${version}
 -->
 
 ## [Unreleased]
 
+## [0.3.1]
+
+### Fixed
+
+-   Correctly JSON serialize `Task` kwargs when going from the in-memory representation contained in the task registry to actual model instances in the database. First reported by [@joshuadavidthomas](https://github.com/joshuadavidthomas) in [#30](https://github.com/westerveltco/django-q-registry/issues/30).
+
 ## [0.3.0]
 
 ### Changed
 
 -   Now using v2024.18 of `django-twc-package`.
 
 ### Removed
@@ -74,12 +80,13 @@
 -   Autodiscovery of periodic tasks from a Django project's `tasks.py` files.
 -   A `setup_periodic_tasks` management command for setting up periodic tasks in the Django Q2 broker.
 
 ### New Contributors
 
 -   Josh Thomas <josh@joshthomas.dev> (maintainer)
 
-[unreleased]: https://github.com/westerveltco/django-q-registry/compare/v0.3.0...HEAD
+[unreleased]: https://github.com/westerveltco/django-q-registry/compare/v0.3.1...HEAD
 [0.1.0]: https://github.com/westerveltco/django-q-registry/releases/tag/v0.1.0
 [0.2.0]: https://github.com/westerveltco/django-q-registry/releases/tag/v0.2.0
 [0.2.1]: https://github.com/westerveltco/django-q-registry/releases/tag/v0.2.1
 [0.3.0]: https://github.com/westerveltco/django-q-registry/releases/tag/v0.3.0
+[0.3.1]: https://github.com/westerveltco/django-q-registry/releases/tag/v0.3.1
```

### Comparing `django_q_registry-0.3.0/CONTRIBUTING.md` & `django_q_registry-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/RELEASING.md` & `django_q_registry-0.3.1/RELEASING.md`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/noxfile.py` & `django_q_registry-0.3.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/docs/conf.py` & `django_q_registry-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/docs/development/just.md` & `django_q_registry-0.3.1/docs/development/just.md`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/src/django_q_registry/conf.py` & `django_q_registry-0.3.1/src/django_q_registry/conf.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/src/django_q_registry/models.py` & `django_q_registry-0.3.1/src/django_q_registry/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             if task.pk:
                 logger.error(f"Task {task.pk} has already been registered")
                 continue
 
             obj, _ = self.update_or_create(
                 name=task.name,
                 func=task.func,
-                kwargs=task.kwargs,
+                kwargs=json.dumps(task.kwargs, cls=DjangoJSONEncoder),
             )
 
             if obj.q_schedule is None:
                 obj.q_schedule = Schedule.objects.create(
                     **task.to_schedule_dict(),
                 )
                 obj.save()
```

### Comparing `django_q_registry-0.3.0/src/django_q_registry/registry.py` & `django_q_registry-0.3.1/src/django_q_registry/registry.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/src/django_q_registry/management/commands/setup_periodic_tasks.py` & `django_q_registry-0.3.1/src/django_q_registry/management/commands/setup_periodic_tasks.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/src/django_q_registry/migrations/0001_initial.py` & `django_q_registry-0.3.1/src/django_q_registry/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/tests/conftest.py` & `django_q_registry-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/tests/settings.py` & `django_q_registry-0.3.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/tests/test_conf.py` & `django_q_registry-0.3.1/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/tests/test_models.py` & `django_q_registry-0.3.1/tests/test_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import itertools
+from datetime import datetime
 
 import pytest
 from django_q.models import Schedule
 from model_bakery import baker
 
 from django_q_registry.conf import app_settings
 from django_q_registry.models import Task
@@ -257,14 +258,29 @@
             _quantity=3,
         )
 
         Task.objects.delete_dangling_objects(registry)
 
         assert Schedule.objects.count() == len(schedules)
 
+    def test_create_in_memory_with_datetime(self):
+        # sanity check for this related issue:
+        # https://github.com/westerveltco/django-q-registry/issues/30
+        def test_task():
+            pass
+
+        task_kwargs = {
+            "datetime": datetime(2024, 5, 8),
+        }
+
+        in_memory_task = Task.objects.create_in_memory(test_task, task_kwargs)
+
+        assert not in_memory_task.pk
+        assert in_memory_task.kwargs["datetime"] == task_kwargs["datetime"]
+
 
 class TestTask:
     def test_hash_in_memory(self):
         task = Task(
             name="test",
             func="tests.test_task.test_hash",
             kwargs={"foo": "bar"},
```

### Comparing `django_q_registry-0.3.0/tests/test_registry.py` & `django_q_registry-0.3.1/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/tests/test_setup_periodic_tasks.py` & `django_q_registry-0.3.1/tests/test_setup_periodic_tasks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import itertools
+from datetime import datetime
 
 import pytest
 from django_q.models import Schedule
 from model_bakery import baker
 
 from django_q_registry.conf import app_settings
 from django_q_registry.management.commands import setup_periodic_tasks
@@ -15,71 +16,82 @@
 
 
 @registry.register(name="test_task")
 def task():
     return "test"
 
 
+# https://github.com/westerveltco/django-q-registry/issues/30
+@registry.register(
+    name="Issue 30 regression",
+    next_run=datetime(2024, 5, 8),
+    repeats=-1,
+    schedule_type=Schedule.QUARTERLY,
+)
+def issue_30_regression():
+    return "test"
+
+
 def test_setup_periodic_tasks():
-    assert len(registry.registered_tasks) == 1
+    assert len(registry.registered_tasks) == 2
     assert Task.objects.count() == 0
     assert Schedule.objects.count() == 0
 
     setup_periodic_tasks.Command().handle()
 
-    assert len(registry.registered_tasks) == 1
-    assert len(registry.created_tasks) == 1
-    assert Task.objects.count() == 1
-    assert Schedule.objects.count() == 1
+    assert len(registry.registered_tasks) == 2
+    assert len(registry.created_tasks) == 2
+    assert Task.objects.count() == 2
+    assert Schedule.objects.count() == 2
 
 
 def test_setup_periodic_tasks_dangling_tasks():
     baker.make("django_q_registry.Task", _quantity=3)
 
-    assert len(registry.registered_tasks) == 1
+    assert len(registry.registered_tasks) == 2
     assert Task.objects.count() == 3
 
     setup_periodic_tasks.Command().handle()
 
-    assert len(registry.registered_tasks) == 1
-    assert len(registry.created_tasks) == 1
-    assert Task.objects.count() == 1
+    assert len(registry.registered_tasks) == 2
+    assert len(registry.created_tasks) == 2
+    assert Task.objects.count() == 2
 
 
 def test_setup_periodic_tasks_dangling_schedules():
     baker.make(
         "django_q.Schedule",
         name=itertools.cycle(
             [
                 f"dangling_schedule{i}{app_settings.PERIODIC_TASK_SUFFIX}"
                 for i in range(3)
             ]
         ),
         _quantity=3,
     )
 
-    assert len(registry.registered_tasks) == 1
+    assert len(registry.registered_tasks) == 2
     assert Schedule.objects.count() == 3
 
     setup_periodic_tasks.Command().handle()
 
-    assert len(registry.registered_tasks) == 1
-    assert len(registry.created_tasks) == 1
-    assert Schedule.objects.count() == 1
+    assert len(registry.registered_tasks) == 2
+    assert len(registry.created_tasks) == 2
+    assert Schedule.objects.count() == 2
 
 
 def test_setup_periodic_tasks_dangling_legacy_schedules():
     schedules = baker.make("django_q.Schedule", _quantity=3)
     baker.make(
         "django_q.Schedule",
         name=itertools.cycle([f"dangling_schedule{i} - CRON" for i in range(3)]),
         _quantity=len(schedules),
     )
 
-    assert len(registry.registered_tasks) == 1
+    assert len(registry.registered_tasks) == 2
     assert Schedule.objects.count() == 6
 
     setup_periodic_tasks.Command().handle()
 
-    assert len(registry.registered_tasks) == 1
-    assert len(registry.created_tasks) == 1
-    assert Schedule.objects.count() == 1 + len(schedules)
+    assert len(registry.registered_tasks) == 2
+    assert len(registry.created_tasks) == 2
+    assert Schedule.objects.count() == 2 + len(schedules)
```

### Comparing `django_q_registry-0.3.0/.gitignore` & `django_q_registry-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/LICENSE` & `django_q_registry-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/README.md` & `django_q_registry-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_q_registry-0.3.0/pyproject.toml` & `django_q_registry-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 Documentation = "https://django-q-registry.westervelt.dev/"
 Issues = "https://github.com/westerveltco/django-q-registry/issues"
 Source = "https://github.com/westerveltco/django-q-registry"
 
 [tool.bumpver]
 commit = true
 commit_message = ":bookmark: bump version {old_version} -> {new_version}"
-current_version = "0.3.0"
+current_version = "0.3.1"
 push = false  # set to false for CI
 tag = false
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 
 [tool.bumpver.file_patterns]
 ".copier/package.yml" = ['current_version: {version}']
 "src/django_q_registry/__init__.py" = ['__version__ = "{version}"']
```

### Comparing `django_q_registry-0.3.0/PKG-INFO` & `django_q_registry-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-q-registry
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Django app to register periodic Django Q tasks.
 Project-URL: Documentation, https://django-q-registry.westervelt.dev/
 Project-URL: Issues, https://github.com/westerveltco/django-q-registry/issues
 Project-URL: Source, https://github.com/westerveltco/django-q-registry
 Author-email: Josh Thomas <josh@joshthomas.dev>
 License: MIT License
```

