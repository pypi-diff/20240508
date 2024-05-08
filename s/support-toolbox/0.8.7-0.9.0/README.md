# Comparing `tmp/support-toolbox-0.8.7.tar.gz` & `tmp/support-toolbox-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "support-toolbox-0.8.7.tar", last modified: Thu Apr 25 15:01:52 2024, max compression
+gzip compressed data, was "support-toolbox-0.9.0.tar", last modified: Wed May  8 14:50:45 2024, max compression
```

## Comparing `support-toolbox-0.8.7.tar` & `support-toolbox-0.9.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:52.853061 support-toolbox-0.8.7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-04-25 15:01:52.853061 support-toolbox-0.8.7/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2495 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-25 15:01:52.853061 support-toolbox-0.8.7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:52.849060 support-toolbox-0.8.7/support_toolbox/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:52.849060 support-toolbox-0.8.7/support_toolbox/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1551 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4522 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/entitlements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      615 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2720 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/org.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1338 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3675 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/service_account.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2377 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/site.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2022 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/api/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:52.853061 support-toolbox-0.8.7/support_toolbox/app_handler/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/app_handler/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/app_handler/app.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/app_handler/app_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      761 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/app_handler/auto_updater.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/app_handler/token_manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3845 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/clear_user_layer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4590 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/delete_users.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2208 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/deploy_browse_card.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1355 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/deploy_ctk_service_account.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5379 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/deploy_integrations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18802 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/deploy_pi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      294 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2728 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/onboard_ctk_orgs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2158 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/revert_soft_delete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1319 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/update_saml.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:52.853061 support-toolbox-0.8.7/support_toolbox/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1695 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/utils/api_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/utils/csv_to_iris.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6826 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/utils/metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/utils/resource_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2024-04-25 15:01:45.000000 support-toolbox-0.8.7/support_toolbox/utils/saml_parser.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 15:01:52.853061 support-toolbox-0.8.7/support_toolbox.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-04-25 15:01:52.000000 support-toolbox-0.8.7/support_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1331 2024-04-25 15:01:52.000000 support-toolbox-0.8.7/support_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-25 15:01:52.000000 support-toolbox-0.8.7/support_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2024-04-25 15:01:52.000000 support-toolbox-0.8.7/support_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-04-25 15:01:52.000000 support-toolbox-0.8.7/support_toolbox.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-25 15:01:52.000000 support-toolbox-0.8.7/support_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:45.433811 support-toolbox-0.9.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-05-08 14:50:45.433811 support-toolbox-0.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2495 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-08 14:50:45.433811 support-toolbox-0.9.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:45.425810 support-toolbox-0.9.0/support_toolbox/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:45.433811 support-toolbox-0.9.0/support_toolbox/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4294 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/entitlements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      615 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2549 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/org.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1338 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3675 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/service_account.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2206 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/site.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1853 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:45.433811 support-toolbox-0.9.0/support_toolbox/app_handler/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/app_handler/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/app_handler/app.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/app_handler/app_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      761 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/app_handler/auto_updater.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/app_handler/token_manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3845 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/clear_user_layer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4590 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/delete_users.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2208 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/deploy_browse_card.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1355 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/deploy_ctk_service_account.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5379 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/deploy_integrations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18802 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/deploy_pi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      294 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2728 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/onboard_ctk_orgs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2158 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/revert_soft_delete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1319 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/update_saml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:45.433811 support-toolbox-0.9.0/support_toolbox/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1969 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/utils/api_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/utils/csv_to_iris.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6168 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/utils/metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/utils/resource_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/utils/saml_parser.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:45.433811 support-toolbox-0.9.0/support_toolbox.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-05-08 14:50:45.000000 support-toolbox-0.9.0/support_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1331 2024-05-08 14:50:45.000000 support-toolbox-0.9.0/support_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-08 14:50:45.000000 support-toolbox-0.9.0/support_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2024-05-08 14:50:45.000000 support-toolbox-0.9.0/support_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-05-08 14:50:45.000000 support-toolbox-0.9.0/support_toolbox.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-08 14:50:45.000000 support-toolbox-0.9.0/support_toolbox.egg-info/top_level.txt
```

### Comparing `support-toolbox-0.8.7/PKG-INFO` & `support-toolbox-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: support-toolbox
-Version: 0.8.7
+Version: 0.9.0
 Summary: A suite of CLI tools for the data.world support team
 Home-page: https://github.com/datadotworld/support-toolbox/tree/main
 Author: Jack Compton
 Author-email: jack.compton@data.world
 Requires-Dist: certifi==2023.7.22
 Requires-Dist: charset-normalizer==3.2.0
 Requires-Dist: defusedxml==0.7.1
```

### Comparing `support-toolbox-0.8.7/README.md` & `support-toolbox-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/setup.py` & `support-toolbox-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/api/dataset.py` & `support-toolbox-0.9.0/support_toolbox/api/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,29 +31,25 @@
 
 def set_dataset_ingest(api_url, admin_token, org_id, dataset_id):
     set_ingest_limit_url = f"{api_url}/admin/datasets/{org_id}/{dataset_id}/ingest"
 
     header = {
         'Accept': 'application/json',
         'Content-Type': 'application/json',
-        'Authorization': f'Bearer {admin_token}'
-    }
-
-    cookies = {
-        'adminToken': admin_token
+        'Cookie': f'token={admin_token};adminToken={admin_token}'
     }
 
     payload = {
         "agentid": org_id,
         "datasetid": dataset_id,
         # 50GB as requested by Bernie for PMs to upload implementation recordings
         "ingestQuota": 53690000000
     }
 
     body = json.dumps(payload)
 
-    response = requests.put(set_ingest_limit_url, body, cookies=cookies, headers=header)
+    response = requests.put(set_ingest_limit_url, body, headers=header)
 
     if response.status_code == 200:
         print(f"Set 50GB ingest limit for: {org_id}/{dataset_id}")
     else:
         print(response.text)
```

### Comparing `support-toolbox-0.8.7/support_toolbox/api/entitlements.py` & `support-toolbox-0.9.0/support_toolbox/api/entitlements.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,19 +21,15 @@
 
 def update_org_entitlements(api_url, admin_token, org_id, product_id, order, source, name):
     update_entitlements_url = f"{api_url}/entitlements"
 
     header = {
         'Accept': 'application/json',
         'Content-Type': 'application/json',
-        'Authorization': f'Bearer {admin_token}'
-    }
-
-    cookies = {
-        'adminToken': admin_token
+        'Cookie': f'token={admin_token};adminToken={admin_token}'
     }
 
     # Format the datetime as a string in the expected format
     now = datetime.now()
     timestamp = now.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
 
     data = {
@@ -46,37 +42,33 @@
       ],
       "order": order,
       "source": source,
       "startDate": timestamp
     }
 
     body = json.dumps(data)
-    response = requests.post(update_entitlements_url, body, cookies=cookies, headers=header)
+    response = requests.post(update_entitlements_url, body, headers=header)
 
     # Verify the update
     if response.status_code == 200:
         print(f"Successfully updated {org_id} with {name}")
     else:
         print(response.text)
 
 
 def get_entitlements(api_url, admin_token, org_id):
     get_entitlements_url = f"{api_url}/entitlements/{org_id}"
 
     header = {
         'Accept': 'application/json',
         'Content-Type': 'application/json',
-        'Authorization': f'Bearer {admin_token}'
-    }
-
-    cookies = {
-        'adminToken': admin_token
+        'Cookie': f'token={admin_token};adminToken={admin_token}'
     }
 
-    response = requests.get(get_entitlements_url, cookies=cookies, headers=header)
+    response = requests.get(get_entitlements_url, headers=header)
 
     # Verify the response
     if response.status_code == 200:
         response_json = response.json()
         return response_json['records'][0]['source']
     else:
         print(response.text)
@@ -84,22 +76,18 @@
 
 def get_default_values(api_url, admin_token, agent_type):
     get_offering_url = f"{api_url}/offerings/agentTypes/{agent_type}"
 
     header = {
         'Accept': 'application/json',
         'Content-Type': 'application/json',
-        'Authorization': f'Bearer {admin_token}'
+        'Cookie': f'token={admin_token};adminToken={admin_token}'
     }
 
-    cookies = {
-        'adminToken': admin_token
-    }
-
-    response = requests.get(get_offering_url, cookies=cookies, headers=header)
+    response = requests.get(get_offering_url, headers=header)
 
     # Verify the response
     if response.status_code == 200:
         response_json = response.json()
 
         result = {
             'agent_type': response_json['records'][0]['agentType'],
@@ -116,19 +104,15 @@
 # Take an agentType (org or user) as parameter to update the default plan
 def update_default_plan(api_url, admin_token, offering_id, agent_type, offering_slug, product_ids):
     update_default_plan_url = f"{api_url}/offerings/{offering_id}"
 
     header = {
         'Accept': 'application/json',
         'Content-Type': 'application/json',
-        'Authorization': f'Bearer {admin_token}'
-    }
-
-    cookies = {
-        'adminToken': admin_token
+        'Cookie': f'token={admin_token};adminToken={admin_token}'
     }
 
     # Format the datetime as a string in the expected format
     now = datetime.now()
     timestamp = now.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
 
     data = {
@@ -139,15 +123,15 @@
         "pricingModel": {},
         "productids": product_ids,
         "requiresPayment": False,
         "startDate": timestamp
     }
 
     body = json.dumps(data)
-    response = requests.put(update_default_plan_url, body, cookies=cookies, headers=header)
+    response = requests.put(update_default_plan_url, body, headers=header)
 
     if response.status_code == 200:
         all_products = {**ORG_DEFAULT_ENTITLEMENTS, **ORG_ADDON_ENTITLEMENTS, **USER_DEFAULT_ENTITLEMENTS}
         deployed_products = [key for key, value in all_products.items() if value in product_ids]
         print(f"Successfully updated the {agent_type} Default Plan with: {deployed_products}")
     else:
         print(response.text)
```

### Comparing `support-toolbox-0.8.7/support_toolbox/api/file.py` & `support-toolbox-0.9.0/support_toolbox/api/file.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/api/org.py` & `support-toolbox-0.9.0/support_toolbox/api/site.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,80 @@
-import json
 import requests
-import re
-import urllib.parse
-
-
-def validate_org_input(org_name):
-    # Check for anything NOT letter, digit, underscore, or space
-    regex = re.compile(r'[^\w\s-]')
-    return not regex.search(org_name)
+import json
 
 
-def onboard_org(api_url, admin_token, org_id, org_display_name, avatar_url=''):
-    onboard_org_url = f"{api_url}/organizations/onboard"
+def create_site(admin_token, entity_id, public_slug, sso_url, x509_cert, api_url):
+    url = f"{api_url}/admin/sites/create"
 
     header = {
         'Accept': 'application/json',
         'Content-Type': 'application/json',
-        'Authorization': f'Bearer {admin_token}'
-    }
-
-    cookies = {
-        'adminToken': admin_token
+        'Cookie': f'token={admin_token};adminToken={admin_token}'
     }
 
     data = {
-        "agentid": org_id,
-        "avatarUrl": avatar_url,
-        "displayName": org_display_name,
-        "orgDetails": {
-            "allowMembership": True,
-            "allowMembershipRequest": False,
-            "allowProposals": False,
-            "defaultMembershipType": 'PUBLIC'
-        },
-        "visibility": 'OPEN'
+        'entityid': entity_id,
+        'publicSlug': public_slug,
+        'ssoUrl': sso_url,
+        'x509Certificate': x509_cert
     }
 
     body = json.dumps(data)
-    response = requests.post(onboard_org_url, body, cookies=cookies, headers=header)
+    response = requests.post(url, body, headers=header)
 
-    # Verify the creation
     if response.status_code == 200:
-        print(f"Successfully created {org_id}")
+        print(f"Successfully created the site: {response.text}")
     else:
         print(response.text)
 
 
-# By default, authorizes a party or agent_id access to any org_id passed in
-def authorize_access_to_org(api_url, admin_token, org_id, party):
-    encoded_party = urllib.parse.quote(party, safe='')
-
-    authorize_access_to_org_url = f"{api_url}/admin/organizations/{org_id}/authorizations/{encoded_party}"
+def edit_saml(admin_token, entity_id, site_id, default_org_list, sso_url, x509_cert, api_url):
+    resource_id = f"site%3A{site_id}"
+    url = f"{api_url}/admin/saml/{resource_id}"
 
     header = {
         'Accept': 'application/json',
         'Content-Type': 'application/json',
-        'Authorization': f'Bearer {admin_token}'
-    }
-
-    cookies = {
-        'adminToken': admin_token
+        'Cookie': f'token={admin_token};adminToken={admin_token}'
     }
 
+    # Prepare the data to be sent in the request
     data = {
-        "level": "ADMIN",
-        "visibility": "PUBLIC"
+      "agentid": site_id,
+      "defaultOrgList": default_org_list,
+      "entityid": entity_id,
+      "ssoUrl": sso_url,
+      "x509Certificate": x509_cert
     }
 
     body = json.dumps(data)
-    response = requests.put(authorize_access_to_org_url, body, cookies=cookies, headers=header)
+    response = requests.put(url, body, headers=header)
 
-    # Verify the authorization
     if response.status_code == 200:
-        print(f"Authorized {party} ADMIN in {org_id}")
+        print(f"Successfully updated SAML!")
+        print(f"Entity ID: {entity_id}")
+        print(f"SSO Url: {sso_url}")
+        print(f"x509 Certificate: {x509_cert}")
     else:
         print(response.text)
 
 
-def deauthorize_access_to_org(api_url, admin_token, agent_id, org_id):
-    deauthorize_access_to_org_url = f"{api_url}/organizations/{org_id}/authorizations/agent%3A{agent_id}"
+def get_site_id(admin_token, public_slug, api_url):
+    url = f"{api_url}/site/slug/{public_slug}"
 
     header = {
         'Accept': 'application/json',
         'Content-Type': 'application/json',
-        'Authorization': f'Bearer {admin_token}'
+        'Cookie': f'token={admin_token};adminToken={admin_token}'
     }
 
-    cookies = {
-        'adminToken': admin_token
-    }
-
-    response = requests.delete(deauthorize_access_to_org_url, cookies=cookies, headers=header)
+    response = requests.get(url, headers=header)
 
-    # Verify the authorization
     if response.status_code == 200:
-        print(f"Removed {agent_id} from {org_id}")
+        response_json = response.json()
+        site_id = response_json['site']
+        print(f"Found site_id: {site_id} for {public_slug}")
+
+        return site_id, True
     else:
         print(response.text)
+        return None, False
```

### Comparing `support-toolbox-0.8.7/support_toolbox/api/project.py` & `support-toolbox-0.9.0/support_toolbox/api/project.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/api/service_account.py` & `support-toolbox-0.9.0/support_toolbox/api/service_account.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/app_handler/app.py` & `support-toolbox-0.9.0/support_toolbox/app_handler/app.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/app_handler/auto_updater.py` & `support-toolbox-0.9.0/support_toolbox/app_handler/auto_updater.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/app_handler/token_manager.py` & `support-toolbox-0.9.0/support_toolbox/app_handler/token_manager.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/clear_user_layer.py` & `support-toolbox-0.9.0/support_toolbox/clear_user_layer.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/delete_users.py` & `support-toolbox-0.9.0/support_toolbox/delete_users.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/deploy_browse_card.py` & `support-toolbox-0.9.0/support_toolbox/deploy_browse_card.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/deploy_ctk_service_account.py` & `support-toolbox-0.9.0/support_toolbox/deploy_ctk_service_account.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/deploy_integrations.py` & `support-toolbox-0.9.0/support_toolbox/deploy_integrations.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/deploy_pi.py` & `support-toolbox-0.9.0/support_toolbox/deploy_pi.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/onboard_ctk_orgs.py` & `support-toolbox-0.9.0/support_toolbox/onboard_ctk_orgs.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/revert_soft_delete.py` & `support-toolbox-0.9.0/support_toolbox/revert_soft_delete.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/update_saml.py` & `support-toolbox-0.9.0/support_toolbox/update_saml.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/utils/metrics.py` & `support-toolbox-0.9.0/support_toolbox/utils/metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,85 +38,73 @@
 * **Resources** - _granular inventory of resources_
 * **Tops** - _most active users, most frequent searches, etc._
 * **Visits** - _how often is the tool used, by whom_"""
 
 
 def deploy_metrics(api_url, admin_token, public_slug):
     # Ask user to select an option
-    print("Before we continue, please select an option (1/2): ")
+    print("Before we continue, select an option (1/2): ")
     print("1. Existing customer moving to a PI")
     print("2. New customer PI deployment")
     user_choice = input()
 
     # Set existing_customer based on user input
     if user_choice == "1":
         existing_customer = True
     elif user_choice == "2":
         existing_customer = False
     else:
         print("Invalid selection.")
         return
 
-    metrics_deployment_choice = input("Start metrics deployment? (y/n): ")
+    # Standard Org for Metrics
+    org_id = "data-catalog-team"
+    org_display_name = "Data Catalog Team"
+
+    # Optional override of standard naming convention (rare but has happened before)
+    standard_org_choice = input("Use the standard Data Catalog Team org (y/n): ")
+    if standard_org_choice.lower() == 'n':
+        org_id = input("Enter the org id: ")
+        org_display_name = input("Enter the org display name: ")
+
+    print(f"Onboarding {org_id}...")
+    onboard_org(api_url, admin_token, org_id, org_display_name)
+
+    print(f"Authorizing datadotworldsupport access to {org_id}...")
+    authorize_access_to_org(api_url, admin_token, org_id, party='group:datadotworldsupport/members')
+
+    if existing_customer:
+        # Create the baseplatformdata dataset and subsequent four datasets that makeup baseplatformdata - this is default an "All Time" metrics deployment for Existing Customers
+        for dataset in BASEPLATFORM_DATASETS:
+            dataset_id = dataset['title']
+            summary = dataset['summary']
+            visibility = dataset['visibility']
+            create_dataset(admin_token, org_id, dataset_id=dataset_id, visibility=visibility, summary=summary)
 
-    if metrics_deployment_choice.lower() == 'y':
-        org_id = "data-catalog-team"
-        org_display_name = "Data Catalog Team"
+        # Create ddw-metrics-{public_slug} dataset - this is default an "All Time" metrics deployment for Existing Customers
+        create_dataset(admin_token, org_id, dataset_id=f"ddw-metrics-{public_slug}", visibility="PRIVATE", summary=DDW_METRICS_SUMMARY)
 
-        standard_org_choice = input("Use the standard Data Catalog Team org (y/n): ")
-
-        if standard_org_choice.lower() == 'n':
-            org_id = input("Enter the org id: ")
-            org_display_name = input("Enter the org display name: ")
-
-        print(f"Onboarding {org_id}...")
-        onboard_org(api_url, admin_token, org_id, org_display_name)
-
-        print(f"Authorizing datadotworldsupport access to {org_id}...")
-        authorize_access_to_org(api_url, admin_token, org_id, party='group:datadotworldsupport/members')
+    else:
+        all_time_metrics_choice = input("Is the customer paying for the 'All-time' metrics upgrade (y/n): ")
 
-        if existing_customer:
-            # Create the baseplatformdata dataset and subsequent four datasets that makeup baseplatformdata - this is default an "All Time" metrics deployment for Existing Customers
+        if all_time_metrics_choice.lower() == 'y':
+            # Create the baseplatformdata dataset and subsequent four datasets that makeup baseplatformdata - this handles when the NEW customer is paying for the "All Time" metrics deployment
             for dataset in BASEPLATFORM_DATASETS:
                 dataset_id = dataset['title']
                 summary = dataset['summary']
                 visibility = dataset['visibility']
                 create_dataset(admin_token, org_id, dataset_id=dataset_id, visibility=visibility, summary=summary)
 
-            # Create ddw-metrics-{public_slug} dataset - this is default an "All Time" metrics deployment for Existing Customers
+            # Create ddw-metrics-{public_slug} dataset - this handles when the NEW customer is paying for the "All Time" metrics deployment
             create_dataset(admin_token, org_id, dataset_id=f"ddw-metrics-{public_slug}", visibility="PRIVATE", summary=DDW_METRICS_SUMMARY)
-
         else:
-            all_time_metrics_choice = input("Is the customer paying for the 'All-time' metrics upgrade (y/n): ")
-
-            if all_time_metrics_choice.lower() == 'y':
-                # Create the baseplatformdata dataset and subsequent four datasets that makeup baseplatformdata - this handles when the NEW customer is paying for the "All Time" metrics deployment
-                for dataset in BASEPLATFORM_DATASETS:
-                    dataset_id = dataset['title']
-                    summary = dataset['summary']
-                    visibility = dataset['visibility']
-                    create_dataset(admin_token, org_id, dataset_id=dataset_id, visibility=visibility, summary=summary)
-
-                # Create ddw-metrics-{public_slug} dataset - this handles when the NEW customer is paying for the "All Time" metrics deployment
-                create_dataset(admin_token, org_id, dataset_id=f"ddw-metrics-{public_slug}", visibility="PRIVATE", summary=DDW_METRICS_SUMMARY)
-            else:
-                # Create the baseplatformdata dataset and subsequent four datasets that makeup baseplatformdata - this handles the default LAST 90 DAYS metrics provided to NEW customers
-                for dataset in BASEPLATFORM_DATASETS:
-                    dataset_id = dataset['title'] + '-last-90-days'
-                    summary = dataset['summary']
-                    visibility = dataset['visibility']
-                    create_dataset(admin_token, org_id, dataset_id=dataset_id, visibility=visibility, summary=summary)
-
-                # Create ddw-metrics-{public_slug}-last-90-days dataset - this handles the default LAST 90 DAYS metrics provided to NEW customers
-                create_dataset(admin_token, org_id, dataset_id=f"ddw-metrics-{public_slug}-last-90-days", visibility="PRIVATE", summary=DDW_METRICS_SUMMARY)
-
-        return org_id, existing_customer
+            # Create the baseplatformdata dataset and subsequent four datasets that makeup baseplatformdata - this handles the default LAST 90 DAYS metrics provided to NEW customers
+            for dataset in BASEPLATFORM_DATASETS:
+                dataset_id = dataset['title'] + '-last-90-days'
+                summary = dataset['summary']
+                visibility = dataset['visibility']
+                create_dataset(admin_token, org_id, dataset_id=dataset_id, visibility=visibility, summary=summary)
 
-    else:
-        metrics_continue_choice = input("Do you want to continue without completing the metrics setup?\n"
-                                        "We will skip creating the necessary org and datasets for metric deployment (y/n): ")
+            # Create ddw-metrics-{public_slug}-last-90-days dataset - this handles the default LAST 90 DAYS metrics provided to NEW customers
+            create_dataset(admin_token, org_id, dataset_id=f"ddw-metrics-{public_slug}-last-90-days", visibility="PRIVATE", summary=DDW_METRICS_SUMMARY)
 
-        if metrics_continue_choice.lower() == 'n':
-            # Restart the metrics deployment process
-            deploy_metrics(api_url, admin_token, public_slug)
-        else:
-            print("Continuing without metrics setup...")
+    return org_id, existing_customer
```

### Comparing `support-toolbox-0.8.7/support_toolbox/utils/resource_type.py` & `support-toolbox-0.9.0/support_toolbox/utils/resource_type.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox/utils/saml_parser.py` & `support-toolbox-0.9.0/support_toolbox/utils/saml_parser.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.8.7/support_toolbox.egg-info/PKG-INFO` & `support-toolbox-0.9.0/support_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: support-toolbox
-Version: 0.8.7
+Version: 0.9.0
 Summary: A suite of CLI tools for the data.world support team
 Home-page: https://github.com/datadotworld/support-toolbox/tree/main
 Author: Jack Compton
 Author-email: jack.compton@data.world
 Requires-Dist: certifi==2023.7.22
 Requires-Dist: charset-normalizer==3.2.0
 Requires-Dist: defusedxml==0.7.1
```

### Comparing `support-toolbox-0.8.7/support_toolbox.egg-info/SOURCES.txt` & `support-toolbox-0.9.0/support_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

