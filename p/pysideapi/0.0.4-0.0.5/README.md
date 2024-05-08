# Comparing `tmp/pysideapi-0.0.4.tar.gz` & `tmp/pysideapi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysideapi-0.0.4.tar", last modified: Mon Feb 26 18:28:57 2024, max compression
+gzip compressed data, was "pysideapi-0.0.5.tar", last modified: Wed May  8 09:11:57 2024, max compression
```

## Comparing `pysideapi-0.0.4.tar` & `pysideapi-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-02-26 18:28:57.767615 pysideapi-0.0.4/
--rw-r--r--   0 jhoncastro   (501) staff       (20)       30 2023-08-30 21:11:24.000000 pysideapi-0.0.4/LICENSE.txt
--rw-r--r--   0 jhoncastro   (501) staff       (20)      268 2024-02-26 18:28:57.767691 pysideapi-0.0.4/PKG-INFO
--rw-r--r--   0 jhoncastro   (501) staff       (20)     1596 2023-08-30 22:11:02.000000 pysideapi-0.0.4/README.md
-drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-02-26 18:28:57.763155 pysideapi-0.0.4/dictamen/
--rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-06-16 06:55:59.000000 pysideapi-0.0.4/dictamen/__init__.py
--rw-r--r--   0 jhoncastro   (501) staff       (20)     1638 2023-08-30 22:37:29.000000 pysideapi-0.0.4/dictamen/dictamen.py
--rw-r--r--   0 jhoncastro   (501) staff       (20)      214 2023-06-17 23:42:41.000000 pysideapi-0.0.4/dictamen/validator_rule.py
-drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-02-26 18:28:57.763378 pysideapi-0.0.4/dictionary/
--rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-06-16 06:58:46.000000 pysideapi-0.0.4/dictionary/__init__.py
-drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-02-26 18:28:57.763487 pysideapi-0.0.4/jira/
--rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-08-30 22:34:45.000000 pysideapi-0.0.4/jira/__init__.py
-drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-02-26 18:28:57.763997 pysideapi-0.0.4/jira/api_client/
--rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-08-29 23:03:21.000000 pysideapi-0.0.4/jira/api_client/__init__.py
--rw-r--r--   0 jhoncastro   (501) staff       (20)     3804 2023-08-30 20:10:03.000000 pysideapi-0.0.4/jira/api_client/jira_api.py
--rw-r--r--   0 jhoncastro   (501) staff       (20)      910 2023-08-31 05:31:06.000000 pysideapi-0.0.4/jira/api_client/jira_session.py
-drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-02-26 18:28:57.764383 pysideapi-0.0.4/jira/commons/
--rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-08-29 23:29:47.000000 pysideapi-0.0.4/jira/commons/__init__.py
--rw-r--r--   0 jhoncastro   (501) staff       (20)     2106 2023-08-30 00:05:15.000000 pysideapi-0.0.4/jira/commons/constants.py
-drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-02-26 18:28:57.765788 pysideapi-0.0.4/jira/model/
--rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-08-29 23:04:19.000000 pysideapi-0.0.4/jira/model/__init__.py
--rw-r--r--   0 jhoncastro   (501) staff       (20)     3519 2023-08-30 20:40:19.000000 pysideapi-0.0.4/jira/model/feature.py
--rw-r--r--   0 jhoncastro   (501) staff       (20)     2339 2024-02-26 18:13:05.000000 pysideapi-0.0.4/jira/model/issue_base.py
--rw-r--r--   0 jhoncastro   (501) staff       (20)      305 2023-08-29 23:23:35.000000 pysideapi-0.0.4/jira/model/issue_status.py
--rw-r--r--   0 jhoncastro   (501) staff       (20)      206 2023-08-29 23:23:35.000000 pysideapi-0.0.4/jira/model/issue_task.py
--rw-r--r--   0 jhoncastro   (501) staff       (20)     3147 2023-08-30 20:40:19.000000 pysideapi-0.0.4/jira/model/story.py
-drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-02-26 18:28:57.766166 pysideapi-0.0.4/jira/producer/
--rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-08-29 23:22:37.000000 pysideapi-0.0.4/jira/producer/__init__.py
--rw-r--r--   0 jhoncastro   (501) staff       (20)     1604 2023-08-30 08:50:27.000000 pysideapi-0.0.4/jira/producer/jira_producer.py
-drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-02-26 18:28:57.766546 pysideapi-0.0.4/jira/utils/
--rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-08-30 00:18:49.000000 pysideapi-0.0.4/jira/utils/__init__.py
--rw-r--r--   0 jhoncastro   (501) staff       (20)     4128 2023-08-30 00:34:53.000000 pysideapi-0.0.4/jira/utils/issue_utils.py
-drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-02-26 18:28:57.767509 pysideapi-0.0.4/pysideapi.egg-info/
--rw-r--r--   0 jhoncastro   (501) staff       (20)      268 2024-02-26 18:28:57.000000 pysideapi-0.0.4/pysideapi.egg-info/PKG-INFO
--rw-r--r--   0 jhoncastro   (501) staff       (20)      700 2024-02-26 18:28:57.000000 pysideapi-0.0.4/pysideapi.egg-info/SOURCES.txt
--rw-r--r--   0 jhoncastro   (501) staff       (20)        1 2024-02-26 18:28:57.000000 pysideapi-0.0.4/pysideapi.egg-info/dependency_links.txt
--rw-r--r--   0 jhoncastro   (501) staff       (20)       14 2024-02-26 18:28:57.000000 pysideapi-0.0.4/pysideapi.egg-info/requires.txt
--rw-r--r--   0 jhoncastro   (501) staff       (20)       25 2024-02-26 18:28:57.000000 pysideapi-0.0.4/pysideapi.egg-info/top_level.txt
--rw-r--r--   0 jhoncastro   (501) staff       (20)       79 2024-02-26 18:28:57.767936 pysideapi-0.0.4/setup.cfg
--rw-r--r--   0 jhoncastro   (501) staff       (20)      551 2024-02-26 17:57:31.000000 pysideapi-0.0.4/setup.py
+drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-05-08 09:11:57.819916 pysideapi-0.0.5/
+-rw-r--r--   0 jhoncastro   (501) staff       (20)       30 2023-08-30 21:11:24.000000 pysideapi-0.0.5/LICENSE.txt
+-rw-r--r--   0 jhoncastro   (501) staff       (20)      268 2024-05-08 09:11:57.820016 pysideapi-0.0.5/PKG-INFO
+-rw-r--r--   0 jhoncastro   (501) staff       (20)     1596 2023-08-30 22:11:02.000000 pysideapi-0.0.5/README.md
+drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-05-08 09:11:57.815252 pysideapi-0.0.5/dictamen/
+-rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-06-16 06:55:59.000000 pysideapi-0.0.5/dictamen/__init__.py
+-rw-r--r--   0 jhoncastro   (501) staff       (20)     1638 2023-08-30 22:37:29.000000 pysideapi-0.0.5/dictamen/dictamen.py
+-rw-r--r--   0 jhoncastro   (501) staff       (20)      214 2023-06-17 23:42:41.000000 pysideapi-0.0.5/dictamen/validator_rule.py
+drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-05-08 09:11:57.815529 pysideapi-0.0.5/dictionary/
+-rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-06-16 06:58:46.000000 pysideapi-0.0.5/dictionary/__init__.py
+drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-05-08 09:11:57.815639 pysideapi-0.0.5/jira/
+-rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-08-30 22:34:45.000000 pysideapi-0.0.5/jira/__init__.py
+drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-05-08 09:11:57.816176 pysideapi-0.0.5/jira/api_client/
+-rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-08-29 23:03:21.000000 pysideapi-0.0.5/jira/api_client/__init__.py
+-rw-r--r--   0 jhoncastro   (501) staff       (20)     3804 2023-08-30 20:10:03.000000 pysideapi-0.0.5/jira/api_client/jira_api.py
+-rw-r--r--   0 jhoncastro   (501) staff       (20)      910 2023-08-31 05:31:06.000000 pysideapi-0.0.5/jira/api_client/jira_session.py
+drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-05-08 09:11:57.816608 pysideapi-0.0.5/jira/commons/
+-rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-08-29 23:29:47.000000 pysideapi-0.0.5/jira/commons/__init__.py
+-rw-r--r--   0 jhoncastro   (501) staff       (20)     2218 2024-05-08 08:15:22.000000 pysideapi-0.0.5/jira/commons/constants.py
+drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-05-08 09:11:57.818057 pysideapi-0.0.5/jira/model/
+-rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-08-29 23:04:19.000000 pysideapi-0.0.5/jira/model/__init__.py
+-rw-r--r--   0 jhoncastro   (501) staff       (20)     3519 2023-08-30 20:40:19.000000 pysideapi-0.0.5/jira/model/feature.py
+-rw-r--r--   0 jhoncastro   (501) staff       (20)     2339 2024-02-26 18:13:05.000000 pysideapi-0.0.5/jira/model/issue_base.py
+-rw-r--r--   0 jhoncastro   (501) staff       (20)      305 2023-08-29 23:23:35.000000 pysideapi-0.0.5/jira/model/issue_status.py
+-rw-r--r--   0 jhoncastro   (501) staff       (20)      206 2023-08-29 23:23:35.000000 pysideapi-0.0.5/jira/model/issue_task.py
+-rw-r--r--   0 jhoncastro   (501) staff       (20)     5117 2024-05-08 09:03:07.000000 pysideapi-0.0.5/jira/model/story.py
+drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-05-08 09:11:57.818494 pysideapi-0.0.5/jira/producer/
+-rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-08-29 23:22:37.000000 pysideapi-0.0.5/jira/producer/__init__.py
+-rw-r--r--   0 jhoncastro   (501) staff       (20)     1604 2023-08-30 08:50:27.000000 pysideapi-0.0.5/jira/producer/jira_producer.py
+drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-05-08 09:11:57.818870 pysideapi-0.0.5/jira/utils/
+-rw-r--r--   0 jhoncastro   (501) staff       (20)        0 2023-08-30 00:18:49.000000 pysideapi-0.0.5/jira/utils/__init__.py
+-rw-r--r--   0 jhoncastro   (501) staff       (20)     4128 2023-08-30 00:34:53.000000 pysideapi-0.0.5/jira/utils/issue_utils.py
+drwxr-xr-x   0 jhoncastro   (501) staff       (20)        0 2024-05-08 09:11:57.819782 pysideapi-0.0.5/pysideapi.egg-info/
+-rw-r--r--   0 jhoncastro   (501) staff       (20)      268 2024-05-08 09:11:57.000000 pysideapi-0.0.5/pysideapi.egg-info/PKG-INFO
+-rw-r--r--   0 jhoncastro   (501) staff       (20)      700 2024-05-08 09:11:57.000000 pysideapi-0.0.5/pysideapi.egg-info/SOURCES.txt
+-rw-r--r--   0 jhoncastro   (501) staff       (20)        1 2024-05-08 09:11:57.000000 pysideapi-0.0.5/pysideapi.egg-info/dependency_links.txt
+-rw-r--r--   0 jhoncastro   (501) staff       (20)       14 2024-05-08 09:11:57.000000 pysideapi-0.0.5/pysideapi.egg-info/requires.txt
+-rw-r--r--   0 jhoncastro   (501) staff       (20)       25 2024-05-08 09:11:57.000000 pysideapi-0.0.5/pysideapi.egg-info/top_level.txt
+-rw-r--r--   0 jhoncastro   (501) staff       (20)       79 2024-05-08 09:11:57.820293 pysideapi-0.0.5/setup.cfg
+-rw-r--r--   0 jhoncastro   (501) staff       (20)      552 2024-05-08 09:11:56.000000 pysideapi-0.0.5/setup.py
```

### Comparing `pysideapi-0.0.4/README.md` & `pysideapi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pysideapi-0.0.4/dictamen/dictamen.py` & `pysideapi-0.0.5/dictamen/dictamen.py`

 * *Files identical despite different names*

### Comparing `pysideapi-0.0.4/jira/api_client/jira_api.py` & `pysideapi-0.0.5/jira/api_client/jira_api.py`

 * *Files identical despite different names*

### Comparing `pysideapi-0.0.4/jira/api_client/jira_session.py` & `pysideapi-0.0.5/jira/api_client/jira_session.py`

 * *Files identical despite different names*

### Comparing `pysideapi-0.0.4/jira/commons/constants.py` & `pysideapi-0.0.5/jira/commons/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 class Constants:
     CRITERIA_TO_FIND_TABLE = "|\r\n|"
+    CRITERIA_TO_FIND_START_TEAM_BACKLOG = 'Peru'
+    CRITERIA_TO_FIND_END_TEAM_BACKLOG = '</span>\n  </button>'
     PIPE_ID = "|"
     CRITERIA_TO_FIND_GS = "spreadsheets/d/"
     SLASH_ID = "/"
     JIRA_SERVER = "https://jira.globaldevtools.bbva.com"
     JIRA_API_SESSION = f"{JIRA_SERVER}/rest/auth/1/session"
     JIRA_API_JQL = f"{JIRA_SERVER}/rest/api/2/search?jql="
```

### Comparing `pysideapi-0.0.4/jira/model/feature.py` & `pysideapi-0.0.5/jira/model/feature.py`

 * *Files identical despite different names*

### Comparing `pysideapi-0.0.4/jira/model/issue_base.py` & `pysideapi-0.0.5/jira/model/issue_base.py`

 * *Files identical despite different names*

### Comparing `pysideapi-0.0.4/jira/producer/jira_producer.py` & `pysideapi-0.0.5/jira/producer/jira_producer.py`

 * *Files identical despite different names*

### Comparing `pysideapi-0.0.4/jira/utils/issue_utils.py` & `pysideapi-0.0.5/jira/utils/issue_utils.py`

 * *Files identical despite different names*

### Comparing `pysideapi-0.0.4/pysideapi.egg-info/SOURCES.txt` & `pysideapi-0.0.5/pysideapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysideapi-0.0.4/setup.py` & `pysideapi-0.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from setuptools import setup,  find_packages
 
 setup(
     name="pysideapi",
     packages=['jira','jira.producer','jira.model','jira.utils','jira.commons','jira.api_client',
         'dictamen','dictionary'],
     include_package_data=True,
-    version="0.0.4",
+    version="0.0.5",
     license = "MIT",
     description= "Paquete que me permite trabajar con jira, dicccionario y dictamen",
     author="Jhon Castro",
     author_email= "jhoncc20@gmail.com",
     install_requires=['requests','pytz'],
     classifiers = ["Programming Language :: Python :: 3"]
 
-)
+)
```

