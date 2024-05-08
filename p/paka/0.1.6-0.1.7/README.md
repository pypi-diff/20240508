# Comparing `tmp/paka-0.1.6.tar.gz` & `tmp/paka-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paka-0.1.6.tar", max compression
+gzip compressed data, was "paka-0.1.7.tar", max compression
```

## Comparing `paka-0.1.6.tar` & `paka-0.1.7.tar`

### file list

```diff
@@ -1,65 +1,69 @@
--rw-r--r--   0        0        0     1072 2024-04-29 21:50:17.981877 paka-0.1.6/LICENSE
--rw-r--r--   0        0        0     4467 2024-04-29 21:50:17.981877 paka-0.1.6/README.md
--rw-r--r--   0        0        0      153 2024-04-29 21:50:17.985877 paka-0.1.6/paka/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/__init__.py
--rw-r--r--   0        0        0     1608 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/__main__.py
--rw-r--r--   0        0        0     1141 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/build.py
--rw-r--r--   0        0        0     3845 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/cluster.py
--rw-r--r--   0        0        0     6721 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/function.py
--rw-r--r--   0        0        0     5905 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/job.py
--rw-r--r--   0        0        0      433 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/kubeconfig.py
--rw-r--r--   0        0        0     1938 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/model_group.py
--rw-r--r--   0        0        0     3194 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/run.py
--rw-r--r--   0        0        0     8974 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/utils.py
--rw-r--r--   0        0        0        0 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/cloudwatch.py
--rw-r--r--   0        0        0     3113 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/cluster_autoscaler.py
--rw-r--r--   0        0        0      722 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/container_registry.py
--rw-r--r--   0        0        0     2521 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/ebs_csi_driver.py
--rw-r--r--   0        0        0    12154 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/eks.py
--rw-r--r--   0        0        0     1468 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/elb.py
--rw-r--r--   0        0        0      725 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/object_store.py
--rw-r--r--   0        0        0     4078 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/service_account.py
--rw-r--r--   0        0        0     1932 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/utils.py
--rw-r--r--   0        0        0     4643 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/fluentbit.py
--rw-r--r--   0        0        0     1228 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/keda.py
--rw-r--r--   0        0        0     4956 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/knative.py
--rw-r--r--   0        0        0        0 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/manager/__init__.py
--rw-r--r--   0        0        0     1210 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/manager/aws.py
--rw-r--r--   0        0        0     2609 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/manager/base.py
--rw-r--r--   0        0        0      879 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/namespace.py
--rw-r--r--   0        0        0     3414 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/nvidia_device_plugin.py
--rw-r--r--   0        0        0     4273 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/prometheus.py
--rw-r--r--   0        0        0     3702 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/pulumi.py
--rw-r--r--   0        0        0     4000 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/qdrant.py
--rw-r--r--   0        0        0     2325 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/redis.py
--rw-r--r--   0        0        0      935 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/zipkin.py
--rw-r--r--   0        0        0    16434 2024-04-29 21:50:17.985877 paka-0.1.6/paka/config.py
--rw-r--r--   0        0        0      416 2024-04-29 21:50:17.985877 paka-0.1.6/paka/constants.py
--rw-r--r--   0        0        0     3623 2024-04-29 21:50:17.985877 paka-0.1.6/paka/container/ecr.py
--rw-r--r--   0        0        0     2886 2024-04-29 21:50:17.985877 paka-0.1.6/paka/container/pack.py
--rw-r--r--   0        0        0        0 2024-04-29 21:50:17.985877 paka-0.1.6/paka/k8s/function/__init__.py
--rw-r--r--   0        0        0     5748 2024-04-29 21:50:17.985877 paka-0.1.6/paka/k8s/function/service.py
--rw-r--r--   0        0        0        0 2024-04-29 21:50:17.985877 paka-0.1.6/paka/k8s/job/__init__.py
--rw-r--r--   0        0        0     2365 2024-04-29 21:50:17.985877 paka-0.1.6/paka/k8s/job/autoscaler.py
--rw-r--r--   0        0        0     4137 2024-04-29 21:50:17.985877 paka-0.1.6/paka/k8s/job/worker.py
--rw-r--r--   0        0        0        0 2024-04-29 21:50:17.985877 paka-0.1.6/paka/k8s/model_group/__init__.py
--rw-r--r--   0        0        0     1364 2024-04-29 21:50:17.989877 paka-0.1.6/paka/k8s/model_group/ingress.py
--rw-r--r--   0        0        0      131 2024-04-29 21:50:17.989877 paka-0.1.6/paka/k8s/model_group/manifest.py
--rw-r--r--   0        0        0        0 2024-04-29 21:50:17.989877 paka-0.1.6/paka/k8s/model_group/runtime/__init__.py
--rw-r--r--   0        0        0     4596 2024-04-29 21:50:17.989877 paka-0.1.6/paka/k8s/model_group/runtime/llama_cpp.py
--rw-r--r--   0        0        0    21055 2024-04-29 21:50:17.989877 paka-0.1.6/paka/k8s/model_group/service.py
--rw-r--r--   0        0        0    19377 2024-04-29 21:50:17.989877 paka-0.1.6/paka/k8s/utils.py
--rw-r--r--   0        0        0      761 2024-04-29 21:50:17.989877 paka-0.1.6/paka/logger.py
--rw-r--r--   0        0        0        0 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/__init__.py
--rw-r--r--   0        0        0     3031 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/base_model.py
--rw-r--r--   0        0        0     2352 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/hf_model.py
--rw-r--r--   0        0        0     1378 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/http_model.py
--rw-r--r--   0        0        0     1444 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/manifest.py
--rw-r--r--   0        0        0     2565 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/progress_bar.py
--rw-r--r--   0        0        0     2086 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/settings.py
--rw-r--r--   0        0        0    10057 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/store.py
--rw-r--r--   0        0        0    10896 2024-04-29 21:50:17.989877 paka-0.1.6/paka/utils.py
--rw-r--r--   0        0        0     1410 2024-04-29 21:50:17.989877 paka-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5713 1970-01-01 00:00:00.000000 paka-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-08 07:01:18.660155 paka-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4321 2024-05-08 07:01:18.660155 paka-0.1.7/README.md
+-rw-r--r--   0        0        0      153 2024-05-08 07:01:18.664155 paka-0.1.7/paka/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/__init__.py
+-rw-r--r--   0        0        0     1608 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/__main__.py
+-rw-r--r--   0        0        0     1401 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/build.py
+-rw-r--r--   0        0        0     4652 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/cluster.py
+-rw-r--r--   0        0        0     7308 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/function.py
+-rw-r--r--   0        0        0     6482 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/job.py
+-rw-r--r--   0        0        0      903 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/kubeconfig.py
+-rw-r--r--   0        0        0     2441 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/model_group.py
+-rw-r--r--   0        0        0     3392 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/run.py
+-rw-r--r--   0        0        0    11072 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cluster/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cluster/aws/__init__.py
+-rw-r--r--   0        0        0      968 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cluster/aws/cloudwatch.py
+-rw-r--r--   0        0        0     3049 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cluster/aws/cluster_autoscaler.py
+-rw-r--r--   0        0        0      542 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cluster/aws/container_registry.py
+-rw-r--r--   0        0        0     2466 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cluster/aws/ebs_csi_driver.py
+-rw-r--r--   0        0        0    12290 2024-05-08 07:01:18.664155 paka-0.1.7/paka/cluster/aws/eks.py
+-rw-r--r--   0        0        0     1468 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/aws/elb.py
+-rw-r--r--   0        0        0      569 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/aws/object_store.py
+-rw-r--r--   0        0        0     3969 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/aws/service_account.py
+-rw-r--r--   0        0        0     1904 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/aws/utils.py
+-rw-r--r--   0        0        0     3799 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/context.py
+-rw-r--r--   0        0        0     4580 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/fluentbit.py
+-rw-r--r--   0        0        0     1189 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/keda.py
+-rw-r--r--   0        0        0     4981 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/knative.py
+-rw-r--r--   0        0        0     2480 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/kubectl.py
+-rw-r--r--   0        0        0        0 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/manager/__init__.py
+-rw-r--r--   0        0        0      928 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/manager/aws.py
+-rw-r--r--   0        0        0     2863 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/manager/base.py
+-rw-r--r--   0        0        0      914 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/namespace.py
+-rw-r--r--   0        0        0     3484 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/nvidia_device_plugin.py
+-rw-r--r--   0        0        0     4275 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/prometheus.py
+-rw-r--r--   0        0        0     3600 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/pulumi.py
+-rw-r--r--   0        0        0     3998 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/qdrant.py
+-rw-r--r--   0        0        0     2286 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/redis.py
+-rw-r--r--   0        0        0      284 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/utils.py
+-rw-r--r--   0        0        0      908 2024-05-08 07:01:18.668155 paka-0.1.7/paka/cluster/zipkin.py
+-rw-r--r--   0        0        0    18815 2024-05-08 07:01:18.668155 paka-0.1.7/paka/config.py
+-rw-r--r--   0        0        0      467 2024-05-08 07:01:18.668155 paka-0.1.7/paka/constants.py
+-rw-r--r--   0        0        0     3623 2024-05-08 07:01:18.668155 paka-0.1.7/paka/container/ecr.py
+-rw-r--r--   0        0        0     2627 2024-05-08 07:01:18.668155 paka-0.1.7/paka/container/pack.py
+-rw-r--r--   0        0        0        0 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/function/__init__.py
+-rw-r--r--   0        0        0     5677 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/function/service.py
+-rw-r--r--   0        0        0        0 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/job/__init__.py
+-rw-r--r--   0        0        0     2365 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/job/autoscaler.py
+-rw-r--r--   0        0        0     4093 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/job/worker.py
+-rw-r--r--   0        0        0        0 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/model_group/__init__.py
+-rw-r--r--   0        0        0     1364 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/model_group/ingress.py
+-rw-r--r--   0        0        0      131 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/model_group/manifest.py
+-rw-r--r--   0        0        0        0 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/model_group/runtime/__init__.py
+-rw-r--r--   0        0        0     4820 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/model_group/runtime/llama_cpp.py
+-rw-r--r--   0        0        0     1708 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/model_group/runtime/vllm.py
+-rw-r--r--   0        0        0    21811 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/model_group/service.py
+-rw-r--r--   0        0        0    19234 2024-05-08 07:01:18.668155 paka-0.1.7/paka/k8s/utils.py
+-rw-r--r--   0        0        0      761 2024-05-08 07:01:18.668155 paka-0.1.7/paka/logger.py
+-rw-r--r--   0        0        0        0 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/__init__.py
+-rw-r--r--   0        0        0     2705 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/base_model.py
+-rw-r--r--   0        0        0     2462 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/hf_model.py
+-rw-r--r--   0        0        0     1488 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/http_model.py
+-rw-r--r--   0        0        0     1444 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/manifest.py
+-rw-r--r--   0        0        0     2565 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/progress_bar.py
+-rw-r--r--   0        0        0     2080 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/settings.py
+-rw-r--r--   0        0        0    10006 2024-05-08 07:01:18.668155 paka-0.1.7/paka/model/store.py
+-rw-r--r--   0        0        0    11138 2024-05-08 07:01:18.668155 paka-0.1.7/paka/utils.py
+-rw-r--r--   0        0        0     1477 2024-05-08 07:01:18.668155 paka-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5648 1970-01-01 00:00:00.000000 paka-0.1.7/PKG-INFO
```

### Comparing `paka-0.1.6/LICENSE` & `paka-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `paka-0.1.6/README.md` & `paka-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,15 @@
           metadata:
             type: Utilization
             value: "50"
 ```
 
 Provision the cluster
 ```bash
-paka cluster up -f cluster.yaml -u
+paka cluster up -f cluster.yaml
 ```
 
 ### Deploy an application
 Change to the application directory and add a `Procfile` and a .cnignore file.
 In `Procfile`, add the command to start the application. For example, for a flask app, it would be `web: gunicorn app:app`. In `.cnignore`, add the files to ignore during build.
 
 To pin the version of the language runtime, add a `runtime.txt` file with the version number. For example, for python, it could be `python-3.11.*`.
@@ -101,12 +101,12 @@
 ## Contributing
 - code changes
 - `make check-all`
 - Open a PR
 
 ## Dependencies
 - docker daemon and CLI
-- credentials for the AWS cloud
+- AWS CLI
 ```bash
-# Ensure your AWS credentials are correctly configured. Execute the command below and verify that the keys `aws_access_key_id` and `aws_secret_access_key` are present.
-cat ~/.aws/credentials
+# Ensure your AWS credentials are correctly configured.
+aws configure
 ```
```

### Comparing `paka-0.1.6/paka/cli/__main__.py` & `paka-0.1.7/paka/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.6/paka/cli/build.py` & `paka-0.1.7/paka/cli/build.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,31 @@
+from __future__ import annotations
+
+import os
+from typing import Optional
+
 import typer
 
-from paka.cli.utils import build as build_image
+from paka.cli.utils import build_and_push
 
 build_app = typer.Typer()
 
 
 @build_app.callback(invoke_without_command=True)
 def build(
     source_dir: str = typer.Argument(
         ...,
         help="Source directory of the application.",
     ),
+    cluster_name: Optional[str] = typer.Option(
+        os.getenv("PAKA_CURRENT_CLUSTER"),
+        "--cluster",
+        "-c",
+        help="The name of the cluster.",
+    ),
     image_name: str = typer.Option(
         "",
         "--image-name",
         help="Provide a custom name for the Docker image. If omitted, "
         "the base name of the source code directory will be used as the image name.",
     ),
 ) -> None:
@@ -24,8 +35,8 @@
     defines the commands to run for the application. The .cnignore file defines the
     files and directories to exclude from the image. Once the image is built,
     it will be pushed to the container repository of the current cluster.
 
     A Dockerfile is NOT required. The image will be built using Cloud Native Buildpacks.
     In cluster build is not supported yet. User machine must have Docker installed.
     """
-    build_image(source_dir, image_name)
+    build_and_push(cluster_name, source_dir, image_name)
```

### Comparing `paka-0.1.6/paka/cli/cluster.py` & `paka-0.1.7/paka/cli/cluster.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 from __future__ import annotations
 
+import json
+import threading
+import time
 from typing import List
 
 import click
 import typer
 
-from paka.cli.utils import load_cluster_manager
-from paka.k8s.utils import remove_crd_finalizers
-from paka.k8s.utils import update_kubeconfig as merge_update_kubeconfig
+from paka.cli.utils import load_cluster_manager, load_kubeconfig
+from paka.k8s.utils import remove_crd_finalizers, update_kubeconfig
 from paka.logger import logger
 
 cluster_app = typer.Typer()
 
 
 @cluster_app.command()
 def up(
     cluster_config: str = typer.Option(
         "",
         "--file",
         "-f",
         help="Path to the cluster config file. The cluster config file is a "
         "YAML file that contains the configuration of the cluster",
     ),
-    update_kubeconfig: bool = typer.Option(
+    no_kubeconfig: bool = typer.Option(
         False,
-        "--update-kubeconfig",
-        "-u",
-        help="Updates the default kubeconfig file (~/.kube/config) to include"
-        "the connection details of the newly created Kubernetes cluster"
-        "This allows kubectl to communicate with the new cluster.",
+        "--no-kubeconfig",
+        "-n",
+        help="By default, the connection details of the newly created Kubernetes "
+        "cluster are added to the default kubeconfig file (~/.kube/config). "
+        "This allows kubectl to communicate with the new cluster. "
+        "Use this option to prevent updating the kubeconfig file.",
     ),
 ) -> None:
     """
     Creates or updates a Kubernetes cluster based on the provided configuration.
     """
     cluster_manager = load_cluster_manager(cluster_config)
     cluster_manager.create()
-    if update_kubeconfig:
+    if not no_kubeconfig:
         logger.info("Updating kubeconfig...")
-        merge_update_kubeconfig()
+        update_kubeconfig(json.loads(cluster_manager.ctx.kubeconfig))
         logger.info("Successfully updated kubeconfig.")
 
 
 @cluster_app.command()
 def down(
     cluster_config: str = typer.Option(
         "",
@@ -63,31 +66,50 @@
     Tears down the Kubernetes cluster, removing all associated resources and data.
     """
     if yes or click.confirm(
         f"Are you sure you want to proceed with the operation? Please note that "
         "all resources and data will be permanently deleted.",
         default=False,
     ):
+        cluster_manager = load_cluster_manager(cluster_config)
+
         # Sometime finalizers might block CRD deletion, so we need to force delete those.
         # This is best effort and might not work in all cases.
         # TODO: better way to handle this
-        crds = [
-            "scaledobjects.keda.sh",
-            "routes.serving.knative.dev",
-            "ingresses.networking.internal.knative.dev",
-        ]
+        # https://github.com/kubernetes/kubernetes/issues/60538
+        stop_event = threading.Event()
 
-        for crd in crds:
+        def remove_finalizers_forever() -> None:
             try:
-                remove_crd_finalizers(crd)
-            except Exception as e:
+                crds = [
+                    "scaledobjects.keda.sh",
+                    "routes.serving.knative.dev",
+                    "ingresses.networking.internal.knative.dev",
+                ]
+
+                load_kubeconfig(cluster_manager.cloud_config.cluster.name)
+
+                while not stop_event.is_set():
+                    for crd in crds:
+                        try:
+                            remove_crd_finalizers(crd)
+                        except Exception as e:
+                            pass
+                    time.sleep(1)  # Wait for a second before the next iteration
+            except:
                 pass
 
-        cluster_manager = load_cluster_manager(cluster_config)
-        cluster_manager.destroy()
+        thread = threading.Thread(target=remove_finalizers_forever)
+        thread.start()
+
+        try:
+            cluster_manager.destroy()
+        finally:
+            stop_event.set()
+            thread.join()
 
 
 @cluster_app.command()
 def preview(
     cluster_config: str = typer.Option(
         "",
         "--file",
```

### Comparing `paka-0.1.6/paka/cli/function.py` & `paka-0.1.7/paka/cli/function.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from __future__ import annotations
 
+import os
 from typing import Literal, Optional
 
 import click
 import typer
 from kubernetes.dynamic.exceptions import NotFoundError
 from tabulate import tabulate
 
-from paka.cli.utils import resolve_image
+from paka.cli.utils import get_cluster_namespace, load_kubeconfig, resolve_image
 from paka.k8s.function.service import (
     create_knative_service,
     delete_knative_service,
     list_knative_services,
 )
-from paka.k8s.utils import try_load_kubeconfig
 from paka.logger import logger
-from paka.utils import kubify_name, read_current_cluster_data
-
-try_load_kubeconfig()
+from paka.utils import kubify_name
 
 function_app = typer.Typer()
 
 
 @function_app.command()
 def deploy(
+    cluster_name: Optional[str] = typer.Option(
+        os.getenv("PAKA_CURRENT_CLUSTER"),
+        "--cluster",
+        "-c",
+        help="The name of the cluster.",
+    ),
     name: str = typer.Option(
         ...,
         "--name",
         help="The name of the function to be deployed.",
     ),
     entrypoint: str = typer.Option(
         "web",
@@ -102,41 +106,50 @@
         metric_target (int): The target value for the scaling metric.
         scale_down_delay (str): The delay before scaling down after a spike in traffic. Must be a string
             representing a duration in seconds (e.g. "0s", "1m", "1h").
 
     Returns:
         None
     """
-    resolved_image = resolve_image(image, source_dir)
+    load_kubeconfig(cluster_name)
+    resolved_image = resolve_image(cluster_name, image, source_dir)
 
     logger.info(f"Deploying {name}...")
 
     create_knative_service(
         service_name=kubify_name(name),
-        namespace=read_current_cluster_data("namespace"),
+        namespace=get_cluster_namespace(cluster_name),
         image=resolved_image,
         entrypoint=entrypoint,
         min_instances=min_instances,
         max_instances=max_instances,
         scaling_metric=(scaling_metric, str(metric_target)),
         scale_down_delay=scale_down_delay,
     )
 
     logger.info(f"Successfully deployed {name}")
 
 
 @function_app.command()
-def list() -> None:
+def list(
+    cluster_name: Optional[str] = typer.Option(
+        os.getenv("PAKA_CURRENT_CLUSTER"),
+        "--cluster",
+        "-c",
+        help="The name of the cluster.",
+    ),
+) -> None:
     """
     List all deployed functions.
 
     Returns:
         None
     """
-    services = list_knative_services(read_current_cluster_data("namespace"))
+    load_kubeconfig(cluster_name)
+    services = list_knative_services(get_cluster_namespace(cluster_name))
 
     if not services.items:
         logger.info("No functions found.")
         return
 
     table = [
         (
@@ -163,14 +176,20 @@
         )
     )
 
 
 @function_app.command()
 def delete(
     name: str,
+    cluster_name: Optional[str] = typer.Option(
+        os.getenv("PAKA_CURRENT_CLUSTER"),
+        "--cluster",
+        "-c",
+        help="The name of the cluster.",
+    ),
     yes: bool = typer.Option(
         False,
         "--yes",
         "-y",
         help="Automatic yes to prompts. Use this option to bypass the confirmation "
         "prompt and directly proceed with the deletion.",
     ),
@@ -185,15 +204,16 @@
 
     Returns:
         None
     """
     if yes or click.confirm(
         f"Are you sure you want to delete the function {name}?", default=False
     ):
+        load_kubeconfig(cluster_name)
         logger.info(f"Deleting function {name}")
         try:
             delete_knative_service(
-                kubify_name(name), read_current_cluster_data("namespace")
+                kubify_name(name), get_cluster_namespace(cluster_name)
             )
             logger.info(f"Successfully deleted function {name}")
         except NotFoundError:
             logger.error(f"Function {name} not found.")
```

### Comparing `paka-0.1.6/paka/cli/job.py` & `paka-0.1.7/paka/cli/job.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,35 +3,38 @@
 import os
 from typing import Optional
 
 import click
 import typer
 from kubernetes import client
 
-from paka.cli.utils import resolve_image
+from paka.cli.utils import get_cluster_namespace, load_kubeconfig, resolve_image
 from paka.k8s.job.worker import create_workers, delete_workers
-from paka.k8s.utils import try_load_kubeconfig
 from paka.logger import logger
-from paka.utils import kubify_name, read_current_cluster_data
-
-try_load_kubeconfig()
+from paka.utils import kubify_name
 
 job_app = typer.Typer()
 
 
 def prefixed_job_name(job_name: str) -> str:
     # Prefix the job name with "job-" to reduce the chances of name collision
     # between jobs and functions.
     if not job_name.startswith("job-"):
         return f"job-{job_name}"
     return job_name
 
 
 @job_app.command()
 def deploy(
+    cluster_name: Optional[str] = typer.Option(
+        os.getenv("PAKA_CURRENT_CLUSTER"),
+        "--cluster",
+        "-c",
+        help="The name of the cluster.",
+    ),
     name: str = typer.Option(
         "",
         "--name",
         help="The name of the job. This name will be used to track the job's "
         "progress and manage its resources. If not provided, the system will use "
         "the base name of the 'source_dir' or the 'image' name as the job name.",
     ),
@@ -86,23 +89,24 @@
     The job can be specified by providing a Docker image or a source directory containing the application code.
 
     If a Docker image is provided, the cluster will run the job using this image.
     If a source directory is provided, the cluster will build a Docker image from the source code and then run the job.
 
     If both an image and a source directory are provided, the Docker image is used and the source directory is ignored.
     """
-    resolved_image = resolve_image(image, source_dir)
+    load_kubeconfig(cluster_name)
+    resolved_image = resolve_image(cluster_name, image, source_dir)
 
     if image:
         job_name = image
     elif source_dir:
         job_name = os.path.basename(source_dir)
 
     create_workers(
-        namespace=read_current_cluster_data("namespace"),
+        namespace=get_cluster_namespace(cluster_name),
         job_name=kubify_name(prefixed_job_name(name or job_name)),
         image=resolved_image,
         entrypoint=entrypoint,
         tasks_per_worker=tasks_per_worker,
         max_replicas=max_workers,
         drain_existing_job=wait_existing_tasks,
     )
@@ -110,14 +114,20 @@
 
 @job_app.command()
 def delete(
     name: str = typer.Argument(
         ...,
         help="The name of the job to delete.",
     ),
+    cluster_name: Optional[str] = typer.Option(
+        os.getenv("PAKA_CURRENT_CLUSTER"),
+        "--cluster",
+        "-c",
+        help="The name of the cluster.",
+    ),
     wait_existing_tasks: bool = typer.Option(
         True,
         "--wait-existing-tasks",
         help="Determines whether the system should wait for existing tasks to "
         "complete before deploying the new job. If set to true, the deployment "
         "will wait until all current tasks have finished.",
     ),
@@ -139,35 +149,44 @@
 
     Returns:
         None
     """
     if yes or click.confirm(
         f"Are you sure you want to delete the job {name}?", default=False
     ):
+        load_kubeconfig(cluster_name)
         logger.info(f"Deleting job {name}")
         delete_workers(
-            read_current_cluster_data("namespace"),
+            get_cluster_namespace(cluster_name),
             prefixed_job_name(name),
             wait_existing_tasks,
         )
         logger.info(f"Successfully deleted job {name}")
 
 
 @job_app.command()
-def list() -> None:
+def list(
+    cluster_name: Optional[str] = typer.Option(
+        os.getenv("PAKA_CURRENT_CLUSTER"),
+        "--cluster",
+        "-c",
+        help="The name of the cluster.",
+    ),
+) -> None:
     """
     Lists all jobs.
     """
+    load_kubeconfig(cluster_name)
     api_instance = client.AppsV1Api()
 
     label_selector = "role=worker"
 
     # List the deployments in the specified namespace that match the field selector
     deployments = api_instance.list_namespaced_deployment(
-        namespace=read_current_cluster_data("namespace"), label_selector=label_selector
+        namespace=get_cluster_namespace(cluster_name), label_selector=label_selector
     )
 
     for deployment in deployments.items:
         logger.info(deployment.metadata.name)
 
     if not deployments.items:
         logger.info("No jobs found.")
```

### Comparing `paka-0.1.6/paka/cli/model_group.py` & `paka-0.1.7/paka/cli/model_group.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 from __future__ import annotations
 
-from typing import Set
+import os
+from typing import Optional, Set
 
 import boto3
 import typer
 from kubernetes import client
 from tabulate import tabulate
 
+from paka.cli.utils import (
+    ensure_cluster_name,
+    get_cluster_namespace,
+    load_kubeconfig,
+    read_pulumi_stack,
+)
 from paka.k8s.model_group.service import MODEL_PATH_PREFIX, filter_services
-from paka.k8s.utils import try_load_kubeconfig
 from paka.logger import logger
-from paka.utils import read_current_cluster_data
-
-try_load_kubeconfig()
 
 model_group_app = typer.Typer()
 
 
 @model_group_app.command()
-def list_downloaded_models() -> None:
+def list_downloaded_models(
+    cluster_name: Optional[str] = typer.Option(
+        os.getenv("PAKA_CURRENT_CLUSTER"),
+        "--cluster",
+        "-c",
+        help="The name of the cluster.",
+    ),
+) -> None:
     """
     List all models that have been downloaded to the object store.
     """
-    bucket = read_current_cluster_data("bucket")
+    load_kubeconfig(cluster_name)
+    cluster_name = ensure_cluster_name(cluster_name)
+    bucket = read_pulumi_stack(cluster_name, "bucket")
+
     s3 = boto3.client("s3")
     response = s3.list_objects_v2(Bucket=bucket, Prefix=MODEL_PATH_PREFIX)
     if "Contents" in response:
         unique_models: Set[str] = set()
         for obj in response["Contents"]:
             key = obj["Key"]
             if key.startswith(f"{MODEL_PATH_PREFIX}/"):
@@ -38,19 +51,27 @@
         for key in unique_models:
             logger.info(key)
     else:
         logger.info("No models found.")
 
 
 @model_group_app.command()
-def list() -> None:
+def list(
+    cluster_name: Optional[str] = typer.Option(
+        os.getenv("PAKA_CURRENT_CLUSTER"),
+        "--cluster",
+        "-c",
+        help="The name of the cluster.",
+    ),
+) -> None:
     """
     List all model groups.
     """
-    services = filter_services(read_current_cluster_data("namespace"))
+    load_kubeconfig(cluster_name)
+    services = filter_services(get_cluster_namespace(cluster_name))
     model_groups = [service.spec.selector.get("model") for service in services]
 
     v1 = client.CoreV1Api()
     cfg = v1.read_namespaced_config_map("config-domain", "knative-serving")
     filtered_keys = [key for key in cfg.data.keys() if key.endswith("sslip.io")]
     if not filtered_keys:
         if not model_groups:
```

### Comparing `paka-0.1.6/paka/cli/run.py` & `paka-0.1.7/paka/cli/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,38 @@
+import os
 import shlex
 from typing import Optional
 
 import typer
 from kubernetes import client
 
-from paka.cli.utils import resolve_image
-from paka.k8s.utils import tail_logs, try_load_kubeconfig
+from paka.cli.utils import get_cluster_namespace, load_kubeconfig, resolve_image
+from paka.k8s.utils import tail_logs
 from paka.logger import logger
-from paka.utils import kubify_name, random_str, read_current_cluster_data
+from paka.utils import kubify_name, random_str
 
 CLEANUP_TIMEOUT = 600  # 10 minutes
 
 run_app = typer.Typer()
 
-try_load_kubeconfig()
-
 
 @run_app.callback(invoke_without_command=True)
 def one_off_script(
     entrypoint: str = typer.Option(
         ...,
         "--entrypoint",
         help="The entrypoint of the application. This refers to the command "
         "defined in the Procfile that will be executed.",
     ),
+    cluster_name: Optional[str] = typer.Option(
+        os.getenv("PAKA_CURRENT_CLUSTER"),
+        "--cluster",
+        "-c",
+        help="The name of the cluster.",
+    ),
     source_dir: Optional[str] = typer.Option(
         None,
         "--source",
         help="The directory containing the source code of the application. If "
         "specified, a new Docker image will be built using the source code from "
         "this directory. A Dockerfile is not required because the build process "
         "uses Cloud Native's Buildpacks, which automatically detect and install "
@@ -44,15 +49,16 @@
     """
     Runs a one-off script.
 
     This command creates a new Kubernetes job that runs the specified entrypoint command
     in a container with the specified Docker image. If a source directory is provided, a new
     Docker image is built using the source code from that directory.
     """
-    resolved_image = resolve_image(image, source_dir)
+    load_kubeconfig(cluster_name)
+    resolved_image = resolve_image(cluster_name, image, source_dir)
 
     # Generate a job name which is the hash of the command
     job_name = f"run-{kubify_name(random_str(10))}"
 
     job = client.V1Job(
         api_version="batch/v1",
         kind="Job",
@@ -72,15 +78,15 @@
                 )
             ),
             backoff_limit=0,
             ttl_seconds_after_finished=CLEANUP_TIMEOUT,
         ),
     )
 
-    namespace = read_current_cluster_data("namespace")
+    namespace = get_cluster_namespace(cluster_name)
 
     logger.info(f"Submitting the task...")
     batch_api = client.BatchV1Api()
     batch_api.create_namespaced_job(namespace=namespace, body=job)
     logger.info(f"Successfully submitted the task.")
 
     logger.info(f"Waiting for the task to complete...")
```

### Comparing `paka-0.1.6/paka/cli/utils.py` & `paka-0.1.7/paka/cli/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 from __future__ import annotations
 
 import functools
 import os
+import platform
 import re
 import subprocess
 from typing import Any, Optional
 
 import typer
+from kubernetes import config as k8s_config
 
 from paka.cluster.manager.aws import AWSClusterManager
 from paka.cluster.manager.base import ClusterManager
-from paka.config import parse_yaml
+from paka.config import CloudConfig, Config, parse_yaml
 from paka.constants import BP_BUILDER_ENV_VAR
 from paka.container.ecr import push_to_ecr
 from paka.container.pack import ensure_pack
 from paka.logger import logger
-from paka.utils import get_pulumi_root, read_current_cluster_data
+from paka.utils import get_pulumi_root, read_pulumi_stack
 
 
-def build(
+def build_and_push(
+    cluster_name: Optional[str],
     source_dir: str,
     image_name: str,
 ) -> str:
     """
     Builds a Docker image from the source code in the specified directory.
 
     This function uses the Cloud Native Buildpacks (pack) tool to build a Docker image from the source code
     in the specified directory. The resulting image is then pushed to the Amazon Elastic Container Registry (ECR).
 
     Args:
+        cluster_name (str): The name of the cluster to build the image for.
         source_dir (str): The directory containing the source code of the application.
         image_name (str): The name of the Docker image to build. If not provided, the name of the source directory is used.
 
     Returns:
         str: The image tag of the built Docker image.
     """
     pack_bin = ensure_pack()
@@ -65,15 +69,17 @@
                 bp_cpython_version = match.group(1)
             else:
                 match = re.search(r"nodejs-(\d+\.\d+(\.\d+|\.\*))", content)
                 if match:
                     bp_node_version = match.group(1)
 
     try:
-        subprocess.run(["cd", source_dir], check=True)
+        if not os.path.exists(source_dir):
+            logger.error(f"Source directory {source_dir} does not exist.")
+            raise typer.Exit(1)
 
         builder = os.environ.get(BP_BUILDER_ENV_VAR, "paketobuildpacks/builder:base")
 
         pack_command = [
             pack_bin,
             "build",
             image_name,
@@ -81,29 +87,43 @@
             builder,
         ]
         if bp_cpython_version:
             pack_command.extend(["--env", f"BP_CPYTHON_VERSION={bp_cpython_version}"])
         elif bp_node_version:
             pack_command.extend(["--env", f"BP_NODE_VERSION={bp_node_version}"])
 
-        subprocess.run(pack_command, check=True)
+        subprocess.run(pack_command, cwd=source_dir, check=True)
         logger.info(f"Successfully built {image_name}")
 
+        cluster_name = ensure_cluster_name(cluster_name)
+
         return push_to_ecr(
             image_name,
-            read_current_cluster_data("registry"),
-            read_current_cluster_data("region"),
+            read_pulumi_stack(cluster_name, "registry"),
+            read_pulumi_stack(cluster_name, "region"),
             image_name,
         )
 
     except subprocess.CalledProcessError as e:
         logger.error(f"An error occurred: {e}")
         raise typer.Exit(1)
 
 
+def load_cluster_config(cluster_config_file: Optional[str]) -> Optional[Config]:
+    if not cluster_config_file:
+        cluster_config_file = "./cluster.yaml"
+    cluster_config_file = os.path.abspath(os.path.expanduser(cluster_config_file))
+    if not os.path.exists(cluster_config_file):
+        return None
+
+    with open(cluster_config_file, "r") as file:
+        config = parse_yaml(file.read())
+        return config
+
+
 def load_cluster_manager(cluster_config: str) -> ClusterManager:
     """
     Loads the cluster manager based on the provided cluster configuration YAML file.
 
     This function reads the cluster configuration file, parses it as YAML, and then
     creates and returns a cluster manager object based on the cloud provider specified
     in the configuration. Currently, only AWS is supported.
@@ -116,29 +136,23 @@
         ClusterManager: An instance of the cluster manager corresponding to the
         cloud provider specified in the configuration.
 
     Raises:
         FileNotFoundError: If the cluster configuration file does not exist.
         ValueError: If the cloud provider specified in the configuration is not supported.
     """
-    if not cluster_config:
-        cluster_config = "./cluster.yaml"
-
-    cluster_config = os.path.abspath(os.path.expanduser(cluster_config))
+    config_data = load_cluster_config(cluster_config)
 
-    if not os.path.exists(cluster_config):
+    if not config_data:
         raise FileNotFoundError(f"The cluster config file does not exist")
 
-    with open(cluster_config, "r") as file:
-        config_data = parse_yaml(file.read())
-
-        if config_data.aws:
-            return AWSClusterManager(config=config_data)
-        else:
-            raise ValueError("Unsupported cloud provider")
+    if config_data.aws:
+        return AWSClusterManager(config=config_data)
+    else:
+        raise ValueError("Unsupported cloud provider")
 
 
 def validate_name(func: Any) -> Any:
     """
     Decorator to validate the name argument of a function.
 
     This decorator checks if the name argument of the decorated function matches
@@ -168,15 +182,17 @@
             )
             raise typer.Exit(1)
         return func(name, *args, **kwargs)
 
     return wrapper
 
 
-def resolve_image(image: Optional[str], source_dir: Optional[str]) -> str:
+def resolve_image(
+    cluster_name: Optional[str], image: Optional[str], source_dir: Optional[str]
+) -> str:
     """
     Determines the Docker image to be utilized by either using the provided image
     directly or by building an image from the specified source directory.
 
     This function checks if exactly one of image or source_dir is provided. If
     both or neither are provided, it logs an error message and exits the program.
     If only source_dir is provided, it builds the Docker image from the source
@@ -203,23 +219,24 @@
         raise typer.Exit(1)
 
     result_image = ""
 
     if not image and source_dir:
         source_dir = os.path.abspath(os.path.expanduser(source_dir))
         result_image = os.path.basename(source_dir)
-        result_image = build(source_dir, result_image)
+        result_image = build_and_push(cluster_name, source_dir, result_image)
     elif image:
         result_image = image
 
     # If a fully qualified image name is provided, use it directly. This gives users
     # the flexibility to use images from other registries. Otherwise, the image is assumed
     # to be located in the default registry and will be retrieved from there.
+    cluster_name = ensure_cluster_name(cluster_name)
     if ":" not in result_image:
-        registry_uri = read_current_cluster_data("registry")
+        registry_uri = read_pulumi_stack(cluster_name, "registry")
         result_image = f"{registry_uri}:{result_image}"
 
     return result_image
 
 
 def init_pulumi() -> None:
     """
@@ -236,12 +253,58 @@
     """
     os.environ["PULUMI_CONFIG_PASSPHRASE"] = os.environ.get(
         "PULUMI_CONFIG_PASSPHRASE", ""
     )
 
     pulumi_root = get_pulumi_root()
     os.makedirs(pulumi_root, exist_ok=True)
-    os.environ["PULUMI_BACKEND_URL"] = os.environ.get(
-        "PULUMI_BACKEND_URL", f"file://{pulumi_root}"
+    os.environ["PULUMI_DEBUG_COMMANDS"] = os.environ.get(
+        "PULUMI_DEBUG_COMMANDS", "false"
     )
-    os.environ["PULUMI_DEBUG"] = os.environ.get("PULUMI_DEBUG", "false")
     os.environ["PULUMI_HOME"] = os.environ.get("PULUMI_HOME", pulumi_root)
+
+    system = platform.system().lower()
+    if system == "windows":
+        _, pulumi_root = os.path.splitdrive(pulumi_root)
+        pulumi_url = f"file:///{pulumi_root}"
+    else:
+        pulumi_url = f"file://{pulumi_root}"
+
+    os.environ["PULUMI_BACKEND_URL"] = os.environ.get(
+        "PULUMI_BACKEND_URL",
+        pulumi_url,
+    )
+
+
+def ensure_cluster_name(cluster_name: Optional[str]) -> str:
+    if cluster_name:
+        return cluster_name
+    # This will load the `./cluster.yaml` file if it exists
+    config = load_cluster_config("")
+    if not config:
+        logger.error("Please provide a cluster name.")
+        raise typer.Exit(1)
+
+    assert config.aws, "Only AWS is supported for now"
+    return config.aws.cluster.name
+
+
+def ensure_cluster_config(cluster_file: Optional[str]) -> CloudConfig:
+    config = load_cluster_config(cluster_file)
+    if not config:
+        logger.error("Cannot locate cluster configuration file.")
+        raise typer.Exit(1)
+
+    assert config.aws, "Only AWS is supported for now"
+    return config.aws
+
+
+def get_cluster_namespace(cluster_name: Optional[str]) -> str:
+    cluster_name = ensure_cluster_name(cluster_name)
+    namespace = read_pulumi_stack(cluster_name, "namespace")
+    return namespace
+
+
+def load_kubeconfig(cluster_name: Optional[str]) -> None:
+    cluster_name = ensure_cluster_name(cluster_name)
+    kubeconfig = read_pulumi_stack(cluster_name, "kubeconfig")
+    k8s_config.load_kube_config_from_dict(kubeconfig)
```

### Comparing `paka-0.1.6/paka/cluster/aws/cluster_autoscaler.py` & `paka-0.1.7/paka/cluster/aws/cluster_autoscaler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import pulumi
 import pulumi_aws as aws
 import pulumi_eks as eks
-import pulumi_kubernetes as k8s
 import pulumi_kubernetes.helm.v3 as helm
 
 from paka.cluster.aws.utils import odic_role_for_sa
-from paka.config import CloudConfig
+from paka.cluster.context import Context
 from paka.utils import call_once
 
 
 @call_once
 def create_cluster_autoscaler(
-    config: CloudConfig,
+    ctx: Context,
     cluster: eks.Cluster,
-    k8s_provider: k8s.Provider,
 ) -> None:
     """
     Sets up the cluster autoscaler for an EKS cluster.
 
     Args:
         cluster (eks.Cluster): The EKS cluster.
         k8s_provider (k8s.Provider): The Kubernetes provider.
         config (CloudConfig): The cluster config provided by user.
 
     Returns:
         None
     """
-    project = config.cluster.name
+    cluster_name = ctx.cluster_name
 
     autoscaler_policy_doc = aws.iam.get_policy_document(
         statements=[
             aws.iam.GetPolicyDocumentStatementArgs(
                 actions=[
                     "autoscaling:DescribeAutoScalingGroups",
                     "autoscaling:DescribeAutoScalingInstances",
@@ -43,49 +41,49 @@
                 ],
                 resources=["*"],
             )
         ]
     )
 
     autoscaler_policy = aws.iam.Policy(
-        f"{project}-autoscaler-policy", policy=autoscaler_policy_doc.json
+        f"{cluster_name}-autoscaler-policy", policy=autoscaler_policy_doc.json
     )
 
     # The OIDC provider is required because the cluster autoscaler runs within the Kubernetes
     # cluster and needs to interact with the AWS API to manage the Auto Scaling Groups (ASGs).
     # OIDC provides a secure mechanism for the cluster autoscaler to authenticate with the AWS API.
     autoscaler_role = odic_role_for_sa(
-        config, cluster, "autoscaler", "kube-system:cluster-autoscaler"
+        ctx, cluster, "autoscaler", "kube-system:cluster-autoscaler"
     )
 
     aws.iam.RolePolicyAttachment(
-        f"{project}-autoscaler-role-policy-attachment",
+        f"{cluster_name}-autoscaler-role-policy-attachment",
         policy_arn=autoscaler_policy.arn,
         role=autoscaler_role.name,
     )
 
     helm.Chart(
         "cluster-autoscaler",
         helm.ChartOpts(
             chart="cluster-autoscaler",
             version="9.34.0",
             namespace="kube-system",
             fetch_opts=helm.FetchOpts(repo="https://kubernetes.github.io/autoscaler"),
             values={
                 "autoDiscovery": {"clusterName": cluster.eks_cluster.name},
-                "awsRegion": config.cluster.region,
+                "awsRegion": ctx.region,
                 "rbac": {
                     "create": True,
                     "serviceAccount": {
                         "create": True,
                         "name": "cluster-autoscaler",
                         "annotations": {
                             "eks.amazonaws.com/role-arn": autoscaler_role.arn
                         },
                     },
                 },
                 "serviceMonitor": {"interval": "2s"},
                 "image": {"tag": "v1.28.2"},
             },
         ),
-        opts=pulumi.ResourceOptions(provider=k8s_provider),
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider),
     )
```

### Comparing `paka-0.1.6/paka/cluster/aws/ebs_csi_driver.py` & `paka-0.1.7/paka/cluster/aws/ebs_csi_driver.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import pulumi
 import pulumi_aws as aws
 import pulumi_eks as eks
-import pulumi_kubernetes as k8s
 from pulumi_kubernetes.helm.v3 import Chart, ChartOpts, FetchOpts
 
 from paka.cluster.aws.utils import odic_role_for_sa
-from paka.config import CloudConfig
+from paka.cluster.context import Context
 from paka.utils import call_once
 
 
 @call_once
-def create_ebs_csi_driver(
-    config: CloudConfig, cluster: eks.Cluster, k8s_provider: k8s.Provider
-) -> None:
-    project = config.cluster.name
+def create_ebs_csi_driver(ctx: Context, cluster: eks.Cluster) -> None:
+    cluster_name = ctx.cluster_name
 
     csi_driver_policy_doc = aws.iam.get_policy_document(
         statements=[
             aws.iam.GetPolicyDocumentStatementArgs(
                 actions=[
                     "ec2:CreateSnapshot",
                     "ec2:AttachVolume",
@@ -36,23 +33,23 @@
                 resources=["*"],
                 effect="Allow",
             )
         ]
     )
 
     csi_driver_policy = aws.iam.Policy(
-        f"{project}-csi-driver-policy", policy=csi_driver_policy_doc.json
+        f"{cluster_name}-csi-driver-policy", policy=csi_driver_policy_doc.json
     )
 
     csi_driver_role = odic_role_for_sa(
-        config, cluster, "csi-driver", "kube-system:ebs-csi-controller-sa"
+        ctx, cluster, "csi-driver", "kube-system:ebs-csi-controller-sa"
     )
 
     aws.iam.RolePolicyAttachment(
-        f"{project}-csi-driver-role-policy-attachment",
+        f"{cluster_name}-csi-driver-role-policy-attachment",
         policy_arn=csi_driver_policy.arn,
         role=csi_driver_role.name,
     )
 
     Chart(
         "aws-ebs-csi-driver",
         ChartOpts(
@@ -71,9 +68,9 @@
                             "eks.amazonaws.com/role-arn": csi_driver_role.arn
                         },
                         "automountServiceAccountToken": "true",
                     },
                 }
             },
         ),
-        opts=pulumi.ResourceOptions(provider=k8s_provider),
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider),
     )
```

### Comparing `paka-0.1.6/paka/cluster/aws/eks.py` & `paka-0.1.7/paka/cluster/aws/eks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import List, Optional, cast
 
 import pulumi
 import pulumi_aws as aws
 import pulumi_awsx as awsx
 import pulumi_eks as eks
 import pulumi_kubernetes as k8s
 
 from paka.cluster.aws.cloudwatch import enable_cloudwatch
 from paka.cluster.aws.cluster_autoscaler import create_cluster_autoscaler
 from paka.cluster.aws.ebs_csi_driver import create_ebs_csi_driver
 from paka.cluster.aws.elb import update_elb_idle_timeout
 from paka.cluster.aws.service_account import create_service_accounts
+from paka.cluster.context import Context
 from paka.cluster.keda import create_keda
 from paka.cluster.knative import create_knative_and_istio
 from paka.cluster.namespace import create_namespace
 from paka.cluster.nvidia_device_plugin import install_nvidia_device_plugin
 from paka.cluster.prometheus import create_prometheus
 from paka.cluster.qdrant import create_qdrant
 from paka.cluster.redis import create_redis
 from paka.cluster.zipkin import create_zipkin
-from paka.config import CloudConfig
-from paka.utils import kubify_name, save_kubeconfig
+from paka.config import AwsModelGroup
+from paka.utils import kubify_name
 
 
 def _ignore_tags_transformation(
     args: pulumi.ResourceTransformationArgs,
 ) -> Optional[pulumi.ResourceTransformationResult]:
     """
     EKS adds tags to VPC and Subnet resources that are not managed by Pulumi. This function ignores those tags so that Pulumi does not try to remove them.
@@ -44,15 +45,15 @@
                 args.opts, pulumi.ResourceOptions(ignore_changes=["tags"])
             ),
         )
     return None
 
 
 def create_node_group_for_model_group(
-    config: CloudConfig,
+    ctx: Context,
     cluster: eks.Cluster,
     vpc: awsx.ec2.Vpc,
     worker_role: aws.iam.Role,
 ) -> None:
     """
     Creates a managed node group for each model group in the provided configuration.
 
@@ -66,24 +67,26 @@
         cluster (eks.Cluster): The EKS cluster to create the node groups in.
         vpc (awsx.ec2.Vpc): The VPC to associate the node groups with.
         worker_role (aws.iam.Role): The IAM role for the worker nodes.
 
     Returns:
         None
     """
-    if config.modelGroups is None:
+    if ctx.cloud_config.modelGroups is None:
         return
 
-    project = config.cluster.name
+    cluster_name = ctx.cluster_name
 
-    for model_group in config.modelGroups:
+    model_groups = cast(List[AwsModelGroup], ctx.cloud_config.modelGroups)
+
+    for model_group in model_groups:
         # Create a managed node group for our cluster
         eks.ManagedNodeGroup(
-            f"{project}-{kubify_name(model_group.name)}-group",
-            node_group_name=f"{project}-{kubify_name(model_group.name)}-group",
+            f"{cluster_name}-{kubify_name(model_group.name)}-group",
+            node_group_name=f"{cluster_name}-{kubify_name(model_group.name)}-group",
             cluster=cluster,
             instance_types=[model_group.nodeType],
             scaling_config=aws.eks.NodeGroupScalingConfigArgs(
                 desired_size=model_group.minInstances,
                 min_size=model_group.minInstances,
                 max_size=model_group.maxInstances,
             ),
@@ -99,25 +102,29 @@
                     effect="NO_SCHEDULE", key="app", value="model-group"
                 ),
                 aws.eks.NodeGroupTaintArgs(
                     effect="NO_SCHEDULE", key="model", value=model_group.name
                 ),
             ],
             # Supported AMI types https://docs.aws.amazon.com/eks/latest/APIReference/API_Nodegroup.html#AmazonEKS-Type-Nodegroup-amiType
-            ami_type=("AL2_x86_64_GPU" if model_group.awsGpu else None),
+            ami_type=(
+                "AL2_x86_64_GPU"
+                if model_group.gpu and model_group.gpu.enabled
+                else None
+            ),
             disk_size=(
-                model_group.awsGpu.diskSize
-                if model_group.awsGpu
+                model_group.gpu.diskSize
+                if model_group.gpu and model_group.gpu.enabled
                 else model_group.diskSize
             ),
         )
 
 
 def create_node_group_for_qdrant(
-    config: CloudConfig,
+    ctx: Context,
     cluster: eks.Cluster,
     vpc: awsx.ec2.Vpc,
     worker_role: aws.iam.Role,
 ) -> None:
     """
     Creates a managed node group for Qdrant in the provided EKS cluster.
 
@@ -137,25 +144,25 @@
         cluster (eks.Cluster): The EKS cluster to create the node group in.
         vpc (awsx.ec2.Vpc): The VPC to associate the node group with.
         worker_role (aws.iam.Role): The IAM role for the worker nodes.
 
     Returns:
         None
     """
-    if config.vectorStore is None:
+    if ctx.cloud_config.vectorStore is None:
         return
 
-    project = config.cluster.name
+    cluster_name = ctx.cluster_name
 
-    vectorStore = config.vectorStore
+    vectorStore = ctx.cloud_config.vectorStore
 
     # Create a managed node group for our cluster
     eks.ManagedNodeGroup(
-        f"{project}-qdrant-group",
-        node_group_name=f"{project}-qdrant-group",
+        f"{cluster_name}-qdrant-group",
+        node_group_name=f"{cluster_name}-qdrant-group",
         cluster=cluster,
         instance_types=[vectorStore.nodeType],
         # Scaling down to 0 is not supported
         scaling_config=aws.eks.NodeGroupScalingConfigArgs(
             desired_size=vectorStore.replicas,
             min_size=vectorStore.replicas,
             max_size=vectorStore.replicas,
@@ -168,35 +175,32 @@
         subnet_ids=vpc.private_subnet_ids,
         taints=[
             aws.eks.NodeGroupTaintArgs(effect="NO_SCHEDULE", key="app", value="qdrant"),
         ],
     )
 
 
-def create_k8s_cluster(config: CloudConfig) -> eks.Cluster:
+def create_k8s_cluster(ctx: Context) -> eks.Cluster:
     """
     Provisions an AWS EKS cluster with the necessary resources.
 
     This function creates an EKS cluster, a worker role, a VPC, and other required resources
     for running Kubernetes workloads on AWS.
 
     How does autoscaling work?
     We use two-level scaling strategies. First, we install a Cluster Autoscaler to scale out or in the cluster
     nodes based on the workload. However, the Cluster Autoscaler doesn't scale the nodes based on the CPU and
     memory usage of the nodes. Instead, it scales the nodes based on the number of pending pods in the cluster.
     Second, we install a Horizontal Pod Autoscaler to scale out or in the pods based on the CPU and memory usage of
     the pods. Once the pods are scaled, the Cluster Autoscaler will scale the nodes based on the number of pending pods.
 
-    Args:
-        config (CloudConfig): The cluster config provided by user.
-
     Returns:
-        None
+        eks.Cluster
     """
-    project = config.cluster.name
+    cluster_name = ctx.cluster_name
 
     managed_policy_arns = [
         "arn:aws:iam::aws:policy/AmazonEKSWorkerNodePolicy",
         "arn:aws:iam::aws:policy/AmazonEKS_CNI_Policy",
         "arn:aws:iam::aws:policy/AmazonEC2ContainerRegistryReadOnly",
     ]
     assume_role_policy = aws.iam.get_policy_document(
@@ -211,22 +215,22 @@
                     ),
                 ],
             ),
         ],
     ).json
 
     worker_role = aws.iam.Role(
-        f"{project}-eks-worker-role",
+        f"{cluster_name}-eks-worker-role",
         assume_role_policy=assume_role_policy,
         managed_policy_arns=managed_policy_arns,
     )
 
     # Create a VPC for our cluster
     vpc = awsx.ec2.Vpc(
-        f"{project}-vpc",
+        f"{cluster_name}-vpc",
         subnet_strategy=awsx.ec2.SubnetAllocationStrategy.AUTO,
         # AWS needs these tags for creating load balancers
         # See https://repost.aws/knowledge-center/eks-vpc-subnet-discovery
         subnet_specs=[
             {
                 "type": awsx.ec2.SubnetType.PUBLIC,
                 "tags": {"kubernetes.io/role/elb": "1"},
@@ -236,82 +240,83 @@
                 "tags": {"kubernetes.io/role/internal-elb": "1"},
             },
         ],
         opts=pulumi.ResourceOptions(transformations=[_ignore_tags_transformation]),
     )
 
     cluster = eks.Cluster(
-        project,
+        cluster_name,
         vpc_id=vpc.vpc_id,
         public_subnet_ids=vpc.public_subnet_ids,
         private_subnet_ids=vpc.private_subnet_ids,
         node_associate_public_ip_address=False,
         create_oidc_provider=True,
         skip_default_node_group=True,
         # Use the worker role we created above. This is required for creating the managed node group.
         instance_roles=[worker_role],
     )
 
     # Create a managed node group for our cluster
     eks.ManagedNodeGroup(
-        f"{project}-default-group",
-        node_group_name=f"{project}-default-group",
+        f"{cluster_name}-default-group",
+        node_group_name=f"{cluster_name}-default-group",
         cluster=cluster,
-        instance_types=[config.cluster.nodeType],
+        instance_types=[ctx.cloud_config.cluster.nodeType],
         scaling_config=aws.eks.NodeGroupScalingConfigArgs(
-            desired_size=config.cluster.minNodes,
-            min_size=config.cluster.minNodes,
-            max_size=config.cluster.maxNodes,
+            desired_size=ctx.cloud_config.cluster.minNodes,
+            min_size=ctx.cloud_config.cluster.minNodes,
+            max_size=ctx.cloud_config.cluster.maxNodes,
         ),
-        labels={"size": config.cluster.nodeType, "group": "default"},
+        labels={"size": ctx.cloud_config.cluster.nodeType, "group": "default"},
         node_role_arn=worker_role.arn,
         subnet_ids=vpc.private_subnet_ids,
     )
 
     # Create a managed node group for each model group
-    create_node_group_for_model_group(config, cluster, vpc, worker_role)
+    create_node_group_for_model_group(ctx, cluster, vpc, worker_role)
 
     # Create a managed node group for Qdrant
-    create_node_group_for_qdrant(config, cluster, vpc, worker_role)
+    create_node_group_for_qdrant(ctx, cluster, vpc, worker_role)
 
     def create_eks_resources(kubeconfig_json: str) -> None:
         k8s_provider = k8s.Provider("k8s-provider", kubeconfig=cluster.kubeconfig)
+        ctx.set_k8s_provider(k8s_provider)
+        ctx.set_kubeconfig(kubeconfig_json)
 
-        save_kubeconfig(config.cluster.name, kubeconfig_json)
+        # save_kubeconfig(ctx.cluster_name, kubeconfig_json)
 
         # Deploy the metrics server. This is required for the Horizontal Pod Autoscaler to work.
         # HPA requires metrics to be available in order to scale the pods.
         k8s.yaml.ConfigFile(
             "metrics-server",
             file="https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml",
             opts=pulumi.ResourceOptions(provider=k8s_provider),
         )
 
         # Deploy the cluster autoscaler through Helm
         create_cluster_autoscaler(
-            config,
+            ctx,
             cluster,
-            k8s_provider,
         )
 
-        create_ebs_csi_driver(config, cluster, k8s_provider)
-        create_namespace(k8s_provider, kubeconfig_json)
+        create_ebs_csi_driver(ctx, cluster)
+        create_namespace(ctx, kubeconfig_json)
         # TODO: Decouple knative and istio
-        create_knative_and_istio(config, k8s_provider)
-        create_redis(config, k8s_provider)
-        create_keda(config, k8s_provider)
-        create_qdrant(config, k8s_provider)
-
-        create_service_accounts(config, cluster, k8s_provider)
-        enable_cloudwatch(config, k8s_provider)
-        create_prometheus(config, k8s_provider)
-        create_zipkin(config, k8s_provider)
+        create_knative_and_istio(ctx)
+        create_redis(ctx)
+        create_keda(ctx)
+        create_qdrant(ctx)
+
+        create_service_accounts(ctx, cluster)
+        enable_cloudwatch(ctx)
+        create_prometheus(ctx)
+        create_zipkin(ctx)
         # Install the NVIDIA device plugin for GPU support
         # Even if the cluster doesn't have GPUs, this won't cause any issues
-        install_nvidia_device_plugin(k8s_provider)
+        install_nvidia_device_plugin(ctx)
 
         # TODO: Set timeout to be the one used by knative
         update_elb_idle_timeout(kubeconfig_json, 300)
 
     # Save the kubeconfig to a file
     cluster.kubeconfig_json.apply(create_eks_resources)
```

### Comparing `paka-0.1.6/paka/cluster/aws/elb.py` & `paka-0.1.7/paka/cluster/aws/elb.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.6/paka/cluster/aws/service_account.py` & `paka-0.1.7/paka/cluster/aws/service_account.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import pulumi
 import pulumi_aws as aws
 import pulumi_eks as eks
 import pulumi_kubernetes as k8s
 
 from paka.cluster.aws.utils import odic_role_for_sa
-from paka.config import CloudConfig
+from paka.cluster.context import Context
 from paka.constants import ACCESS_ALL_SA
-from paka.utils import call_once, read_cluster_data, read_current_cluster_data
+from paka.utils import call_once
 
 
 @call_once
 def create_service_accounts(
-    config: CloudConfig,
+    ctx: Context,
     cluster: eks.Cluster,
-    k8s_provider: k8s.Provider,
 ) -> None:
     """
     Creates service accounts with necessary IAM roles and policies.
 
     This function creates two IAM policies: one for S3 access and one for ECR access.
     It then creates an IAM role for the service account and attaches the two policies to this role.
     Finally, it creates a Kubernetes service account and annotates it with the ARN of the IAM role.
@@ -29,19 +28,19 @@
         config (CloudConfig): The cloud configuration containing the cluster name.
         cluster (eks.Cluster): The EKS cluster to create the service accounts in.
         k8s_provider (k8s.Provider): The Kubernetes provider to use when creating the service account.
 
     Returns:
         None
     """
-    project = config.cluster.name
-    bucket = read_cluster_data(project, "bucket")
+    cluster_name = ctx.cluster_name
+    bucket = ctx.bucket
 
     s3_policy = aws.iam.Policy(
-        f"{project}-s3-access-policy",
+        f"{cluster_name}-s3-access-policy",
         policy=aws.iam.get_policy_document(
             statements=[
                 aws.iam.GetPolicyDocumentStatementArgs(
                     effect="Allow",
                     actions=["s3:GetObject", "s3:ListBucket"],
                     resources=[
                         f"arn:aws:s3:::{bucket}/*",
@@ -49,15 +48,15 @@
                     ],
                 )
             ]
         ).json,
     )
 
     ecr_policy = aws.iam.Policy(
-        f"{project}-ecr-access-policy",
+        f"{cluster_name}-ecr-access-policy",
         policy=aws.iam.get_policy_document(
             statements=[
                 aws.iam.GetPolicyDocumentStatementArgs(
                     effect="Allow",
                     actions=[
                         "ecr:GetDownloadUrlForLayer",
                         "ecr:BatchGetImage",
@@ -85,42 +84,42 @@
                     ],
                     resources=["arn:aws:logs:*:*:*"],
                 )
             ]
         ).json,
     )
 
-    ns = read_current_cluster_data("namespace")
+    namespace = ctx.namespace
     sa_role = odic_role_for_sa(
-        config,
+        ctx,
         cluster,
         "sa",
-        f"{ns}:{ACCESS_ALL_SA}",
+        f"{namespace}:{ACCESS_ALL_SA}",
     )
 
     aws.iam.RolePolicyAttachment(
-        f"{project}-sa-s3-role-policy-attachment",
+        f"{cluster_name}-sa-s3-role-policy-attachment",
         role=sa_role.name,
         policy_arn=s3_policy.arn,
     )
 
     aws.iam.RolePolicyAttachment(
-        f"{project}-sa-ecr-role-policy-attachment",
+        f"{cluster_name}-sa-ecr-role-policy-attachment",
         role=sa_role.name,
         policy_arn=ecr_policy.arn,
     )
 
     aws.iam.RolePolicyAttachment(
-        f"{project}-sa-cloudwatch-role-policy-attachment",
+        f"{cluster_name}-sa-cloudwatch-role-policy-attachment",
         role=sa_role.name,
         policy_arn=cloudwatch_policy.arn,
     )
 
     k8s.core.v1.ServiceAccount(
-        f"{project}-service-account",
+        f"{cluster_name}-service-account",
         metadata={
-            "namespace": read_current_cluster_data("namespace"),
+            "namespace": ctx.namespace,
             "name": ACCESS_ALL_SA,
             "annotations": {"eks.amazonaws.com/role-arn": sa_role.arn},
         },
-        opts=pulumi.ResourceOptions(provider=k8s_provider),
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider),
     )
```

### Comparing `paka-0.1.6/paka/cluster/aws/utils.py` & `paka-0.1.7/paka/cluster/aws/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pulumi
 import pulumi_aws as aws
 import pulumi_eks as eks
 
-from paka.config import CloudConfig
+from paka.cluster.context import Context
 
 
 def odic_role_for_sa(
-    config: CloudConfig,
+    ctx: Context,
     cluster: eks.Cluster,
     role_name: str,
     ns_service_account: str,
 ) -> aws.iam.Role:
     """
     Creates an IAM role for a service account in an EKS cluster using OpenID Connect (OIDC) authentication.
 
@@ -19,16 +19,14 @@
         cluster (eks.Cluster): The EKS cluster.
         role_name (str): The name of the role.
         ns_service_account (str): The name of the service account. e.g. "default:sa", "kube-system:auto-scaler"
 
     Returns:
         aws.iam.Role: The IAM role for the service account.
     """
-    project = config.cluster.name
-
     oidc_url = cluster.core.oidc_provider.url
     oidc_arn = cluster.core.oidc_provider.arn
 
     assume_role_policy = pulumi.Output.all(oidc_url, oidc_arn).apply(
         lambda args: aws.iam.get_policy_document(
             statements=[
                 aws.iam.GetPolicyDocumentStatementArgs(
@@ -49,12 +47,12 @@
                     ],
                 )
             ],
         ).json
     )
 
     role = aws.iam.Role(
-        f"{project}-{role_name}-role",
+        f"{ctx.cluster_name}-{role_name}-role",
         assume_role_policy=assume_role_policy,
     )
 
     return role
```

### Comparing `paka-0.1.6/paka/cluster/fluentbit.py` & `paka-0.1.7/paka/cluster/fluentbit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import pulumi
 import pulumi_kubernetes as k8s
 
+from paka.cluster.context import Context
 from paka.constants import ACCESS_ALL_SA
-from paka.utils import call_once, read_current_cluster_data
+from paka.utils import call_once
 
 
 @call_once
-def create_fluentbit(fluent_bit_config: str, k8s_provider: k8s.Provider) -> None:
+def create_fluentbit(ctx: Context, fluent_bit_config: str) -> None:
     """
     Creates a fluentbit daemonset with the given configuration.
     """
 
     parsers_config = """
 [PARSER]
     Name        docker
@@ -18,28 +19,28 @@
     Time_Key    time
     Time_Format %Y-%m-%dT%H:%M:%S.%fZ
 """
     parsers_config_map = k8s.core.v1.ConfigMap(
         "fluent-bit-parsers",
         data={"parsers.conf": parsers_config},
         metadata={
-            "namespace": read_current_cluster_data("namespace"),
+            "namespace": ctx.namespace,
             "name": "fluent-bit-parsers",
         },
-        opts=pulumi.ResourceOptions(provider=k8s_provider),
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider),
     )
 
     fluent_bit_config_map = k8s.core.v1.ConfigMap(
         "fluent-bit-config-map",
         data={"fluent-bit.conf": fluent_bit_config},
         metadata={
-            "namespace": read_current_cluster_data("namespace"),
+            "namespace": ctx.namespace,
             "name": "fluent-bit-config",
         },
-        opts=pulumi.ResourceOptions(provider=k8s_provider),
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider),
     )
 
     k8s.apps.v1.DaemonSet(
         "fluent-bit-daemonset",
         spec=k8s.apps.v1.DaemonSetSpecArgs(
             selector=k8s.meta.v1.LabelSelectorArgs(
                 match_labels={"k8s-app": "fluent-bit-logging"},
@@ -104,10 +105,10 @@
                                 name=parsers_config_map.metadata["name"],
                             ),
                         ),
                     ],
                 ),
             ),
         ),
-        metadata={"namespace": read_current_cluster_data("namespace")},
-        opts=pulumi.ResourceOptions(provider=k8s_provider),
+        metadata={"namespace": ctx.namespace},
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider),
     )
```

### Comparing `paka-0.1.6/paka/cluster/knative.py` & `paka-0.1.7/paka/cluster/knative.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import Any, Callable, Dict
 
 import pulumi
 import pulumi_kubernetes as k8s
 from pulumi import ResourceOptions
 from pulumi_kubernetes.yaml import ConfigFile
 
+from paka.cluster.context import Context
 from paka.cluster.prometheus import create_prometheus
-from paka.config import CloudConfig
 from paka.utils import call_once
 
 VERSION = "v1.12.3"
 ISTIO_VERSION = "v1.12.1"
 
 
 def limit_hpa_min_replicas(args: Any, opts: pulumi.ResourceOptions) -> None:
@@ -71,78 +71,82 @@
 
 only_crd_transform = partial(crd_install_filter, filter=crd_resources)
 non_crd_transform = partial(crd_install_filter, filter=non_crd_resources)
 
 
 # TODO: Decouple knative and istio
 @call_once
-def create_knative_and_istio(config: CloudConfig, k8s_provider: k8s.Provider) -> None:
+def create_knative_and_istio(ctx: Context) -> None:
     ns = k8s.core.v1.Namespace(
         "knative-serving",
         metadata={"name": "knative-serving"},
-        opts=pulumi.ResourceOptions(provider=k8s_provider),
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider),
     )
 
     yaml_files = [
         # TODO: sigstore verification
         # Creates resources under the knative-serving namespace
         f"https://github.com/knative/serving/releases/download/knative-{VERSION}/serving-core.yaml",
     ]
     for i, yaml_file in enumerate(yaml_files):
         ConfigFile(
             yaml_file.split("/")[-1],
             file=yaml_file,
-            opts=pulumi.ResourceOptions(provider=k8s_provider, depends_on=[ns]),
+            opts=pulumi.ResourceOptions(provider=ctx.k8s_provider, depends_on=[ns]),
         )
 
     yaml_file = f"https://github.com/knative/net-istio/releases/download/knative-{ISTIO_VERSION}/istio.yaml"
     istio_crd_install = ConfigFile(
         "istio-crd-install",
         file=yaml_file,
         transformations=[only_crd_transform],
-        opts=pulumi.ResourceOptions(provider=k8s_provider, depends_on=[ns]),
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider, depends_on=[ns]),
     )
 
     istio_full_install = ConfigFile(
         "istio-non-crd-install",
         file=yaml_file,
         transformations=[
             non_crd_transform,
             limit_resources,
             limit_hpa_min_replicas,
             limit_deployment_replicas,
         ],
         opts=pulumi.ResourceOptions(
-            provider=k8s_provider, depends_on=[istio_crd_install, ns]
+            provider=ctx.k8s_provider, depends_on=[istio_crd_install, ns]
         ),
     )
 
     yaml_file = f"https://github.com/knative/net-istio/releases/download/knative-{ISTIO_VERSION}/net-istio.yaml"
     net_istio = ConfigFile(
         "net-istio",
         file=yaml_file,
         opts=pulumi.ResourceOptions(
-            provider=k8s_provider, depends_on=[istio_full_install, ns]
+            provider=ctx.k8s_provider, depends_on=[istio_full_install, ns]
         ),
     )
 
     yaml_file = f"https://github.com/knative/serving/releases/download/knative-{VERSION}/serving-default-domain.yaml"
     ConfigFile(
         "kn-default-domain",
         file=yaml_file,
-        opts=pulumi.ResourceOptions(provider=k8s_provider, depends_on=[net_istio, ns]),
+        opts=pulumi.ResourceOptions(
+            provider=ctx.k8s_provider, depends_on=[net_istio, ns]
+        ),
     )
 
     # Now, install ServiceMonitor and PodMonitor CRDs
-    prometheus = create_prometheus(config, k8s_provider)
+    prometheus = create_prometheus(ctx)
 
     if not prometheus:
         return
 
     yaml_file = "https://raw.githubusercontent.com/knative-extensions/monitoring/main/servicemonitor.yaml"
 
     ConfigFile(
         "kn-prom-monitor",
         file=yaml_file,
         transformations=[exclude_knative_eventing_namespace],
-        opts=pulumi.ResourceOptions(provider=k8s_provider, depends_on=[prometheus, ns]),
+        opts=pulumi.ResourceOptions(
+            provider=ctx.k8s_provider, depends_on=[prometheus, ns]
+        ),
     )
```

### Comparing `paka-0.1.6/paka/cluster/manager/aws.py` & `paka-0.1.7/paka/cluster/manager/aws.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 from paka.cluster.aws.container_registry import create_container_registry
 from paka.cluster.aws.eks import create_k8s_cluster
 from paka.cluster.aws.object_store import create_object_store
 from paka.cluster.manager.base import ClusterManager
 from paka.config import Config
-from paka.utils import save_cluster_data
 
 
 class AWSClusterManager(ClusterManager):
     """
     AWS-specific implementation of the ClusterManager abstract base class.
 
     The AWSClusterManager class is responsible for managing a cluster of AWS resources.
     It provides methods for creating and managing AWS-specific resources such as EKS clusters,
     node groups, and service accounts. It also handles AWS-specific configuration and setup tasks.
     """
 
     def __init__(self, config: Config) -> None:
-        if config.aws is None:
-            raise ValueError("AWS config is required")
         super().__init__(config)
 
     def provision_k8s(self) -> None:
-        # TODO: Hardcoded provider value `aws` should be defined in config
-        save_cluster_data(self.config.cluster.name, "provider", "aws")
-        create_object_store(self.config)
-        create_container_registry(self.config)
-        create_k8s_cluster(self.config)
+        create_object_store(self.ctx)
+        create_container_registry(self.ctx)
+        create_k8s_cluster(self.ctx)
```

### Comparing `paka-0.1.6/paka/cluster/manager/base.py` & `paka-0.1.7/paka/cluster/manager/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,95 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from functools import cached_property
 from typing import Any
 
 from pulumi import automation as auto
 
+from paka.cluster.context import Context
 from paka.cluster.pulumi import ensure_pulumi
 from paka.config import CloudConfig, Config
-from paka.k8s.model_group.service import create_model_group_service
+from paka.constants import PULUMI_STACK_NAME
+from paka.k8s.model_group.service import (
+    cleanup_staled_model_group_services,
+    create_model_group_service,
+)
 from paka.logger import logger
-from paka.utils import read_cluster_data, save_cluster_data
 
 STACK_NAME = "default"
 
 
 class ClusterManager(ABC):
     """
     Abstract base class for a cluster manager.
 
     A ClusterManager is responsible for managing a cluster of compute resources.
 
     Subclasses must implement the abstract methods defined in this class.
     """
 
-    _orig_config: Config
-    config: CloudConfig
+    config: Config
+    cloud_config: CloudConfig
 
     def __init__(self, config: Config) -> None:
-        self._orig_config = config
+        self.config = config
         if not config.aws is None:
-            self.config = config.aws
-        save_cluster_data(
-            self.config.cluster.name, "namespace", self.config.cluster.namespace
-        )
+            self.cloud_config = config.aws
+        self.ctx = Context()
+        self.ctx.set_config(config)
 
     @abstractmethod
     def provision_k8s(self) -> None:
         pass
 
     def _stack_for_program(self, program: auto.PulumiFn) -> auto.Stack:
         return auto.create_or_select_stack(
-            stack_name=STACK_NAME,
-            project_name=self.config.cluster.name,
+            stack_name=PULUMI_STACK_NAME,
+            project_name=self.cloud_config.cluster.name,
             program=program,
         )
 
-    @property
+    @cached_property
     def _stack(self) -> auto.Stack:
         ensure_pulumi()
 
         def program() -> None:
             self.provision_k8s()
 
         return self._stack_for_program(program)
 
     def create(self) -> None:
-        if self._orig_config.aws:
+        if self.config.aws is None:
+            raise ValueError("Only AWS is supported.")
+
+        if self.config.aws:
             self._stack.set_config(
-                "aws:region", auto.ConfigValue(value=self.config.cluster.region)
+                "aws:region", auto.ConfigValue(value=self.cloud_config.cluster.region)
             )
 
-        save_cluster_data(
-            self.config.cluster.name, "region", self.config.cluster.region
-        )
-
         logger.info("Creating resources...")
         self._stack.up(on_output=logger.info)
 
-        if self.config.modelGroups is None:
+        if self.cloud_config.modelGroups is None:
             return
 
-        namespace = read_cluster_data(self.config.cluster.name, "namespace")
+        namespace = self.cloud_config.cluster.namespace
+
+        # Clean up staled model group resources before creating new ones
+        cleanup_staled_model_group_services(
+            namespace, [mg.name for mg in self.config.aws.modelGroups or []]
+        )
 
-        for model_group in self.config.modelGroups:
-            create_model_group_service(namespace, self._orig_config, model_group)
+        for model_group in self.cloud_config.modelGroups:
+            create_model_group_service(self.ctx, namespace, model_group)
 
-    def destroy(self) -> None:
+    def destroy(self) -> Any:
         logger.info("Destroying resources...")
-        self._stack.destroy(on_output=logger.info)
+        return self._stack.destroy(on_output=logger.info)
 
     def refresh(self) -> None:
         logger.info("Refreshing the stack...")
         self._stack.refresh(on_output=logger.info)
 
     def preview(self, *args: Any, **kwargs: Any) -> None:
         if not "on_output" in kwargs:
```

### Comparing `paka-0.1.6/paka/cluster/nvidia_device_plugin.py` & `paka-0.1.7/paka/cluster/nvidia_device_plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import pulumi
 import pulumi_kubernetes as k8s
 
+from paka.cluster.context import Context
+from paka.utils import call_once
 
-def install_nvidia_device_plugin(
-    k8s_provider: k8s.Provider, version: str = "v0.15.0-rc.2"
-) -> None:
+
+@call_once
+def install_nvidia_device_plugin(ctx: Context, version: str = "v0.15.0-rc.2") -> None:
     """
     Installs the NVIDIA device plugin for GPU support in the cluster.
 
     This function deploys the NVIDIA device plugin to the cluster using a DaemonSet.
     The device plugin allows Kubernetes to discover and manage GPU resources on the nodes.
 
     Args:
@@ -79,9 +81,9 @@
                                 path="/var/lib/kubelet/device-plugins",
                             ),
                         )
                     ],
                 ),
             ),
         ),
-        opts=pulumi.ResourceOptions(provider=k8s_provider),
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider),
     )
```

### Comparing `paka-0.1.6/paka/cluster/prometheus.py` & `paka-0.1.7/paka/cluster/prometheus.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,42 +2,41 @@
 
 from typing import Any, Callable, Dict, Optional, Tuple
 
 import pulumi
 import pulumi_kubernetes as k8s
 from pulumi_kubernetes.helm.v3 import Chart, ChartOpts, FetchOpts
 
-from paka.config import CloudConfig
+from paka.cluster.context import Context
 
 
 def memoize(func: Callable[..., Any]) -> Callable[..., Any]:
     cache: Dict[Callable[..., Any], Any] = dict()
 
     def memoized_func(*args: Tuple[Any, ...], **kwargs: Dict[str, Any]) -> Any:
         if func not in cache:
             cache[func] = func(*args, **kwargs)
         return cache[func]
 
     return memoized_func
 
 
 @memoize
-def create_prometheus(
-    config: CloudConfig, k8s_provider: k8s.Provider
-) -> Optional[Chart]:
+def create_prometheus(ctx: Context) -> Optional[Chart]:
     """
     Installs a Prometheus chart.
     """
+    config = ctx.cloud_config
     if not config.prometheus or not config.prometheus.enabled:
         return None
 
     ns = k8s.core.v1.Namespace(
         "prometheus",
         metadata={"name": "prometheus"},
-        opts=pulumi.ResourceOptions(provider=k8s_provider),
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider),
     )
 
     return Chart(
         "kube-prometheus-stack",
         ChartOpts(
             chart="kube-prometheus-stack",
             version="56.3.0",
@@ -110,9 +109,9 @@
                                 }
                             }
                         },
                     }
                 },
             },
         ),
-        opts=pulumi.ResourceOptions(provider=k8s_provider, depends_on=[ns]),
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider, depends_on=[ns]),
     )
```

### Comparing `paka-0.1.6/paka/cluster/pulumi.py` & `paka-0.1.7/paka/cluster/pulumi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import platform
 import shutil
 import tarfile
-import tempfile
 import zipfile
 from pathlib import Path
 
 import requests
 
+from paka.cluster.kubectl import ensure_kubectl
 from paka.logger import logger
-from paka.utils import calculate_sha256, get_project_data_dir
+from paka.utils import calculate_sha256, download_url, get_project_data_dir
 
 # Pin the Pulumi version to avoid breaking changes
 PULUMI_VERSION = "v3.114.0"
 
 
 def change_permissions_recursive(path: Path, mode: int) -> None:
     for child in path.iterdir():
@@ -21,33 +21,35 @@
             child.chmod(mode)
         elif child.is_dir():
             child.chmod(mode)
             change_permissions_recursive(child, mode)
 
 
 def ensure_pulumi() -> None:
+    # Plulumi kubernetes provider requires kubectl to be installed
+    ensure_kubectl()
     paka_home = Path(get_project_data_dir())
 
     bin_dir = paka_home / "bin"
     bin_dir.mkdir(parents=True, exist_ok=True)
 
+    system = platform.system().lower()
+    arch = platform.machine().lower()
+
     current_path = os.environ.get("PATH", "")
 
     pulumi_files = list(bin_dir.glob("pulumi-*"))
     if pulumi_files:
-        os.environ["PATH"] = f"{pulumi_files[0]}:{current_path}"
+        os.environ["PATH"] = f"{pulumi_files[0]}{os.pathsep}{current_path}"
         return
 
     pulumi_version = PULUMI_VERSION
 
     new_pulumi_path = bin_dir / f"pulumi-{pulumi_version}"
 
-    system = platform.system().lower()
-    arch = platform.machine().lower()
-
     if arch in ["amd64", "x86_64"]:
         arch = "x64"
     elif arch == "arm64":
         arch = "arm64"
     else:
         raise Exception(f"Unsupported architecture: {arch}")
 
@@ -69,25 +71,15 @@
         expected_sha256, filename = line.strip().split()
         file_sha256_dict[filename] = expected_sha256
 
     url = f"https://github.com/pulumi/pulumi/releases/download/{pulumi_version}/{pulumi_file}"
 
     logger.info(f"Downloading {pulumi_file}...")
 
-    with tempfile.NamedTemporaryFile() as tf:
-        with requests.get(url, stream=True) as r:
-            r.raise_for_status()
-            for chunk in r.iter_content(chunk_size=8192):
-                tf.write(chunk)
-
-        tf.flush()
-        os.fsync(tf.fileno())
-
-        archive_file = tf.name
-
+    with download_url(url) as archive_file:
         archive_file_sha256 = calculate_sha256(archive_file)
 
         if pulumi_file not in file_sha256_dict:
             raise Exception(f"SHA256 not found for {pulumi_file}")
 
         expected_sha256 = file_sha256_dict[pulumi_file]
 
@@ -113,8 +105,8 @@
         windows_bin_path = pulumi_path / "bin"
         for file in windows_bin_path.iterdir():
             if file.is_file():
                 shutil.move(str(file), str(pulumi_path))
 
     logger.info("Pulumi installed successfully.")
 
-    os.environ["PATH"] = f"{pulumi_path}:{current_path}"
+    os.environ["PATH"] = f"{pulumi_path}{os.pathsep}{current_path}"
```

### Comparing `paka-0.1.6/paka/cluster/qdrant.py` & `paka-0.1.7/paka/cluster/qdrant.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import pulumi
 import pulumi_kubernetes as k8s
 from pulumi_kubernetes.helm.v3 import Chart, ChartOpts, FetchOpts
 
-from paka.config import CloudConfig
+from paka.cluster.context import Context
 from paka.utils import call_once
 
 
 @call_once
-def create_qdrant(
-    config: CloudConfig,
-    k8s_provider: k8s.Provider,
-) -> None:
+def create_qdrant(ctx: Context) -> None:
     """
     Installs the qdrant helm chart.
     """
+    config = ctx.cloud_config
+
     if not config.vectorStore:
         return
 
     ns = k8s.core.v1.Namespace(
         "qdrant",
         metadata={"name": "qdrant", "labels": {"istio-injection": "enabled"}},
-        opts=pulumi.ResourceOptions(provider=k8s_provider),
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider),
     )
 
     resource_request = (
         {
             "resources": {
                 "requests": {
                     "cpu": config.vectorStore.resourceRequest.cpu,
@@ -108,9 +107,9 @@
                         "whenUnsatisfiable": "ScheduleAnyway",
                         "labelSelector": {"matchLabels": {"app": "qdrant"}},
                     }
                 ],
                 **resource_request,
             },
         ),
-        opts=pulumi.ResourceOptions(provider=k8s_provider, depends_on=[ns]),
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider, depends_on=[ns]),
     )
```

### Comparing `paka-0.1.6/paka/cluster/redis.py` & `paka-0.1.7/paka/cluster/redis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 import pulumi
 import pulumi_kubernetes as k8s
 from pulumi_kubernetes.apiextensions import CustomResource
 from pulumi_kubernetes.helm.v3 import Chart, ChartOpts, FetchOpts
 
-from paka.config import CloudConfig
-from paka.utils import call_once, read_current_cluster_data
+from paka.cluster.context import Context
+from paka.utils import call_once
 
 
 @call_once
-def create_redis(config: CloudConfig, k8s_provider: k8s.Provider) -> None:
+def create_redis(ctx: Context) -> None:
     """
     Installs redis with a helm chart.
     """
+    config = ctx.cloud_config
+
     if not config.job or not config.job.enabled:
         return
 
     ns = k8s.core.v1.Namespace(
         "redis",
         metadata={"name": "redis"},
-        opts=pulumi.ResourceOptions(provider=k8s_provider),
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider),
     )
 
     chart = Chart(
         "redis",
         ChartOpts(
             chart="redis",
             version="18.6.1",
-            namespace=read_current_cluster_data("namespace"),
+            namespace=ctx.namespace,
             fetch_opts=FetchOpts(repo="https://charts.bitnami.com/bitnami"),
             values={
                 "architecture": "standalone",
                 "master": {
                     "persistence": {
                         "enabled": True,
                         "size": config.job.broker_storage_size,
                     },
                 },
                 "metrics": {"enabled": True},  # For enabling metrics
             },
         ),
-        opts=pulumi.ResourceOptions(provider=k8s_provider, depends_on=[ns]),
+        opts=pulumi.ResourceOptions(provider=ctx.k8s_provider, depends_on=[ns]),
     )
 
     if not config.prometheus or not config.prometheus.enabled:
         return
 
     CustomResource(
         "redis-metrics-monitor",
@@ -68,11 +70,11 @@
                 {
                     "port": "http-metrics",
                     "interval": "15s",
                 },
             ],
         },
         opts=pulumi.ResourceOptions(
-            provider=k8s_provider,
+            provider=ctx.k8s_provider,
             depends_on=[chart],
         ),
     )
```

### Comparing `paka-0.1.6/paka/config.py` & `paka-0.1.7/paka/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from __future__ import annotations
 
 import re
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, Generic, List, Optional, TypeVar
 
-from pydantic import BaseModel, field_validator, model_validator
+from pydantic import BaseModel, ConfigDict, Field, field_validator, model_validator
 from ruamel.yaml import YAML
 
 from paka.utils import to_yaml
 
+CONFIG_VERSION = "1.0"
+
+
+class PakaBaseModel(BaseModel):
+    model_config = ConfigDict(extra="forbid")
+
 
 def validate_size(v: str, error_message: str = "Invalid size format") -> str:
     """
     Validates the format of the size field.
 
     Args:
         v (str): The value of the size field.
@@ -24,27 +30,22 @@
         ValueError: If the format of the input value is invalid. The error message is specified by the `error_message` parameter.
     """
     if not re.match(r"^\d+(Mi|Gi)$", v):
         raise ValueError(error_message)
     return v
 
 
-class ResourceRequest(BaseModel):
+class ResourceRequest(PakaBaseModel):
     """
     Represents the resource request for a container.
-
-    Attributes:
-        cpu (str): The amount of CPU to request.
-        memory (str): The amount of memory to request.
-        gpu (Optional[int]): The number of GPUs to request. Defaults to None.
     """
 
-    cpu: str
-    memory: str
-    gpu: Optional[int] = None
+    cpu: str = Field(..., description="The amount of CPU to request.")
+    memory: str = Field(..., description="The amount of memory to request.")
+    gpu: Optional[int] = Field(None, description="The number of GPUs to request.")
 
     @field_validator("cpu", mode="before")
     def validate_cpu(cls, v: str) -> str:
         """
         Validates the format of the cpu field.
 
         Args:
@@ -72,15 +73,15 @@
             str: The input value if validation is successful.
 
         Raises:
             ValueError: If the format of the input value is invalid.
         """
         return validate_size(v, "Invalid memory format")
 
-    @field_validator("gpu")
+    @field_validator("gpu", mode="before")
     def validate_gpu(cls, v: Optional[int]) -> Optional[int]:
         """
         Validates the value of the gpu field.
 
         Args:
             v (Optional[int]): The value of the gpu field.
 
@@ -91,116 +92,112 @@
             ValueError: If the value is less than 0.
         """
         if v is not None and v < 0:
             raise ValueError("GPU count cannot be less than 0")
         return v
 
 
-class AwsGpuNode(BaseModel):
+class AwsGpuNodeConfig(PakaBaseModel):
     """
     Represents a configuration for an AWS GPU node.
-
-    Attributes:
-        diskSize (int): The size of the disk for the GPU node in GB.
     """
 
-    diskSize: int
+    enabled: bool = Field(False, description="Whether the GPU node is enabled.")
+
+    # At least 40 GB is required for the disk size
+    diskSize: Optional[int] = Field(
+        40, description="The size of the disk for the GPU node in GB."
+    )
 
 
-class GcpGpuNode(BaseModel):
+class GcpGpuNodeConfig(PakaBaseModel):
     """
     Represents a Google Cloud Platform GPU node.
+    """
 
-    Attributes:
-        imageType (str): The type of image used for the GPU node.
-        acceleratorType (str): The type of accelerator used for the GPU node.
-        acceleratorCount (int): The number of accelerators attached to the GPU node.
-        diskType (str): The type of disk used for the GPU node.
-        diskSize (int): The size of the disk attached to the GPU node in GB.
-    """
-
-    imageType: str
-    acceleratorType: str
-    acceleratorCount: int
-    diskType: str
-    diskSize: int
+    imageType: str = Field(..., description="The type of image used for the GPU node.")
+    acceleratorType: str = Field(
+        ..., description="The type of accelerator used for the GPU node."
+    )
+    acceleratorCount: int = Field(
+        ..., description="The number of accelerators attached to the GPU node."
+    )
+    diskType: str = Field(..., description="The type of disk used for the GPU node.")
+    diskSize: int = Field(
+        ..., description="The size of the disk attached to the GPU node in GB."
+    )
 
 
-class CloudNode(BaseModel):
+class CloudNode(PakaBaseModel):
     """
     Represents a node in the cloud cluster.
+    """
+
+    nodeType: str = Field(..., description="The type of the node.")
+    diskSize: int = Field(
+        20, description="The size of the disk attached to the node in GB."
+    )
+
 
-    Attributes:
-        nodeType (str): The type of the node.
-        diskSize (int): The size of the disk attached to the node in GB.
-        awsGpu (Optional[AwsGpuNode]): The AWS GPU node configuration, if applicable.
-        gcpGpu (Optional[GcpGpuNode]): The GCP GPU node configuration, if applicable.
+class AwsNode(CloudNode):
+    """
+    Represents an AWS cloud node configuration.
     """
 
-    nodeType: str
-    diskSize: int = 20
-    awsGpu: Optional[AwsGpuNode] = None
-    gcpGpu: Optional[GcpGpuNode] = None
+    model_config = ConfigDict(extra="forbid")
 
-    @model_validator(mode="before")
-    def validate_gpu(
-        cls, values: Dict[str, Union[AwsGpuNode, GcpGpuNode]]
-    ) -> Dict[str, Union[AwsGpuNode, GcpGpuNode]]:
-        if values.get("awsGpu") and values.get("gcpGpu"):
-            raise ValueError("At most one of awsGpu or gcpGpu can exist")
-        return values
+    gpu: Optional[AwsGpuNodeConfig] = Field(
+        None, description="The AWS GPU node configuration, if applicable."
+    )
 
 
-class Runtime(BaseModel):
+class Runtime(PakaBaseModel):
     """
     Represents a runtime for a model.
-
-    Attributes:
-        image (str): The Docker image to use for the runtime.
-        command (List[str], optional): The command to run in the Docker container.
     """
 
-    image: str
-    command: Optional[List[str]] = None
+    image: str = Field(..., description="The Docker image to use for the runtime.")
+    command: Optional[List[str]] = Field(
+        None, description="The command to run in the Docker container."
+    )
 
 
-class Model(BaseModel):
+class Model(PakaBaseModel):
     """
     Represents a model.
-
-    Attributes:
-        hfRepoId (str, optional): The HuggingFace repository ID for the model.
-        files (List[str], optional): The list of files to include from the repository. Defaults to all files ("*").
-        useModelStore (bool, optional): Whether to save the model to a model store, such as s3. Defaults to True.
     """
 
-    hfRepoId: Optional[str] = None
-    files: List[str] = ["*"]
+    hfRepoId: Optional[str] = Field(
+        None, description="The HuggingFace repository ID for the model."
+    )
+    files: List[str] = Field(
+        ["*"], description="The list of files to include from the repository."
+    )
+    useModelStore: bool = Field(
+        True, description="Whether to save the model to a model store, such as s3."
+    )
 
-    useModelStore: bool = True
 
-
-class ModelGroup(BaseModel):
+class ModelGroup(PakaBaseModel):
     """
     Represents a group of VMs that serve the inference for a specific type of model.
-
-    Attributes:
-        name (str): The name of the model group.
-        minInstances (int): The minimum number of instances to provision.
-        maxInstances (int): The maximum number of instances to provision.
-        model (Optional[Model]): The model to deploy in the model group. If None, runtime image is responsible for loading the model.
-        runtime (Runtime): The runtime for the model group.
     """
 
-    name: str
-    minInstances: int
-    maxInstances: int
-
-    model: Optional[Model] = None
-    runtime: Runtime
+    name: str = Field(..., description="The name of the model group.")
+    minInstances: int = Field(
+        ..., description="The minimum number of instances to provision."
+    )
+    maxInstances: int = Field(
+        ..., description="The maximum number of instances to provision."
+    )
+    model: Optional[Model] = Field(
+        None,
+        description="The model to deploy in the model group. If None, runtime image is responsible for loading the model.",
+    )
+    runtime: Runtime = Field(..., description="The runtime for the model group.")
 
     @model_validator(mode="before")
     def check_instances_num(cls, values: Dict[str, int]) -> Dict[str, int]:
         min_instances, max_instances = values.get("minInstances"), values.get(
             "maxInstances"
         )
         if min_instances and max_instances and max_instances < min_instances:
@@ -225,40 +222,38 @@
             ValueError: If the value of the input value is invalid.
         """
         if v <= 0:
             raise ValueError("minInstances must be greater than 0")
         return v
 
 
-class Trigger(BaseModel):
-    type: str
-    metadata: Dict[str, str]
+class Trigger(PakaBaseModel):
+    """
+    Represents a trigger.
+    """
+
+    type: str = Field(..., description="The type of the trigger.")
+    metadata: Dict[str, str] = Field(
+        ..., description="The metadata associated with the trigger."
+    )
 
 
 class CloudModelGroup(ModelGroup, CloudNode):
     """
     Represents a group of cloud models.
-
-    This class inherits from both the `ModelGroup` and `CloudNode` classes.
-
-    Attributes:
-        resourceRequest (Optional[ResourceRequest]): The resource request for the model group, specifying the amount of CPU and memory to request.
-
-    Inherited Attributes:
-        name (str): The name of the model group.
-        minInstances (int): The minimum number of instances to provision for the model group.
-        maxInstances (int): The maximum number of instances to provision for the model group.
-        nodeType (str): The type of the node.
     """
 
-    # TODO: make required for HPA to work
-    resourceRequest: Optional[ResourceRequest] = None
-
-    autoScaleTriggers: Optional[List[Trigger]] = None
-    """
+    resourceRequest: ResourceRequest = Field(
+        ...,
+        description="The resource request for the model group, specifying the amount of CPU and memory to request.",
+    )
+
+    autoScaleTriggers: Optional[List[Trigger]] = Field(
+        None,
+        description="""The list of triggers for auto-scaling.
     Triggers for autoscaling the model group. Trigger are not strongly typed, so we use a list of dictionaries to represent them.
     For example:
 
     autoScaleTriggers=[
         # CPU trigger example
         Trigger(
             type="cpu",
@@ -274,62 +269,57 @@
                 "serverAddress": "http://prometheus-operated.default.svc.cluster.local",
                 "metricName": "http_requests_total",
                 "threshold": "100",
                 "query": "sum(rate(http_requests_total{job=\"example-job\"}[2m]))"
             }
         )
     ]
-    """
+    """,
+    )
+
 
+class AwsModelGroup(CloudModelGroup, AwsNode):
+    pass
 
-class ClusterConfig(BaseModel):
+
+class ClusterConfig(PakaBaseModel):
     """
     Represents the configuration for a cluster.
+    """
 
-    Attributes:
-        name (str): The name of the cluster.
-        region (str): The default region for the cluster.
-        namespace (str, optional): The namespace in which the cluster is deployed. Defaults to 'default'.
-        nodeType (str): The type of nodes in the cluster.
-        minNodes (int): The minimum number of nodes in the cluster.
-        maxNodes (int): The maximum number of nodes in the cluster.
-        logRetentionDays (int, optional): The number of days to retain log entries. Defaults to 14.
-    """
-
-    name: str
-    region: str
-
-    namespace: str = "default"
-
-    nodeType: str
-    minNodes: int
-    maxNodes: int
-
-    logRetentionDays: int = 14
+    name: str = Field(..., description="The name of the cluster.")
+    region: str = Field(..., description="The default region for the cluster.")
+    namespace: str = Field(
+        "default", description="The namespace in which the cluster is deployed."
+    )
+    nodeType: str = Field(..., description="The type of nodes in the cluster.")
+    minNodes: int = Field(
+        ..., description="The minimum number of nodes in the cluster."
+    )
+    maxNodes: int = Field(
+        ..., description="The maximum number of nodes in the cluster."
+    )
+    logRetentionDays: int = Field(
+        14, description="The number of days to retain log entries."
+    )
 
 
 class CloudVectorStore(CloudNode):
     """
     Represents a cloud vector store.
-
-    Attributes:
-        replicas (int): The number of replicas for the vector store. Defaults to 1.
-        storage_size (str): The size of the storage of one node for the vector store. Defaults to "10Gi".
-        resourceRequest (Optional[ResourceRequest]): The resource request for the vector store, specifying the amount of CPU and memory to request.
-
-    Inherited Attributes:
-        nodeType (str): The type of the node.
-
-    Methods:
-        validate_storage_size: Validates the format of the storage_size field.
     """
 
-    replicas: int = 1
-    storage_size: str = "10Gi"
-    resourceRequest: Optional[ResourceRequest] = None
+    replicas: int = Field(1, description="The number of replicas for the vector store.")
+    storage_size: str = Field(
+        "10Gi", description="The size of the storage of one node for the vector store."
+    )
+    resourceRequest: Optional[ResourceRequest] = Field(
+        None,
+        description="The resource request for the vector store, specifying the amount of CPU and memory to request.",
+    )
 
     @field_validator("storage_size", mode="before")
     def validate_storage_size(cls, v: str) -> str:
         """
         Validates the format of the storage_size field.
 
         Args:
@@ -358,25 +348,23 @@
             ValueError: If the value of the input value is invalid.
         """
         if v <= 0:
             raise ValueError("replicas must be greater than 0")
         return v
 
 
-class Job(BaseModel):
+class Job(PakaBaseModel):
     """
     Represents a job cluster configuration.
-
-    Attributes:
-        broker_storage_size (str): The size of the storage for the broker. Defaults to "10Gi".
     """
 
-    enabled: bool = False
-
-    broker_storage_size: str = "10Gi"
+    enabled: bool = Field(False, description="Whether the job cluster is enabled.")
+    broker_storage_size: str = Field(
+        "10Gi", description="The size of the storage for the broker."
+    )
 
     @field_validator("broker_storage_size", mode="before")
     def validate_broker_storage_size(cls, v: str) -> str:
         """
         Validates the format of the broker_storage_size field.
 
         Args:
@@ -387,30 +375,51 @@
 
         Raises:
             ValueError: If the format of the input value is invalid.
         """
         return validate_size(v, "Invalid storage size format")
 
 
-class Prometheus(BaseModel):
-    enabled: bool = False
+class Prometheus(PakaBaseModel):
+    """
+    Represents a Prometheus configuration.
+    """
 
-    storage_size: str = "10Gi"
-    grafana: bool = False
-    alertmanager: bool = False
-    kube_api_server: bool = False
-    kubelet: bool = False
-    kube_controller_manager: bool = False
-    core_dns: bool = False
-    kube_etcd: bool = False
-    kube_scheduler: bool = False
-    kube_proxy: bool = False
-    kube_state_metrics: bool = False
-    node_exporter: bool = False
-    thanos_ruler: bool = False
+    enabled: bool = Field(False, description="Whether Prometheus is enabled.")
+    storage_size: str = Field(
+        "10Gi", description="The size of the storage for Prometheus."
+    )
+    grafana: bool = Field(False, description="Whether Grafana is enabled.")
+    alertmanager: bool = Field(False, description="Whether Alertmanager is enabled.")
+    kube_api_server: bool = Field(
+        False, description="Whether the Kubernetes API server is enabled."
+    )
+    kubelet: bool = Field(False, description="Whether the Kubelet is enabled.")
+    kube_controller_manager: bool = Field(
+        False, description="Whether the Kubernetes controller manager is enabled."
+    )
+    core_dns: bool = Field(False, description="Whether CoreDNS is enabled.")
+    kube_etcd: bool = Field(
+        False, description="Whether the Kubernetes etcd is enabled."
+    )
+    kube_scheduler: bool = Field(
+        False, description="Whether the Kubernetes scheduler is enabled."
+    )
+    kube_proxy: bool = Field(
+        False, description="Whether the Kubernetes proxy is enabled."
+    )
+    kube_state_metrics: bool = Field(
+        False, description="Whether the Kubernetes state metrics are enabled."
+    )
+    node_exporter: bool = Field(
+        False, description="Whether the Node Exporter is enabled."
+    )
+    thanos_ruler: bool = Field(
+        False, description="Whether the Thanos Ruler is enabled."
+    )
 
     @field_validator("storage_size", mode="before")
     def validate_storage_size(cls, v: str) -> str:
         """
         Validates the format of the storage_size field.
 
         Args:
@@ -421,96 +430,112 @@
 
         Raises:
             ValueError: If the format of the input value is invalid.
         """
         return validate_size(v, "Invalid storage size format")
 
 
-class Tracing(BaseModel):
-    """Represents the configuration for tracing."""
+class Tracing(PakaBaseModel):
+    """
+    Represents the configuration for tracing.
+    """
 
-    enabled: bool = False
+    enabled: bool = Field(False, description="Whether tracing is enabled.")
+    autoScalingEnabled: bool = Field(
+        False, description="Whether auto-scaling is enabled for tracing."
+    )
+    zipkinHelmSettings: Optional[Dict[str, Any]] = Field(
+        None,
+        description="The settings for the Zipkin Helm chart. See https://github.com/openzipkin/zipkin-helm",
+    )
 
-    autoScalingEnabled: bool = False
 
-    zipkinHelmSettings: Optional[Dict[str, Any]] = None
-    """https://github.com/openzipkin/zipkin-helm"""
+T_CloudModelGroup = TypeVar("T_CloudModelGroup", bound=CloudModelGroup)
 
 
-class CloudConfig(BaseModel):
+class CloudConfig(PakaBaseModel, Generic[T_CloudModelGroup]):
     """
     Represents the configuration for the cloud environment.
+    """
 
-    Attributes:
-        cluster (ClusterConfig): The configuration for the Kubernetes cluster.
-        modelGroups (List[CloudModelGroup], optional): The list of model groups
-            to be deployed in the cloud. If None, no model groups will be deployed. Defaults to None.
-        vectorStore (CloudVectorStore, optional): The configuration
-            for the vector store in the cloud. If None, the vector store will
-            not be provisioned. Defaults to None.
-        job (Job, optional): The configuration for the job broker. If None, the
-            job broker will not be provisioned. Defaults to None.
-        prometheus (Prometheus, optional): The configuration for Prometheus.
-            If None, Prometheus will not be provisioned. Defaults to None.
-    """
-
-    cluster: ClusterConfig
-    modelGroups: Optional[List[CloudModelGroup]] = None
-    vectorStore: Optional[CloudVectorStore] = None
-    job: Optional[Job] = None
-
-    prometheus: Optional[Prometheus] = None
-    tracing: Optional[Tracing] = None
+    cluster: ClusterConfig = Field(
+        ..., description="The configuration for the Kubernetes cluster."
+    )
+    modelGroups: Optional[List[T_CloudModelGroup]] = Field(
+        None,
+        description="The list of model groups to be deployed in the cloud. Default is None. If None, no model groups are deployed.",
+    )
+    vectorStore: Optional[CloudVectorStore] = Field(
+        None,
+        description="The configuration for the vector store in the cloud. Default is None. If None, no vector store is deployed",
+    )
+    job: Optional[Job] = Field(
+        None,
+        description="The configuration for the job broker. Default is None. If None, no job broker is deployed.",
+    )
+    prometheus: Optional[Prometheus] = Field(
+        None,
+        description="The configuration for Prometheus. Default is None. If None, Prometheus is not deployed.",
+    )
+    tracing: Optional[Tracing] = Field(
+        None,
+        description="The configuration for tracing. Default is None. If None, tracing is not enabled.",
+    )
 
     @field_validator("modelGroups", mode="before")
     def check_model_group(cls, v: List[Any]) -> List[Any]:
         if v is None or len(v) == 0:
             return v
         # Check if there are duplicated model group names
         model_group_names = [dict(group)["name"] for group in v]
         if len(set(model_group_names)) != len(model_group_names):
             raise ValueError("Duplicate model group names are not allowed")
         return v
 
 
-class Config(BaseModel):
-    """
-    Configuration class for managing cloud cluster settings.
+class AwsConfig(CloudConfig[AwsModelGroup]):
+    modelGroups: Optional[List[AwsModelGroup]] = Field(
+        None,
+        description="The list of model groups to be deployed in the cloud. Default is None. If None, no model groups are deployed.",
+    )
 
-    Attributes:
-        aws (Optional[CloudConfig]): AWS cloud configuration.
-        gcp (Optional[CloudConfig]): GCP cloud configuration.
 
-    Methods:
-        check_one_field: Validates that exactly one cloud configuration (aws or gcp) is provided.
+class Config(PakaBaseModel):
+    """
+    Configuration class for managing cloud cluster settings.
     """
 
-    aws: Optional[CloudConfig] = None
-    gcp: Optional[CloudConfig] = None
+    version: str = Field(..., description="The version of the configuration.")
+    aws: Optional[AwsConfig] = Field(None, description="The AWS cloud configuration.")
 
     @model_validator(mode="before")
-    def check_one_field(cls, values: Dict[str, CloudConfig]) -> Dict[str, CloudConfig]:
+    def check_one_field(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """
         Validates that exactly one cloud configuration is provided.
 
         Args:
-            values (Dict[str, CloudConfig]): Dictionary of field values, where keys are the cloud providers (aws, gcp) and values are the corresponding cloud configurations.
+            values (Dict[str, Any]): Dictionary of field values for the Config class.
 
         Returns:
-            Dict[str, CloudConfig]: The input values if validation is successful.
+            Dict[str, Any]: The input values if validation is successful.
 
         Raises:
             ValueError: If more or less than one cloud configuration is provided.
         """
-        non_none_fields = sum(value is not None for value in values.values())
-        if non_none_fields != 1:
+        if "aws" not in values:
             raise ValueError("Exactly one cloud configuration must be provided")
 
         return values
 
+    @field_validator("version", mode="before")
+    def validate_version(cls, v: str) -> str:
+        if not re.match(r"^\d+\.\d+$", v):
+            raise ValueError('version must be in the format "x.x"')
+        return v
+
 
 def generate_yaml(config: Config) -> str:
     """
     Generate a YAML string representation of the given config object.
 
     Args:
         config (Config): The config object to generate YAML from.
@@ -529,8 +554,34 @@
         yaml_str (str): The YAML string to parse.
 
     Returns:
         Config: The parsed Config object.
     """
     yaml = YAML()
     data = yaml.load(yaml_str)
+    version = data.get("version", None)
+    if version is None:
+        raise ValueError("Invalid configuration: The 'version' field is missing.")
+
+    if not re.match(r"^\d+\.\d+$", version):
+        raise ValueError('version must be in the format "x.x"')
+
+    # Make sure the major version matches
+    major_version, minor_version = map(int, version.split("."))
+    tool_major_version, tool_minor_version = map(int, CONFIG_VERSION.split("."))
+
+    if major_version < tool_major_version:
+        raise ValueError(
+            f"Invalid configuration: This tool supports versions starting from {tool_major_version}.0."
+            " Please use an older version of the tool if you need to work with a previous configuration version."
+        )
+    elif major_version > tool_major_version:
+        raise ValueError(
+            f"Invalid configuration: Your current tool is too old. Please upgrade your tool to handle this configuration."
+        )
+    elif minor_version > tool_minor_version:  # No forward compatibility
+        raise ValueError(
+            f"Invalid configuration: This tool supports versions up to {tool_major_version}.{tool_minor_version}."
+            " Please upgrade your tool to handle this configuration."
+        )
+
     return Config(**data)
```

### Comparing `paka-0.1.6/paka/container/ecr.py` & `paka-0.1.7/paka/container/ecr.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.6/paka/container/pack.py` & `paka-0.1.7/paka/container/pack.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pathlib import Path
 
 import requests
 
 from paka.logger import logger
 from paka.utils import (
     calculate_sha256,
+    download_url,
     get_gh_release_latest_version,
     get_project_data_dir,
 )
 
 
 def ensure_pack() -> str:
     paka_home = Path(get_project_data_dir())
@@ -55,25 +56,15 @@
     else:
         raise Exception(f"Unsupported architecture: {arch}")
 
     url = f"https://github.com/buildpacks/pack/releases/download/{pack_version}/{pack_file}"
 
     logger.info(f"Downloading {pack_file}...")
 
-    with tempfile.NamedTemporaryFile() as tf:
-        with requests.get(url, stream=True) as r:
-            r.raise_for_status()
-            for chunk in r.iter_content(chunk_size=8192):
-                tf.write(chunk)
-
-        tf.flush()
-        os.fsync(tf.fileno())
-
-        archive_file = tf.name
-
+    with download_url(url) as archive_file:
         archive_file_sha256 = calculate_sha256(archive_file)
 
         # Now, fetch the sha256 file and compare the hash
         sha256_url = f"{url}.sha256"
 
         response = requests.get(sha256_url)
         response.raise_for_status()
@@ -88,18 +79,19 @@
 
         if system == "windows":
             with zipfile.ZipFile(archive_file, "r") as zip_ref:
                 zip_ref.extractall(bin_dir)
         else:
             with tarfile.open(archive_file, "r:gz") as tar:
                 tar.extractall(bin_dir)
-        pack_path = bin_dir / "pack"
 
-        if system == "windows":
-            pack_path = pack_path.with_suffix(".exe")
+    pack_path = bin_dir / "pack"
+
+    if system == "windows":
+        pack_path = pack_path.with_suffix(".exe")
 
-        pack_path.chmod(0o755)
-        pack_path.rename(new_pack_path)
+    pack_path.chmod(0o755)
+    pack_path.rename(new_pack_path)
 
     logger.info("Pack installed successfully.")
 
     return str(new_pack_path)
```

### Comparing `paka-0.1.6/paka/k8s/function/service.py` & `paka-0.1.7/paka/k8s/function/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 import shlex
 from typing import Any, Literal, Tuple
 
 from kubernetes import client
 from kubernetes.dynamic import DynamicClient
 from kubernetes.dynamic.exceptions import NotFoundError
 
-from paka.k8s.utils import try_load_kubeconfig
-
-try_load_kubeconfig()
-
 
 def enable_scale_to_zero(namespace: str = "knative-serving") -> None:
     """
     Enable scale to zero for the knative-serving namespace.
     """
     config_map = client.V1ConfigMap(
         api_version="v1",
```

### Comparing `paka-0.1.6/paka/k8s/job/autoscaler.py` & `paka-0.1.7/paka/k8s/job/autoscaler.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.6/paka/k8s/job/worker.py` & `paka-0.1.7/paka/k8s/job/worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import shlex
 import time
 
 from kubernetes import client
 
 from paka.constants import ACCESS_ALL_SA
 from paka.k8s.job.autoscaler import create_autoscaler, delete_autoscaler
-from paka.k8s.utils import apply_resource, create_namespace, try_load_kubeconfig
+from paka.k8s.utils import apply_resource, create_namespace
 from paka.logger import logger
 
-try_load_kubeconfig()
-
 
 def wait_for_pods_to_drain(namespace: str, deployment_name: str) -> None:
     """
     Waits for all worker pods of a specific deployment in a namespace to drain.
 
     This function continuously checks for the existence of worker pods associated with a specific deployment
     in a given namespace. If any such pods exist, the function waits for 10 seconds before checking again.
```

### Comparing `paka-0.1.6/paka/k8s/model_group/ingress.py` & `paka-0.1.7/paka/k8s/model_group/ingress.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.6/paka/k8s/model_group/runtime/llama_cpp.py` & `paka-0.1.7/paka/k8s/model_group/runtime/llama_cpp.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 import os
 import re
 from typing import List, Optional
 
 from huggingface_hub import HfFileSystem
 from huggingface_hub.utils import validate_repo_id
 
+from paka.cluster.context import Context
+from paka.cluster.utils import get_model_store
 from paka.config import CloudModelGroup
 from paka.constants import MODEL_MOUNT_PATH
-from paka.model.base_model import BaseMLModel
 
 
 # Heuristic to determine if the image is a llama.cpp image
 def is_llama_cpp_image(image: str) -> bool:
     return "llama.cpp" in image.lower()
 
 
 def get_model_file_from_model_store(
+    ctx: Context,
     model_group: CloudModelGroup,
 ) -> Optional[str]:
     if model_group.model and model_group.model.useModelStore:
-        store = BaseMLModel.get_model_store(with_progress_bar=False)
+        store = get_model_store(ctx, with_progress_bar=False)
         # Find the file that ends with .gguf or .ggml
         model_files = [
             file
             for file in store.glob(f"{model_group.name}/*")
             if re.search(r"\.(gguf|ggml)$", file, re.IGNORECASE)
         ]
 
@@ -46,30 +48,32 @@
 
         if len(model_files) == 1:
             return os.path.basename(model_files[0])
 
     return None
 
 
-def get_runtime_command_llama_cpp(model_group: CloudModelGroup) -> List[str]:
+def get_runtime_command_llama_cpp(
+    ctx: Context, model_group: CloudModelGroup
+) -> List[str]:
     runtime = model_group.runtime
     if runtime.command:
         command_str = " ".join(runtime.command) if runtime.command else ""
         # If the command knows where or how to load the model file, we don't need to do anything.
         if (
             re.search(r"(--model|-m)[ \t]*\S+", command_str)
             or (
                 re.search(r"--hf-repo|-hfr", command_str)
                 and re.search(r"--hf-file|-hff", command_str)
             )
             or re.search(r"--model-url|-mu[ \t]*\S+", command_str)
         ):
             return runtime.command
 
-    model_file = get_model_file_from_model_store(model_group)
+    model_file = get_model_file_from_model_store(ctx, model_group)
 
     def attach_model_to_command(command: List[str]) -> List[str]:
         if model_file:
             return command + ["--model", f"{MODEL_MOUNT_PATH}/{model_file}"]
         elif model_group.model and model_group.model.hfRepoId:
 
             validate_repo_id(model_group.model.hfRepoId)
@@ -116,16 +120,18 @@
         "--batch-size",  # Maximum number of tokens to decode in a batch
         "512",
         "--ubatch-size",  # Physical batch size
         "512",
         "--n-predict",  # Maximum number of tokens to predict.
         "-1",
         "--embedding",
+        "--flash-attn",  # Enable flash attention
+        "--metrics",  # Enable metrics
     ]
 
-    if model_group.awsGpu:
+    if hasattr(model_group, "gpu") and model_group.gpu and model_group.gpu.enabled:
         # The value 999 is typically sufficient for most models, as it attempts to offload as many layers as possible to the GPU.
         # However, for particularly large models, this may result in exceeding the GPU's memory capacity and cause errors.
         # A more effective approach would be to conduct a series of experiments with varying values for --n-gpu-layers to find the optimal setting.
         command.extend(["--n-gpu-layers", "999"])
 
     return attach_model_to_command(command)
```

### Comparing `paka-0.1.6/paka/k8s/model_group/service.py` & `paka-0.1.7/paka/k8s/model_group/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,88 @@
 from __future__ import annotations
 
+import json
 from typing import List, Optional, Tuple, cast
 
 from kubernetes import client
+from kubernetes import config as k8s_config
 
-from paka.config import CloudConfig, CloudModelGroup, Config
+from paka.cluster.context import Context
+from paka.cluster.utils import get_model_store
+from paka.config import T_CloudModelGroup
 from paka.constants import ACCESS_ALL_SA, MODEL_MOUNT_PATH
 from paka.k8s.model_group.ingress import create_model_vservice
 from paka.k8s.model_group.runtime.llama_cpp import (
     get_runtime_command_llama_cpp,
     is_llama_cpp_image,
 )
-from paka.k8s.utils import CustomResource, apply_resource, try_load_kubeconfig
+from paka.k8s.model_group.runtime.vllm import get_runtime_command_vllm, is_vllm_image
+from paka.k8s.utils import CustomResource, apply_resource
 from paka.logger import logger
 from paka.model.hf_model import HuggingFaceModel
 from paka.model.store import MODEL_PATH_PREFIX
-from paka.utils import kubify_name, read_cluster_data
+from paka.utils import kubify_name
 
-try_load_kubeconfig()
 
-
-def get_runtime_command(model_group: CloudModelGroup, port: int) -> List[str]:
+def get_runtime_command(
+    ctx: Context, model_group: T_CloudModelGroup, port: int
+) -> List[str]:
     """
     Gets the runtime command for a machine learning model group.
 
     Args:
-        model_group (CloudModelGroup): The model group to get the runtime command for.
+        model_group (T_CloudModelGroup): The model group to get the runtime command for.
 
     Returns:
         List[str]: The runtime command.
     """
     command = []  # Default to the command in images
     runtime = model_group.runtime
     if runtime.command and not is_llama_cpp_image(runtime.image):
         command = runtime.command
 
     # If user did not provide a command, we need to provide a default command with heuristics.
     if is_llama_cpp_image(runtime.image):
-        command = get_runtime_command_llama_cpp(model_group)
-
-        # Add or replace the port in the command
-        for i in range(len(command)):
-            if command[i] == "--port":
-                command[i + 1] = str(port)
-                break
-        else:
-            command.extend(["--port", str(port)])
+        command = get_runtime_command_llama_cpp(ctx, model_group)
+    elif is_vllm_image(runtime.image):
+        command = get_runtime_command_vllm(ctx, model_group)
+
+    # Add or replace the port in the command
+    for i in range(len(command)):
+        if command[i] == "--port":
+            command[i + 1] = str(port)
+            break
+    else:
+        command.extend(["--port", str(port)])
 
     return command
 
 
-def get_health_check_paths(model_group: CloudModelGroup) -> Tuple[str, str]:
+def get_health_check_paths(model_group: T_CloudModelGroup) -> Tuple[str, str]:
     # Return a tuple for ready and live probes
     if is_llama_cpp_image(model_group.runtime.image):
         return ("/health", "/health")
+    elif is_vllm_image(model_group.runtime.image):
+        return ("/health", "/health")
 
     raise ValueError("Unsupported runtime image for health check paths.")
 
 
-def init_aws(config: CloudConfig, model_group: CloudModelGroup) -> client.V1Container:
+def init_aws(ctx: Context, model_group: T_CloudModelGroup) -> client.V1Container:
     """
     Initializes an AWS container for downloading a model from S3.
 
     Args:
         config (CloudConfig): The cloud configuration.
-        model_group (CloudModelGroup): The cloud model group.
+        model_group (T_CloudModelGroup): The cloud model group.
 
     Returns:
         client.V1Container: The initialized AWS container.
     """
-    bucket = read_cluster_data(config.cluster.name, "bucket")
+    bucket = ctx.bucket
 
     return client.V1Container(
         name="init-s3-model-download",
         image="amazon/aws-cli",
         command=[
             "aws",
             "s3",
@@ -88,48 +97,45 @@
                 mount_path=MODEL_MOUNT_PATH,
             )
         ],
     )
 
 
 def create_pod(
+    ctx: Context,
     namespace: str,
-    config: Config,
-    model_group: CloudModelGroup,
+    model_group: T_CloudModelGroup,
     port: int,
 ) -> client.V1Pod:
     """
     Creates a Kubernetes Pod for a machine learning model group.
 
     This function creates a Kubernetes Pod with the specified configuration. The Pod runs a container
     with the specified runtime image and exposes the specified port. The container runs a machine learning
     model from the model group.
 
     Args:
         namespace (str): The namespace to create the Pod in.
         config (Config): The configuration for the Pod.
-        model_group (CloudModelGroup): The model group to run in the Pod.
+        model_group (T_CloudModelGroup): The model group to run in the Pod.
         runtime_image (str): The runtime image for the container.
         port (int): The port to expose on the container.
 
     Raises:
         ValueError: If the AWS configuration is not provided.
 
     Returns:
         client.V1Pod: The created Pod.
     """
-    if config.aws is None:
-        raise ValueError("Only AWS is supported at this time")
-
     ready_probe_path, live_probe_path = get_health_check_paths(model_group)
 
     container_args = {
         "name": f"{kubify_name(model_group.name)}",
         "image": model_group.runtime.image,
-        "command": get_runtime_command(model_group, port),
+        "command": get_runtime_command(ctx, model_group, port),
         "volume_mounts": [
             client.V1VolumeMount(
                 name="model-data",
                 mount_path=MODEL_MOUNT_PATH,
             )
         ],
         "env": [
@@ -167,15 +173,15 @@
         container_args["resources"] = client.V1ResourceRequirements(
             requests={
                 "cpu": model_group.resourceRequest.cpu,
                 "memory": model_group.resourceRequest.memory,
             },
         )
 
-    if model_group.awsGpu:
+    if hasattr(model_group, "gpu") and model_group.gpu and model_group.gpu.enabled:
         if "resources" not in container_args:
             container_args["resources"] = client.V1ResourceRequirements()
         if container_args["resources"].limits is None:
             container_args["resources"].limits = {}
         gpu_count = 1
         if model_group.resourceRequest and model_group.resourceRequest.gpu:
             gpu_count = model_group.resourceRequest.gpu
@@ -197,15 +203,15 @@
                 client.V1Volume(
                     name="model-data",
                     empty_dir=client.V1EmptyDirVolumeSource(),
                 )
             ],
             # Download models from s3 only when s3 is used as a model store
             init_containers=(
-                [init_aws(config.aws, model_group)]
+                [init_aws(ctx, model_group)]
                 if model_group.model and model_group.model.useModelStore
                 else []
             ),
             containers=[client.V1Container(**container_args)],
             tolerations=[
                 client.V1Toleration(
                     key="app",
@@ -252,22 +258,22 @@
                 ),
             ),
         ),
     )
 
 
 def create_deployment(
-    namespace: str, model_group: CloudModelGroup, pod: client.V1Pod
+    namespace: str, model_group: T_CloudModelGroup, pod: client.V1Pod
 ) -> client.V1Deployment:
     """
     Creates a Kubernetes Deployment for a machine learning model group.
 
     Args:
         namespace (str): The namespace to create the Deployment in.
-        model_group (CloudModelGroup): The model group to run in the Deployment.
+        model_group (T_CloudModelGroup): The model group to run in the Deployment.
         pod (client.V1Pod): The Pod to use as a template for the Deployment.
 
     Returns:
         client.V1Deployment: The created Deployment.
     """
     return client.V1Deployment(
         api_version="apps/v1",
@@ -285,15 +291,15 @@
                 }
             ),
             template=pod,
         ),
     )
 
 
-def create_service_monitor(namespace: str, model_group: CloudModelGroup) -> None:
+def create_service_monitor(namespace: str, model_group: T_CloudModelGroup) -> None:
     monitor = CustomResource(
         api_version="monitoring.coreos.com/v1",
         kind="ServiceMonitor",
         plural="servicemonitors",
         metadata=client.V1ObjectMeta(
             name=kubify_name(model_group.name), namespace=namespace
         ),
@@ -309,26 +315,38 @@
                     "port": "http-envoy-prom",
                     "path": "/stats/prometheus",
                     "interval": "15s",
                 },
             ],
         },
     )
+
+    # Both llama-cpp and vllm servers expose metrics on /metrics
+    if is_llama_cpp_image(model_group.runtime.image) or is_vllm_image(
+        model_group.runtime.image
+    ):
+        monitor.spec["endpoints"].append(
+            {
+                "port": "http",
+                "path": "/metrics",
+                "interval": "15s",
+            }
+        )
     apply_resource(monitor)
 
 
 def create_service(
-    namespace: str, model_group: CloudModelGroup, port: int, sidecar_port: int = 15090
+    namespace: str, model_group: T_CloudModelGroup, port: int, sidecar_port: int = 15090
 ) -> client.V1Service:
     """
     Creates a Kubernetes Service for a machine learning model group.
 
     Args:
         namespace (str): The namespace to create the Service in.
-        model_group (CloudModelGroup): The model group to expose with the Service.
+        model_group (T_CloudModelGroup): The model group to expose with the Service.
         port (int): The port to expose on the Service.
         sidecar_port (int): The port on which the istio sidecar is exposing metrics.
 
 
     Returns:
         client.V1Service: The created Service.
     """
@@ -386,28 +404,28 @@
         and service.spec.selector.get("model")
     ]
 
     return filtered_services
 
 
 def create_hpa(
-    namespace: str, model_group: CloudModelGroup, deployment: client.V1Deployment
+    namespace: str, model_group: T_CloudModelGroup, deployment: client.V1Deployment
 ) -> client.V2HorizontalPodAutoscaler:
     """
     Creates a Kubernetes Horizontal Pod Autoscaler (HPA) for a machine learning model group.
 
     This function creates a Kubernetes HPA with the specified namespace, model group, and deployment.
     The HPA automatically scales the number of Pods in the deployment based on the CPU utilization.
 
     The HPA is configured to maintain a specified number of replicas of the Pod.
     The HPA increases the number of replicas when the average CPU utilization exceeds 95%.
 
     Args:
         namespace (str): The namespace to create the HPA in.
-        model_group (CloudModelGroup): The model group to scale with the HPA.
+        model_group (T_CloudModelGroup): The model group to scale with the HPA.
         deployment (client.V1Deployment): The deployment to scale.
 
     Returns:
         client.V2HorizontalPodAutoscaler: The created HPA.
     """
     return client.V2HorizontalPodAutoscaler(
         api_version="autoscaling/v2",
@@ -437,25 +455,25 @@
                 )
             ],
         ),
     )
 
 
 def create_scaled_object(
-    namespace: str, model_group: CloudModelGroup, deployment: client.V1Deployment
+    namespace: str, model_group: T_CloudModelGroup, deployment: client.V1Deployment
 ) -> Optional[CustomResource]:
     """
     Creates a KEDA ScaledObject for a given model group.
 
     This function creates a ScaledObject custom resource for Kubernetes Event-driven Autoscaling (KEDA).
     The ScaledObject is used to scale a Kubernetes Deployment based on the triggers defined in the model group.
 
     Args:
         namespace (str): The namespace in which to create the ScaledObject.
-        model_group (CloudModelGroup): The model group for which to create the ScaledObject.
+        model_group (T_CloudModelGroup): The model group for which to create the ScaledObject.
             This object should have `autoScaleTriggers`, `minInstances`, and `maxInstances` attributes.
         deployment (client.V1Deployment): The Kubernetes Deployment that the ScaledObject should scale.
 
     Returns:
         None
     """
     if not model_group.autoScaleTriggers:
@@ -486,69 +504,70 @@
                 )
             ),
         },
     )
 
 
 def create_model_group_service(
+    ctx: Context,
     namespace: str,
-    config: Config,
-    model_group: CloudModelGroup,
+    model_group: T_CloudModelGroup,
 ) -> None:
     """
     Creates a Kubernetes service for a machine learning model group.
 
     Args:
         namespace (str): The namespace to create the service in.
         config (Config): The configuration for the service.
-        model_group (CloudModelGroup): The model group to create the service for.
+        model_group (T_CloudModelGroup): The model group to create the service for.
 
     Raises:
         ValueError: If the AWS configuration is not provided.
 
     Returns:
         None
     """
-    if config.aws is None:
-        raise ValueError("Only AWS is supported at this time")
+    k8s_config.load_kube_config_from_dict(json.loads(ctx.kubeconfig))
 
+    config = ctx.cloud_config
     # Download the model to S3 first
     if model_group.model and model_group.model.useModelStore:
         if model_group.model.hfRepoId:
             model = HuggingFaceModel(
                 name=model_group.name,
                 repo_id=model_group.model.hfRepoId,
                 files=model_group.model.files,
+                model_store=get_model_store(ctx),
             )
             # If the model is not already in the model store, save it
             # That means users cannot update the model in the model store
             # They have to create a new model group or delete the old one
             if not model.model_store.glob(f"{model_group.name}/*"):
                 model.save()
             else:
                 logger.info(
                     f"Model {model_group.name} already exists in the model store. Skipping download."
                 )
 
     port = 8000
 
     pod = create_pod(
+        ctx,
         namespace,
-        config,
         model_group,
         port,
     )
 
     deployment = create_deployment(namespace, model_group, pod)
     apply_resource(deployment)
 
     svc = create_service(namespace, model_group, port)
     apply_resource(svc)
 
-    if config.aws.prometheus and config.aws.prometheus.enabled:
+    if config.prometheus and config.prometheus.enabled:
         create_service_monitor(namespace, model_group)
 
     scaled_object = create_scaled_object(namespace, model_group, deployment)
     if scaled_object:
         apply_resource(scaled_object)
 
     # Create a vservice to export the model group to the outside world
@@ -624,14 +643,15 @@
 
 
 def cleanup_staled_model_group_services(
     namespace: str, source_of_truth_model_groups: List[str]
 ) -> None:
     services = filter_services(namespace)
     model_groups: List[str] = [
+        # Get the model group name from the service selector
         cast(client.V1ServiceSpec, service.spec).selector.get("model")
         for service in services
     ]
 
     source_of_truth_model_groups_set = set(source_of_truth_model_groups)
 
     for model_group in model_groups:
```

### Comparing `paka-0.1.6/paka/k8s/utils.py` & `paka-0.1.7/paka/k8s/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 import select
 import socket
 import threading
 import time
 from functools import partial
 from typing import Any, Callable, Dict, List, Literal, Optional, Protocol, Tuple
 
-from kubernetes import client, config, watch
+from kubernetes import client, watch
 from kubernetes.client.rest import ApiException
 from kubernetes.stream import portforward
 from ruamel.yaml import YAML
+from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_fixed
 from typing_extensions import TypeAlias
 
 from paka.logger import logger
-from paka.utils import get_project_data_dir, read_yaml_file
+from paka.utils import read_yaml_file
 
 KubernetesResourceKind: TypeAlias = Literal[
     "Deployment",
     "Service",
     "HorizontalPodAutoscaler",
     "ScaledObject",
     "TriggerAuthentication",
@@ -510,24 +511,14 @@
                 wait_duration = max_duration
 
     logger.debug(f"Port forward from local port {local_port} started")
 
     return str(local_port), stop_forward
 
 
-def try_load_kubeconfig() -> bool:
-    try:
-        # read kube config from the file specified by env var KUBECONFIG or the default location ~/.kube/config
-        config.load_kube_config()
-        return True
-    except Exception as e:
-        logger.debug(f"Error loading kubeconfig: {e}")
-        return False
-
-
 class KubeconfigMerger:
     def __init__(self, config: Optional[Dict[str, Any]] = None) -> None:
         self.config = config or {}
 
     def _entries_by_key(self, key: str) -> List[Any]:
         self.config[key] = self.config.get(key) or []
         entries = self.config[key]
@@ -568,24 +559,20 @@
         self.config["current-context"] = new_config["current-context"]
 
         for key in new_config.keys():
             if key not in ["clusters", "users", "contexts", "current-context"]:
                 self.config[key] = new_config[key]
 
 
-def update_kubeconfig() -> None:
+def update_kubeconfig(kubeconfig: Dict[str, Any]) -> None:
     system_kubeconfig_path = os.path.expanduser("~/.kube/config")
     current_config = read_yaml_file(system_kubeconfig_path)
     merger = KubeconfigMerger(current_config)
 
-    cluster_kubeconfig_path = os.path.join(
-        get_project_data_dir(), "current_cluster", "kubeconfig.yaml"
-    )
-    new_config = read_yaml_file(cluster_kubeconfig_path)
-    merger.merge(new_config)
+    merger.merge(kubeconfig)
 
     # Convert OrderedDict to dict and sort keys
     sorted_config = {k: merger.config[k] for k in sorted(merger.config)}
 
     # Dump the sorted config to a YAML-formatted string
     with open(system_kubeconfig_path, "w") as file:
         yaml = YAML()
@@ -614,15 +601,24 @@
         namespace=namespace,
         name=pod_name,
         container=container_name,
     ):
         logger.info(event)
 
 
+@retry(
+    stop=stop_after_attempt(1),
+    wait=wait_fixed(1),
+    retry=retry_if_exception_type(ApiException),
+)
 def remove_crd_finalizers(name: str) -> None:
-    api = client.ApiextensionsV1Api()
-    body = [{"op": "remove", "path": "/metadata/finalizers"}]
-    api.patch_custom_resource_definition(name, body)
-
-
-# Load the kubeconfig when this module is imported
-try_load_kubeconfig()
+    try:
+        api = client.ApiextensionsV1Api()
+        crd = api.read_custom_resource_definition(name)
+        if crd.metadata.finalizers:
+            body = [{"op": "remove", "path": "/metadata/finalizers"}]
+            api.patch_custom_resource_definition(name, body)
+    except ApiException as e:
+        if e.status == 404:
+            pass
+        else:
+            raise
```

### Comparing `paka-0.1.6/paka/logger.py` & `paka-0.1.7/paka/logger.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.6/paka/model/base_model.py` & `paka-0.1.7/paka/model/base_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,56 @@
 from __future__ import annotations
 
 import os
 from abc import ABC, abstractmethod
-from typing import Any, List, Optional, Tuple
+from typing import List, Optional, Tuple
 
 from paka.logger import logger
 from paka.model.manifest import ModelFile, ModelManifest
 from paka.model.settings import ModelSettings
-from paka.model.store import ModelStore, S3ModelStore, StreamLike
-from paka.utils import read_current_cluster_data, to_yaml
+from paka.model.store import ModelStore, StreamLike
+from paka.utils import to_yaml
 
 
 class BaseMLModel(ABC):
     def __init__(
         self,
         name: str,
+        model_store: ModelStore,
         quantization: Optional[str],
         prompt_template_name: Optional[str],
         prompt_template_str: Optional[str],
         # Max concurrency for saving model streams
         concurrency: int = 1,
     ) -> None:
         self.name = name
         self.completed_files: List[Tuple[str, str]] = []
         self.settings = ModelSettings(
             quantization=quantization,
             prompt_template_name=prompt_template_name,
             prompt_template_str=prompt_template_str,
         )
 
-        self.model_store = self.get_model_store()
+        self.model_store = model_store
         self.concurrency = concurrency
 
-    @staticmethod
-    def get_model_store(*args: Any, **kwargs: Any) -> ModelStore:
-        provider = read_current_cluster_data("provider")
-        if provider != "aws":
-            raise ValueError("Only AWS is supported.")
-
-        return S3ModelStore(*args, **kwargs)
-
     def save_manifest_yml(self, manifest: Optional[ModelManifest] = None) -> None:
         if manifest is None:
             manifest = ModelManifest(
                 name=self.name,
                 files=[
                     ModelFile(name=name, sha256=sha256)
                     for (name, sha256) in self.completed_files
                 ],
                 quantization=self.settings.quantization,
                 prompt_template_name=self.settings.prompt_template_name,
                 prompt_template_str=self.settings.prompt_template_str,
             )
 
-        model_store = self.get_model_store(with_progress_bar=False)
+        model_store = self.model_store
 
         manifest_yml = to_yaml(manifest.model_dump(exclude_none=True))
 
         file_path = f"{self.name}/manifest.yml"
         if model_store.file_exists(file_path):
             logger.info(
                 f"manifest.yml file already exists at {file_path}. Overwriting..."
```

### Comparing `paka-0.1.6/paka/model/hf_model.py` & `paka-0.1.7/paka/model/hf_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,31 @@
 from typing import Any, Dict, List, Optional
 
 from huggingface_hub import HfFileSystem
 from huggingface_hub.utils import validate_repo_id
 
 from paka.logger import logger
 from paka.model.base_model import BaseMLModel
+from paka.model.store import ModelStore
 
 
 class HuggingFaceModel(BaseMLModel):
     def __init__(
         self,
         name: str,
         repo_id: str,
         files: List[str],
+        model_store: ModelStore,
         quantization: Optional[str] = None,
         prompt_template_name: Optional[str] = None,
         prompt_template_str: Optional[str] = None,
     ) -> None:
         super().__init__(
             name=name,
+            model_store=model_store,
             quantization=quantization,
             prompt_template_name=prompt_template_name,
             prompt_template_str=prompt_template_str,
         )
         validate_repo_id(repo_id)
         self.repo_id: str = repo_id
         self.fs = HfFileSystem()
```

### Comparing `paka-0.1.6/paka/model/http_model.py` & `paka-0.1.7/paka/model/http_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 
 import concurrent.futures
 from typing import List, Optional
 
 import requests
 
 from paka.model.base_model import BaseMLModel
+from paka.model.store import ModelStore
 
 
 class HttpSourceModel(BaseMLModel):
     def __init__(
         self,
         name: str,
         urls: List[str],
+        model_store: ModelStore,
         quantization: Optional[str] = None,
         prompt_template_name: Optional[str] = None,
         prompt_template_str: Optional[str] = None,
     ) -> None:
         super().__init__(
             name=name,
+            model_store=model_store,
             quantization=quantization,
             prompt_template_name=prompt_template_name,
             prompt_template_str=prompt_template_str,
         )
         self.urls = urls
 
     def save(self) -> None:
```

### Comparing `paka-0.1.6/paka/model/manifest.py` & `paka-0.1.7/paka/model/manifest.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.6/paka/model/progress_bar.py` & `paka-0.1.7/paka/model/progress_bar.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.6/paka/model/settings.py` & `paka-0.1.7/paka/model/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import List, Optional
+from typing import Optional
 
 from pydantic import BaseModel, Field, field_validator
 
 
 class ModelSettings(BaseModel):
     quantization: Optional[str] = Field(
         None, description="The quantization method (GPTQ, AWQ, GGUF_Q4_0, etc) to use."
```

### Comparing `paka-0.1.6/paka/model/store.py` & `paka-0.1.7/paka/model/store.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import requests
 from botocore.client import Config
 from botocore.exceptions import ClientError
 from typing_extensions import TypeAlias
 
 from paka.logger import logger
 from paka.model.progress_bar import NullProgressBar, ProgressBar
-from paka.utils import read_current_cluster_data
 
 MODEL_PATH_PREFIX = "models"
 
 StreamLike: TypeAlias = Union[requests.Response, IOBase]
 
 T = TypeVar("T", bound=Callable[..., Any])
 
@@ -74,20 +73,21 @@
     from an S3 bucket.
     """
 
     progress_bar: Union[ProgressBar, NullProgressBar]
 
     def __init__(
         self,
+        s3_bucket: str,
         s3_chunk_size: int = 8 * 1024 * 1024,
         s3_max_concurrency: int = 20,
         with_progress_bar: bool = True,
     ) -> None:
         # s3 bucket
-        self.s3_bucket = read_current_cluster_data("bucket")
+        self.s3_bucket = s3_bucket
         self.s3_chunk_size = s3_chunk_size
         self.s3_max_concurrency = s3_max_concurrency
         self.s3 = boto3.client("s3", config=Config(signature_version="s3v4"))
         self.with_progress_bar = with_progress_bar
 
         if with_progress_bar:
             self.progress_bar = ProgressBar("Saving model(s) to S3")
```

### Comparing `paka-0.1.6/pyproject.toml` & `paka-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "paka"
-version = "0.1.6"
+version = "0.1.7"
 description = "LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications"
 authors = ["Jijun Leng"]
 readme = "README.md"
 
 [tool.codespell]
 check-filenames = true
 
 [tool.mypy]
 ignore_missing_imports = true
 disallow_untyped_defs = true
 check_untyped_defs = true
 plugins = "pydantic.mypy"
+warn_unused_configs = true
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 filterwarnings = ["ignore::DeprecationWarning"]
 
@@ -37,14 +38,16 @@
 requests = "^2.31.0"
 kubernetes = "^29.0.0"
 boto3 = "^1.34.86"
 tabulate = "^0.9.0"
 huggingface-hub = "^0.22.2"
 tqdm = "^4.66.2"
 typing-extensions = "^4.11.0"
+fasteners = "^0.19"
+tenacity = "^8.2.3"
 
 [tool.poetry.group.dev.dependencies]
 codespell = "^2.2.6"
 mypy = "^1.9.0"
 pre-commit = "3.5.0"
 pytest = "^8.1.1"
 pytest-snapshot = "^0.9.0"
```

### Comparing `paka-0.1.6/PKG-INFO` & `paka-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: paka
-Version: 0.1.6
+Version: 0.1.7
 Summary: LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications
 Author: Jijun Leng
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.86,<2.0.0)
+Requires-Dist: fasteners (>=0.19,<0.20)
 Requires-Dist: huggingface-hub (>=0.22.2,<0.23.0)
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0)
 Requires-Dist: pathspec (>=0.12.1,<0.13.0)
 Requires-Dist: pulumi (==3.105.0)
 Requires-Dist: pulumi-aws (>=6.31.0,<7.0.0)
 Requires-Dist: pulumi-awsx (>=2.7.0,<3.0.0)
 Requires-Dist: pulumi-eks (>=2.3.0,<3.0.0)
 Requires-Dist: pulumi-kubernetes (>=4.8.1,<5.0.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ruamel-yaml (>=0.18.6,<0.19.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Welcome to Paka
 
@@ -102,15 +104,15 @@
           metadata:
             type: Utilization
             value: "50"
 ```
 
 Provision the cluster
 ```bash
-paka cluster up -f cluster.yaml -u
+paka cluster up -f cluster.yaml
 ```
 
 ### Deploy an application
 Change to the application directory and add a `Procfile` and a .cnignore file.
 In `Procfile`, add the command to start the application. For example, for a flask app, it would be `web: gunicorn app:app`. In `.cnignore`, add the files to ignore during build.
 
 To pin the version of the language runtime, add a `runtime.txt` file with the version number. For example, for python, it could be `python-3.11.*`.
@@ -131,13 +133,13 @@
 ## Contributing
 - code changes
 - `make check-all`
 - Open a PR
 
 ## Dependencies
 - docker daemon and CLI
-- credentials for the AWS cloud
+- AWS CLI
 ```bash
-# Ensure your AWS credentials are correctly configured. Execute the command below and verify that the keys `aws_access_key_id` and `aws_secret_access_key` are present.
-cat ~/.aws/credentials
+# Ensure your AWS credentials are correctly configured.
+aws configure
 ```
```

