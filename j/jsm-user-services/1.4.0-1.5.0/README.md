# Comparing `tmp/jsm_user_services-1.4.0.tar.gz` & `tmp/jsm_user_services-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsm_user_services-1.4.0.tar", max compression
+gzip compressed data, was "jsm_user_services-1.5.0.tar", max compression
```

## Comparing `jsm_user_services-1.4.0.tar` & `jsm_user_services-1.5.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
--rw-r--r--   0        0        0     1070 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/LICENSE
--rw-r--r--   0        0        0    10306 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/README.md
--rw-r--r--   0        0        0       54 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/__init__.py
--rw-r--r--   0        0        0      107 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/apps.py
--rw-r--r--   0        0        0        0 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/decorators/__init__.py
--rw-r--r--   0        0        0     3795 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/decorators/lgpd.py
--rw-r--r--   0        0        0     5933 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/decorators/lgpd_utils.py
--rw-r--r--   0        0        0        0 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/drf_tools/__init__.py
--rw-r--r--   0        0        0     2475 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/drf_tools/helpers.py
--rw-r--r--   0        0        0    14221 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/drf_tools/permissions.py
--rw-r--r--   0        0        0      692 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/exception.py
--rw-r--r--   0        0        0        0 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/flask/__init__.py
--rw-r--r--   0        0        0     3462 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/flask/middleware.py
--rw-r--r--   0        0        0     3292 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/middleware.py
--rw-r--r--   0        0        0        0 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/services/__init__.py
--rw-r--r--   0        0        0     4247 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/services/everest.py
--rw-r--r--   0        0        0     1996 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/services/google.py
--rw-r--r--   0        0        0     5640 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/services/user.py
--rw-r--r--   0        0        0     1840 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/settings.py
--rw-r--r--   0        0        0        0 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/__init__.py
--rw-r--r--   0        0        0     1262 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/auth_jwt.py
--rw-r--r--   0        0        0      866 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/email_utils.py
--rw-r--r--   0        0        0     2333 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/http_utils.py
--rw-r--r--   0        0        0      304 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/import_utils.py
--rw-r--r--   0        0        0      415 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/local_threading_utils.py
--rw-r--r--   0        0        0      268 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/logging_utils.py
--rw-r--r--   0        0        0     2185 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/request_id.py
--rw-r--r--   0        0        0      618 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/settings_utils.py
--rw-r--r--   0        0        0      237 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/jsm_user_services/support/string_utils.py
--rw-r--r--   0        0        0     1574 2024-04-10 12:16:16.879741 jsm_user_services-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    11293 1970-01-01 00:00:00.000000 jsm_user_services-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/LICENSE
+-rw-r--r--   0        0        0    10313 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/README.md
+-rw-r--r--   0        0        0       54 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/__init__.py
+-rw-r--r--   0        0        0      107 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/apps.py
+-rw-r--r--   0        0        0        0 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/decorators/__init__.py
+-rw-r--r--   0        0        0     3795 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/decorators/lgpd.py
+-rw-r--r--   0        0        0     5933 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/decorators/lgpd_utils.py
+-rw-r--r--   0        0        0        0 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/drf_tools/__init__.py
+-rw-r--r--   0        0        0     2449 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/drf_tools/authentications.py
+-rw-r--r--   0        0        0      451 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/drf_tools/exceptions.py
+-rw-r--r--   0        0        0     2475 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/drf_tools/helpers.py
+-rw-r--r--   0        0        0    14833 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/drf_tools/permissions.py
+-rw-r--r--   0        0        0      692 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/exception.py
+-rw-r--r--   0        0        0        0 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/flask_module/__init__.py
+-rw-r--r--   0        0        0     3476 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/flask_module/middleware.py
+-rw-r--r--   0        0        0     3292 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/middleware.py
+-rw-r--r--   0        0        0        0 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/services/__init__.py
+-rw-r--r--   0        0        0     4247 2024-05-08 20:30:57.755619 jsm_user_services-1.5.0/jsm_user_services/services/everest.py
+-rw-r--r--   0        0        0     1996 2024-05-08 20:30:57.759619 jsm_user_services-1.5.0/jsm_user_services/services/google.py
+-rw-r--r--   0        0        0     6210 2024-05-08 20:30:57.759619 jsm_user_services-1.5.0/jsm_user_services/services/user.py
+-rw-r--r--   0        0        0     2436 2024-05-08 20:30:57.759619 jsm_user_services-1.5.0/jsm_user_services/settings.py
+-rw-r--r--   0        0        0        0 2024-05-08 20:30:57.759619 jsm_user_services-1.5.0/jsm_user_services/support/__init__.py
+-rw-r--r--   0        0        0     1262 2024-05-08 20:30:57.759619 jsm_user_services-1.5.0/jsm_user_services/support/auth_jwt.py
+-rw-r--r--   0        0        0      866 2024-05-08 20:30:57.759619 jsm_user_services-1.5.0/jsm_user_services/support/email_utils.py
+-rw-r--r--   0        0        0     2333 2024-05-08 20:30:57.759619 jsm_user_services-1.5.0/jsm_user_services/support/http_utils.py
+-rw-r--r--   0        0        0      304 2024-05-08 20:30:57.759619 jsm_user_services-1.5.0/jsm_user_services/support/import_utils.py
+-rw-r--r--   0        0        0      415 2024-05-08 20:30:57.759619 jsm_user_services-1.5.0/jsm_user_services/support/local_threading_utils.py
+-rw-r--r--   0        0        0      268 2024-05-08 20:30:57.759619 jsm_user_services-1.5.0/jsm_user_services/support/logging_utils.py
+-rw-r--r--   0        0        0     2185 2024-05-08 20:30:57.759619 jsm_user_services-1.5.0/jsm_user_services/support/request_id.py
+-rw-r--r--   0        0        0      618 2024-05-08 20:30:57.759619 jsm_user_services-1.5.0/jsm_user_services/support/settings_utils.py
+-rw-r--r--   0        0        0      237 2024-05-08 20:30:57.759619 jsm_user_services-1.5.0/jsm_user_services/support/string_utils.py
+-rw-r--r--   0        0        0     1633 2024-05-08 20:30:57.759619 jsm_user_services-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11344 1970-01-01 00:00:00.000000 jsm_user_services-1.5.0/PKG-INFO
```

### Comparing `jsm_user_services-1.4.0/LICENSE` & `jsm_user_services-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.4.0/README.md` & `jsm_user_services-1.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 `pip install jsm-user-services[flask]`
 
 Add the middleware in your Flask app:
 
 ```python
 from flask import Flask
-from jsm_user_services.flask import middleware
+from jsm_user_services.flask_module import middleware
 
 app = Flask(__name__)
 
 middleware.JsmJwtService(app)
 app.config.update(
     USER_API_HOST="http://ishtar-gate.dev.juntossomosmaisi.com.br/api/v1", USER_API_TOKEN="user_api_token"
 )
```

### Comparing `jsm_user_services-1.4.0/jsm_user_services/decorators/lgpd.py` & `jsm_user_services-1.5.0/jsm_user_services/decorators/lgpd.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.4.0/jsm_user_services/decorators/lgpd_utils.py` & `jsm_user_services-1.5.0/jsm_user_services/decorators/lgpd_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.4.0/jsm_user_services/drf_tools/helpers.py` & `jsm_user_services-1.5.0/jsm_user_services/drf_tools/helpers.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.4.0/jsm_user_services/drf_tools/permissions.py` & `jsm_user_services-1.5.0/jsm_user_services/drf_tools/permissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 from rest_framework.exceptions import APIException
 from rest_framework.request import Request
 
 from jsm_user_services.drf_tools.helpers import AllowClassBehaviorAsFunction
 from jsm_user_services.drf_tools.helpers import is_exception_related_to_api_exception
 from jsm_user_services.exception import IncorrectTypePermissionConfiguration
 from jsm_user_services.services.google import perform_recaptcha_validation
+from jsm_user_services.services.user import get_jwt_algorithm
 from jsm_user_services.services.user import get_user_data_from_server
+from jsm_user_services.services.user import get_user_id_auth_or_user_id_ref_in_jwt
 
 logger = logging.getLogger(__name__)
 
 
 class JSMUserBasePermission(permissions.BasePermission):
     """
     Base class for JSM user permissions. Implements methods for validating requests against
@@ -371,7 +373,21 @@
             full_match=self.full_match,
         )
 
         if use_received_exception and not is_allowed:
             raise self.exception_in_case_of_failed_verification  # type: ignore
 
         return is_allowed
+
+
+class JuntosIdUserIsAuthenticatedInLOPermission(JSMUserBasePermission):
+    """
+    Permission to check if the user is authenticated with an Oauth or Loyalty JWT.
+    """
+
+    def has_permission(self, request, *args, **kwargs):
+        alg = get_jwt_algorithm()
+        if alg == "RS256":
+            user = get_user_id_auth_or_user_id_ref_in_jwt()
+            return bool(user)
+        else:
+            return bool(request.user and request.user.is_authenticated)
```

### Comparing `jsm_user_services-1.4.0/jsm_user_services/exception.py` & `jsm_user_services-1.5.0/jsm_user_services/exception.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.4.0/jsm_user_services/flask/middleware.py` & `jsm_user_services-1.5.0/jsm_user_services/flask_module/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,25 +24,25 @@
         have the option to initialize it later.
 
         Examples:
         - Initialize as soon as possible:
 
         ```
         from flask import Flask
-        from jsm_user_services.flask.middleware import JsmJwtService
+        from jsm_user_services.flask_module.middleware import JsmJwtService
 
         app = Flask(__name__)
         JsmJwtService(app)
         ```
 
         - Postpone initialization:
 
         ```
         from flask import Flask
-        from jsm_user_services.flask.middleware import JsmJwtService
+        from jsm_user_services.flask_module.middleware import JsmJwtService
 
         app, middleware = Flask(__name__), JsmJwtService()
         middleware.init_app(app)
         ```
         """
 
         self.app = app
```

### Comparing `jsm_user_services-1.4.0/jsm_user_services/middleware.py` & `jsm_user_services-1.5.0/jsm_user_services/middleware.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.4.0/jsm_user_services/services/everest.py` & `jsm_user_services-1.5.0/jsm_user_services/services/everest.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.4.0/jsm_user_services/services/google.py` & `jsm_user_services-1.5.0/jsm_user_services/services/google.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.4.0/jsm_user_services/services/user.py` & `jsm_user_services-1.5.0/jsm_user_services/services/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import hashlib
 
 from importlib import import_module
 from typing import Any
 from typing import List
 from typing import Optional
 
+import jwt
+
 from jsm_user_services.support.auth_jwt import get_decoded_jwt_token
 from jsm_user_services.support.auth_jwt import get_decoded_oauth_token
 from jsm_user_services.support.http_utils import get_response_body
 from jsm_user_services.support.http_utils import request
 from jsm_user_services.support.local_threading_utils import get_from_local_threading
 from jsm_user_services.support.request_id import current_request_id
 from jsm_user_services.support.request_id import request_id_header_name
@@ -37,14 +39,23 @@
     return any([(jwt_token_role in jwt_required_roles) for jwt_token_role in jwt_token_roles])
 
 
 def current_jwt_token() -> Optional[str]:
     return get_from_local_threading("authorization_token")
 
 
+def get_jwt_algorithm() -> str:
+    """
+    Retrieves the algorithm used in the JWT token.
+    """
+    token = current_jwt_token()
+    header = jwt.get_unverified_header(token)
+    return header.get("alg")
+
+
 def get_jsm_token() -> Optional[str]:
     token = current_jwt_token()
     if token:
         return get_decoded_jwt_token(token)["jsm_identity"]
 
     return None
 
@@ -191,7 +202,18 @@
     This function retrieves the user's email from an OAuth JWT token.
     If the "email" field is not present, it returns None.
     """
     user_data = get_oauth_token()
     if user_data:
         return user_data.get("email")
     return None
+
+
+def get_user_id_auth_or_user_id_ref_in_jwt() -> Optional[str]:
+    """
+    Retrieves the user_id_auth or user_id_ref from the JWT token according to the algorithm used.
+    """
+    alg = get_jwt_algorithm()
+
+    alg_to_user_id_map = {"RS256": get_user_id_auth, "HS256": get_user_id_from_jwt}
+
+    return alg_to_user_id_map.get(alg, lambda: None)()
```

### Comparing `jsm_user_services-1.4.0/jsm_user_services/support/auth_jwt.py` & `jsm_user_services-1.5.0/jsm_user_services/support/auth_jwt.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.4.0/jsm_user_services/support/email_utils.py` & `jsm_user_services-1.5.0/jsm_user_services/support/email_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.4.0/jsm_user_services/support/http_utils.py` & `jsm_user_services-1.5.0/jsm_user_services/support/http_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.4.0/jsm_user_services/support/request_id.py` & `jsm_user_services-1.5.0/jsm_user_services/support/request_id.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.4.0/jsm_user_services/support/settings_utils.py` & `jsm_user_services-1.5.0/jsm_user_services/support/settings_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.4.0/pyproject.toml` & `jsm_user_services-1.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.poetry]
 name = "jsm-user-services"
-version = "1.4.0"
+version = "1.5.0"
 description = "Middleware to intercept JWT auth token and more utils functions"
 authors = ["Juntos Somos Mais <labs@juntossomosmais.com.br>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "jsm_user_services"}]
 classifiers=[
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.7",
-    "Framework :: Django :: 2.1",
+    "Programming Language :: Python :: 3.10",
+    "Framework :: Django :: 5.0",
     "Environment :: Web Environment",
     "Natural Language :: Portuguese (Brazilian)",
     "Development Status :: 4 - Beta",
     "Framework :: Django",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 PyJWT = "^2.4.0"
 requests = "*"
+djangorestframework-simplejwt = "^5.3.1"
+pytest = "8.1.1"
 
 [tool.poetry.extras]
 flask = ["flask", "flask-log-request-id"]
 drf = ["djangorestframework", "request-id-django-log"]
 
 [tool.poetry.group.dev.dependencies]
 django = "*"
```

### Comparing `jsm_user_services-1.4.0/PKG-INFO` & `jsm_user_services-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: jsm-user-services
-Version: 1.4.0
+Version: 1.5.0
 Summary: Middleware to intercept JWT auth token and more utils functions
 License: MIT
 Author: Juntos Somos Mais
 Author-email: labs@juntossomosmais.com.br
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.1
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: drf
 Provides-Extra: flask
 Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
+Requires-Dist: djangorestframework-simplejwt (>=5.3.1,<6.0.0)
+Requires-Dist: pytest (==8.1.1)
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # JSM User JWT Service
 
 Middleware to intercept JWT auth token and more utils functions
 
@@ -75,15 +76,15 @@
 
 `pip install jsm-user-services[flask]`
 
 Add the middleware in your Flask app:
 
 ```python
 from flask import Flask
-from jsm_user_services.flask import middleware
+from jsm_user_services.flask_module import middleware
 
 app = Flask(__name__)
 
 middleware.JsmJwtService(app)
 app.config.update(
     USER_API_HOST="http://ishtar-gate.dev.juntossomosmaisi.com.br/api/v1", USER_API_TOKEN="user_api_token"
 )
```

