# Comparing `tmp/simple_kfp_task-0.0.8.tar.gz` & `tmp/simple_kfp_task-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_kfp_task-0.0.8.tar", last modified: Tue May  7 16:34:34 2024, max compression
+gzip compressed data, was "simple_kfp_task-0.0.9.tar", last modified: Wed May  8 12:41:47 2024, max compression
```

## Comparing `simple_kfp_task-0.0.8.tar` & `simple_kfp_task-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:34:34.042199 simple_kfp_task-0.0.8/
--rw-r--r--   0 sebastian   (501) staff       (20)     1077 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.8/LICENSE
--rw-r--r--   0 sebastian   (501) staff       (20)      852 2024-05-07 16:34:34.041426 simple_kfp_task-0.0.8/PKG-INFO
--rw-r--r--   0 sebastian   (501) staff       (20)      788 2024-05-07 16:34:14.000000 simple_kfp_task-0.0.8/pyproject.toml
--rw-r--r--   0 sebastian   (501) staff       (20)      161 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.8/requirements.txt
--rw-r--r--   0 sebastian   (501) staff       (20)       38 2024-05-07 16:34:34.042361 simple_kfp_task-0.0.8/setup.cfg
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:34:34.036358 simple_kfp_task-0.0.8/simple_kfp_task/
--rw-r--r--   0 sebastian   (501) staff       (20)       59 2024-05-07 09:31:11.000000 simple_kfp_task-0.0.8/simple_kfp_task/__init__.py
--rwxr-xr-x   0 sebastian   (501) staff       (20)     2442 2024-05-07 13:30:40.000000 simple_kfp_task-0.0.8/simple_kfp_task/cli.py
--rw-r--r--   0 sebastian   (501) staff       (20)    10826 2024-05-07 07:04:14.000000 simple_kfp_task-0.0.8/simple_kfp_task/deploykf.py
--rw-r--r--   0 sebastian   (501) staff       (20)     5166 2024-05-07 16:29:26.000000 simple_kfp_task-0.0.8/simple_kfp_task/git_helper.py
--rw-r--r--   0 sebastian   (501) staff       (20)     8727 2024-05-07 16:07:33.000000 simple_kfp_task-0.0.8/simple_kfp_task/pipeline.py
--rw-r--r--   0 sebastian   (501) staff       (20)     7583 2024-05-07 16:33:40.000000 simple_kfp_task-0.0.8/simple_kfp_task/task.py
--rw-r--r--   0 sebastian   (501) staff       (20)     1410 2024-05-07 16:24:19.000000 simple_kfp_task-0.0.8/simple_kfp_task/utils.py
-drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2024-05-07 16:34:34.040394 simple_kfp_task-0.0.8/simple_kfp_task.egg-info/
--rw-r--r--   0 sebastian   (501) staff       (20)      852 2024-05-07 16:34:34.000000 simple_kfp_task-0.0.8/simple_kfp_task.egg-info/PKG-INFO
--rw-r--r--   0 sebastian   (501) staff       (20)      461 2024-05-07 16:34:34.000000 simple_kfp_task-0.0.8/simple_kfp_task.egg-info/SOURCES.txt
--rw-r--r--   0 sebastian   (501) staff       (20)        1 2024-05-07 16:34:34.000000 simple_kfp_task-0.0.8/simple_kfp_task.egg-info/dependency_links.txt
--rw-r--r--   0 sebastian   (501) staff       (20)       61 2024-05-07 16:34:34.000000 simple_kfp_task-0.0.8/simple_kfp_task.egg-info/entry_points.txt
--rw-r--r--   0 sebastian   (501) staff       (20)      162 2024-05-07 16:34:34.000000 simple_kfp_task-0.0.8/simple_kfp_task.egg-info/requires.txt
--rw-r--r--   0 sebastian   (501) staff       (20)       16 2024-05-07 16:34:34.000000 simple_kfp_task-0.0.8/simple_kfp_task.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:41:47.461560 simple_kfp_task-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-08 12:41:30.000000 simple_kfp_task-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-08 12:41:47.457560 simple_kfp_task-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-08 12:41:30.000000 simple_kfp_task-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-08 12:41:30.000000 simple_kfp_task-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:41:47.461560 simple_kfp_task-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:41:47.457560 simple_kfp_task-0.0.9/simple_kfp_task/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 12:41:30.000000 simple_kfp_task-0.0.9/simple_kfp_task/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2666 2024-05-08 12:41:30.000000 simple_kfp_task-0.0.9/simple_kfp_task/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-08 12:41:30.000000 simple_kfp_task-0.0.9/simple_kfp_task/deploykf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-08 12:41:30.000000 simple_kfp_task-0.0.9/simple_kfp_task/git_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-05-08 12:41:30.000000 simple_kfp_task-0.0.9/simple_kfp_task/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-05-08 12:41:30.000000 simple_kfp_task-0.0.9/simple_kfp_task/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-08 12:41:30.000000 simple_kfp_task-0.0.9/simple_kfp_task/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:41:47.457560 simple_kfp_task-0.0.9/simple_kfp_task.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-08 12:41:47.000000 simple_kfp_task-0.0.9/simple_kfp_task.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-08 12:41:47.000000 simple_kfp_task-0.0.9/simple_kfp_task.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:41:47.000000 simple_kfp_task-0.0.9/simple_kfp_task.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-08 12:41:47.000000 simple_kfp_task-0.0.9/simple_kfp_task.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-08 12:41:47.000000 simple_kfp_task-0.0.9/simple_kfp_task.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 12:41:47.000000 simple_kfp_task-0.0.9/simple_kfp_task.egg-info/top_level.txt
```

### Comparing `simple_kfp_task-0.0.8/LICENSE` & `simple_kfp_task-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_kfp_task-0.0.8/PKG-INFO` & `simple_kfp_task-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-kfp-task
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generate a simple Kubeflow Pipeline task
 Author-email: Sebastian Alberternst <sebastian.alberternst@dfki.de>
 Project-URL: Homepage, https://github.com/salberternst/simple-kfp-task
 Project-URL: Issues, https://github.com/salberternst/simple-kfp-task/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_kfp_task-0.0.8/pyproject.toml` & `simple_kfp_task-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=61.0", "setuptools-git-versioning>=2.0,<3"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools-git-versioning]
+enabled = true
+
 [project]
 name = "simple-kfp-task"
-version = "0.0.8"
+dynamic = ["version", "dependencies"]
 authors = [
   { name="Sebastian Alberternst", email="sebastian.alberternst@dfki.de" },
 ]
 description = "Generate a simple Kubeflow Pipeline task"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.scripts]
 simple-kfp-task = "simple_kfp_task.cli:main"
 
 [project.urls]
 Homepage = "https://github.com/salberternst/simple-kfp-task"
-Issues = "https://github.com/salberternst/simple-kfp-task/issues"
+Issues = "https://github.com/salberternst/simple-kfp-task/issues"
```

### Comparing `simple_kfp_task-0.0.8/simple_kfp_task/cli.py` & `simple_kfp_task-0.0.9/simple_kfp_task/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     parser.add_argument("--memory-request", default="1Gi")
     parser.add_argument("--gpu-vendor", default="nvidia.com/gpu")
     parser.add_argument("--container-image", default="python:3.12.3-slim")
     parser.add_argument("--volume-name", default=None)
     parser.add_argument("--disable-git-detection", action="store_true", default=False)
     parser.add_argument("--dry-run", action="store_true", default=False)
     parser.add_argument("--wait-for-run", action="store_true", default=False)
+    parser.add_argument("--kfp-host", default="https://10-101-20-33.sslip.io")
+    parser.add_argument("--verify-ssl", action="store_true", default=False)
 
     args, command_args = parser.parse_known_args()
 
     task = Task.init(
         run_name=args.run_name,
         experiment_name=args.experiment_name,
         namespace=args.namespace,
@@ -51,15 +53,17 @@
         gpu_limit=args.gpu_limit,
         gpu_vendor=args.gpu_vendor,
         cpu_limit=args.cpu_limit,
         cpu_request=args.cpu_request,
         memory_limit=args.memory_limit,
         memory_request=args.memory_request,
         volume_name=args.volume_name,
-        container_image=args.container_image
+        container_image=args.container_image,
+        kfp_host=args.kfp_host,
+        verify_ssl=args.verify_ssl,
     )
 
     if not args.dry_run:
         run = task.run()
         if args.wait_for_run:
             run_response = run.wait_for_run_completion()
             run = run_response.run.id
```

### Comparing `simple_kfp_task-0.0.8/simple_kfp_task/deploykf.py` & `simple_kfp_task-0.0.9/simple_kfp_task/deploykf.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,18 +275,18 @@
 
     _patched_client = kfp.Client
     _patched_client._load_config = _patched_load_config
 
     return _patched_client
 
 
-def create_kfp_client(host="https://10-101-20-33.sslip.io", namespace='kubeflow'):
+def create_kfp_client(host="https://10-101-20-33.sslip.io", namespace='kubeflow', verify_ssl=False):
     credentials = DeployKFCredentialsOutOfBand(
         issuer_url=f"{host}/dex",
-        skip_tls_verify=True,
+        skip_tls_verify=not verify_ssl,
     )
 
     return patched_kfp_client(verify_ssl=not credentials.skip_tls_verify)(
         host=f"{host}/pipeline",
         credentials=credentials,
         namespace=namespace
     )
```

### Comparing `simple_kfp_task-0.0.8/simple_kfp_task/git_helper.py` & `simple_kfp_task-0.0.9/simple_kfp_task/git_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import os
 import sys
-from simple_kfp_task.utils import is_remote_execution
-
-if not is_remote_execution():
-    from git import Repo
+from git import Repo
 
 class GitHelper:
     """
     A helper class for interacting with Git repositories.
     """
 
     def __init__(self):
```

### Comparing `simple_kfp_task-0.0.8/simple_kfp_task/pipeline.py` & `simple_kfp_task-0.0.9/simple_kfp_task/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,72 +27,77 @@
         sidecars=[
             kubernetes_client.V1Container(
                 name='git-clone',
                 image='alpine/git:2.43.0',
                 command=['sh', '-c'],
                 args=[
                     f"""
-git clone --single-branch --branch {branch} {remote_url} /app --depth=1 > /ipc/git-clone.log 2>&1
+touch /ipc/log && \
+git clone --progress --single-branch --branch {branch} {remote_url} /app --depth=1 > /ipc/log 2>&1 && \
+  cd /app && \
+  git fetch --depth=1 origin {commit} > /ipc/log 2>&1 && \
+  git checkout {commit} > /ipc/log 2>&1
+
 git_clone_exit_code=$?
 echo $git_clone_exit_code > /ipc/git-clone
 if [ $git_clone_exit_code -ne 0 ]; then
     exit 1
 fi
 
 if [ -n "{git_diff}" ]; then
     cd /app && \
-    git fetch origin {commit} && \
-    echo '{git_diff}' | base64 -d | gunzip | git apply --verbose - > /ipc/git-apply.log 2>&1
+    echo '{git_diff}' | base64 -d | gunzip | git apply --verbose - > /ipc/log 2>&1
     git_apply_exit_code=$?
     echo $git_apply_exit_code > /ipc/git-apply
     if [ $git_apply_exit_code -ne 0 ]; then
         exit 1
-    fi    
+    fi
 fi
                     """
                 ],
                 volume_mounts=[
-                    kubernetes_client.V1VolumeMount(name='app-volume', mount_path='/app'),
-                    kubernetes_client.V1VolumeMount(name='ipc-volume', mount_path='/ipc')
-                ], 
+                    kubernetes_client.V1VolumeMount(
+                        name='app-volume', mount_path='/app'),
+                    kubernetes_client.V1VolumeMount(
+                        name='ipc-volume', mount_path='/ipc')
+                ],
             ),
         ],
         command=['sh', '-c'],
         arguments=[
             f"""
-#            
+#
 # Wait for the git clone to finish
 #
-            
-until [ -f /ipc/git-clone.log ]; do sleep 1; done
-tail -f /ipc/git-clone.log &
+
+touch /ipc/log
+tail -F /ipc/log &
 TAIL_PID=$!
 
-until [ -f /ipc/git-clone ]; 
-    do sleep 1; 
+until [ -f /ipc/git-clone ];
+    do sleep 1;
 done
 
-kill $TAIL_PID
-
 if [ $(cat /ipc/git-clone) -ne 0 ]; then
     exit 1
 fi
 
 #
 # Wait for the git apply to finish
 #
 
 if [ -n "{git_diff}" ]; then
     until [ -f /ipc/git-apply ]; do sleep 1; done
-    while read -r line; do echo $line; done < /ipc/git-apply.log
     if [ $(cat /ipc/git-apply) -ne 0 ]; then
         exit 1
     fi
 fi
 
+kill $TAIL_PID
+
 cd {cwd} && \
 if [ -n "{requirements}" ]; then pip install -r {requirements}; fi && \
 if [ -n "{packages}" ]; then echo "{packages}" | xargs pip install; fi && \
 python {command} {args}
             """
         ],
         container_kwargs={'working_dir': '/app'},
@@ -114,15 +119,16 @@
             name='ipc-volume', mount_path='/ipc')
     ).add_env_variable(kubernetes_client.V1EnvVar(
         name="MLFLOW_TRACKING_URI", value="http://mlflow-server:5000"
     )).add_env_variable(kubernetes_client.V1EnvVar(
         name="MLFLOW_REGISTRY_URI", value="http://mlflow-server:5000"
     )).add_env_variable(kubernetes_client.V1EnvVar(
         name='INSIDE_KFP_FUNC_CONTAINER', value='true'))
-        
+
+
 @dsl.pipeline(
     name='Simple Task Pipeline',
     description='A simple pipeline that clones a Git repository, creates a virtual environment, runs pip, and executes a script.'
 )
 def simple_task_pipeline(
     remote_url: str = 'https://github.com/your/repo.git',
     branch: str = 'main',
@@ -201,15 +207,16 @@
             requirements=requirements,
             packages=packages,
             git_diff=git_diff,
             commit=commit
         ).add_volume(
             kubernetes_client.V1Volume(
                 name="data-volume",
-                persistent_volume_claim=kubernetes_client.V1PersistentVolumeClaimVolumeSource(claim_name=volume_name)
+                persistent_volume_claim=kubernetes_client.V1PersistentVolumeClaimVolumeSource(
+                    claim_name=volume_name)
             )
         ).add_volume_mount(
             kubernetes_client.V1VolumeMount(
                 name="data-volume", mount_path='/volume'
             )
         )
```

### Comparing `simple_kfp_task-0.0.8/simple_kfp_task/task.py` & `simple_kfp_task-0.0.9/simple_kfp_task/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 from simple_kfp_task.deploykf import create_kfp_client
 from typing import Callable
 from simple_kfp_task.pipeline import simple_task_pipeline
-from simple_kfp_task.utils import encode_string_to_base64, get_caller_filename, is_remote_execution
-if not is_remote_execution():
-    from simple_kfp_task.git_helper import GitHelper
+from simple_kfp_task.utils import encode_string_to_base64, get_caller_filename
+from simple_kfp_task.git_helper import GitHelper
 
 GIT_DIFF_MAX_LENGTH = 10000
-PIP_PACKAGE_NAME = "simple-kfp-task"
+PIP_PACKAGE_NAME = "simple-kfp-task-stub"
 
 
 class Task:
     """
     Represents a task to be executed in a Kubeflow Pipelines (KFP) environment.
 
     Args:
@@ -42,14 +41,16 @@
         ValueError: If the branch is not available on the remote repository.
         ValueError: If the Git diff is too long. Please commit and push your changes first.
 
     """
 
     def __init__(
         self,
+        kfp_host = "https://10-101-20-33.sslip.io",
+        verify_ssl = False,
         namespace: str = None,
         run_name: str = None,
         experiment_name: str = None,
         func: Callable = None,
         command=None,
         args=None,
         cwd=None,
@@ -85,17 +86,16 @@
         self.gpu_limit = gpu_limit
         self.gpu_vendor = gpu_vendor
         self.cpu_limit = cpu_limit
         self.cpu_request = cpu_request
         self.memory_limit = memory_limit
         self.memory_request = memory_request
         self.volume_name = volume_name
-
-        if is_remote_execution():
-            return
+        self.kfp_host = kfp_host
+        self.verify_ssl = verify_ssl
 
         git_helper = GitHelper()
 
         if self.func:
             self.command = os.path.relpath(get_caller_filename(), os.getcwd())
             if self.packages is None:
                 self.packages = [PIP_PACKAGE_NAME]
@@ -148,21 +148,15 @@
         """
         Run the task using the provided configuration.
 
         Returns:
             kfp_client.create_run_from_pipeline_func: The KFP run created for the task.
 
         """
-        if is_remote_execution():
-            if self.func:
-                return self.func()
-            else:
-                raise ValueError("Function is required for remote execution.")
-
-        kfp_client = create_kfp_client(namespace=self.namespace)
+        kfp_client = create_kfp_client(namespace=self.namespace, host=self.kfp_host, verify_ssl=self.verify_ssl)
         return kfp_client.create_run_from_pipeline_func(
             pipeline_func=simple_task_pipeline,
             experiment_name=self.experiment_name,
             run_name=self.run_name,
             arguments={
                 "command": self.command if self.command else "",
                 "args": " ".join(self.args) if self.args else "",
```

### Comparing `simple_kfp_task-0.0.8/simple_kfp_task.egg-info/PKG-INFO` & `simple_kfp_task-0.0.9/simple_kfp_task.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-kfp-task
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generate a simple Kubeflow Pipeline task
 Author-email: Sebastian Alberternst <sebastian.alberternst@dfki.de>
 Project-URL: Homepage, https://github.com/salberternst/simple-kfp-task
 Project-URL: Issues, https://github.com/salberternst/simple-kfp-task/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

