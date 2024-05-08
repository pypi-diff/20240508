# Comparing `tmp/open_fleet-0.0.3.tar.gz` & `tmp/open_fleet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_fleet-0.0.3.tar", last modified: Fri Apr 19 10:22:17 2024, max compression
+gzip compressed data, was "open_fleet-0.0.4.tar", last modified: Wed May  8 06:35:17 2024, max compression
```

## Comparing `open_fleet-0.0.3.tar` & `open_fleet-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-19 10:22:17.395015 open_fleet-0.0.3/
--rw-r--r--   0 huangshiyu   (501) staff       (20)    11357 2024-04-17 07:28:40.000000 open_fleet-0.0.3/LICENSE
--rw-r--r--   0 huangshiyu   (501) staff       (20)     2824 2024-04-19 10:22:17.394745 open_fleet-0.0.3/PKG-INFO
--rw-r--r--   0 huangshiyu   (501) staff       (20)     1502 2024-04-19 10:21:25.000000 open_fleet-0.0.3/README.md
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-19 10:22:17.390547 open_fleet-0.0.3/fleet/
--rw-r--r--   0 huangshiyu   (501) staff       (20)      457 2024-04-19 03:11:12.000000 open_fleet-0.0.3/fleet/__init__.py
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-19 10:22:17.390886 open_fleet-0.0.3/fleet/config/
--rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-17 08:43:11.000000 open_fleet-0.0.3/fleet/config/__init__.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)      741 2024-04-19 03:23:03.000000 open_fleet-0.0.3/fleet/config/config.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)     9966 2024-04-19 08:08:58.000000 open_fleet-0.0.3/fleet/manager.py
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-19 10:22:17.391350 open_fleet-0.0.3/fleet/manager_utils/
--rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-19 05:23:58.000000 open_fleet-0.0.3/fleet/manager_utils/__init__.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)     3506 2024-04-19 09:51:32.000000 open_fleet-0.0.3/fleet/manager_utils/assign_jobs.py
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-19 10:22:17.392783 open_fleet-0.0.3/fleet/utils/
--rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-17 08:43:03.000000 open_fleet-0.0.3/fleet/utils/__init__.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)      517 2024-04-19 06:51:31.000000 open_fleet-0.0.3/fleet/utils/file_utils.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)      573 2024-04-16 07:33:32.000000 open_fleet-0.0.3/fleet/utils/host_utils.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)     2186 2024-04-19 03:24:42.000000 open_fleet-0.0.3/fleet/utils/time_tracker.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)     6733 2024-04-19 06:50:33.000000 open_fleet-0.0.3/fleet/worker.py
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-19 10:22:17.394041 open_fleet-0.0.3/open_fleet.egg-info/
--rw-r--r--   0 huangshiyu   (501) staff       (20)     2824 2024-04-19 10:22:17.000000 open_fleet-0.0.3/open_fleet.egg-info/PKG-INFO
--rw-r--r--   0 huangshiyu   (501) staff       (20)      465 2024-04-19 10:22:17.000000 open_fleet-0.0.3/open_fleet.egg-info/SOURCES.txt
--rw-r--r--   0 huangshiyu   (501) staff       (20)        1 2024-04-19 10:22:17.000000 open_fleet-0.0.3/open_fleet.egg-info/dependency_links.txt
--rw-r--r--   0 huangshiyu   (501) staff       (20)       94 2024-04-19 10:22:17.000000 open_fleet-0.0.3/open_fleet.egg-info/requires.txt
--rw-r--r--   0 huangshiyu   (501) staff       (20)        6 2024-04-19 10:22:17.000000 open_fleet-0.0.3/open_fleet.egg-info/top_level.txt
--rw-r--r--   0 huangshiyu   (501) staff       (20)       38 2024-04-19 10:22:17.395069 open_fleet-0.0.3/setup.cfg
--rw-r--r--   0 huangshiyu   (501) staff       (20)     2455 2024-04-19 10:21:57.000000 open_fleet-0.0.3/setup.py
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-05-08 06:35:17.050205 open_fleet-0.0.4/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)    11357 2024-04-17 07:28:40.000000 open_fleet-0.0.4/LICENSE
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     2876 2024-05-08 06:35:17.049991 open_fleet-0.0.4/PKG-INFO
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     1554 2024-05-08 06:33:31.000000 open_fleet-0.0.4/README.md
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-05-08 06:35:17.046480 open_fleet-0.0.4/fleet/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      456 2024-05-08 06:35:03.000000 open_fleet-0.0.4/fleet/__init__.py
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-05-08 06:35:17.047019 open_fleet-0.0.4/fleet/config/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-17 08:43:11.000000 open_fleet-0.0.4/fleet/config/__init__.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     1075 2024-05-08 06:02:04.000000 open_fleet-0.0.4/fleet/config/config.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)    10645 2024-04-22 06:45:29.000000 open_fleet-0.0.4/fleet/manager.py
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-05-08 06:35:17.047340 open_fleet-0.0.4/fleet/manager_utils/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-19 05:23:58.000000 open_fleet-0.0.4/fleet/manager_utils/__init__.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     3549 2024-04-19 13:04:01.000000 open_fleet-0.0.4/fleet/manager_utils/assign_jobs.py
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-05-08 06:35:17.048340 open_fleet-0.0.4/fleet/utils/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-17 08:43:03.000000 open_fleet-0.0.4/fleet/utils/__init__.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      517 2024-04-19 06:51:31.000000 open_fleet-0.0.4/fleet/utils/file_utils.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      573 2024-04-16 07:33:32.000000 open_fleet-0.0.4/fleet/utils/host_utils.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     2186 2024-04-19 03:24:42.000000 open_fleet-0.0.4/fleet/utils/time_tracker.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     8844 2024-05-08 06:30:15.000000 open_fleet-0.0.4/fleet/worker.py
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-05-08 06:35:17.049365 open_fleet-0.0.4/open_fleet.egg-info/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     2876 2024-05-08 06:35:17.000000 open_fleet-0.0.4/open_fleet.egg-info/PKG-INFO
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      465 2024-05-08 06:35:17.000000 open_fleet-0.0.4/open_fleet.egg-info/SOURCES.txt
+-rw-r--r--   0 huangshiyu   (501) staff       (20)        1 2024-05-08 06:35:17.000000 open_fleet-0.0.4/open_fleet.egg-info/dependency_links.txt
+-rw-r--r--   0 huangshiyu   (501) staff       (20)       94 2024-05-08 06:35:17.000000 open_fleet-0.0.4/open_fleet.egg-info/requires.txt
+-rw-r--r--   0 huangshiyu   (501) staff       (20)        6 2024-05-08 06:35:17.000000 open_fleet-0.0.4/open_fleet.egg-info/top_level.txt
+-rw-r--r--   0 huangshiyu   (501) staff       (20)       38 2024-05-08 06:35:17.050256 open_fleet-0.0.4/setup.cfg
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     2455 2024-04-19 10:21:57.000000 open_fleet-0.0.4/setup.py
```

### Comparing `open_fleet-0.0.3/LICENSE` & `open_fleet-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `open_fleet-0.0.3/PKG-INFO` & `open_fleet-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-fleet
-Version: 0.0.3
+Version: 0.0.4
 Summary: distributed task distribution framework
 Author: Shiyu Huang
 Author-email: huangsy1314@163.com
 Project-URL: Documentation, https://github.com/huangshiyu13/Fleet
 Keywords: distributed framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -39,14 +39,15 @@
 
 ## Features
 - Distributed task distribution based on a shared file system
 - Supports dynamic scaling
 - Supports worker node heartbeat
 - Supports manager node restart
 - Supports set timeout for each task
+- Supports set max_job and max_work_time for worker
 - Pure Python implementation
 
 ## Install
 
 ```bash
 pip install open-fleet
 ```
```

### Comparing `open_fleet-0.0.3/README.md` & `open_fleet-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 ## Features
 - Distributed task distribution based on a shared file system
 - Supports dynamic scaling
 - Supports worker node heartbeat
 - Supports manager node restart
 - Supports set timeout for each task
+- Supports set max_job and max_work_time for worker
 - Pure Python implementation
 
 ## Install
 
 ```bash
 pip install open-fleet
 ```
```

### Comparing `open_fleet-0.0.3/fleet/manager.py` & `open_fleet-0.0.4/fleet/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List, Any, Dict
 import time
 import json
 from multiprocessing import Process
+from datetime import datetime
 
 from pathlib import Path
 from rich.console import Console
 from rich.progress import Progress, BarColumn, TextColumn
 
 from fleet.utils.file_utils import safe_load_json
 from fleet.utils.time_tracker import TimeTracker
@@ -127,30 +128,29 @@
 
                 if status_info and status_info['status'] == 'assigned':
                     status_info['status'] = 'crashed'
                     Path(task_status_path).write_text(json.dumps(status_info))
                     node_info['status'] = 'dead'
                     node_file.write_text(json.dumps(node_info))
 
-
     def log_status(self):
         current_time = time.time()
         if self.previous_log_time is None or current_time - self.previous_log_time > 1 or self.finished_num == self.total_jobs:
             self.previous_log_time = current_time
         else:
             return
 
         if self.finished_num == 0:
             success_rate = 0
         else:
             success_rate = self.success_num / self.finished_num * 100
         time_summary = self.time_tracker.summary
 
-
-        self.progress.update(self.task_id, description=f"Success Rate: {success_rate:.2f}% Finished/Working: {self.finished_num}/{self.working_num}/{self.total_jobs} Nodes(Good/Dead): {len(self.available_nodes)}/{len(self.dead_nodes)} {time_summary}")
+        self.progress.update(self.task_id,
+                             description=f"Success Rate: {success_rate:.2f}% Finished/Working: {self.finished_num}/{self.working_num}/{self.total_jobs} Nodes(Good/Dead): {len(self.available_nodes)}/{len(self.dead_nodes)} {time_summary}")
 
     def check_task_status_and_assign(self):
         self.monitor_heartbeats()
         self.check_working_tasks()
         self.log_status()
 
     def check_working_tasks(self):
@@ -189,15 +189,14 @@
                 self.finished_num += 1
                 # self.new_finished_num += 1
                 # self.console.log(f"{self.finished_num}/{self.new_finished_num}")
 
                 self.time_tracker.update()
                 self.progress.update(self.task_id, advance=1)
 
-
     def loop_assignment(self):
         loop_assignment(self.available_dir, self.nodes_dir, self.working_dir, self.unassigned_task_status, self.console)
 
     def start_job_assignment(self):
         self.job_assign_process = Process(target=self.loop_assignment)
         self.job_assign_process.start()
 
@@ -218,35 +217,49 @@
             # self.pbar = tqdm(total=len(self.job_list), desc="Processing Jobs")
             self.initialize_tasks()
 
             self.start_job_assignment()
 
             try:
                 while True:
-                    if self.finished_num == self.total_jobs:
+                    if self.finished_num == self.total_jobs or self.working_num + self.finished_num == self.total_jobs:
                         if not self.finished_file.exists():
                             self.finished_file.touch()
+
+                    if self.finished_num == self.total_jobs:
                         break
 
                     self.check_task_status_and_assign()
+
             finally:
                 self.stop_job_assignment()
 
     def monitor_heartbeats(self, heartbeat_timeout: int = 120):
         self.available_nodes = {}
         new_dead_nodes = {}
 
         current_time = int(time.time())
         for node_file in self.heart_dir.iterdir():
             if node_file.stem in self.dead_nodes:
                 continue
 
             node_info = safe_load_json(node_file)
+
             if node_info and node_info['status'] == "available" and current_time - node_info.get("last_heartbeat",
                                                                                                  0) <= heartbeat_timeout:
                 self.available_nodes[node_file.stem] = node_info
+
             else:
+                if node_info is None:
+                    dead_reason = f"can not load node info from {str(node_file)}"
+                else:
+                    if node_info['status'] == 'dead':
+                        dead_reason = f"worker sends dead"
+                    else:
+                        dead_reason = f"no heartbeat, last heartbeat: {datetime.fromtimestamp(node_info.get('last_heartbeat', 0)).strftime('%Y-%m-%d %H:%M:%S')}"
                 node_info['status'] = 'dead'
+                node_info['dead_reason'] = dead_reason
+
                 node_file.write_text(json.dumps(node_info))
                 self.dead_nodes[node_file.stem] = node_info
                 new_dead_nodes[node_file.stem] = node_info
         self.process_dead_nodes(new_dead_nodes)
```

### Comparing `open_fleet-0.0.3/fleet/manager_utils/assign_jobs.py` & `open_fleet-0.0.4/fleet/manager_utils/assign_jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 def loop_assignment(available_dir, nodes_dir, working_dir, unassigned_task_status, console):
     while len(unassigned_task_status) > 0:
         unassigned_task_status, working_task_status = process_assignment(available_dir, nodes_dir, working_dir,
                                                                          unassigned_task_status, console)
         if len(working_task_status) == 0:
             time.sleep(0.1)
+    console.log("All tasks are assigned.")
 
 
 def process_assignment(available_dir, nodes_dir, working_dir: Path, unassigned_task_status, console):
     working_task_status = {}
     if len(unassigned_task_status) == 0:
         return unassigned_task_status, working_task_status
```

### Comparing `open_fleet-0.0.3/fleet/utils/file_utils.py` & `open_fleet-0.0.4/fleet/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `open_fleet-0.0.3/fleet/utils/host_utils.py` & `open_fleet-0.0.4/fleet/utils/host_utils.py`

 * *Files identical despite different names*

### Comparing `open_fleet-0.0.3/fleet/utils/time_tracker.py` & `open_fleet-0.0.4/fleet/utils/time_tracker.py`

 * *Files identical despite different names*

### Comparing `open_fleet-0.0.3/fleet/worker.py` & `open_fleet-0.0.4/fleet/worker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,36 @@
-from typing import Callable, Dict
+from typing import Callable, Dict, List
 import time
 import uuid
 import json
 from multiprocessing import Process, Queue
 import traceback
 
 from pathlib import Path
 
 from fleet.utils.file_utils import safe_load_json
 
+
 def run_job(job_func, job_input, info, output_queue):
     try:
         result = job_func(job_input, info)
         output_queue.put(result)
     except Exception as e:
         error_message = traceback.format_exc()
+        print(error_message)
         output_queue.put({"error": error_message, "status": "crashed"})
 
 
 class Worker:
     def __init__(self, args, job_func: Callable, info: Dict = {}):
         self.base_dir = Path(args.base_dir)
         self.timeout = args.timeout
+        self.wait_manager = args.wait_manager
+        self.max_job = args.max_job
+        self.max_work_time = args.max_work_time
         unique_id = str(uuid.uuid4())
         self.node_id = f"{args.node_id}_{unique_id}" if args.node_id else unique_id
         self.nodes_dir = self.base_dir / 'nodes'
         self.status_dir = self.base_dir / 'status'
         self.heart_dir = self.base_dir / 'heart'
         self.finished_file = self.base_dir / 'finished'
         self.available_dir = self.base_dir / 'available'
@@ -38,14 +43,40 @@
         self.info = info
 
         # self.unassigned_task_status = {}
         self.not_find_job_num = 0
 
         self.heartbeat_process = None  # 添加一个属性来保存心跳进程的引用
 
+        if self.wait_manager:
+            wait_time = 0
+            missing_dirs = self.check_dirs()
+            while len(missing_dirs) > 0:
+                if wait_time % 30 == 0:
+                    print(f"Waiting for manager to create dirs...")
+                    for missing_dir in missing_dirs:
+                        print(f"Missing dir: {missing_dir}")
+                time.sleep(1)
+                wait_time += 1
+                missing_dirs = self.check_dirs()
+
+        else:
+            missing_dirs = self.check_dirs()
+            assert len(missing_dirs) == 0, f"Missing dirs: {missing_dirs}"
+
+        self.finished_job_num = 0
+        self.worker_start_time = time.time()
+
+    def check_dirs(self) -> List[str]:
+        missing_dirs = []
+        for dir in [self.nodes_dir, self.status_dir, self.heart_dir, self.available_dir]:
+            if not dir.exists():
+                missing_dirs.append(str(dir))
+        return missing_dirs
+
     def create_available_file(self):
         if not self.available_file.exists():
             self.available_file.touch()
 
     def heartbeat_daemon(self):
         """这个函数将作为独立的进程运行，负责发送心跳信号。"""
         try:
@@ -130,28 +161,31 @@
                     job_process.terminate()
                     job_process.join()
                     result = {"error": "job timeout", "status": "crashed"}
                 else:
                     result = output_queue.get()
 
             print(f"Task {job_input} Done!")
+            self.finished_job_num += 1
             if 'error' in result:
                 status_info['error'] = result['error']
 
             # 更新任务状态为完成
             status_info['status'] = result['status']
 
             task_status_file.write_text(json.dumps(status_info))
 
             # 标记节点为空闲
             node_info = {
                 "status": "idle"
             }
             self.node_status_path.write_text(json.dumps(node_info))
-            self.create_available_file()
+            worker_status = self.check_worker_status()
+            if worker_status == "running":
+                self.create_available_file()
             return find_job
         return find_job
 
     def check_and_process_tasks(self):
         find_job = self.process_job()
 
         if not find_job:
@@ -163,23 +197,41 @@
             else:
                 time.sleep(0.5)
 
             self.not_find_job_num += 1
         else:
             self.not_find_job_num = 0
 
+    def check_worker_status(self)->str:
+        if self.max_job is not None and self.finished_job_num >= self.max_job:
+            return "max_job_reached"
+        if self.max_work_time is not None and time.time() - self.worker_start_time > self.max_work_time:
+            return "max_work_time_reached"
+        if self.finished_file.exists():
+            return "finished_file_exists"
+        if not self.check_heart():
+            return "heart_dead"
+        return "running"
+
     def run(self):
         self.register_node()
 
         try:
             while True:
                 self.check_and_process_tasks()
-                if self.finished_file.exists():
+                worker_status = self.check_worker_status()
+                if worker_status == "finished_file_exists":
+                    node_info = safe_load_json(self.node_status_path)
+                    if node_info and node_info['status'] == 'busy':
+                        continue
+
+                    print("Finished file exists, exit!")
                     break
-                if not self.check_heart():
+                if worker_status != "running":
+                    print(f"Worker finish reason: {worker_status}")
                     break
 
         except Exception as e:
             # traceback.print_exc()  # 打印异常信息和堆栈跟踪
             error_message = traceback.format_exc()
             print(error_message)
         finally:
```

### Comparing `open_fleet-0.0.3/open_fleet.egg-info/PKG-INFO` & `open_fleet-0.0.4/open_fleet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-fleet
-Version: 0.0.3
+Version: 0.0.4
 Summary: distributed task distribution framework
 Author: Shiyu Huang
 Author-email: huangsy1314@163.com
 Project-URL: Documentation, https://github.com/huangshiyu13/Fleet
 Keywords: distributed framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -39,14 +39,15 @@
 
 ## Features
 - Distributed task distribution based on a shared file system
 - Supports dynamic scaling
 - Supports worker node heartbeat
 - Supports manager node restart
 - Supports set timeout for each task
+- Supports set max_job and max_work_time for worker
 - Pure Python implementation
 
 ## Install
 
 ```bash
 pip install open-fleet
 ```
```

### Comparing `open_fleet-0.0.3/setup.py` & `open_fleet-0.0.4/setup.py`

 * *Files identical despite different names*

