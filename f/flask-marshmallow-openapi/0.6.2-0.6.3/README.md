# Comparing `tmp/flask_marshmallow_openapi-0.6.2.tar.gz` & `tmp/flask_marshmallow_openapi-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_marshmallow_openapi-0.6.2.tar", last modified: Sat May  4 08:16:52 2024, max compression
+gzip compressed data, was "flask_marshmallow_openapi-0.6.3.tar", last modified: Wed May  8 07:40:33 2024, max compression
```

## Comparing `flask_marshmallow_openapi-0.6.2.tar` & `flask_marshmallow_openapi-0.6.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.076809 flask_marshmallow_openapi-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-04 08:16:52.076809 flask_marshmallow_openapi-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 08:16:52.076809 flask_marshmallow_openapi-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.060808 flask_marshmallow_openapi-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.064808 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.064808 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/flask_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/schemas_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/securities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.064808 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/redoc_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.072808 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/index.css
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
--rw-r--r--   0 runner    (1001) docker     (127)  1045708 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   368781 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
--rw-r--r--   0 runner    (1001) docker     (127)  1045498 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   322863 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 runner    (1001) docker     (127)   145206 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
--rw-r--r--   0 runner    (1001) docker     (127)   256702 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.072808 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/templates/re_doc.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.072808 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-04 08:16:52.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-04 08:16:52.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:16:52.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:16:51.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-04 08:16:52.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-04 08:16:52.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:40:33.693403 flask_marshmallow_openapi-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-08 07:40:33.693403 flask_marshmallow_openapi-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:40:33.693403 flask_marshmallow_openapi-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:40:33.677403 flask_marshmallow_openapi-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:40:33.681403 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:40:33.685403 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/decorators/decorate_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/decorators/decorate_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/decorators/decorate_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/decorators/decorate_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/decorators/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/flask_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16060 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/schemas_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/securities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:40:33.685403 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/redoc_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:40:33.689403 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1045708 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   368781 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1045498 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   322863 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (127)   145206 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
+-rw-r--r--   0 runner    (1001) docker     (127)   256702 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:40:33.689403 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/templates/re_doc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-08 07:40:29.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:40:33.689403 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-08 07:40:33.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-08 07:40:33.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:40:33.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:40:33.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-08 07:40:33.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 07:40:33.000000 flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi.egg-info/top_level.txt
```

### Comparing `flask_marshmallow_openapi-0.6.2/.gitignore` & `flask_marshmallow_openapi-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/LICENSE` & `flask_marshmallow_openapi-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/MANIFEST.in` & `flask_marshmallow_openapi-0.6.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/PKG-INFO` & `flask_marshmallow_openapi-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.6.2
+Version: 0.6.3
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -30,14 +30,15 @@
 Requires-Dist: black>=22.1.0; extra == "dev"
 Requires-Dist: bump2version>=1.0.1; extra == "dev"
 Requires-Dist: check-manifest>=0.47; extra == "dev"
 Requires-Dist: flask-shell-ipython>=0.5.1; extra == "dev"
 Requires-Dist: ipython>=8.6.0; extra == "dev"
 Requires-Dist: isort>=5.10.1; extra == "dev"
 Requires-Dist: pip-tools>=6.5.1; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx>5.2.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Provides-Extra: tests
```

### Comparing `flask_marshmallow_openapi-0.6.2/README.md` & `flask_marshmallow_openapi-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/pyproject.toml` & `flask_marshmallow_openapi-0.6.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65", "wheel"]
 
 
 [project]
 name = "flask-marshmallow-openapi"
-version = "0.6.2"
+version = "0.6.3"
 description = "Flask + marshmallow + OpenAPI"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
@@ -43,14 +43,15 @@
     "black >= 22.1.0",
     "bump2version >= 1.0.1",
     "check-manifest >= 0.47",
     "flask-shell-ipython >= 0.5.1",
     "ipython >= 8.6.0",
     "isort >= 5.10.1",
     "pip-tools >= 6.5.1",
+    "ruff",
 ]
 # For dev machines and CI generating docs
 docs = [
     "furo",
     "myst-parser",
     "sphinx > 5.2.0",
     "sphinx_rtd_theme",
@@ -122,7 +123,48 @@
 branch = true
 source = ["src", "tests"]
 
 
 [tool.coverage.report]
 show_missing = true
 precision = 2
+
+
+[tool.ruff]
+exclude = [".git", ".venv", "build", "dist"]
+line-length = 88                             # Same as Black.
+target-version = "py310"
+cache-dir = "~/.cache/ruff"
+src = ["src"]
+
+[tool.ruff.lint.isort]
+known-local-folder = ["src"]
+
+[tool.ruff.lint]
+select = [
+    "E",
+    "F",
+    "I",   # isort (I)
+    "C90", # mccabe (C90)
+    "UP",  # pyupgrade (UP)
+    "S",   # flake8-bandit (S)
+    "FBT", # flake8-boolean-trap (FBT)
+    "B",   # flake8-bugbear (B)
+    "C4",  # flake8-comprehensions (C4)
+    "DTZ", # flake8-datetimez (DTZ)
+    "FA",  # flake8-future-annotations (FA)
+    "G",   # flake8-logging-format (G)
+    "PIE", # flake8-pie (PIE)
+    "PT",  # flake8-pytest-style (PT)
+    "RET", # flake8-return (RET)
+    "SIM", # flake8-simplify (SIM)
+    "TCH", # flake8-type-checking (TCH)
+    "PTH", # flake8-use-pathlib (PTH)
+    "PL",  # Pylint (PL)
+    "TRY", # tryceratops (TRY)
+    "RUF", # Ruff-specific rules (RUF)
+]
+
+[tool.ruff.lint.per-file-ignores]
+"__init__.py" = [
+    "F401", # unused-import (F401)
+]
```

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_delete.py` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/decorators/decorate_delete.py`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_get.py` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/decorators/decorate_get.py`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_patch.py` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/decorators/decorate_patch.py`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_post.py` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/decorators/decorate_post.py`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/helpers.py` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/decorators/helpers.py`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/flask_paths.py` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/flask_paths.py`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/middleware.py` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 import os
 from dataclasses import dataclass
 from typing import Callable
 
 import apispec
 import flask
```

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/schemas_registry.py` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/schemas_registry.py`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/redoc_favicon.png` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/redoc_favicon.png`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/index.html` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/index.html`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static_collector.py` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/static_collector.py`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/templates/changelog.html.jinja2` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/templates/changelog.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/templates/re_doc.jinja2` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/templates/re_doc.jinja2`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2`

 * *Files identical despite different names*

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/PKG-INFO` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.6.2
+Version: 0.6.3
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -30,14 +30,15 @@
 Requires-Dist: black>=22.1.0; extra == "dev"
 Requires-Dist: bump2version>=1.0.1; extra == "dev"
 Requires-Dist: check-manifest>=0.47; extra == "dev"
 Requires-Dist: flask-shell-ipython>=0.5.1; extra == "dev"
 Requires-Dist: ipython>=8.6.0; extra == "dev"
 Requires-Dist: isort>=5.10.1; extra == "dev"
 Requires-Dist: pip-tools>=6.5.1; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx>5.2.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Provides-Extra: tests
```

### Comparing `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/SOURCES.txt` & `flask_marshmallow_openapi-0.6.3/src/flask_marshmallow_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

