# Comparing `tmp/fab_react_toolkit-0.4.5.tar.gz` & `tmp/fab_react_toolkit-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fab_react_toolkit-0.4.5.tar", last modified: Fri May  3 07:14:53 2024, max compression
+gzip compressed data, was "fab_react_toolkit-0.4.6.tar", last modified: Wed May  8 11:13:43 2024, max compression
```

## Comparing `fab_react_toolkit-0.4.5.tar` & `fab_react_toolkit-0.4.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:14:53.259945 fab_react_toolkit-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-03 07:14:53.259945 fab_react_toolkit-0.4.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:14:53.251946 fab_react_toolkit-0.4.5/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:14:53.255946 fab_react_toolkit-0.4.5/example/app/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/example/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/example/app/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/example/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/example/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/example/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/example/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/example/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:14:53.255946 fab_react_toolkit-0.4.5/fab_react_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/fab_react_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:14:53.255946 fab_react_toolkit-0.4.5/fab_react_toolkit/api/
--rw-r--r--   0 runner    (1001) docker     (127)    21837 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/fab_react_toolkit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/fab_react_toolkit/api/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/fab_react_toolkit/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/fab_react_toolkit/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/fab_react_toolkit/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/fab_react_toolkit/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/fab_react_toolkit/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/fab_react_toolkit/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:14:53.259945 fab_react_toolkit-0.4.5/fab_react_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-03 07:14:53.000000 fab_react_toolkit-0.4.5/fab_react_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-03 07:14:53.000000 fab_react_toolkit-0.4.5/fab_react_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:14:53.000000 fab_react_toolkit-0.4.5/fab_react_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-03 07:14:53.000000 fab_react_toolkit-0.4.5/fab_react_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 07:14:53.000000 fab_react_toolkit-0.4.5/fab_react_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-03 07:14:44.000000 fab_react_toolkit-0.4.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 07:14:53.259945 fab_react_toolkit-0.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:13:43.347860 fab_react_toolkit-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-08 11:13:43.343860 fab_react_toolkit-0.4.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:13:43.339860 fab_react_toolkit-0.4.6/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:13:43.343860 fab_react_toolkit-0.4.6/example/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/example/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/example/app/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/example/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/example/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/example/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:13:43.343860 fab_react_toolkit-0.4.6/fab_react_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:13:43.343860 fab_react_toolkit-0.4.6/fab_react_toolkit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    21837 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/api/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29193 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/fab_react_toolkit/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:13:43.343860 fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-08 11:13:43.000000 fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-08 11:13:43.000000 fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:13:43.000000 fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 11:13:43.000000 fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 11:13:43.000000 fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-08 11:13:32.000000 fab_react_toolkit-0.4.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 11:13:43.347860 fab_react_toolkit-0.4.6/setup.cfg
```

### Comparing `fab_react_toolkit-0.4.5/LICENSE` & `fab_react_toolkit-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.5/PKG-INFO` & `fab_react_toolkit-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.4.5
+Version: 0.4.6
 Summary: A small example package
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fab_react_toolkit-0.4.5/example/app/__init__.py` & `fab_react_toolkit-0.4.6/example/app/__init__.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.5/example/app/apis.py` & `fab_react_toolkit-0.4.6/example/app/apis.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.5/example/app/config.py` & `fab_react_toolkit-0.4.6/example/app/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
 from flask_appbuilder.security.manager import (
     AUTH_DB,
+    AUTH_OAUTH,
 )
 
 basedir = os.path.abspath(os.path.dirname(__file__))
 
 # Your App secret key
 SECRET_KEY = "\2\1thisismyscretkey\1\2\e\y\y\h"
 
@@ -29,33 +30,54 @@
 # AUTHENTICATION CONFIG
 # ----------------------------------------------------
 # The authentication type
 # AUTH_OID : Is for OpenID
 # AUTH_DB : Is for database (username/password()
 # AUTH_LDAP : Is for LDAP
 # AUTH_REMOTE_USER : Is for using REMOTE_USER from web server
+# AUTH_OAUTH : Is for OAuth
 AUTH_TYPE = AUTH_DB
 
 FAB_REACT_CONFIG = {'foo': 'bar'}
 
 # Uncomment to setup Full admin role name
-# AUTH_ROLE_ADMIN = 'Admin'
+AUTH_ROLE_ADMIN = 'Admin'
 
 # Uncomment to setup Public role name, no authentication needed
 # AUTH_ROLE_PUBLIC = 'Public'
 
 # Will allow user self registration
 # AUTH_USER_REGISTRATION = True
 
 # The default user self registration role
 # AUTH_USER_REGISTRATION_ROLE = "Public"
 
 # When using LDAP Auth, setup the ldap server
 # AUTH_LDAP_SERVER = "ldap://ldapserver.new"
 
+# REDIRECT_URI = "http://localhost:6006/"
+# OAUTH_PROVIDERS = [
+#     {
+#         "name": "google",
+#         "icon": "fa-google",
+#         "token_key": "access_token",
+#         "remote_app": {
+#             "client_id": "CLIENTID",
+#             "client_secret": "CLIENTSECRET",
+#             "api_base_url": "https://www.googleapis.com/oauth2/v2/",
+#             "client_kwargs": {"scope": "email profile"},
+#             "request_token_url": None,
+#             "access_token_url": "https://accounts.google.com/o/oauth2/token",
+#             "authorize_url": "https://accounts.google.com/o/oauth2/auth",
+#             "jwks_uri": "https://www.googleapis.com/oauth2/v3/certs",
+#             "redirect_uri": "http://localhost:6060/api/v1/auth/login/google/callback",
+#         },
+#     },
+# ]
+
 # Uncomment to setup OpenID providers example for OpenID authentication
 # OPENID_PROVIDERS = [
 #    { 'name': 'Yahoo', 'url': 'https://me.yahoo.com' },
 #    { 'name': 'AOL', 'url': 'http://openid.aol.com/<username>' },
 #    { 'name': 'Flickr', 'url': 'http://www.flickr.com/<username>' },
 #    { 'name': 'MyOpenID', 'url': 'https://www.myopenid.com' }]
 # ---------------------------------------------------
@@ -68,8 +90,9 @@
 # The allowed translation for you app
 LANGUAGES = {
     "en": {"flag": "gb", "name": "English"},
 }
 
 # Session Cookie settings
 SESSION_COOKIE_SECURE = True
-SESSION_COOKIE_SAMESITE = "Strict"
+# Use "Strict" for maximum security but it breaks the OAuth workflow
+SESSION_COOKIE_SAMESITE = "Lax"
```

### Comparing `fab_react_toolkit-0.4.5/example/app/models.py` & `fab_react_toolkit-0.4.6/example/app/models.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.5/example/run.py` & `fab_react_toolkit-0.4.6/example/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 from datetime import datetime, date
 import random
 from app import app, db
 from app.models import Asset, Unit, Application, AssetApplication
 
 
+# Create a google username myusername
+# google = app.appbuilder.sm.find_user(username="myusername")
+# if not google:
+#     app.appbuilder.sm.add_user(
+#         username="myusername",
+#         first_name="google",
+#         last_name="google",
+#         email="myemail",
+#         role=app.appbuilder.sm.find_role("Admin"),
+#         password="google"
+#     )
 
 user = app.appbuilder.sm.find_user(username="admin")
 if not user:
     app.appbuilder.sm.add_user(
         username="admin",
         first_name="admin",
         last_name="admin",
```

### Comparing `fab_react_toolkit-0.4.5/fab_react_toolkit/__init__.py` & `fab_react_toolkit-0.4.6/fab_react_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.5/fab_react_toolkit/api/__init__.py` & `fab_react_toolkit-0.4.6/fab_react_toolkit/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.5/fab_react_toolkit/api/convert.py` & `fab_react_toolkit-0.4.6/fab_react_toolkit/api/convert.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.5/fab_react_toolkit/api/utils.py` & `fab_react_toolkit-0.4.6/fab_react_toolkit/api/utils.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.5/fab_react_toolkit/apis.py` & `fab_react_toolkit-0.4.6/fab_react_toolkit/apis.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
                     if "email" in userinfo and re.search(email, userinfo["email"]):
                         allow = True
                         break
                 if not allow:
                     self.response_401()
             user = self.appbuilder.sm.auth_user_oauth(userinfo)
         if user is None:
-            self.response_400(message="Invalid login. Please try again.")
+            return self.response_400(message="Invalid login. Please try again.")
         else:
             login_user(user)
             try:
                 # redirect uri could be stored in state, I don't see the point though
                 state = jwt.decode(
                     request.args["state"],
                     self.appbuilder.app.config["SECRET_KEY"],
```

### Comparing `fab_react_toolkit-0.4.5/fab_react_toolkit/filters.py` & `fab_react_toolkit-0.4.6/fab_react_toolkit/filters.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.5/fab_react_toolkit/views.py` & `fab_react_toolkit-0.4.6/fab_react_toolkit/views.py`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.5/fab_react_toolkit.egg-info/PKG-INFO` & `fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.4.5
+Version: 0.4.6
 Summary: A small example package
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fab_react_toolkit-0.4.5/fab_react_toolkit.egg-info/SOURCES.txt` & `fab_react_toolkit-0.4.6/fab_react_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fab_react_toolkit-0.4.5/pyproject.toml` & `fab_react_toolkit-0.4.6/pyproject.toml`

 * *Files identical despite different names*

