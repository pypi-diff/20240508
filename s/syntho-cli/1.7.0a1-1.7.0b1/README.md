# Comparing `tmp/syntho-cli-1.7.0a1.tar.gz` & `tmp/syntho-cli-1.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntho-cli-1.7.0a1.tar", last modified: Wed Mar 20 09:30:16 2024, max compression
+gzip compressed data, was "syntho-cli-1.7.0b1.tar", last modified: Wed Mar 20 10:24:33 2024, max compression
```

## Comparing `syntho-cli-1.7.0a1.tar` & `syntho-cli-1.7.0b1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:30:16.092715 syntho-cli-1.7.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-20 09:30:16.092715 syntho-cli-1.7.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:30:16.088714 syntho-cli-1.7.0a1/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18008 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/dc_deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/k8s_deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:30:16.088714 syntho-cli-1.7.0a1/cli/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1369 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/authenticate-syntho-registry.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2602 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/cleanup-docker-compose.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3192 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/cleanup-kubernetes.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2948 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/configuration-questions-dc.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    12997 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/configuration-questions.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    10298 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/create-offline-registry.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      878 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/deauthenticate-syntho-registry.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1183 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/deploy-kubernetes.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    13423 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/deploy-ray-and-syntho-stack-dc.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    16966 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/deploy-ray-and-syntho-stack.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1794 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/download-syntho-charts-release-dc.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1956 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/download-syntho-charts-release.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/get-k8s-cluster-context-name.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     4319 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/k8s-deployment-preparation.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     5685 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/major-pre-deployment-operations.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1176 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/package-offline-registry.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     5268 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/pre-requirements-dc.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     5056 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/pre-requirements-kubernetes.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     7503 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/prepull-images.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     5738 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/utils.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1303 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/scripts/validate-prepull-images-process.sh
--rw-r--r--   0 runner    (1001) docker     (127)    30345 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/syntho_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:30:16.092715 syntho-cli-1.7.0a1/cli/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/utilities/offline_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/utilities/prepull_images.py
--rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-03-20 09:30:13.000000 syntho-cli-1.7.0a1/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 09:30:16.092715 syntho-cli-1.7.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-03-20 09:30:15.000000 syntho-cli-1.7.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:30:16.092715 syntho-cli-1.7.0a1/syntho_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-20 09:30:16.000000 syntho-cli-1.7.0a1/syntho_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-20 09:30:16.000000 syntho-cli-1.7.0a1/syntho_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 09:30:16.000000 syntho-cli-1.7.0a1/syntho_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-20 09:30:16.000000 syntho-cli-1.7.0a1/syntho_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-20 09:30:16.000000 syntho-cli-1.7.0a1/syntho_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-20 09:30:16.000000 syntho-cli-1.7.0a1/syntho_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:24:33.359649 syntho-cli-1.7.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-20 10:24:33.359649 syntho-cli-1.7.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:24:33.355649 syntho-cli-1.7.0b1/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18008 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/dc_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/k8s_deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:24:33.359649 syntho-cli-1.7.0b1/cli/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1369 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/authenticate-syntho-registry.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2602 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/cleanup-docker-compose.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3192 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/cleanup-kubernetes.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2948 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/configuration-questions-dc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12997 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/configuration-questions.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10298 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/create-offline-registry.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      878 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/deauthenticate-syntho-registry.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1183 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/deploy-kubernetes.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13423 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/deploy-ray-and-syntho-stack-dc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16966 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/deploy-ray-and-syntho-stack.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1794 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/download-syntho-charts-release-dc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1956 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/download-syntho-charts-release.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/get-k8s-cluster-context-name.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4319 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/k8s-deployment-preparation.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5685 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/major-pre-deployment-operations.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1176 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/package-offline-registry.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4405 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/pre-requirements-dc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5056 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/pre-requirements-kubernetes.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7503 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/prepull-images.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5738 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/utils.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1303 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/scripts/validate-prepull-images-process.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    30196 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/syntho_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:24:33.359649 syntho-cli-1.7.0b1/cli/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/utilities/offline_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/utilities/prepull_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-03-20 10:24:30.000000 syntho-cli-1.7.0b1/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 10:24:33.359649 syntho-cli-1.7.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-20 10:24:32.000000 syntho-cli-1.7.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:24:33.359649 syntho-cli-1.7.0b1/syntho_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-20 10:24:33.000000 syntho-cli-1.7.0b1/syntho_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-20 10:24:33.000000 syntho-cli-1.7.0b1/syntho_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 10:24:33.000000 syntho-cli-1.7.0b1/syntho_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-20 10:24:33.000000 syntho-cli-1.7.0b1/syntho_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-20 10:24:33.000000 syntho-cli-1.7.0b1/syntho_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-20 10:24:33.000000 syntho-cli-1.7.0b1/syntho_cli.egg-info/top_level.txt
```

### Comparing `syntho-cli-1.7.0a1/LICENSE` & `syntho-cli-1.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/MANIFEST.in` & `syntho-cli-1.7.0b1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/PKG-INFO` & `syntho-cli-1.7.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: syntho-cli
-Version: 1.7.0a1
+Version: 1.7.0b1
 Summary: Syntho Stack Deployment CLI
 Home-page: https://github.com/syntho-ai/syntho-cli
-Download-URL: https://github.com/syntho-ai/syntho-cli/tarball/1.7.0.alpha1
+Download-URL: https://github.com/syntho-ai/syntho-cli/tarball/1.7.0.beta1
 Author: Syntho B.V.
 Author-email: info@syntho.ai
 License: MIT
 Keywords: syntho,synthetic data,deployment
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
```

### Comparing `syntho-cli-1.7.0a1/cli/dc_deployment.py` & `syntho-cli-1.7.0b1/cli/dc_deployment.py`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/k8s_deployment.py` & `syntho-cli-1.7.0b1/cli/k8s_deployment.py`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/authenticate-syntho-registry.sh` & `syntho-cli-1.7.0b1/cli/scripts/authenticate-syntho-registry.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/cleanup-docker-compose.sh` & `syntho-cli-1.7.0b1/cli/scripts/cleanup-docker-compose.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/cleanup-kubernetes.sh` & `syntho-cli-1.7.0b1/cli/scripts/cleanup-kubernetes.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/configuration-questions-dc.sh` & `syntho-cli-1.7.0b1/cli/scripts/configuration-questions-dc.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/configuration-questions.sh` & `syntho-cli-1.7.0b1/cli/scripts/configuration-questions.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/create-offline-registry.sh` & `syntho-cli-1.7.0b1/cli/scripts/create-offline-registry.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/deauthenticate-syntho-registry.sh` & `syntho-cli-1.7.0b1/cli/scripts/deauthenticate-syntho-registry.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/deploy-kubernetes.sh` & `syntho-cli-1.7.0b1/cli/scripts/deploy-kubernetes.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/deploy-ray-and-syntho-stack-dc.sh` & `syntho-cli-1.7.0b1/cli/scripts/deploy-ray-and-syntho-stack-dc.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/deploy-ray-and-syntho-stack.sh` & `syntho-cli-1.7.0b1/cli/scripts/deploy-ray-and-syntho-stack.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/download-syntho-charts-release-dc.sh` & `syntho-cli-1.7.0b1/cli/scripts/download-syntho-charts-release-dc.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/download-syntho-charts-release.sh` & `syntho-cli-1.7.0b1/cli/scripts/download-syntho-charts-release.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/k8s-deployment-preparation.sh` & `syntho-cli-1.7.0b1/cli/scripts/k8s-deployment-preparation.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/major-pre-deployment-operations.sh` & `syntho-cli-1.7.0b1/cli/scripts/major-pre-deployment-operations.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/package-offline-registry.sh` & `syntho-cli-1.7.0b1/cli/scripts/package-offline-registry.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/pre-requirements-dc.sh` & `syntho-cli-1.7.0b1/cli/scripts/pre-requirements-dc.sh`

 * *Files 13% similar despite different names*

```diff
@@ -110,26 +110,16 @@
     fi
 
     if $CHECK_ARCH; then
         VERSION_INFO=$(DOCKER_HOST=$DOCKER_HOST docker version)
         CLIENT_ARCH=$(echo "$VERSION_INFO" | grep "OS/Arch" | awk 'NR==1{print $2}' | awk -F'/' '{print $2}')
         SERVER_ARCH=$(echo "$VERSION_INFO" | grep "OS/Arch" | awk 'NR==2{print $2}' | awk -F'/' '{print $2}')
 
-        if [[ $GIVEN_ARCH != $SERVER_ARCH ]]; then
-            errors+="given --arch parameter isn't consistent with the docker server's architecture($SERVER_ARCH). Supported --arch parameters are amd or arm and eventually both will be converted to amd64 or arm64. No other architectures are supported by the cli.\n"
-        else
-            if [[ $CLIENT_ARCH != $SERVER_ARCH ]]; then
-                if [[ $CLIENT_ARCH != "amd64" && $CLIENT_ARCH != "arm64" ]]; then
-                    errors+="Docker client's architecture($CLIENT_ARCH) isn't compatible: amd64 and arm64 is supported.\n"
-                elif [[ $SERVER_ARCH != "amd64" && $SERVER_ARCH != "arm64" ]]; then
-                    errors+="Docker server's architecture(amd64) isn't compatible: amd64 and arm64 is supported.\n"
-                elif [[ $CLIENT_ARCH == "amd64" && $SERVER_ARCH == "arm64" ]]; then
-                    errors+="Docker client's architecture(amd64) isn't compatible with the docker server's architecture(arm64)\n"
-                fi
-            fi
+        if [[ $CLIENT_ARCH != $SERVER_ARCH ]]; then
+            errors+="Docker client($CLIENT_ARCH) and server($SERVER_ARCH) architecture isn't compatible with each other.\n"
         fi
     fi
 
     if [ -z "$errors" ]; then
         cat << EOF > "$DEPLOYMENT_DIR/.docker-arch.env"
 CLIENT_ARCH=$CLIENT_ARCH
 SERVER_ARCH=$SERVER_ARCH
```

### Comparing `syntho-cli-1.7.0a1/cli/scripts/pre-requirements-kubernetes.sh` & `syntho-cli-1.7.0b1/cli/scripts/pre-requirements-kubernetes.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/prepull-images.sh` & `syntho-cli-1.7.0b1/cli/scripts/prepull-images.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/utils.sh` & `syntho-cli-1.7.0b1/cli/scripts/utils.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/scripts/validate-prepull-images-process.sh` & `syntho-cli-1.7.0b1/cli/scripts/validate-prepull-images-process.sh`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/syntho_cli.py` & `syntho-cli-1.7.0b1/cli/syntho_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -488,21 +488,14 @@
     "--docker-ssh-user-private-key",
     type=str,
     help="Specify a private key for remote docker host access via ssh. Default: null",
     default=None,
     required=False
 )
 @click.option(
-    "--arch",
-    type=str,
-    help=("Specify the architecture. Default: amd"),
-    default="amd",
-    required=False
-)
-@click.option(
     "--version",
     type=str,
     help=("Specify a version for Syntho stack."),
     required=True
 )
 @click.option(
     "--docker-config",
@@ -533,15 +526,14 @@
 )
 def dc_deployment(
     license_key: str,
     registry_user: str,
     registry_pwd: str,
     docker_host: str,
     docker_ssh_user_private_key: str,
-    arch: Optional[str],
     version: Optional[str],
     docker_config: str,
     skip_configuration: bool,
     use_trusted_registry: bool,
     use_offline_registry: bool,
 ):
     try:
@@ -552,15 +544,15 @@
             use_offline_registry,
             trusted_registry_image_pull_secret=None,
             is_k8s=False
         )
     except click.BadParameter as exc:
         raise click.UsageError(str(exc))
 
-    arch = arch.lower()
+    arch = utils.get_architecture()
     if not utils.is_arch_supported(arch):
         raise click.ClickException(
             f"Unsupported architecture: {arch}. Only AMD/ARM is supported."
         )
     arch_text = f"Architecture: {arch}64"
     if arch == "arm":
         arch_text += " - Beta"
```

### Comparing `syntho-cli-1.7.0a1/cli/utilities/offline_ops.py` & `syntho-cli-1.7.0b1/cli/utilities/offline_ops.py`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/utilities/prepull_images.py` & `syntho-cli-1.7.0b1/cli/utilities/prepull_images.py`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/cli/utils.py` & `syntho-cli-1.7.0b1/cli/utils.py`

 * *Files identical despite different names*

### Comparing `syntho-cli-1.7.0a1/setup.py` & `syntho-cli-1.7.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup, find_packages
 
 README = open(os.path.join(os.path.dirname(__file__), "README.md")).read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
-version = "1.7.0.alpha1"
+version = "1.7.0.beta1"
 
 setup(
     name="syntho-cli",
     version=version,
     description="Syntho Stack Deployment CLI",
     long_description=README,
     long_description_content_type='text/markdown',
```

### Comparing `syntho-cli-1.7.0a1/syntho_cli.egg-info/PKG-INFO` & `syntho-cli-1.7.0b1/syntho_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: syntho-cli
-Version: 1.7.0a1
+Version: 1.7.0b1
 Summary: Syntho Stack Deployment CLI
 Home-page: https://github.com/syntho-ai/syntho-cli
-Download-URL: https://github.com/syntho-ai/syntho-cli/tarball/1.7.0.alpha1
+Download-URL: https://github.com/syntho-ai/syntho-cli/tarball/1.7.0.beta1
 Author: Syntho B.V.
 Author-email: info@syntho.ai
 License: MIT
 Keywords: syntho,synthetic data,deployment
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
```

### Comparing `syntho-cli-1.7.0a1/syntho_cli.egg-info/SOURCES.txt` & `syntho-cli-1.7.0b1/syntho_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

