# Comparing `tmp/datagov_harvesting_logic-0.4.0.tar.gz` & `tmp/datagov_harvesting_logic-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagov_harvesting_logic-0.4.0.tar", max compression
+gzip compressed data, was "datagov_harvesting_logic-0.4.1.tar", max compression
```

## Comparing `datagov_harvesting_logic-0.4.0.tar` & `datagov_harvesting_logic-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1878 2024-05-06 18:08:58.498361 datagov_harvesting_logic-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     5935 2024-05-06 18:08:58.498361 datagov_harvesting_logic-0.4.0/README.md
--rw-r--r--   0        0        0      164 2024-05-06 18:08:58.506361 datagov_harvesting_logic-0.4.0/harvester/__init__.py
--rw-r--r--   0        0        0     8369 2024-05-06 18:08:58.506361 datagov_harvesting_logic-0.4.0/harvester/ckan_utils.py
--rw-r--r--   0        0        0     2158 2024-05-06 18:08:58.506361 datagov_harvesting_logic-0.4.0/harvester/exceptions.py
--rw-r--r--   0        0        0    14138 2024-05-06 18:08:58.506361 datagov_harvesting_logic-0.4.0/harvester/harvest.py
--rw-r--r--   0        0        0      589 2024-05-06 18:08:58.506361 datagov_harvesting_logic-0.4.0/harvester/logger_config.py
--rw-r--r--   0        0        0     4039 2024-05-06 18:08:58.506361 datagov_harvesting_logic-0.4.0/harvester/utils.py
--rw-r--r--   0        0        0     2275 2024-05-06 18:08:58.506361 datagov_harvesting_logic-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7180 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1878 2024-05-07 22:36:52.669434 datagov_harvesting_logic-0.4.1/LICENSE.md
+-rw-r--r--   0        0        0     5935 2024-05-07 22:36:52.669434 datagov_harvesting_logic-0.4.1/README.md
+-rw-r--r--   0        0        0      164 2024-05-07 22:36:52.677434 datagov_harvesting_logic-0.4.1/harvester/__init__.py
+-rw-r--r--   0        0        0     8369 2024-05-07 22:36:52.677434 datagov_harvesting_logic-0.4.1/harvester/ckan_utils.py
+-rw-r--r--   0        0        0     2158 2024-05-07 22:36:52.677434 datagov_harvesting_logic-0.4.1/harvester/exceptions.py
+-rw-r--r--   0        0        0    14138 2024-05-07 22:36:52.677434 datagov_harvesting_logic-0.4.1/harvester/harvest.py
+-rw-r--r--   0        0        0      589 2024-05-07 22:36:52.677434 datagov_harvesting_logic-0.4.1/harvester/logger_config.py
+-rw-r--r--   0        0        0     4058 2024-05-07 22:36:52.677434 datagov_harvesting_logic-0.4.1/harvester/utils.py
+-rw-r--r--   0        0        0     2275 2024-05-07 22:36:52.677434 datagov_harvesting_logic-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7180 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.4.1/PKG-INFO
```

### Comparing `datagov_harvesting_logic-0.4.0/LICENSE.md` & `datagov_harvesting_logic-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.0/README.md` & `datagov_harvesting_logic-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.0/harvester/ckan_utils.py` & `datagov_harvesting_logic-0.4.1/harvester/ckan_utils.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.0/harvester/exceptions.py` & `datagov_harvesting_logic-0.4.1/harvester/exceptions.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.0/harvester/harvest.py` & `datagov_harvesting_logic-0.4.1/harvester/harvest.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.0/harvester/logger_config.py` & `datagov_harvesting_logic-0.4.1/harvester/logger_config.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.4.0/harvester/utils.py` & `datagov_harvesting_logic-0.4.1/harvester/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 def get_title_from_fgdc(xml_str: str) -> str:
     tree = ET.ElementTree(ET.fromstring(xml_str))
     return tree.find(".//title").text
 
 
 def parse_args(args):
-
     parser = argparse.ArgumentParser(
         prog="Harvest Runner", description="etl harvest sources"
     )
     parser.add_argument("-j", "--jobid")
 
     return parser.parse_args(args)
 
@@ -110,14 +109,15 @@
 
 
 class CFHandler:
     def __init__(self, url: str, user: str, password: str):
         self.url = url
         self.user = user
         self.password = password
+        self.setup()
 
     def setup(self):
         self.client = CloudFoundryClient(self.url)
         self.client.init_with_user_credentials(self.user, self.password)
         self.task_mgr = TaskManager(self.url, self.client)
 
     def start_task(self, app_guuid, command, task_id):
@@ -132,11 +132,10 @@
     def get_all_app_tasks(self, app_guuid):
         return [task for task in self.client.v3.apps[app_guuid].tasks()]
 
     def get_all_running_tasks(self, tasks):
         return sum(1 for _ in filter(lambda task: task["state"] == "RUNNING", tasks))
 
     def read_recent_app_logs(self, app_guuid, task_id=None):
-
         app = self.client.v2.apps[app_guuid]
         logs = filter(lambda lg: task_id in lg, [str(log) for log in app.recent_logs()])
         return "\n".join(logs)
```

### Comparing `datagov_harvesting_logic-0.4.0/pyproject.toml` & `datagov_harvesting_logic-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datagov-harvesting-logic"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 # authors = [
 #     {name = "Jin Sun", email = "jin.sun@gsa.gov"},
 #     {name = "Tyler Burton", email = "tyler.burton@gsa.gov"},
 # ]
 authors = [
     "Datagov Team <datagov@gsa.gov>",
```

### Comparing `datagov_harvesting_logic-0.4.0/PKG-INFO` & `datagov_harvesting_logic-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagov-harvesting-logic
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Home-page: https://github.com/GSA/datagov-harvesting-logic
 License: LICENSE.md
 Author: Datagov Team
 Author-email: datagov@gsa.gov
 Maintainer: Datagov Team
 Maintainer-email: datagov@gsa.gov
```

