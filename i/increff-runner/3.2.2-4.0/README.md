# Comparing `tmp/increff_runner-3.2.2-py3-none-any.whl.zip` & `tmp/increff_runner-4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 13321 bytes, number of entries: 16
+Zip file size: 12996 bytes, number of entries: 16
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-05 05:14 increff_runner/__init__.py
--rw-r--r--  2.0 unx     9762 b- defN 24-Apr-30 04:29 increff_runner/function.py
+-rw-r--r--  2.0 unx     9847 b- defN 24-May-08 08:15 increff_runner/function.py
 -rw-r--r--  2.0 unx     4143 b- defN 24-Feb-22 04:41 increff_runner/commons/algo_block_downloader.py
--rw-r--r--  2.0 unx     3105 b- defN 24-May-07 02:58 increff_runner/commons/callback_helper.py
+-rw-r--r--  2.0 unx     2757 b- defN 24-May-08 08:15 increff_runner/commons/callback_helper.py
 -rw-r--r--  2.0 unx      351 b- defN 24-Feb-15 07:21 increff_runner/commons/constants.py
--rw-r--r--  2.0 unx     3520 b- defN 24-May-03 10:42 increff_runner/commons/db_helper.py
+-rw-r--r--  2.0 unx     3559 b- defN 24-May-08 08:15 increff_runner/commons/db_helper.py
 -rw-r--r--  2.0 unx      905 b- defN 24-Feb-22 04:41 increff_runner/commons/db_service.py
--rw-r--r--  2.0 unx      349 b- defN 24-Apr-30 04:29 increff_runner/commons/event_helper.py
--rw-r--r--  2.0 unx     8405 b- defN 24-May-03 10:38 increff_runner/commons/graphdb_helper.py
--rw-r--r--  2.0 unx     4177 b- defN 24-May-02 06:39 increff_runner/commons/mse_helper.py
+-rw-r--r--  2.0 unx      481 b- defN 24-May-08 08:15 increff_runner/commons/event_helper.py
+-rw-r--r--  2.0 unx     8405 b- defN 24-May-07 09:07 increff_runner/commons/graphdb_helper.py
+-rw-r--r--  2.0 unx     3057 b- defN 24-May-08 08:15 increff_runner/commons/mse_helper.py
 -rw-r--r--  2.0 unx      687 b- defN 24-Feb-22 04:41 increff_runner/commons/setup.py
 -rw-r--r--  2.0 unx     2104 b- defN 24-Feb-22 04:41 increff_runner/commons/utils.py
--rw-r--r--  2.0 unx      612 b- defN 24-May-07 03:00 increff_runner-3.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-07 03:00 increff_runner-3.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-May-07 03:00 increff_runner-3.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1424 b- defN 24-May-07 03:00 increff_runner-3.2.2.dist-info/RECORD
-16 files, 39651 bytes uncompressed, 10927 bytes compressed:  72.4%
+-rw-r--r--  2.0 unx      610 b- defN 24-May-08 08:16 increff_runner-4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 08:16 increff_runner-4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-08 08:16 increff_runner-4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1416 b- defN 24-May-08 08:16 increff_runner-4.0.dist-info/RECORD
+16 files, 38429 bytes uncompressed, 10618 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: increff_runner/commons/setup.py
 Comment: 
 
 Filename: increff_runner/commons/utils.py
 Comment: 
 
-Filename: increff_runner-3.2.2.dist-info/METADATA
+Filename: increff_runner-4.0.dist-info/METADATA
 Comment: 
 
-Filename: increff_runner-3.2.2.dist-info/WHEEL
+Filename: increff_runner-4.0.dist-info/WHEEL
 Comment: 
 
-Filename: increff_runner-3.2.2.dist-info/top_level.txt
+Filename: increff_runner-4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: increff_runner-3.2.2.dist-info/RECORD
+Filename: increff_runner-4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## increff_runner/function.py

```diff
@@ -107,14 +107,15 @@
                 read_json_file(output_path + "/" + SCRIPT_OUTPUT_DATA, job["id"]),
                 read_json_file(output_path + "/" + SCRIPT_ERROR_DATA, job["id"]),
                 job,
             )
 
     else:
         add_info_logs(job["id"], f"Script run failed for the job {job['id']}")
+        add_error_logs(job["id"],f"Script failed with error {script_status.stderr}")
         change_job_to_failure_state(job, script_status.stderr)
         if "callBackUri" in job["data"] and job["data"]["callBackUri"] != "":
             send_failure_callback(
                 job["data"]["callBackUri"],
                 script_status.stderr,
                 read_json_file(output_path + "/" + SCRIPT_OUTPUT_DATA, job["id"]),
                 read_json_file(output_path + "/" + SCRIPT_ERROR_DATA, job["id"]),
@@ -180,15 +181,15 @@
     else:
         status = FAILED
 
     command = ""
     if "run_cmd" not in job["data"]["script_info"]:
         command = algo_block["run_cmd"]
     else:
-        command = job["data"]["script_info"]["run_cmd"]
+        command = job['data']['script_info']["run_cmd"]
         
     run_command = (
         str(command)
         .replace("${" + "root_dir" + "}", output_path)
         .replace("${" + "job_id" + "}", job_id)
     )
     add_info_logs(job_id, f"run command for the script is {run_command}")
```

## increff_runner/commons/callback_helper.py

```diff
@@ -45,32 +45,26 @@
     add_info_logs(job["id"], f" failure message -> {str(body)}")
     job["callback_status"] = 400
     update_job(job)
     response = requests.post(url, data=json.dumps(body))
 
 
 def send_failure_webhook(url, task_id, error, job):
-    # interim_task = get_interim_tasks(INTERIM_TASK_TABLE, task_id, job["data"]["algo_name"], job["data"]["level"])
     node = get_task_node(job["data"]["algo_name"],task_id,job["data"]["level"])
     add_error_logs(job["id"], "Hitting Failure WebHook Callback with error -> "+str(error))
     data = {"status": "FAILED", "taskId": task_id, "subtaskName":  node['parent_task'],"reason":str(error)}
 
-    # TODO @jaynit to move this config at the client level
     headers = {
         "Content-Type": "application/json",
         "authUsername":"caas-user@increff.com",
         "authPassword":"caasuser@123",
-        "authdomainname":"celio",
-        "project_name":"celio-ars",
+        "authdomainname": job["data"]["client"],
         "Conection":"keep-alive"
     }
     add_info_logs(job["id"], f" failure message -> {str(data)}")
     job["webhook_status"] = 400
     update_job(job)
-    
-    # TODO @jaynit ensure that they are not moved to Success again #cr1_unni
-    # TODO @jaynit kill the kube jobs also if it is running #cr1_unni
 
     change_status_of_task_node(job["data"]["algo_name"], job["data"]["task_id"], job["data"]["level"], FAILED)
     mark_dependant_as_failed(task_id,job["data"]["webHookUri"])
     response = requests.put(url, params=data,headers=headers)
     add_info_logs(job["id"], f"Failure Webhook Response -> {response.status_code}")
```

## increff_runner/commons/db_helper.py

```diff
@@ -1,10 +1,11 @@
 import pymongo
 import configparser
 from .event_helper import *
+from logging_increff.function import *
 from .graphdb_helper import *
 config = configparser.ConfigParser()
 config.read("config.ini")
 
 
 def change_id_to_mongo_id(data):
     data["_id"] = data["id"]
```

## increff_runner/commons/event_helper.py

```diff
@@ -1,15 +1,17 @@
 import json
 import requests
-
+from logging_increff.function import *
 
 def create_caas_job(url, data):
     data["subject"] = "mse-runner"
     response = requests.post(url, data=json.dumps(data))
     return response.json()
 
 def stop_caas_job(url,job_id):
     data = {
         'subject':'stop-mse-runner',
-        'job_id':job_id
+        'job_id':job_id,
+        'app_name':'mse'
     }
+    add_info_logs(job_id, f"Stopping the job with job_id {job_id}")
     response = requests.post(url, data=json.dumps(data))
```

## increff_runner/commons/mse_helper.py

```diff
@@ -24,72 +24,40 @@
     app,
     app_id,
     masterUri,
     script_info,
     webHookUri,
 ):
     return {
-        "client": client,
+        "client":client,
         "task_id": task_id,
         "algo_name": algo_name,
         "level": level,
         "block_identifier": block_identifier,
         "app_name": app,
         "app_id": app_id,
         "masterUri": masterUri,
         "script_info": script_info,
         "webHookUri": webHookUri,
     }
 
 
 def create_events_for_next_blocks(url, master_url, output, error_data, job):
-    # interim_task = get_interim_tasks(
-    #     INTERIM_TASK_TABLE,
-    #     job["data"]["task_id"],
-    #     job["data"]["algo_name"],
-    #     job["data"]["level"],
-    # )
-    # interim_task["status"] = "SUCCESS"
     change_status_of_task_node(job["data"]["algo_name"], job["data"]["task_id"], job["data"]["level"], "SUCCESS")
-    
-    # persist_value(INTERIM_TASK_TABLE, interim_task["id"], interim_task)
 
     node = get_task_node(job["data"]["algo_name"],job["data"]["task_id"],job["data"]["level"])
     if(str(node['last_block'])=="1"):
         status = check_last_block_status(job["data"]["task_id"], job["data"]["algo_name"])
         if status:
             add_info_logs(job["id"], "All levels for the block are completed")
             send_subtask_success_callback(
                 master_url, job["data"]["task_id"], node['parent_task']
             )
 
     next_nodes = get_next_task_nodes(job["data"]["algo_name"], job["data"]["task_id"], job["data"]["level"])
-    
-    # dag = copy.copy(job["data"]["dag"])
-    # algo_name = job["data"]["algo_name"]
-    # next_blocks = dag[algo_name]
-    # del dag[algo_name]
-    # if dag == {}:
-    #     return
-
-    # for block in next_blocks:
-    #     new_dag = create_next_dag(
-    #         copy.copy(block), copy.copy(next_blocks), copy.copy(dag)
-    #     )
-    #     add_info_logs(
-    #         job["id"],
-    #         f"Getting levels for {job['data']['task_id']} and {list(new_dag.keys())[0]}",
-    #     )
-    #     all_levels = get_levels_for_block(
-    #         INTERIM_TASK_TABLE, job["data"]["task_id"], list(new_dag.keys())[0]
-    #     )
-    #     all_levels = (
-    #         [job["data"]["level"]] if job["data"]["level"] in all_levels else all_levels
-    #     )
-    #     for level in all_levels:
     for next_node in next_nodes:
         change_edge_between_task_nodes(node,next_node)
         data = create_algo_block_runner_data(
             job["data"]["client"],
             job["data"]["task_id"],
             next_node['name'],
             next_node['level'],
@@ -102,23 +70,22 @@
         )
         add_info_logs(job["id"], f"Success message -> {str(data)}")
         job["webhook_status"] = "200"
         update_job(job)
         response = create_caas_job(url, data)
 
 
-def send_subtask_success_callback(url, task_id, algo_name):
+def send_subtask_success_callback(url, task_id, algo_name,level,client):
     if url == "":
         return
     data = {"status": "SUCCESS", "taskId": task_id, "subtaskName": algo_name,"reason":"Success"}
     headers = {
         "Content-Type": "application/json",
         "authUsername":"caas-user@increff.com",
         "authPassword":"caasuser@123",
-        "authdomainname":"celio",
-        "project_name":"celio-ars",
+        "authdomainname": client,
         "Conection":"keep-alive"
     }
     add_info_logs(task_id, f"Hitting Success Callback on {url} with data {data} ")
     response = requests.put(url, headers=headers,params=data)
     if response.status_code!=200:
         add_error_logs(task_id, f"Failed to hit the callback with status code {response.text}")
```

## Comparing `increff_runner-3.2.2.dist-info/METADATA` & `increff_runner-4.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: increff-runner
-Version: 3.2.2
+Version: 4.0
 Summary: Algo Runner For Increff CaaS
 Author: Jaynit Patel
 Author-email: jaynitpatel11062001@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pytz ==2023.3.post1
 Requires-Dist: requests ==2.31.0
 Requires-Dist: azure-functions ==1.12.0
```

## Comparing `increff_runner-3.2.2.dist-info/RECORD` & `increff_runner-4.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 increff_runner/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-increff_runner/function.py,sha256=Kk2mSezi3ypvYkjbSrMtxXoO5qwc29uYHAoTk_-W_Yo,9762
+increff_runner/function.py,sha256=blXpb4Rx0WY9B4_iZnqbyzhn0yTDeV_i9eOiNGv8KOU,9847
 increff_runner/commons/algo_block_downloader.py,sha256=JSZLYpIuWhybRD13sHPu_05X4KoeMApa5qELLkqA9R4,4143
-increff_runner/commons/callback_helper.py,sha256=G36Y_HjoRpZdGLgdUveL6H-nyyPuWsdLtmRZRg7rYa8,3105
+increff_runner/commons/callback_helper.py,sha256=eLlRYyjLqsq6_GvNn78FhwvQd6Qq0nybS1TSJWihfDU,2757
 increff_runner/commons/constants.py,sha256=dJRawPQQduTe1BqN6SrLYYpzI5bVqS6AbuYwj6Qa6is,351
-increff_runner/commons/db_helper.py,sha256=CmLWncHnvo0AS_cVlC5m6_FqwPLeqBvpEI40a7lyJKY,3520
+increff_runner/commons/db_helper.py,sha256=APr9mTd2RkEL1caxysuUgmCVQBH-izskLbVjpAf_Alo,3559
 increff_runner/commons/db_service.py,sha256=5PtU_AQCwm5FVmRXjJprysNoIy_vKt06vN1IlnxuH-c,905
-increff_runner/commons/event_helper.py,sha256=MN1XR6yielNYXLbLxi3uuiDyXZ-lmVKszL9DOL4swBY,349
+increff_runner/commons/event_helper.py,sha256=5aILmAJwk3TxiUYGKkmjh7rGwIJdu3ybTAcLbg8ApRI,481
 increff_runner/commons/graphdb_helper.py,sha256=c6cnD2He-xMer4dejiFKvAvM1qsbPlDoNqNKkz1mtZE,8405
-increff_runner/commons/mse_helper.py,sha256=m2JNRs72goahs3s3OSwwWvsoP_SWjRbOPfW-MEBP4lA,4177
+increff_runner/commons/mse_helper.py,sha256=qfPGwMs4_Nbs2nUaY-agA15qbMzJx0TIa9Ec3FOBdpo,3057
 increff_runner/commons/setup.py,sha256=iwg58X1DKaSP8hKlXLvH5OXSEW8N_UuRMDb2CocaAfY,687
 increff_runner/commons/utils.py,sha256=PUKWRMYzTTWK7pTK2S5DM0szru4zGmmVKfPpXhnmPUM,2104
-increff_runner-3.2.2.dist-info/METADATA,sha256=oL6QtcJFuELnGRsn4iAV5BRs1EL0bALCdwRbBw0gvDw,612
-increff_runner-3.2.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-increff_runner-3.2.2.dist-info/top_level.txt,sha256=pL8Rxzd3TVe5jhZdPB1tmORoBiwmdtiDgfNAvJtCl1s,15
-increff_runner-3.2.2.dist-info/RECORD,,
+increff_runner-4.0.dist-info/METADATA,sha256=fMBugBy7Nmj9Z2z9Ci_e5mqHCviOPooYNKB9NjwGU0g,610
+increff_runner-4.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+increff_runner-4.0.dist-info/top_level.txt,sha256=pL8Rxzd3TVe5jhZdPB1tmORoBiwmdtiDgfNAvJtCl1s,15
+increff_runner-4.0.dist-info/RECORD,,
```

