# Comparing `tmp/star-local-0.0.8.tar.gz` & `tmp/star-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "star-local-0.0.8.tar", last modified: Wed Dec  6 21:01:34 2023, max compression
+gzip compressed data, was "star-local-0.0.9.tar", last modified: Wed Dec  6 22:27:01 2023, max compression
```

## Comparing `star-local-0.0.8.tar` & `star-local-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 21:01:34.121928 star-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-06 21:01:34.121928 star-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-12-06 21:01:05.000000 star-local-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-06 21:01:05.000000 star-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 21:01:34.121928 star-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-12-06 21:01:05.000000 star-local-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 21:01:34.117927 star-local-0.0.8/star_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 21:01:34.121928 star-local-0.0.8/star_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 21:01:05.000000 star-local-0.0.8/star_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2023-12-06 21:01:05.000000 star-local-0.0.8/star_local/src/entity_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-06 21:01:05.000000 star-local-0.0.8/star_local/src/exception_star.py
--rw-r--r--   0 runner    (1001) docker     (127)     6498 2023-12-06 21:01:05.000000 star-local-0.0.8/star_local/src/star_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-12-06 21:01:05.000000 star-local-0.0.8/star_local/src/star_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 21:01:34.121928 star-local-0.0.8/star_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-06 21:01:34.000000 star-local-0.0.8/star_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-06 21:01:34.000000 star-local-0.0.8/star_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 21:01:34.000000 star-local-0.0.8/star_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-06 21:01:34.000000 star-local-0.0.8/star_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-06 21:01:34.000000 star-local-0.0.8/star_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 22:27:01.369508 star-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-06 22:27:01.369508 star-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-12-06 22:26:37.000000 star-local-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-06 22:26:37.000000 star-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 22:27:01.369508 star-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-12-06 22:26:37.000000 star-local-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 22:27:01.365508 star-local-0.0.9/star_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 22:27:01.369508 star-local-0.0.9/star_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 22:26:37.000000 star-local-0.0.9/star_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2023-12-06 22:26:37.000000 star-local-0.0.9/star_local/src/entity_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-06 22:26:37.000000 star-local-0.0.9/star_local/src/exception_star.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2023-12-06 22:26:37.000000 star-local-0.0.9/star_local/src/star_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-12-06 22:26:37.000000 star-local-0.0.9/star_local/src/star_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 22:27:01.369508 star-local-0.0.9/star_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-06 22:27:01.000000 star-local-0.0.9/star_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-06 22:27:01.000000 star-local-0.0.9/star_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 22:27:01.000000 star-local-0.0.9/star_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-06 22:27:01.000000 star-local-0.0.9/star_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-06 22:27:01.000000 star-local-0.0.9/star_local.egg-info/top_level.txt
```

### Comparing `star-local-0.0.8/PKG-INFO` & `star-local-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: star-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles <short-project-name-with-dash> Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `star-local-0.0.8/README.md` & `star-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `star-local-0.0.8/pyproject.toml` & `star-local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `star-local-0.0.8/setup.py` & `star-local-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 PACKAGE_NAME = "star-local"
 # Since all PACAKGE_NAMEs are with an underscore, we don't need this. Why do we need it?
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix). Only lowercase, no underlines.
     name=PACKAGE_NAME,
-    version='0.0.8',  # update only the minor version each time # https://pypi.org/project/<short-project-name-with-underscores>/
+    version='0.0.9',  # update only the minor version each time # https://pypi.org/project/<short-project-name-with-underscores>/
     
     author="Circles",
     author_email="info@circlez.ai",
     # TODO: Please update the description and delete this line
     description="PyPI Package for Circles <short-project-name-with-dash> Python",
     long_description="PyPI Package for Circles <short-project-name-with-dash> Python",
     long_description_content_type='text/markdown',
```

### Comparing `star-local-0.0.8/star_local/src/entity_constants.py` & `star-local-0.0.9/star_local/src/entity_constants.py`

 * *Files identical despite different names*

### Comparing `star-local-0.0.8/star_local/src/star_local.py` & `star-local-0.0.9/star_local/src/star_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 object1 =StarLocalConstants.STAR_LOCAL_PYTHON_CODE_LOGGER_OBJECT
 logger=Logger.create_logger(object=object1)
 
 
 class StarsLocal(GenericCRUD):
     def __init__(self) -> None:
         super().__init__(default_schema_name="action_star_subscription")
-
+   
     @staticmethod
-    def _get_the_action_stars_by_profile_id_action_id(profile_id, action_id)->int:
+    def __get_the_action_stars_by_profile_id_action_id(profile_id, action_id)->int:
         start_obj = {"profile_id": str(profile_id), "action_id": str(action_id)}
         logger.start(object=start_obj)
         try:
             user=UserContext.login_using_user_identification_and_password()
             subscription_id = user.get_effective_subscription_id()
             select_clause = "action_stars"
             where = "subscription_id = {} AND action_id = {}".format(subscription_id, action_id)
@@ -36,20 +36,20 @@
             action_star = stars_local.select_one_tuple_by_where(
                     view_table_name="action_star_subscription_view", select_clause_value=select_clause, where=where)
         except Exception as e:
             logger.exception(object=e)
             raise
         logger.end(object={'action_star': str(action_star[0])})
         return action_star[0]
-    
-    def _update_profile_stars(profile_id:int,action_id:int):
+    @staticmethod
+    def __update_profile_stars(profile_id:int,action_id:int):
         start_obj = {"profile_id": str(profile_id), "action_id": str(action_id)}
         logger.start(object=start_obj)
         try:
-            action_stars = StarsLocal._get_the_action_stars_by_profile_id_action_id(profile_id, action_id)
+            action_stars = StarsLocal.__get_the_action_stars_by_profile_id_action_id(profile_id, action_id)
             connection = Connector.connect("profile")
             cursor = connection.cursor()
             query = """ UPDATE profile.profile_table SET stars=stars+ %s WHERE profile_id= %s"""
             try:
                 cursor.execute(query, (action_stars,profile_id))
             except mysql.connector.errors.DataError as excption:
                 logger.exception(object=excption)
@@ -63,50 +63,50 @@
         except Exception as e:
             logger.exception(object=e)
             raise
         logger.info( {'action_id': action_id, #'stars': stars,# 
                       'action_stars': action_stars })
         logger.end()
 
-
-    def _api_executed(api_type_id:int):
+    @staticmethod
+    def api_executed(api_type_id:int):
         start_obj = {"api_type_id": str(api_type_id)}
         logger.start(object=start_obj)
         try:
             
             connection = Connector.connect("api_type")
             cursor = connection.cursor()
             query = f"""SELECT action_id FROM api_type.api_type_view WHERE api_type_id=%s"""
             cursor.execute(query, (api_type_id,))
             action_id=cursor.fetchone()
             user_context=UserContext.login_using_user_identification_and_password()
             profile_id = user_context.get_effective_profile_id()
-            StarsLocal._update_profile_stars(profile_id,action_id[0])
+            StarsLocal.__update_profile_stars(profile_id,action_id[0])
         except Exception as e:
             logger.exception(object=e)
             raise
         logger.end()
-    
-    def how_many_stars_for_action_id(action_id:int)->int:
+    @staticmethod
+    def __how_many_stars_for_action_id(action_id:int)->int:
         start_obj = {"action_id": str(action_id)}
         logger.start(object=start_obj)
         try:
             connection = Connector.connect("action_star_subscription")
             cursor = connection.cursor()
             query="SELECT action_stars FROM action_star_subscription.action_star_subscription_view WHERE action_id=%s"
             cursor.execute(query, (action_id,))
             action_stars=cursor.fetchone()
         except Exception as e:
             logger.exception(object=e)
             raise
         logger.end(object={'action_star': str(action_stars[0])})
 
         return action_stars[0]
-   
-    def how_many_stars_for_profile_id(profile_id:int,user_id:int)->int:
+    @staticmethod
+    def __how_many_stars_for_profile_id_and_user_id(profile_id:int,user_id:int)->int:
         start_obj = {"profile_id": str(profile_id)}
         logger.start(object=start_obj)
         try:
             connection = Connector.connect("profile")
             cursor = connection.cursor()
             query ="SELECT stars FROM profile.profile_view WHERE profile_id=%s"
             cursor.execute(query, (profile_id,))
@@ -117,24 +117,24 @@
             star_total=profile_stars[0]+user_stars[0]
         except Exception as e:
             logger.exception(object=e)
             raise
         logger.end(object={'action_star': str(star_total)})
         return star_total
         
-    
-    def _profile_star_before_action(action_id:int):
+    @staticmethod
+    def profile_star_before_action(action_id:int):
         start_obj = {"action_id": str(action_id)}
         logger.start(object=start_obj)
         try:
-            stars_for_action=StarsLocal.how_many_stars_for_action_id(action_id)
+            stars_for_action=StarsLocal.__how_many_stars_for_action_id(action_id)
             user_context=UserContext.login_using_user_identification_and_password()
             profile_id=user_context.get_effective_profile_id()
             user_id=user_context.get_effective_user_id()
-            stars_for_profile=StarsLocal.how_many_stars_for_profile_id(profile_id,user_id)
+            stars_for_profile=StarsLocal.__how_many_stars_for_profile_id_and_user_id(profile_id,user_id)
             if stars_for_profile+stars_for_action < 0:
                 raise NotEnoughStarsForActivityException
             else:
                 return
         except Exception as e:
             logger.exception(object=e)
             raise
```

### Comparing `star-local-0.0.8/star_local/src/star_transaction.py` & `star-local-0.0.9/star_local/src/star_transaction.py`

 * *Files identical despite different names*

### Comparing `star-local-0.0.8/star_local.egg-info/PKG-INFO` & `star-local-0.0.9/star_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: star-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles <short-project-name-with-dash> Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

