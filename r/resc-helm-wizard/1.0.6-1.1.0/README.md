# Comparing `tmp/resc_helm_wizard-1.0.6.tar.gz` & `tmp/resc_helm_wizard-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_helm_wizard-1.0.6.tar", last modified: Fri Jul  7 10:58:25 2023, max compression
+gzip compressed data, was "resc_helm_wizard-1.1.0.tar", last modified: Wed May  8 13:51:10 2024, max compression
```

## Comparing `resc_helm_wizard-1.0.6.tar` & `resc_helm_wizard-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:58:25.404952 resc_helm_wizard-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-07 10:58:25.404952 resc_helm_wizard-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-07 10:58:25.404952 resc_helm_wizard-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:58:25.400952 resc_helm_wizard-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:58:25.404952 resc_helm_wizard-1.0.6/src/resc_helm_wizard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:58:25.404952 resc_helm_wizard-1.0.6/src/resc_helm_wizard/config/
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/config/example-values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/helm_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/helm_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/kubernetes_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/questions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/run_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-07 10:58:18.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:58:25.404952 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-07 10:58:25.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-07 10:58:25.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:58:25.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 10:58:25.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:58:25.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 10:58:25.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-07 10:58:25.000000 resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:51:10.443813 resc_helm_wizard-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-08 13:51:10.443813 resc_helm_wizard-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-08 13:51:10.443813 resc_helm_wizard-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:51:10.439813 resc_helm_wizard-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:51:10.443813 resc_helm_wizard-1.1.0/src/resc_helm_wizard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14797 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:51:10.443813 resc_helm_wizard-1.1.0/src/resc_helm_wizard/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard/config/example-values.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard/helm_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      970 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard/helm_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard/kubernetes_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard/questions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1910 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard/run_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-08 13:51:06.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:51:10.443813 resc_helm_wizard-1.1.0/src/resc_helm_wizard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-08 13:51:10.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-08 13:51:10.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:51:10.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 13:51:10.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:51:10.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 13:51:10.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 13:51:10.000000 resc_helm_wizard-1.1.0/src/resc_helm_wizard.egg-info/top_level.txt
```

### Comparing `resc_helm_wizard-1.0.6/PKG-INFO` & `resc_helm_wizard-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,10 @@
-Metadata-Version: 2.1
-Name: resc_helm_wizard
-Version: 1.0.6
-Summary: Repository Scanner - Helm Wizard
-Home-page: https://github.com/ABNAMRO/repository-scanner
-Author: ABN AMRO
-Author-email: resc@nl.abnamro.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # Repository Scanner Helm Wizard (resc-helm-wizard)
+[![Python][python-shield]][python-url]
+[![CI][ci-shield]][ci-url]
 
 <!-- TABLE OF CONTENTS -->
 ## Table of contents
 1. [About the component](#about-the-component)
 2. [Getting started](#getting-started)
     - [Prerequisites](#prerequisites)
     - [Usage](#usage)
@@ -30,15 +21,15 @@
 <!-- GETTING STARTED -->
 ## Getting started
 
 These instructions will help you to get a copy of the project up and running on your local machine for development and testing purposes.
 
 ### Prerequisites
 - [Git](https://git-scm.com/downloads)
-- [Python (v3.9.0 or higher)](https://www.python.org/downloads/release/python-390/)
+- [Python (v3.12.0 or higher)](https://www.python.org/downloads/release/python-3120/)
 - [Docker Desktop](https://www.docker.com/products/docker-desktop/)
 - [Kubernetes](https://kubernetes.io/)
 - [Helm](https://helm.sh/)
 
 ### Usage
 Install the package:
 ```bash
@@ -87,16 +78,20 @@
 [(Back to top)](#table-of-contents)
 
 ### Run unit tests, linting and import checks locally:
 See below commands for running various (unit/linting) tests locally. To run these tests you need to install [tox](https://pypi.org/project/tox/). This can be done on Linux and Windows with Git Bash.
 
 Run below commands to make sure that the unit tests are running and that the code matches quality standards:
 ```bash
-pip install tox      # install tox locally
+pip install tox         # install tox locally
 
-tox -v -e sort       # Run this command to validate the import sorting
-tox -v -e lint       # Run this command to lint the code according to this repository's standard
-tox -v -e pytest     # Run this command to run the unit tests
-tox -v               # Run this command to run all of the above tests
+tox run -e py -v        # Run this command to run the unit tests
+tox run -e isort -v     # Run this command to validate the import sorting
+tox run -e pylint -v    # Run this command for Python static code analysis
+tox run -e flake8 -v    # Run this command for Python linting
 ```
 
-
+<!-- MARKDOWN LINKS & IMAGES -->
+[python-shield]: https://img.shields.io/badge/Python-3670A0?style=flat&logo=python&logoColor=ffdd54
+[python-url]: https://www.python.org
+[ci-shield]: https://img.shields.io/github/actions/workflow/status/abnamro/repository-scanner/helm-wizard-ci.yaml?style=flat&logo=github
+[ci-url]: https://github.com/abnamro/repository-scanner/actions/workflows/helm-wizard-ci.yaml
```

### Comparing `resc_helm_wizard-1.0.6/setup.cfg` & `resc_helm_wizard-1.1.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [metadata]
 name = resc_helm_wizard
 description = Repository Scanner - Helm Wizard
-version = 1.0.6
+version = 1.1.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
+license_files = LICENSE.md
+requirements_files = file: requirements.txt
 
 [options]
-requires_python = >=3.9
+python_requires = >=3.12
 include_package_data = True
 zip_safe = False
 package_dir = = src
 packages = find:
 
 [options.packages.find]
 where = src
```

### Comparing `resc_helm_wizard-1.0.6/src/resc_helm_wizard/common.py` & `resc_helm_wizard-1.1.0/src/resc_helm_wizard/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # First Party
 from resc_helm_wizard import constants, questions
 from resc_helm_wizard.helm_utilities import (
     add_helm_repository,
     check_helm_release_exists,
     install_or_upgrade_helm_release,
     update_helm_repository,
-    validate_helm_deployment_status
+    validate_helm_deployment_status,
 )
 from resc_helm_wizard.helm_value import HelmValue
 from resc_helm_wizard.kubernetes_utilities import create_namespace_if_not_exists
 from resc_helm_wizard.vcs_instance import VcsInstance
 
 logging.basicConfig(level=logging.INFO)
 
@@ -48,44 +48,76 @@
         operating system
     :return: dict
         Returns dictionary containing database storage and rabbitmq storage path
     """
     local_storage = questions.ask_local_storage_path()
 
     if os.path.exists(local_storage):
-        db_storage_path = generate_pvc_path(operating_system=operating_system, path=local_storage, tool_type="database",
-                                            create_dir=True)
-        rabbitmq_storage_path = generate_pvc_path(operating_system=operating_system, path=local_storage,
-                                                  tool_type="rabbitmq", create_dir=True)
+        db_storage_path = generate_pvc_path(
+            operating_system=operating_system,
+            path=local_storage,
+            tool_type="database",
+            create_dir=True,
+        )
+        rabbitmq_storage_path = generate_pvc_path(
+            operating_system=operating_system,
+            path=local_storage,
+            tool_type="rabbitmq",
+            create_dir=True,
+        )
     else:
         dir_confirm_msg = f"Do you want to create the directory {local_storage}?"
         dir_confirm = questions.ask_user_confirmation(msg=dir_confirm_msg)
         if dir_confirm is True:
-            db_storage_path = generate_pvc_path(operating_system=operating_system, path=local_storage,
-                                                tool_type="database", create_dir=True)
-            rabbitmq_storage_path = generate_pvc_path(operating_system=operating_system, path=local_storage,
-                                                      tool_type="rabbitmq", create_dir=True)
+            db_storage_path = generate_pvc_path(
+                operating_system=operating_system,
+                path=local_storage,
+                tool_type="database",
+                create_dir=True,
+            )
+            rabbitmq_storage_path = generate_pvc_path(
+                operating_system=operating_system,
+                path=local_storage,
+                tool_type="rabbitmq",
+                create_dir=True,
+            )
         else:
             logging.warning(
                 "Warning! Please ensure the provided directory exists on the system where you are running the "
-                "deployment")
-            proceed_confirm = questions.ask_user_confirmation(msg="Are you sure you want to proceed?")
+                "deployment"
+            )
+            proceed_confirm = questions.ask_user_confirmation(
+                msg="Are you sure you want to proceed?"
+            )
             if proceed_confirm is True:
-                db_storage_path = generate_pvc_path(operating_system=operating_system, path=local_storage,
-                                                    tool_type="database", create_dir=False)
-                rabbitmq_storage_path = generate_pvc_path(operating_system=operating_system, path=local_storage,
-                                                          tool_type="rabbitmq", create_dir=False)
+                db_storage_path = generate_pvc_path(
+                    operating_system=operating_system,
+                    path=local_storage,
+                    tool_type="database",
+                    create_dir=False,
+                )
+                rabbitmq_storage_path = generate_pvc_path(
+                    operating_system=operating_system,
+                    path=local_storage,
+                    tool_type="rabbitmq",
+                    create_dir=False,
+                )
             else:
                 logging.info("Aborting the program!!")
                 sys.exit(1)
-    storage_path = {"db_storage_path": db_storage_path, "rabbitmq_storage_path": rabbitmq_storage_path}
+    storage_path = {
+        "db_storage_path": db_storage_path,
+        "rabbitmq_storage_path": rabbitmq_storage_path,
+    }
     return storage_path
 
 
-def generate_pvc_path(operating_system: str, path: str, tool_type: str, create_dir: bool) -> str:
+def generate_pvc_path(
+    operating_system: str, path: str, tool_type: str, create_dir: bool
+) -> str:
     """
         Generates volume claim path for database and rabbitmq
     :param operating_system:
         operating system
     :param path:
         path provided by user
     :param tool_type:
@@ -100,20 +132,22 @@
     if tool_type == "rabbitmq":
         path = os.path.join(path, "resc-rabbitmq-storage")
     if create_dir:
         if not os.path.exists(path):
             os.makedirs(path)
             logging.info(f"Storage created for {tool_type} at {path}")
         else:
-            logging.info(f"Path already exists. Going to use {path} for {tool_type} storage")
+            logging.info(
+                f"Path already exists. Going to use {path} for {tool_type} storage"
+            )
 
     if operating_system == "windows":
-        pvc_path = path.replace(path.split(':')[0], path.split(':')[0].lower())
-        pvc_path = pvc_path.replace('\\', '/')
-        pvc_path = pvc_path.replace(':', '')
+        pvc_path = path.replace(path.split(":")[0], path.split(":")[0].lower())
+        pvc_path = pvc_path.replace("\\", "/")
+        pvc_path = pvc_path.replace(":", "")
         pvc_path = f"/run/desktop/mnt/host/{pvc_path}"
     else:
         pvc_path = path
     return pvc_path
 
 
 def prepare_vcs_instances_for_helm_values(helm_values: HelmValue) -> List[VcsInstance]:
@@ -131,70 +165,105 @@
             token = "GITHUB_PUBLIC_TOKEN"
         if vcs.provider_type == "AZURE_DEVOPS":
             user_name = "AZURE_DEVOPS_USERNAME"
             token = "AZURE_DEVOPS_TOKEN"
         if vcs.provider_type == "BITBUCKET":
             user_name = "BITBUCKET_USERNAME"
             token = "BITBUCKET_TOKEN"
-        vcs_instance_obj = {"name": vcs.provider_type, "scope": vcs.scope, "exceptions": [],
-                            "providerType": vcs.provider_type, "hostname": vcs.host, "port": vcs.port,
-                            "scheme": vcs.scheme, "username": user_name, "usernameValue": vcs.username,
-                            "organization": vcs.organization, "token": token, "tokenValue": vcs.password}
+        vcs_instance_obj = {
+            "name": vcs.provider_type,
+            "scope": vcs.scope,
+            "exceptions": [],
+            "providerType": vcs.provider_type,
+            "hostname": vcs.host,
+            "port": vcs.port,
+            "scheme": vcs.scheme,
+            "username": user_name,
+            "usernameValue": vcs.username,
+            "organization": vcs.organization,
+            "token": token,
+            "tokenValue": vcs.password,
+        }
         vcs_instances.append(vcs_instance_obj)
     return vcs_instances
 
 
-def create_helm_values_yaml(helm_values: HelmValue, input_values_yaml_file: str) -> bool:
+def create_helm_values_yaml(
+    helm_values: HelmValue, input_values_yaml_file: str
+) -> bool:
     """
         Generates values yaml file for helm deployment of resc
     :param helm_values:
         object of HelmValue
     :param input_values_yaml_file:
         input values.yaml_file path
     :return: bool
         Returns True if file created else returns false
     :raises FileNotFoundError: if example-values.yaml file was not found
     :raises KeyError: if any expected key was not found in the values dictionary
     """
     output_file_generated = False
     output_values_yaml_file = constants.VALUES_FILE
-    helm_deployment_help_link = "https://github.com/abnamro/repository-scanner/" \
-                                "blob/main/deployment/kubernetes/README.md"
+    helm_deployment_help_link = (
+        "https://github.com/abnamro/repository-scanner/"
+        "blob/main/deployment/kubernetes/README.md"
+    )
 
     try:
         values_dict = read_yaml_file(input_values_yaml_file)
 
         values_dict["resc-database"]["hostOS"] = helm_values.operating_system
-        values_dict["resc-database"]["database"]["pvc_path"] = helm_values.db_storage_path
+        values_dict["resc-database"]["database"]["pvc_path"] = (
+            helm_values.db_storage_path
+        )
 
         values_dict["resc-rabbitmq"]["filemountType"] = helm_values.operating_system
-        values_dict["resc-rabbitmq"]["rabbitMQ"]["pvc_path"] = helm_values.rabbitmq_storage_path
-
-        values_dict["resc-database"]["database"]["config"]["password"] = helm_values.db_password
-        values_dict["resc-database-init"]["resc"]["config"]["dbPass"] = helm_values.db_password
-        values_dict["resc-web-service"]["resc"]["config"]["dbPass"] = helm_values.db_password
-        values_dict["resc-web-service-no-auth"]["resc"]["config"]["dbPass"] = helm_values.db_password
-
-        values_dict["resc-vcs-instances"]["vcsInstances"] = prepare_vcs_instances_for_helm_values(
-            helm_values=helm_values)
+        values_dict["resc-rabbitmq"]["rabbitMQ"]["pvc_path"] = (
+            helm_values.rabbitmq_storage_path
+        )
+
+        values_dict["resc-database"]["database"]["config"]["password"] = (
+            helm_values.db_password
+        )
+        values_dict["resc-database-init"]["resc"]["config"]["dbPass"] = (
+            helm_values.db_password
+        )
+        values_dict["resc-web-service"]["resc"]["config"]["dbPass"] = (
+            helm_values.db_password
+        )
+        values_dict["resc-web-service-no-auth"]["resc"]["config"]["dbPass"] = (
+            helm_values.db_password
+        )
+
+        values_dict["resc-vcs-instances"]["vcsInstances"] = (
+            prepare_vcs_instances_for_helm_values(helm_values=helm_values)
+        )
 
         with open(output_values_yaml_file, "w", encoding="utf-8") as file_out:
             yaml.dump(values_dict, file_out)
         output_values_yaml_file_path = os.path.abspath(output_values_yaml_file)
         if os.path.exists(output_values_yaml_file_path):
-            logging.info(f"Helm values yaml file has been successfully generated at {output_values_yaml_file_path}")
-            logging.info(f"You can proceed with deployment or you can refer to this link "
-                         f"to make any customizations in helm values yaml file: {helm_deployment_help_link}")
+            logging.info(
+                f"Helm values yaml file has been successfully generated at {output_values_yaml_file_path}"
+            )
+            logging.info(
+                f"You can proceed with deployment or you can refer to this link "
+                f"to make any customizations in helm values yaml file: {helm_deployment_help_link}"
+            )
             output_file_generated = True
 
     except FileNotFoundError:
-        logging.error(f"Aborting the program! {input_values_yaml_file} file was not found")
+        logging.error(
+            f"Aborting the program! {input_values_yaml_file} file was not found"
+        )
         sys.exit(1)
     except KeyError as error:
-        logging.error(f"Aborting the program! {error} was missing in {input_values_yaml_file}")
+        logging.error(
+            f"Aborting the program! {error} was missing in {input_values_yaml_file}"
+        )
         sys.exit(1)
     return output_file_generated
 
 
 def read_yaml_file(file_path):
     """
         Read content of yaml file
@@ -238,49 +307,54 @@
 
     vcs_instances: List[VcsInstance] = []
 
     for vcs in vcs_instance_answers:
         vcs_instance_info = questions.ask_vcs_instance_details(vcs_type=vcs)
         scheme, host, port = get_scheme_host_port_from_url(vcs_instance_info["url"])
         if vcs == "GitHub":
-            default_github_accounts = f"{vcs_instance_info['username']}, kubernetes, docker"
+            default_github_accounts = (
+                f"{vcs_instance_info['username']}, kubernetes, docker"
+            )
             github_accounts = questions.ask_which_github_accounts_to_scan(
-                default_github_accounts=default_github_accounts)
-            github_account_list = [account.strip() for account in github_accounts.split(",")]
+                default_github_accounts=default_github_accounts
+            )
+            github_account_list = [
+                account.strip() for account in github_accounts.split(",")
+            ]
             vcs_instance = VcsInstance(
                 provider_type="GITHUB_PUBLIC",
                 scheme=scheme,
                 host=host,
                 port=port,
                 username=vcs_instance_info["username"],
                 password=vcs_instance_info["token"],
                 organization=vcs_instance_info["organization"],
-                scope=github_account_list
+                scope=github_account_list,
             )
         if vcs == "Azure Devops":
             vcs_instance = VcsInstance(
                 provider_type="AZURE_DEVOPS",
                 scheme=scheme,
                 host=host,
                 port=port,
                 username=vcs_instance_info["username"],
                 password=vcs_instance_info["token"],
                 organization=vcs_instance_info["organization"],
-                scope=[]
+                scope=[],
             )
         if vcs == "Bitbucket":
             vcs_instance = VcsInstance(
                 provider_type="BITBUCKET",
                 scheme=scheme,
                 host=host,
                 port=port,
                 username=vcs_instance_info["username"],
                 password=vcs_instance_info["token"],
                 organization=vcs_instance_info["organization"],
-                scope=[]
+                scope=[],
             )
         vcs_instances.append(vcs_instance)
     return vcs_instances
 
 
 def download_rule_toml_file(url: str, file: str) -> bool:
     """
@@ -289,61 +363,73 @@
         url of the file to download
     :param file:
         path of the downloaded file
     :return: bool
         Returns true if rule downloaded successfully else returns false
     """
     downloaded = False
-    verify_ssl = questions.ask_ssl_verification(msg="Do you want to verify SSL certificates for HTTPS requests?")
+    verify_ssl = questions.ask_ssl_verification(
+        msg="Do you want to verify SSL certificates for HTTPS requests?"
+    )
     response = requests.get(url, timeout=100, verify=verify_ssl)
     with open(file, "wb") as output:
         output.write(response.content)
     if os.path.exists(file) and os.path.getsize(file) > 0:
         downloaded = True
         logging.debug(f"{file} successfully downloaded")
     else:
         logging.error("Unable to download the rule file")
     return downloaded
 
 
 def run_deployment_as_per_user_confirmation():
     """
-        Run deployment as per user confirmation
+    Run deployment as per user confirmation
     """
     run_deployment_confirm_msg = "Do you want to run deployment?"
-    run_deployment_confirm = questions.ask_user_confirmation(msg=run_deployment_confirm_msg)
+    run_deployment_confirm = questions.ask_user_confirmation(
+        msg=run_deployment_confirm_msg
+    )
     if run_deployment_confirm is True:
         run_deployment()
     else:
         logging.info("Skipping deployment...")
 
 
 def run_deployment():
     """
         Runs a helm deployment
     :return: bool
         Returns true if deployment successful else returns false
     """
     deployment_status = False
 
-    rule_file_downloaded = download_rule_toml_file(url=constants.RULE_FILE_URL, file=constants.RULE_FILE)
+    rule_file_downloaded = download_rule_toml_file(
+        url=constants.RULE_FILE_URL, file=constants.RULE_FILE
+    )
 
     add_helm_repository()
     update_helm_repository()
 
     if rule_file_downloaded:
-        namespace_created = create_namespace_if_not_exists(namespace_name=constants.NAMESPACE)
+        namespace_created = create_namespace_if_not_exists(
+            namespace_name=constants.NAMESPACE
+        )
 
     if namespace_created:
         # Check if release already exists
         helm_release_exists = check_helm_release_exists()
         if helm_release_exists:
-            run_upgrade_confirm_msg = f"Release {constants.RELEASE_NAME} is already installed in " \
-                                      f"{constants.NAMESPACE} namespace. Do you want to upgrade the release?"
-            run_upgrade_confirm = questions.ask_user_confirmation(msg=run_upgrade_confirm_msg)
+            run_upgrade_confirm_msg = (
+                f"Release {constants.RELEASE_NAME} is already installed in "
+                f"{constants.NAMESPACE} namespace. Do you want to upgrade the release?"
+            )
+            run_upgrade_confirm = questions.ask_user_confirmation(
+                msg=run_upgrade_confirm_msg
+            )
             if run_upgrade_confirm is True:
                 deployment_status = install_or_upgrade_helm_release(action="upgrade")
                 validate_helm_deployment_status()
             else:
                 logging.info("Skipping deployment...")
 
         else:
```

### Comparing `resc_helm_wizard-1.0.6/src/resc_helm_wizard/config/example-values.yaml` & `resc_helm_wizard-1.1.0/src/resc_helm_wizard/config/example-values.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 global:
   # Authentication is disabled by default, to enable it set authenticationEnabled to true and provide correct values for ssoConfig attributes
   rulePackVersion: "1.0.0" # Default rule pack version set to 1.0.0, increment the version for any rule pack change
   authenticationEnabled: "false"
   enableInClusterRabbitMqMgmt: "true"
+  enableInClusterRedis: "true"
+  enableRedisCache: "true"
   resc:
     image:
       repository: rescabnamro/
       name: resc-backend
       tag: latest
   rescFrontend:
     image:
@@ -59,29 +61,36 @@
   exposeToHostPort: 30800
   resc:
     config:
       dbConnectionString: "mssql+pyodbc://{MSSQL_USERNAME}:{MSSQL_PASSWORD}@{MSSQL_DB_HOST}:{MSSQL_DB_PORT}/{MSSQL_SCHEMA}?driver={MSSQL_ODBC_DRIVER}&Encrypt=yes&TrustServerCertificate=yes"
       dbSchema: "master" # <enter database schema name here, default to master>
       dbUser: "sa" # <enter database username here, default to sa>
       dbPass: "Y0urStr0ngPassword" # <enter database password here, default to Y0urStr0ngPassword>
+      redisPass: "Y0urStr0ngPassword" # <enter Redis password here for caching, default to Y0urStr0ngPassword>
     # To configure single sign on provide below values for ssoConfig attributes
     # These attributes will be used in the RESC API to validate access token
     ssoConfig:
       ssoAccessTokenIssuerUrl: "<enter Access token issuer url here>" # optional
       ssoAccessTokenJwksUrl: "<enter Access token JWKS url here>" # optional
+      ssoJwtSignAlgorithm: "<enter Access token sign algorithm>" # optional
+      ssoJwtRequiredClaims: "<enter Access token required claims as comma separated string>" # optional
+      soJwtClaimKeyUserId: "<enter Access token claim key used for the user id>" # optional
+      ssoJwtClaimKeyAuthorization: "<enter Access token claim key used for the authorization>" # optional
+      ssoJwtClaimValueAuthorization: "<enter Access token claim value to look for in the key for authorization>" # optional
     corsAllowedDomains: "http://localhost:8080, http://localhost:30000"
     authRequired: "false"
 
 resc-web-service-no-auth:
   exposeToHostPort: 30900
   resc:
     config:
       dbSchema: "master" # <enter database schema name here, default to master>
       dbUser: "sa" # <enter database username here, default to sa>
       dbPass: "Y0urStr0ngPassword" # <enter database password here, default to Y0urStr0ngPassword>
+      redisPass: "Y0urStr0ngPassword" # <enter Redis password here for caching, default to Y0urStr0ngPassword>
 
 resc-database:
   hostOS: "windows" # possible values windows/linux
   database:
     exposeToHostPort: 30880
     pvc_path: "/run/desktop/mnt/host/c/Users/<username>/resc/database" # "<enter path to store database data>" # Linux: /Users/<username>/var/resc/database, Windows: # /run/desktop/mnt/host/c/Users/<username>/resc/database
     config:
@@ -103,14 +112,21 @@
       admin_username: "admin" # <enter rabbitmq admin username, default to admin>
       admin_password: "Y0urStr0ngPassword" # <enter rabbitmq admin password, default to Y0urStr0ngPassword>
       queues_username: "queue_user" # <enter queue username, default to queue_user>
       queues_password: "Y0urStr0ngPassword" # <enter queue password, default to Y0urStr0ngPassword>
     pvc_path: "/run/desktop/mnt/host/c/Users/<username>/resc/rabbitmq" # "<enter path to store rabbitmq data>" # Linux: /Users/<username>/var/resc/rabbitmq, Windows: # /run/desktop/mnt/host/c/Users/<username>/resc/rabbitmq
   filemountType: "windows" # possible values windows/linux/azure
 
+resc-redis:
+  redis:
+    exposeToHostPort: 32379
+    config:
+      port: 6379
+      password: "Y0urStr0ngPassword" # <enter Redis password here for caching, default to Y0urStr0ngPassword>
+
 resc-vcs-instances:
   vcsInstances:
     ### Github ###
     - name: "GITHUB_PUBLIC"
       scope: ["kubernetes", "docker"] # Enter comma separated list of github accounts to scan, For example: ["kubernetes", "docker"] for https://github.com/kubernetes and https://github.com/docker
       exceptions: [] # Enter comma separated list of github accounts to exclude from scan
       providerType: "GITHUB_PUBLIC"
```

### Comparing `resc_helm_wizard-1.0.6/src/resc_helm_wizard/helm_utilities.py` & `resc_helm_wizard-1.1.0/src/resc_helm_wizard/helm_utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,28 @@
         Install or upgrade a helm release
     :param action:
         action to perform like install or upgrade
     :return: bool
         Returns true if install or upgrade succeeded else returns false
     """
     logging.info(f"Running {action}. Please wait for a moment...")
-    helm_command = ["helm", action, "--timeout", constants.HELM_DEPLOY_TIMEOUT, "-n",
-                    constants.NAMESPACE, constants.RELEASE_NAME, constants.CHART_NAME, "-f",
-                    constants.VALUES_FILE, "--set-file", "global.secretScanRulePackConfig=" + constants.RULE_FILE]
+    helm_command = [
+        "helm",
+        action,
+        "--timeout",
+        constants.HELM_DEPLOY_TIMEOUT,
+        "-n",
+        constants.NAMESPACE,
+        constants.RELEASE_NAME,
+        constants.CHART_NAME,
+        "-f",
+        constants.VALUES_FILE,
+        "--set-file",
+        "global.secretScanRulePackConfig=" + constants.RULE_FILE,
+    ]
     try:
         output = subprocess.check_output(helm_command)
         logging.info(output.decode("utf-8"))
         return True
     except subprocess.CalledProcessError:
         logging.error(f"An error occurred during {constants.CHART_NAME} deployment")
         return False
@@ -33,68 +44,92 @@
 
 def check_helm_release_exists() -> bool:
     """
         Checks if helm release exists or not
     :return: bool
         Returns true if helm release exists else returns false
     """
-    output = subprocess.run(["helm", "list", "-f", constants.RELEASE_NAME, "-n", constants.NAMESPACE],
-                            capture_output=True, text=True, check=True)
+    output = subprocess.run(
+        ["helm", "list", "-f", constants.RELEASE_NAME, "-n", constants.NAMESPACE],
+        capture_output=True,
+        text=True,
+        check=True,
+    )
     return bool(constants.RELEASE_NAME in output.stdout.strip())
 
 
 def get_version_from_downloaded_chart() -> str:
     """
         Get version of the downloaded chart
     :return: str
         Returns version of the downloaded chart
     """
-    cmd = f"helm search repo {constants.HELM_REPO_NAME} -n {constants.NAMESPACE} -o json"
+    cmd = (
+        f"helm search repo {constants.HELM_REPO_NAME} -n {constants.NAMESPACE} -o json"
+    )
     output = subprocess.check_output(cmd, shell=True)
     chart_info = json.loads(output.decode("utf-8"))
 
     if chart_info:
         return chart_info[0]["version"]
     return None
 
 
 def add_helm_repository():
     """
-        Adds a helm repository
+    Adds a helm repository
     """
-    cmd = ["helm", "repo", "add", constants.HELM_REPO_NAME, constants.RESC_HELM_REPO_URL, "-n", constants.NAMESPACE]
+    cmd = [
+        "helm",
+        "repo",
+        "add",
+        constants.HELM_REPO_NAME,
+        constants.RESC_HELM_REPO_URL,
+        "-n",
+        constants.NAMESPACE,
+    ]
     try:
         subprocess.run(cmd, check=True)
     except subprocess.CalledProcessError:
         logging.error("An error occurred while adding the helm repository")
         sys.exit(1)
 
 
 def update_helm_repository():
     """
-        Updates a helm repository
+    Updates a helm repository
     """
     cmd = ["helm", "repo", "update", "-n", constants.NAMESPACE]
     try:
         subprocess.run(cmd, check=True)
     except subprocess.CalledProcessError:
         logging.error("An error occurred while updating the helm repository")
         sys.exit(1)
 
 
 def validate_helm_deployment_status():
     """
-        Validate the status of the helm deployment
+    Validate the status of the helm deployment
     """
     try:
-        result = subprocess.run(['helm', 'status', constants.RELEASE_NAME, "-n", constants.NAMESPACE],
-                                capture_output=True, check=True, text=True)
+        result = subprocess.run(
+            ["helm", "status", constants.RELEASE_NAME, "-n", constants.NAMESPACE],
+            capture_output=True,
+            check=True,
+            text=True,
+        )
         output = result.stdout.strip()
         if "STATUS: deployed" in output:
-            logging.info("The deployment was successful. Visit http://127.0.0.1:30000 to get started with RESC!")
-            logging.info("Refer this link for more information on how to trigger the scan: "
-                         "https://github.com/abnamro/repository-scanner/tree/main/"
-                         "deployment/kubernetes#trigger-scanning")
+            logging.info(
+                "The deployment was successful. Visit http://127.0.0.1:30000 to get started with RESC!"
+            )
+            logging.info(
+                "Refer this link for more information on how to trigger the scan: "
+                "https://github.com/abnamro/repository-scanner/tree/main/"
+                "deployment/kubernetes#trigger-scanning"
+            )
     except subprocess.CalledProcessError:
-        logging.error("An error occurred during deployment. Please run this command to debug any issue: "
-                      "kubectl get pods -n resc")
+        logging.error(
+            "An error occurred during deployment. Please run this command to debug any issue: "
+            "kubectl get pods -n resc"
+        )
         sys.exit(1)
```

### Comparing `resc_helm_wizard-1.0.6/src/resc_helm_wizard/helm_value.py` & `resc_helm_wizard-1.1.0/src/resc_helm_wizard/helm_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,20 @@
         Database storage path
     rabbitmq_storage_path : str
         Rabbitmq storage path
     vcs_instances : list
         List of VCS instances
     """
 
-    def __init__(self,
-                 operating_system: str,
-                 db_password: str,
-                 db_storage_path: str,
-                 rabbitmq_storage_path: str,
-                 vcs_instances: List[VcsInstance]):
+    def __init__(
+        self,
+        operating_system: str,
+        db_password: str,
+        db_storage_path: str,
+        rabbitmq_storage_path: str,
+        vcs_instances: List[VcsInstance],
+    ):
         self.operating_system: str = operating_system
         self.db_password: str = db_password
         self.db_storage_path: str = db_storage_path
         self.rabbitmq_storage_path: str = rabbitmq_storage_path
         self.vcs_instances: list = vcs_instances
```

### Comparing `resc_helm_wizard-1.0.6/src/resc_helm_wizard/kubernetes_utilities.py` & `resc_helm_wizard-1.1.0/src/resc_helm_wizard/kubernetes_utilities.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,21 +11,33 @@
     :param namespace_name:
         name of the namespace you want to create
     :return: bool
         Returns true if namespace created else returns false
     """
     created = False
     # Check if the namespace already exists
-    check_namespace = subprocess.run(["kubectl", "get", "namespace", namespace_name], capture_output=True, text=True,
-                                     check=False)
+    check_namespace = subprocess.run(
+        ["kubectl", "get", "namespace", namespace_name],
+        capture_output=True,
+        text=True,
+        check=False,
+    )
     if "NotFound" in check_namespace.stderr:
         # Namespace doesn't exist, create it
-        create_namespace = subprocess.run(["kubectl", "create", "namespace", namespace_name], check=True)
+        create_namespace = subprocess.run(
+            ["kubectl", "create", "namespace", namespace_name], check=True
+        )
         if create_namespace.returncode == 0:
             created = True
-            logging.info(f"Namespace {namespace_name} created. Preparing for deployment...")
+            logging.info(
+                f"Namespace {namespace_name} created. Preparing for deployment..."
+            )
         else:
-            logging.error(f"Error reading namespace: {namespace_name}. Aborting deployment...")
+            logging.error(
+                f"Error reading namespace: {namespace_name}. Aborting deployment..."
+            )
     else:
         created = True
-        logging.info(f"Namespace {namespace_name} already exists. Preparing for deployment...")
+        logging.info(
+            f"Namespace {namespace_name} already exists. Preparing for deployment..."
+        )
     return created
```

### Comparing `resc_helm_wizard-1.0.6/src/resc_helm_wizard/questions.py` & `resc_helm_wizard-1.1.0/src/resc_helm_wizard/questions.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,50 +9,56 @@
 from resc_helm_wizard.validator import (
     azure_devops_token_validator,
     bitbucket_token_validator,
     github_account_name_validator,
     github_token_validator,
     github_username_validator,
     password_validator,
-    vcs_url_validator
+    vcs_url_validator,
 )
 
 
 def ask_operating_system() -> str:
     """
         Asks user to select operating system
     :return: str
         Returns user selected operating system
     """
     answer = questionary.select(
         message="Which operating system are you running on the target environment",
-        choices=["Microsoft Windows", "macOS", "Linux"]).unsafe_ask()
+        choices=["Microsoft Windows", "macOS", "Linux"],
+    ).unsafe_ask()
     return answer
 
 
 def ask_local_storage_path() -> str:
     """
         Asks user to provide path for local storage
     :return: str
         Returns user provided local storage path
     """
-    default_local_storage = os.path.expanduser('~')
-    answer = questionary.path(message="Where would you like to create the local storage for RESC. default is ",
-                              default=default_local_storage, only_directories=True).unsafe_ask()
+    default_local_storage = os.path.expanduser("~")
+    answer = questionary.path(
+        message="Where would you like to create the local storage for RESC. default is ",
+        default=default_local_storage,
+        only_directories=True,
+    ).unsafe_ask()
     return answer
 
 
 def ask_password_for_database() -> str:
     """
         Asks user to provide password for database
     :return: str
         Returns user provided password for database
     """
-    answer = questionary.password("Please enter the password you want to set for database",
-                                  validate=password_validator).unsafe_ask()
+    answer = questionary.password(
+        "Please enter the password you want to set for database",
+        validate=password_validator,
+    ).unsafe_ask()
     return answer
 
 
 def ask_user_confirmation(msg: str) -> bool:
     """
         Asks user to provide confirmation
     :param msg:
@@ -67,69 +73,91 @@
 def ask_user_to_select_vcs_instance() -> [str]:
     """
         Asks user to select vcs instances
     :return: [str]
         Returns array of user selected vcs instances
     """
     answer = questionary.checkbox(
-        'Select VCS instance for which you want to run the scan',
+        "Select VCS instance for which you want to run the scan",
         choices=[
             "GitHub",
             "Azure Devops",
             "Bitbucket",
         ],
-        default="GitHub").unsafe_ask()
+        default="GitHub",
+    ).unsafe_ask()
     return answer
 
 
 def ask_vcs_instance_details(vcs_type: str) -> dict:
     """
         Asks user to provide vcs instances details
     :return: dict
         Returns vcs instance info
     """
     username = "NA"
     organization = ""
 
     if vcs_type == "GitHub":
-        url = questionary.text(f"Please enter {vcs_type} url",
-                               default=constants.DEFAULT_GITHUB_URL,
-                               validate=vcs_url_validator).unsafe_ask()
-        username = questionary.text(f"What's your {vcs_type} username",
-                                    validate=github_username_validator).unsafe_ask()
-        token = questionary.password(f"Please enter your {vcs_type} personal access token",
-                                     validate=github_token_validator).unsafe_ask()
+        url = questionary.text(
+            f"Please enter {vcs_type} url",
+            default=constants.DEFAULT_GITHUB_URL,
+            validate=vcs_url_validator,
+        ).unsafe_ask()
+        username = questionary.text(
+            f"What's your {vcs_type} username", validate=github_username_validator
+        ).unsafe_ask()
+        token = questionary.password(
+            f"Please enter your {vcs_type} personal access token",
+            validate=github_token_validator,
+        ).unsafe_ask()
 
     if vcs_type == "Bitbucket":
-        url = questionary.text(f"Please enter {vcs_type} url",
-                               validate=vcs_url_validator).unsafe_ask()
+        url = questionary.text(
+            f"Please enter {vcs_type} url", validate=vcs_url_validator
+        ).unsafe_ask()
         username = questionary.text(f"What's your {vcs_type} username").unsafe_ask()
-        token = questionary.password(f"Please enter your {vcs_type} personal access token",
-                                     validate=bitbucket_token_validator).unsafe_ask()
+        token = questionary.password(
+            f"Please enter your {vcs_type} personal access token",
+            validate=bitbucket_token_validator,
+        ).unsafe_ask()
 
     if vcs_type == "Azure Devops":
-        url = questionary.text(f"Please enter {vcs_type} url",
-                               default=constants.DEFAULT_AZURE_DEVOPS_URL,
-                               validate=vcs_url_validator).unsafe_ask()
-        organization = questionary.text(f"What's your organization name in {vcs_type}").unsafe_ask()
-        token = questionary.password(f"Please enter your {vcs_type} personal access token",
-                                     validate=azure_devops_token_validator).unsafe_ask()
-    vcs_instance_info = {"url": url, "organization": organization, "username": username, "token": token}
+        url = questionary.text(
+            f"Please enter {vcs_type} url",
+            default=constants.DEFAULT_AZURE_DEVOPS_URL,
+            validate=vcs_url_validator,
+        ).unsafe_ask()
+        organization = questionary.text(
+            f"What's your organization name in {vcs_type}"
+        ).unsafe_ask()
+        token = questionary.password(
+            f"Please enter your {vcs_type} personal access token",
+            validate=azure_devops_token_validator,
+        ).unsafe_ask()
+    vcs_instance_info = {
+        "url": url,
+        "organization": organization,
+        "username": username,
+        "token": token,
+    }
     return vcs_instance_info
 
 
 def ask_which_github_accounts_to_scan(default_github_accounts: str) -> [str]:
     """
         Asks user to provide GitHub account names to scan
     :return: [str]
         Returns array of GitHub account names
     """
-    github_accounts = questionary.text("Enter a comma separated list of GitHub accounts you want to scan",
-                                       default=default_github_accounts,
-                                       validate=github_account_name_validator).unsafe_ask()
+    github_accounts = questionary.text(
+        "Enter a comma separated list of GitHub accounts you want to scan",
+        default=default_github_accounts,
+        validate=github_account_name_validator,
+    ).unsafe_ask()
     return github_accounts
 
 
 def ask_ssl_verification(msg: str) -> bool:
     """
         Asks for ssl verification
     :param msg:
```

### Comparing `resc_helm_wizard-1.0.6/src/resc_helm_wizard/run_wizard.py` & `resc_helm_wizard-1.1.0/src/resc_helm_wizard/run_wizard.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,35 +14,43 @@
     """
     try:
         os_input = questions.ask_operating_system()
         if os_input:
             operating_system = common.get_operating_system(user_input=os_input)
 
         if operating_system:
-            storage_path = common.create_storage_for_db_and_rabbitmq(operating_system=operating_system)
+            storage_path = common.create_storage_for_db_and_rabbitmq(
+                operating_system=operating_system
+            )
             db_storage_path = storage_path["db_storage_path"]
             rabbitmq_storage_path = storage_path["rabbitmq_storage_path"]
 
             db_password = questions.ask_password_for_database()
 
             vcs_instances = common.get_vcs_instance_question_answers()
 
-            if (db_password and db_storage_path and
-                    rabbitmq_storage_path and vcs_instances):
+            if (
+                db_password
+                and db_storage_path
+                and rabbitmq_storage_path
+                and vcs_instances
+            ):
                 helm_values = HelmValue(
                     operating_system=operating_system,
                     db_password=db_password,
                     db_storage_path=db_storage_path,
                     rabbitmq_storage_path=rabbitmq_storage_path,
-                    vcs_instances=vcs_instances
+                    vcs_instances=vcs_instances,
                 )
 
-                common.create_helm_values_yaml(helm_values=helm_values,
-                                               input_values_yaml_file="config/example-values.yaml")
+                common.create_helm_values_yaml(
+                    helm_values=helm_values,
+                    input_values_yaml_file="config/example-values.yaml",
+                )
                 common.run_deployment_as_per_user_confirmation()
     except KeyboardInterrupt:
         logging.error("Aborting the program! operation cancelled by user")
         sys.exit(-1)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     prompt_questions()
```

### Comparing `resc_helm_wizard-1.0.6/src/resc_helm_wizard/validator.py` & `resc_helm_wizard-1.1.0/src/resc_helm_wizard/validator.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,23 @@
         Password validator for database
     :param password:
         password which needs to be validated
     :return: str or bool.
         If validation fails, the output will contain a validation error message.
         Otherwise, the output will return true if validation was successful
     """
-    regex = re.compile(r"^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*#?&])[A-Za-z\d@$!#%*?&]{8,128}$")
+    regex = re.compile(
+        r"^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*#?&])[A-Za-z\d@$!#%*?&]{8,128}$"
+    )
 
     if not re.fullmatch(regex, password):
-        return "Password must contain at least one upper case, one lower case, one number, " \
-               "one special character and the length of the password to be between 8 and 128"
+        return (
+            "Password must contain at least one upper case, one lower case, one number, "
+            "one special character and the length of the password to be between 8 and 128"
+        )
     return True
 
 
 def github_token_validator(token: str):
     """
         Personal access token validator for GitHub
     :param token:
@@ -27,15 +31,17 @@
     :return: str or bool.
         If validation fails, the output will contain a validation error message.
         Otherwise, the output will return true if validation was successful
     """
     classic_pat_regex = re.compile(r"^ghp_[a-zA-Z0-9]{36}$")
     fine_grained_pat_regex = re.compile(r"^github_pat_[a-zA-Z0-9]{22}_[a-zA-Z0-9]{59}$")
 
-    if not re.fullmatch(classic_pat_regex, token) and not re.fullmatch(fine_grained_pat_regex, token):
+    if not re.fullmatch(classic_pat_regex, token) and not re.fullmatch(
+        fine_grained_pat_regex, token
+    ):
         return "Validation failed for provided GitHub token"
     return True
 
 
 def azure_devops_token_validator(token: str):
     """
         Personal access token validator for Azure Devops
@@ -78,17 +84,19 @@
         Otherwise, the output will return true if validation was successful
     """
     input_list = [elem.strip() for elem in github_accounts.split(",")]
     regex = re.compile(r"^[a-zA-Z\d](?:[a-zA-Z\d]|-(?=[a-zA-Z\d])){0,38}$")
     for account in input_list:
         if not re.fullmatch(regex, account):
             if account:
-                msg = f"{account} is not a valid GitHub account. " \
-                      f"GitHub account must contain alphanumeric characters or single hyphens, " \
-                      f"can't begin or end with a hyphen and maximum 39 characters allowed."
+                msg = (
+                    f"{account} is not a valid GitHub account. "
+                    f"GitHub account must contain alphanumeric characters or single hyphens, "
+                    f"can't begin or end with a hyphen and maximum 39 characters allowed."
+                )
             else:
                 msg = "Please enter a valid comma separated list of GitHub accounts you want to scan"
             return msg
     return True
 
 
 def github_username_validator(username):
@@ -99,34 +107,38 @@
     :return: str or bool.
         If validation fails, the output will contain a validation error message.
         Otherwise, the output will return true if validation was successful
     """
     regex = re.compile(r"^[a-zA-Z\d](?:[a-zA-Z\d]|-(?=[a-zA-Z\d])){0,38}$")
 
     if not re.fullmatch(regex, username):
-        msg = f"{username} is not a valid GitHub username. " \
-              f"GitHub username must contain alphanumeric characters or single hyphens, " \
-              f"can't begin or end with a hyphen and maximum 39 characters allowed."
+        msg = (
+            f"{username} is not a valid GitHub username. "
+            f"GitHub username must contain alphanumeric characters or single hyphens, "
+            f"can't begin or end with a hyphen and maximum 39 characters allowed."
+        )
         return msg
     return True
 
 
 def vcs_url_validator(url):
     """
         VCS provider url validator
     :param url:
         url which needs to be validated
     :return: str or bool.
         If validation fails, the output will contain a validation error message.
         Otherwise, the output will return true if validation was successful
     """
     regex = re.compile(
-        r'^(?:http)s?://'  # Scheme
-        r'(?:(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+(?:[A-Z]{2,6}\.?|[A-Z0-9-]{2,}\.?)|'  # Domain
-        r'localhost|'  # Localhost
-        r'\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})'  # IP address
-        r'(?::\d+)?'  # Port (optional)
-        r'(?:/?|[/?]\S+)$', re.IGNORECASE)  # Path and query (optional)
+        r"^(?:http)s?://"  # Scheme
+        r"(?:(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+(?:[A-Z]{2,6}\.?|[A-Z0-9-]{2,}\.?)|"  # Domain
+        r"localhost|"  # Localhost
+        r"\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})"  # IP address
+        r"(?::\d+)?"  # Port (optional)
+        r"(?:/?|[/?]\S+)$",
+        re.IGNORECASE,
+    )  # Path and query (optional)
 
     if not re.fullmatch(regex, url):
         return "Please provide a valid URL"
     return True
```

### Comparing `resc_helm_wizard-1.0.6/src/resc_helm_wizard/vcs_instance.py` & `resc_helm_wizard-1.1.0/src/resc_helm_wizard/vcs_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,25 @@
         password of vcs instance
     organization : str
         organization of vcs instance
     scope : list
         List of scope
     """
 
-    def __init__(self,
-                 provider_type: str,
-                 scheme: str,
-                 host: str,
-                 port: str,
-                 username: str,
-                 password: str,
-                 organization: str,
-                 scope: List[str]):
+    def __init__(
+        self,
+        provider_type: str,
+        scheme: str,
+        host: str,
+        port: str,
+        username: str,
+        password: str,
+        organization: str,
+        scope: List[str],
+    ):
         self.provider_type: str = provider_type
         self.scheme: str = scheme
         self.host: str = host
         self.port: str = port
         self.username: str = username
         self.password: str = password
         self.organization: str = organization
```

### Comparing `resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/PKG-INFO` & `resc_helm_wizard-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 Metadata-Version: 2.1
-Name: resc-helm-wizard
-Version: 1.0.6
+Name: resc_helm_wizard
+Version: 1.1.0
 Summary: Repository Scanner - Helm Wizard
 Home-page: https://github.com/ABNAMRO/repository-scanner
+Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
-License: UNKNOWN
-Platform: UNKNOWN
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: questionary==2.0.1
+Requires-Dist: requests==2.31.0
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: setuptools<=69.5.1
 
 # Repository Scanner Helm Wizard (resc-helm-wizard)
+[![Python][python-shield]][python-url]
+[![CI][ci-shield]][ci-url]
 
 <!-- TABLE OF CONTENTS -->
 ## Table of contents
 1. [About the component](#about-the-component)
 2. [Getting started](#getting-started)
     - [Prerequisites](#prerequisites)
     - [Usage](#usage)
@@ -30,15 +37,15 @@
 <!-- GETTING STARTED -->
 ## Getting started
 
 These instructions will help you to get a copy of the project up and running on your local machine for development and testing purposes.
 
 ### Prerequisites
 - [Git](https://git-scm.com/downloads)
-- [Python (v3.9.0 or higher)](https://www.python.org/downloads/release/python-390/)
+- [Python (v3.12.0 or higher)](https://www.python.org/downloads/release/python-3120/)
 - [Docker Desktop](https://www.docker.com/products/docker-desktop/)
 - [Kubernetes](https://kubernetes.io/)
 - [Helm](https://helm.sh/)
 
 ### Usage
 Install the package:
 ```bash
@@ -87,16 +94,20 @@
 [(Back to top)](#table-of-contents)
 
 ### Run unit tests, linting and import checks locally:
 See below commands for running various (unit/linting) tests locally. To run these tests you need to install [tox](https://pypi.org/project/tox/). This can be done on Linux and Windows with Git Bash.
 
 Run below commands to make sure that the unit tests are running and that the code matches quality standards:
 ```bash
-pip install tox      # install tox locally
+pip install tox         # install tox locally
 
-tox -v -e sort       # Run this command to validate the import sorting
-tox -v -e lint       # Run this command to lint the code according to this repository's standard
-tox -v -e pytest     # Run this command to run the unit tests
-tox -v               # Run this command to run all of the above tests
+tox run -e py -v        # Run this command to run the unit tests
+tox run -e isort -v     # Run this command to validate the import sorting
+tox run -e pylint -v    # Run this command for Python static code analysis
+tox run -e flake8 -v    # Run this command for Python linting
 ```
 
-
+<!-- MARKDOWN LINKS & IMAGES -->
+[python-shield]: https://img.shields.io/badge/Python-3670A0?style=flat&logo=python&logoColor=ffdd54
+[python-url]: https://www.python.org
+[ci-shield]: https://img.shields.io/github/actions/workflow/status/abnamro/repository-scanner/helm-wizard-ci.yaml?style=flat&logo=github
+[ci-url]: https://github.com/abnamro/repository-scanner/actions/workflows/helm-wizard-ci.yaml
```

### Comparing `resc_helm_wizard-1.0.6/src/resc_helm_wizard.egg-info/SOURCES.txt` & `resc_helm_wizard-1.1.0/src/resc_helm_wizard.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+LICENSE.md
+README.md
+requirements.txt
 setup.cfg
 setup.py
 src/resc_helm_wizard/__init__.py
 src/resc_helm_wizard/common.py
 src/resc_helm_wizard/constants.py
 src/resc_helm_wizard/helm_utilities.py
 src/resc_helm_wizard/helm_value.py
```

