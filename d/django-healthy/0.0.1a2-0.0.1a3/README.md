# Comparing `tmp/django_healthy-0.0.1a2.tar.gz` & `tmp/django_healthy-0.0.1a3.tar.gz`

## Comparing `django_healthy-0.0.1a2.tar` & `django_healthy-0.0.1a3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/ruff_defaults.toml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/src/healthy/__init__.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/src/healthy/apps.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/src/healthy/backends.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/src/healthy/compat.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/src/healthy/responses.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/src/healthy/urls.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/src/healthy/views.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/tests/__init__.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/tests/settings.py
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/tests/test_backends.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/tests/test_responses.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/tests/test_views.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/tests/urls.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/LICENSE.txt
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/README.md
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/ruff_defaults.toml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/src/healthy/__init__.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/src/healthy/apps.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/src/healthy/backends.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/src/healthy/compat.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/src/healthy/handler.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/src/healthy/responses.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/src/healthy/urls.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/src/healthy/views.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/tests/__init__.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/tests/cache.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/tests/settings.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/tests/test_backends.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/tests/test_responses.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/tests/test_views.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/tests/urls.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/LICENSE.txt
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/README.md
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 django_healthy-0.0.1a3/PKG-INFO
```

### Comparing `django_healthy-0.0.1a2/ruff_defaults.toml` & `django_healthy-0.0.1a3/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `django_healthy-0.0.1a2/tests/test_backends.py` & `django_healthy-0.0.1a3/tests/test_backends.py`

 * *Files 18% similar despite different names*

```diff
@@ -81,7 +81,34 @@
     async def test_run_health_check(self):
         backend = backends.LivenessHealthBackend()
 
         got = await backend.run_health_check()
 
         assert isinstance(got, backends.Health)
         assert got.status == backends.HealthStatus.UP
+
+
+@pytest.mark.asyncio
+class TestCacheHealthCheck:
+    async def test_with_working_cache(self):
+        backend = backends.CacheHealthBackend()
+
+        got = await backend.run_health_check()
+
+        assert isinstance(got, backends.Health)
+        assert got.status == backends.HealthStatus.UP
+
+    async def test_with_broken_cache(self):
+        backend = backends.CacheHealthBackend("broken")
+
+        got = await backend.run_health_check()
+
+        assert isinstance(got, backends.Health)
+        assert got.status == backends.HealthStatus.DOWN
+
+    async def test_with_invalid_value(self):
+        backend = backends.CacheHealthBackend("dummy")
+
+        got = await backend.run_health_check()
+
+        assert isinstance(got, backends.Health)
+        assert got.status == backends.HealthStatus.DOWN
```

### Comparing `django_healthy-0.0.1a2/tests/test_responses.py` & `django_healthy-0.0.1a3/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `django_healthy-0.0.1a2/LICENSE.txt` & `django_healthy-0.0.1a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_healthy-0.0.1a2/README.md` & `django_healthy-0.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `django_healthy-0.0.1a2/pyproject.toml` & `django_healthy-0.0.1a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
   "pytest-asyncio",
   "pytest-django",
 ]
+
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
```

### Comparing `django_healthy-0.0.1a2/PKG-INFO` & `django_healthy-0.0.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-healthy
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: Simple health checking for django applications
 Project-URL: Documentation, https://github.com/olist/django-healthy#readme
 Project-URL: Issues, https://github.com/olist/django-healthy/issues
 Project-URL: Source, https://github.com/olist/django-healthy
 Author-email: Christian Hartung <christian.hartung@olist.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

