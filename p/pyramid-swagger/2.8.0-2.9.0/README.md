# Comparing `tmp/pyramid_swagger-2.8.0.tar.gz` & `tmp/pyramid_swagger-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyramid_swagger-2.8.0.tar", last modified: Fri May  3 23:10:01 2024, max compression
+gzip compressed data, was "pyramid_swagger-2.9.0.tar", last modified: Wed May  8 20:50:12 2024, max compression
```

## Comparing `pyramid_swagger-2.8.0.tar` & `pyramid_swagger-2.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:01.299472 pyramid_swagger-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-03 23:10:01.299472 pyramid_swagger-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:01.299472 pyramid_swagger-2.8.0/pyramid_swagger/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/load_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    21771 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/tween.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:01.299472 pyramid_swagger-2.8.0/pyramid_swagger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-03 23:10:01.000000 pyramid_swagger-2.8.0/pyramid_swagger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-03 23:10:01.000000 pyramid_swagger-2.8.0/pyramid_swagger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 23:10:01.000000 pyramid_swagger-2.8.0/pyramid_swagger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-03 23:10:01.000000 pyramid_swagger-2.8.0/pyramid_swagger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 23:10:01.000000 pyramid_swagger-2.8.0/pyramid_swagger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 23:10:01.299472 pyramid_swagger-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:50:12.250499 pyramid_swagger-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-08 20:50:11.000000 pyramid_swagger-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-08 20:50:11.000000 pyramid_swagger-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-08 20:50:12.250499 pyramid_swagger-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-08 20:50:11.000000 pyramid_swagger-2.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:50:12.250499 pyramid_swagger-2.9.0/pyramid_swagger/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-08 20:50:11.000000 pyramid_swagger-2.9.0/pyramid_swagger/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-08 20:50:11.000000 pyramid_swagger-2.9.0/pyramid_swagger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-05-08 20:50:11.000000 pyramid_swagger-2.9.0/pyramid_swagger/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-08 20:50:11.000000 pyramid_swagger-2.9.0/pyramid_swagger/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-08 20:50:11.000000 pyramid_swagger-2.9.0/pyramid_swagger/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-05-08 20:50:11.000000 pyramid_swagger-2.9.0/pyramid_swagger/load_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-08 20:50:11.000000 pyramid_swagger-2.9.0/pyramid_swagger/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-08 20:50:11.000000 pyramid_swagger-2.9.0/pyramid_swagger/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-08 20:50:11.000000 pyramid_swagger-2.9.0/pyramid_swagger/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22321 2024-05-08 20:50:11.000000 pyramid_swagger-2.9.0/pyramid_swagger/tween.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:50:12.250499 pyramid_swagger-2.9.0/pyramid_swagger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-08 20:50:12.000000 pyramid_swagger-2.9.0/pyramid_swagger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-08 20:50:12.000000 pyramid_swagger-2.9.0/pyramid_swagger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:50:12.000000 pyramid_swagger-2.9.0/pyramid_swagger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 20:50:12.000000 pyramid_swagger-2.9.0/pyramid_swagger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 20:50:12.000000 pyramid_swagger-2.9.0/pyramid_swagger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-08 20:50:12.250499 pyramid_swagger-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-08 20:50:11.000000 pyramid_swagger-2.9.0/setup.py
```

### Comparing `pyramid_swagger-2.8.0/LICENSE` & `pyramid_swagger-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.8.0/PKG-INFO` & `pyramid_swagger-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyramid_swagger
-Version: 2.8.0
+Version: 2.9.0
 Summary: Swagger tools for use in pyramid webapps
 Home-page: https://github.com/striglia/pyramid_swagger
 Author: Scott Triglia
 Author-email: scott.triglia@gmail.com
 License: BSD 3-clause
 Keywords: pyramid swagger validation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyramid_swagger-2.8.0/README.rst` & `pyramid_swagger-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.8.0/pyramid_swagger/__about__.py` & `pyramid_swagger-2.9.0/pyramid_swagger/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
     "__email__", "__license__", "__copyright__",
 ]
 
 __title__ = "pyramid_swagger"
 __summary__ = "Swagger tools for use in pyramid webapps"
 __uri__ = "https://github.com/striglia/pyramid_swagger"
 
-__version__ = "2.8.0"
+__version__ = "2.9.0"
 
 __author__ = "Scott Triglia"
 __email__ = "scott.triglia@gmail.com"
 
 __license__ = "BSD 3-clause"
 __copyright__ = "Copyright 2014 Scott Triglia"
```

### Comparing `pyramid_swagger-2.8.0/pyramid_swagger/__init__.py` & `pyramid_swagger-2.9.0/pyramid_swagger/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.8.0/pyramid_swagger/api.py` & `pyramid_swagger-2.9.0/pyramid_swagger/api.py`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.8.0/pyramid_swagger/exceptions.py` & `pyramid_swagger-2.9.0/pyramid_swagger/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.8.0/pyramid_swagger/ingest.py` & `pyramid_swagger-2.9.0/pyramid_swagger/ingest.py`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.8.0/pyramid_swagger/load_schema.py` & `pyramid_swagger-2.9.0/pyramid_swagger/load_schema.py`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.8.0/pyramid_swagger/model.py` & `pyramid_swagger-2.9.0/pyramid_swagger/model.py`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.8.0/pyramid_swagger/renderer.py` & `pyramid_swagger-2.9.0/pyramid_swagger/renderer.py`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.8.0/pyramid_swagger/spec.py` & `pyramid_swagger-2.9.0/pyramid_swagger/spec.py`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.8.0/pyramid_swagger/tween.py` & `pyramid_swagger-2.9.0/pyramid_swagger/tween.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         'swagger20_handler',
         'validate_request',
         'validate_response',
         'validate_path',
         'exclude_paths',
         'exclude_routes',
         'prefer_20_routes',
+        'response_validation_exclude_routes'
     ]
 )):
 
     """A settings object for configurable options.
 
     :param swagger12_handler: a :class:`SwaggerHandler` for v1.2 or None
     :param swagger20_handler: a :class:`SwaggerHandler` for v2.0 or None
@@ -75,14 +76,16 @@
         excluded from validation.
     :rtype: namedtuple
     :param exclude_routes: list of route names that should be excluded from
         validation.
     :param prefer_20_routes: list of route names that should be handled
         via v2.0 spec when `2.0` is in `swagger_versions`. All others will be
         handled via v1.2 spec. [i.e. Make v2.0 an opt-in feature]
+    :param response_validation_exclude_routes: list of route names that should be excluded from
+        response validation.
     """
 
 
 @contextmanager
 def noop_context(request, response=None):
     yield
 
@@ -191,15 +194,15 @@
             def swagger_data(_):
                 return request_data
 
             request.set_property(swagger_data)
 
         response = handler(request)
 
-        if settings.validate_response:
+        if settings.validate_response and not should_exclude_response_validation(settings, route_info):
             with validation_context(request, response=response):
                 swagger_handler.handle_response(response, op_or_validators_map)
 
         return response
 
     return validator_tween
 
@@ -385,14 +388,17 @@
         )),
         exclude_paths=get_exclude_paths(registry),
         exclude_routes=set(aslist(registry.settings.get(
             'pyramid_swagger.exclude_routes',
         ) or [])),
         prefer_20_routes=set(aslist(registry.settings.get(
             'pyramid_swagger.prefer_20_routes') or [])),
+        response_validation_exclude_routes=set(aslist(registry.settings.get(
+            'pyramid_swagger.response_validation_exclude_routes',
+        ) or [])),
     )
 
 
 SwaggerHandler = namedtuple('SwaggerHandler',
                             'op_for_request handle_request handle_response')
 
 
@@ -458,14 +464,18 @@
         disable_all_validation
         or should_exclude_path(settings.exclude_paths, request.path_info)
         or should_exclude_route(settings.exclude_routes, route_info)
         or is_swagger_documentation_route(route_info)
     )
 
 
+def should_exclude_response_validation(settings, route_info):
+    return should_exclude_route(settings.response_validation_exclude_routes, route_info)
+
+
 def should_exclude_path(exclude_path_regexes, path):
     # Skip validation for the specified endpoints
     return any(r.match(path) for r in exclude_path_regexes)
 
 
 def should_exclude_route(excluded_routes, route_info):
     return route_info.get('route') and route_info['route'].name in excluded_routes
```

### Comparing `pyramid_swagger-2.8.0/pyramid_swagger.egg-info/PKG-INFO` & `pyramid_swagger-2.9.0/pyramid_swagger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyramid-swagger
-Version: 2.8.0
+Version: 2.9.0
 Summary: Swagger tools for use in pyramid webapps
 Home-page: https://github.com/striglia/pyramid_swagger
 Author: Scott Triglia
 Author-email: scott.triglia@gmail.com
 License: BSD 3-clause
 Keywords: pyramid swagger validation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyramid_swagger-2.8.0/pyramid_swagger.egg-info/SOURCES.txt` & `pyramid_swagger-2.9.0/pyramid_swagger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.8.0/setup.py` & `pyramid_swagger-2.9.0/setup.py`

 * *Files identical despite different names*

