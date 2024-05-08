# Comparing `tmp/resc_vcs_scanner-3.0.1.tar.gz` & `tmp/resc_vcs_scanner-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_vcs_scanner-3.0.1.tar", last modified: Mon Apr  8 09:39:32 2024, max compression
+gzip compressed data, was "resc_vcs_scanner-3.1.0.tar", last modified: Wed May  8 12:38:12 2024, max compression
```

## Comparing `resc_vcs_scanner-3.0.1.tar` & `resc_vcs_scanner-3.1.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:32.105249 resc_vcs_scanner-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-04-08 09:39:32.105249 resc_vcs_scanner-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 09:39:32.105249 resc_vcs_scanner-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:32.101249 resc_vcs_scanner-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:32.101249 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-04-08 09:39:32.000000 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-08 09:39:32.000000 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:39:32.000000 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 09:39:32.000000 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:39:32.000000 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 09:39:32.000000 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 09:39:32.000000 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:32.101249 resc_vcs_scanner-3.0.1/src/vcs_scanner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:32.101249 resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/env_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/finding_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/finding_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/ignore_list_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/resc_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:32.105249 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/celery_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/git_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12077 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/secret_scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:32.105249 resc_vcs_scanner-3.0.1/src/vcs_scanner/static/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/static/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:12.186023 resc_vcs_scanner-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-08 12:38:12.186023 resc_vcs_scanner-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-08 12:38:12.186023 resc_vcs_scanner-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:12.178023 resc_vcs_scanner-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:12.186023 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-08 12:38:12.000000 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-08 12:38:12.000000 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:38:12.000000 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 12:38:12.000000 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:38:12.000000 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 12:38:12.000000 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 12:38:12.000000 resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:12.182023 resc_vcs_scanner-3.1.0/src/vcs_scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:12.186023 resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/env_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/finding_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/finding_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/ignore_list_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/resc_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:12.186023 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/celery_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15012 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/git_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/secret_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:38:12.186023 resc_vcs_scanner-3.1.0/src/vcs_scanner/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-08 12:38:07.000000 resc_vcs_scanner-3.1.0/src/vcs_scanner/static/logging.ini
```

### Comparing `resc_vcs_scanner-3.0.1/LICENSE.md` & `resc_vcs_scanner-3.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.0.1/PKG-INFO` & `resc_vcs_scanner-3.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: resc_vcs_scanner
-Version: 3.0.1
-Summary: Repository Scanner - Version Control System - Scanner
-Home-page: https://github.com/ABNAMRO/repository-scanner
-Author: ABN AMRO
-Author-email: resc@nl.abnamro.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # Repository Scanner Version Control System Scanner (RESC-VCS-SCANNER)
 [![Python][python-shield]][python-url]
 [![Celery][celery-shield]][celery-url]
 [![Pydantic][pydantic-shield]][pydantic-url]
 [![Gitleaks][gitleaks-shield]][gitleaks-url]
 [![CI][ci-shield]][ci-url]
 [![SonarCloud][sonar-cloud-shield]][sonar-cloud-url]
@@ -261,9 +248,8 @@
 [pydantic-shield]: https://img.shields.io/badge/Pydantic-e92063.svg?logo=pydantic&style=flat
 [pydantic-url]: https://docs.pydantic.dev
 [gitleaks-shield]: https://img.shields.io/badge/Gitleaks-121013?logo=github&logoColor=white
 [gitleaks-url]: https://github.com/zricethezav/gitleaks
 [ci-shield]: https://img.shields.io/github/actions/workflow/status/abnamro/repository-scanner/vcs-scanner-ci.yaml?logo=github
 [ci-url]: https://github.com/abnamro/repository-scanner/actions/workflows/vcs-scanner-ci.yaml
 [sonar-cloud-shield]: https://sonarcloud.io/api/project_badges/measure?project=abnamro-resc_resc-vcs-scanner&metric=alert_status
-[sonar-cloud-url]: https://sonarcloud.io/summary/new_code?id=abnamro-resc_resc-vcs-scanner
-
+[sonar-cloud-url]: https://sonarcloud.io/summary/new_code?id=abnamro-resc_resc-vcs-scanner
```

### Comparing `resc_vcs_scanner-3.0.1/setup.cfg` & `resc_vcs_scanner-3.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_vcs_scanner
 description = Repository Scanner - Version Control System - Scanner
-version = 3.0.1
+version = 3.1.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE.md
```

### Comparing `resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/PKG-INFO` & `resc_vcs_scanner-3.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 Metadata-Version: 2.1
-Name: resc-vcs-scanner
-Version: 3.0.1
+Name: resc_vcs_scanner
+Version: 3.1.0
 Summary: Repository Scanner - Version Control System - Scanner
 Home-page: https://github.com/ABNAMRO/repository-scanner
+Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: celery==5.3.1
+Requires-Dist: amqp==5.1.1
+Requires-Dist: requests==2.31.0
+Requires-Dist: typing==3.7.4.3
+Requires-Dist: pydantic==1.10.15
+Requires-Dist: GitPython==3.1.41
+Requires-Dist: resc-backend>=3.1.1
+Requires-Dist: tenacity==8.2.2
+Requires-Dist: prettytable==3.8.0
+Requires-Dist: termcolor==2.3.0
+Requires-Dist: tomlkit==0.12.1
 
 # Repository Scanner Version Control System Scanner (RESC-VCS-SCANNER)
 [![Python][python-shield]][python-url]
 [![Celery][celery-shield]][celery-url]
 [![Pydantic][pydantic-shield]][pydantic-url]
 [![Gitleaks][gitleaks-shield]][gitleaks-url]
 [![CI][ci-shield]][ci-url]
@@ -262,8 +272,7 @@
 [pydantic-url]: https://docs.pydantic.dev
 [gitleaks-shield]: https://img.shields.io/badge/Gitleaks-121013?logo=github&logoColor=white
 [gitleaks-url]: https://github.com/zricethezav/gitleaks
 [ci-shield]: https://img.shields.io/github/actions/workflow/status/abnamro/repository-scanner/vcs-scanner-ci.yaml?logo=github
 [ci-url]: https://github.com/abnamro/repository-scanner/actions/workflows/vcs-scanner-ci.yaml
 [sonar-cloud-shield]: https://sonarcloud.io/api/project_badges/measure?project=abnamro-resc_resc-vcs-scanner&metric=alert_status
 [sonar-cloud-url]: https://sonarcloud.io/summary/new_code?id=abnamro-resc_resc-vcs-scanner
-
```

### Comparing `resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/SOURCES.txt` & `resc_vcs_scanner-3.1.0/src/resc_vcs_scanner.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 LICENSE.md
+README.md
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 src/resc_vcs_scanner.egg-info/PKG-INFO
 src/resc_vcs_scanner.egg-info/SOURCES.txt
 src/resc_vcs_scanner.egg-info/dependency_links.txt
 src/resc_vcs_scanner.egg-info/entry_points.txt
```

### Comparing `resc_vcs_scanner-3.0.1/src/vcs_scanner/common.py` & `resc_vcs_scanner-3.1.0/src/vcs_scanner/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Standard Library
 import logging.config
 import sys
-from distutils.sysconfig import get_python_lib
+import sysconfig
 from os import path
 from typing import Dict, List, Optional
 
 # Third Party
 import tomlkit
 
 # First Party
 from vcs_scanner.input_parser import parse_vcs_instances_file
 from vcs_scanner.model import VCSInstanceRuntime
 
 logger = logging.getLogger(__name__)
 
 
 def get_logging_settings_path():
-    if path.isfile(get_python_lib() + "/vcs_scanner"):
-        base_dir = get_python_lib() + "/vcs_scanner"
+    if path.isfile(sysconfig.get_path("purelib") + "/vcs_scanner"):
+        base_dir = sysconfig.get_path("purelib") + "/vcs_scanner"
     else:
         base_dir = path.dirname(__file__)
 
     return base_dir + "/static/logging.ini"
 
 
 def generate_logger_config(log_file_path, debug=True):
@@ -38,64 +38,66 @@
     """
 
     logging_level = "DEBUG" if debug else "INFO"
     logging_config = {
         "version": 1,
         "disable_existing_loggers": False,
         "formatters": {
-            "generic-log-formatter": {
-                "format": "[%(levelname)s] [%(name)s] [%(asctime)s] %(message)s"
-            },
+            "generic-log-formatter": {"format": "[%(levelname)s] [%(name)s] [%(asctime)s] %(message)s"},
         },
         "handlers": {
             "console": {
                 "level": logging_level,
                 "class": "logging.StreamHandler",
                 "formatter": "generic-log-formatter",
             },
             "file": {
                 "level": logging_level,
                 "class": "logging.handlers.RotatingFileHandler",
                 "formatter": "generic-log-formatter",
                 "filename": log_file_path,
                 "maxBytes": 100 * 1024 * 1024,
-                "backupCount": 5
-            }
+                "backupCount": 5,
+            },
         },
         "loggers": {
             "": {
                 "handlers": ["console", "file"],
                 "level": logging_level,
-                "propagate": True
+                "propagate": True,
             },
-        }
+        },
     }
 
     return logging_config
 
 
 def initialise_logs(log_file_path: str, debug=True):
     logging_ini_file = get_logging_settings_path()
-    logging.config.fileConfig(logging_ini_file, defaults={'log_file_path': log_file_path},
-                              disable_existing_loggers=False)
-    logger_config = logging.getLogger('root')
+    logging.config.fileConfig(
+        logging_ini_file,
+        defaults={"log_file_path": log_file_path},
+        disable_existing_loggers=False,
+    )
+    logger_config = logging.getLogger("root")
     if int(debug) == 1:
         logger_config.setLevel(logging.DEBUG)
     else:
         logger_config.setLevel(logging.INFO)
     return logger_config
 
 
 def load_vcs_instances(file_path: str) -> Dict[str, VCSInstanceRuntime]:
     vcs_instances_list: List[VCSInstanceRuntime] = parse_vcs_instances_file(file_path)
     if not vcs_instances_list:
         logger.critical(f"Exiting due to issues in VCS Instances definition in file {file_path}")
         sys.exit(-1)
-    vcs_instances_map: Dict[str, VCSInstanceRuntime] = \
-        {vcs_instance.name: vcs_instance for vcs_instance in vcs_instances_list}
+    vcs_instances_map: Dict[str, VCSInstanceRuntime] = {
+        vcs_instance.name: vcs_instance for vcs_instance in vcs_instances_list
+    }
     return vcs_instances_map
 
 
 def get_rule_pack_version_from_file(file_content: str) -> Optional[str]:
     toml_rule_dictionary = tomlkit.loads(file_content)
     rule_pack_version = toml_rule_dictionary["version"] if "version" in toml_rule_dictionary else None
     return rule_pack_version
```

### Comparing `resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/env_default.py` & `resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/env_default.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     Helper for the CLI argparse to allow setting defaults through environment variables
     Usage: In an argparse argument, set the Action to this class.
         Add the extra variable envvar added that has the name of the environment variable containing the default value.
     Example: parser.add_argument("--gitleaks-path", action=EnvDefault, envvar="RESC_GITLEAKS_PATH")
         This would result in the parser reading the env var if it exists and using it as the default,
         always to be overrideable using the cli argument.
     """
+
     def __init__(self, envvar, required=True, default=None, **kwargs):
         if not default and envvar:
             if envvar in os.environ:
                 default = os.environ[envvar]
         if required and default:
             required = False
         super().__init__(default=default, required=required, **kwargs)
```

### Comparing `resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/environment_wrapper.py` & `resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/finding_filter.py` & `resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/finding_filter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Third Party
 import tomlkit
 from resc_backend.resc_web_service.schema.finding import FindingCreate
 
 
-def should_process_finding(finding: FindingCreate, rule_tags: dict = None,
-                           include_tags: [str] = None, ignore_tags: [str] = None) -> bool:
+def should_process_finding(
+    finding: FindingCreate,
+    rule_tags: dict = None,
+    include_tags: [str] = None,
+    ignore_tags: [str] = None,
+) -> bool:
     """
         Determine the action to take for the finding, based on the rule tags
     :param finding:
         FindingCreate instance of the finding
     :param rule_tags:
         Dictionary containing all the rules and there respective tags
     :param include_tags:
@@ -37,11 +41,29 @@
     """
     rule_tags = {}
     # read toml
     with open(toml_rule_file_path, encoding="utf-8") as toml_rule_file:
         toml_rule_dictionary = tomlkit.loads(toml_rule_file.read())
         # convert to dict
         for toml_rule in toml_rule_dictionary["rules"]:
-            rule_id = toml_rule.get('id', None)
+            rule_id = toml_rule.get("id", None)
             if rule_id:
-                rule_tags[rule_id] = toml_rule.get('tags', [])
+                rule_tags[rule_id] = toml_rule.get("tags", [])
     return rule_tags
+
+
+def get_rule_comment(toml_rule_file_path: str) -> dict:
+    """
+        Get the tags per rule from the .toml rule file, from self.toml_rule_file_path
+    :return: dict.
+        The output will contain a dictionary with the rule id as the key and the tags as a list in the value
+    """
+    rule_comments = {}
+    # read toml
+    with open(toml_rule_file_path, encoding="utf-8") as toml_rule_file:
+        toml_rule_dictionary = tomlkit.loads(toml_rule_file.read())
+        # convert to dict
+        for toml_rule in toml_rule_dictionary["rules"]:
+            rule_id = toml_rule.get("id", None)
+            if rule_id:
+                rule_comments[rule_id] = toml_rule.get("comment", "")
+    return rule_comments
```

### Comparing `resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/ignore_list_provider.py` & `resc_vcs_scanner-3.1.0/src/vcs_scanner/helpers/ignore_list_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,39 +6,38 @@
 
 # Third Party
 import dateutil.parser
 
 logger = logging.getLogger(__name__)
 
 
-class IgnoredListProvider():  # pylint: disable=R0902
-
+class IgnoredListProvider:  # pylint: disable=R0902
     def __init__(self, ignore_findings_path: str):
         self.ignore_findings_path: str = ignore_findings_path
         self.today: datetime = datetime.now()
 
     def get_ignore_list(self) -> dict:
         """
-            Get the dictionary of ignored findings according to the file
-            The output will contain a dictionary with the findings id as the key and the tags as a list in the value
+        Get the dictionary of ignored findings according to the file
+        The output will contain a dictionary with the findings id as the key and the tags as a list in the value
         """
         ignored = {}
 
         if self.ignore_findings_path is None:
             return ignored
 
         try:
             # read dsv: `path|rule_name|line_number|expiry_date`
             with open(self.ignore_findings_path, encoding="utf-8") as ignore_findings_file:
-                csv_ignore_list = csv.reader(ignore_findings_file, delimiter='|')
+                csv_ignore_list = csv.reader(ignore_findings_file, delimiter="|")
                 for row in csv_ignore_list:
                     expire: datetime = datetime.now()
 
                     # rows starting with # are comments
-                    if row[0][:1] == '#':
+                    if row[0][:1] == "#":
                         continue
 
                     if len(row) < 3:
                         string_row: str = "".join(row)
                         logger.warning(f"Skipping: incomplete entry for {string_row}")
                         continue
```

### Comparing `resc_vcs_scanner-3.0.1/src/vcs_scanner/input_parser.py` & `resc_vcs_scanner-3.1.0/src/vcs_scanner/input_parser.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.0.1/src/vcs_scanner/model.py` & `resc_vcs_scanner-3.1.0/src/vcs_scanner/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def convert_to_repository(self, vcs_instance_id: int) -> Repository:
         return Repository(
             project_key=self.project_key,
             repository_id=self.repository_id,
             repository_name=self.repository_name,
             repository_url=self.repository_url,
             vcs_instance=vcs_instance_id,
-            latest_commit=self.latest_commit
+            latest_commit=self.latest_commit,
         )
 
 
 class VCSInstanceRuntime(BaseModel):
     id_: Optional[int]
     name: constr(max_length=200)
     provider_type: VCSProviders
@@ -57,26 +57,31 @@
                 raise ValueError("The organization field needs to be specified for Azure devops vcs instances")
         return value
 
     @validator("scope", pre=True)
     @classmethod
     def check_scope_and_exceptions(cls, value, values):
         if value and values["exceptions"]:
-            raise ValueError("You cannot specify bot the scope and exceptions to the scan, only one setting"
-                             " is supported.")
+            raise ValueError(
+                "You cannot specify bot the scope and exceptions to the scan, only one setting" " is supported."
+            )
         return value
 
     @validator("username", pre=True)
     @classmethod
     def check_presence_of_username(cls, value, values):
         if not os.environ.get(value):
-            raise ValueError(f"The username for VCS Instance {values['name']} could not be found in the "
-                             f"environment variable {value}")
+            raise ValueError(
+                f"The username for VCS Instance {values['name']} could not be found in the "
+                f"environment variable {value}"
+            )
         return os.environ.get(value)
 
     @validator("token", pre=True)
     @classmethod
     def check_presence_of_token(cls, value, values):
         if not os.environ.get(value):
-            raise ValueError(f"The access token for VCS Instance {values['name']} could not be found in the "
-                             f"environment variable {value}")
+            raise ValueError(
+                f"The access token for VCS Instance {values['name']} could not be found in the "
+                f"environment variable {value}"
+            )
         return os.environ.get(value)
```

### Comparing `resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/celery_worker.py` & `resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/celery_worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,28 +23,33 @@
     RABBITMQ_SERVICE_HOST,
     RABBITMQ_USERNAME,
     REQUIRED_ENV_VARS,
     RESC_API_NO_AUTH_SERVICE_HOST,
     RESC_API_NO_AUTH_SERVICE_PORT,
     RESC_IGNORE_TAGS,
     RESC_INCLUDE_TAGS,
-    VCS_INSTANCES_FILE_PATH
+    VCS_INSTANCES_FILE_PATH,
 )
 from vcs_scanner.secret_scanners.secret_scanner import SecretScanner
 
 env_variables = validate_environment(REQUIRED_ENV_VARS)
-app = Celery('secret_scanner_worker',
-             broker="amqp://" +
-                    f"{env_variables[RABBITMQ_USERNAME]}" + ":" +
-                    f"{env_variables[RABBITMQ_PASSWORD]}" + "@" +
-                    f"{env_variables[RABBITMQ_SERVICE_HOST]}" + "/" +
-                    f"{env_variables[RABBITMQ_DEFAULT_VHOST]}")
-app.conf.update({'worker_hijack_root_logger': False})
-app.conf.update({'broker_connection_retry': True})
-app.conf.update({'broker_connection_max_retries': 100})
+app = Celery(
+    "secret_scanner_worker",
+    broker="amqp://"
+    + f"{env_variables[RABBITMQ_USERNAME]}"
+    + ":"
+    + f"{env_variables[RABBITMQ_PASSWORD]}"
+    + "@"
+    + f"{env_variables[RABBITMQ_SERVICE_HOST]}"
+    + "/"
+    + f"{env_variables[RABBITMQ_DEFAULT_VHOST]}",
+)
+app.conf.update({"worker_hijack_root_logger": False})
+app.conf.update({"broker_connection_retry": True})
+app.conf.update({"broker_connection_max_retries": 100})
 
 logger = get_task_logger(__name__)
 logger_config = initialise_logs(LOG_FILE_PATH)
 rabbitmq_queue = env_variables[RABBITMQ_QUEUE]
 rws_url = f"http://{env_variables[RESC_API_NO_AUTH_SERVICE_HOST]}:{env_variables[RESC_API_NO_AUTH_SERVICE_PORT]}"
 rws_writer: RESTAPIWriter = RESTAPIWriter(rws_url=rws_url)
 
@@ -63,43 +68,50 @@
     if not DOWNLOADED_RULE_PACK_VERSION:
         DOWNLOADED_RULE_PACK_VERSION = rws_writer.download_rule_pack()
 
     active_rule_pack_version = rws_writer.check_active_rule_pack_version(rule_pack_version=DOWNLOADED_RULE_PACK_VERSION)
 
     repository_runtime = RepositoryRuntime(**json.loads(repository))
 
-    logger.info(f"Received repository to scan via the queue '{rabbitmq_queue}' => "
-                f"{repository_runtime.project_key}/{repository_runtime.repository_name}")
+    logger.info(
+        f"Received repository to scan via the queue '{rabbitmq_queue}' => "
+        f"{repository_runtime.project_key}/{repository_runtime.repository_name}"
+    )
     try:
         vcs_instance = VCS_INSTANCES[repository_runtime.vcs_instance_name]
 
-        repository = Repository(project_key=repository_runtime.project_key,
-                                repository_id=repository_runtime.repository_id,
-                                repository_name=repository_runtime.repository_name,
-                                repository_url=repository_runtime.repository_url,
-                                vcs_instance=vcs_instance.id_
-                                )
+        repository = Repository(
+            project_key=repository_runtime.project_key,
+            repository_id=repository_runtime.repository_id,
+            repository_name=repository_runtime.repository_name,
+            repository_url=repository_runtime.repository_url,
+            vcs_instance=vcs_instance.id_,
+        )
         # Split the include_tags by comma if supplied
         include_tags = env_variables[RESC_INCLUDE_TAGS].split(",") if env_variables[RESC_INCLUDE_TAGS] else None
 
         # Split the ignore_tags by comma if supplied
         ignore_tags = env_variables[RESC_IGNORE_TAGS].split(",") if env_variables[RESC_IGNORE_TAGS] else None
 
         secret_scanner = SecretScanner(
             gitleaks_binary_path=env_variables[GITLEAKS_PATH],
             gitleaks_rules_path=TEMP_RULE_FILE,
             rule_pack_version=active_rule_pack_version,
-            output_plugin=RESTAPIWriter(rws_url=rws_url,
-                                        toml_rule_file_path=TEMP_RULE_FILE,
-                                        include_tags=include_tags,
-                                        ignore_tags=ignore_tags),
+            output_plugin=RESTAPIWriter(
+                rws_url=rws_url,
+                toml_rule_file_path=TEMP_RULE_FILE,
+                include_tags=include_tags,
+                ignore_tags=ignore_tags,
+            ),
             repository=repository,
             username=vcs_instance.username,
             personal_access_token=vcs_instance.token,
-            force_base_scan=os.getenv('FORCE_BASE_SCAN', "false").lower() in "true",
-            latest_commit=repository_runtime.latest_commit
+            force_base_scan=os.getenv("FORCE_BASE_SCAN", "false").lower() in "true",
+            latest_commit=repository_runtime.latest_commit,
         )
 
         secret_scanner.run_repository_scan()
     except KeyError:
-        logger.error(f"No configuration found for vcs instance {repository_runtime.vcs_instance_name}, "
-                     f"unable to scan {repository_runtime.project_key}/{repository_runtime.repository_name}")
+        logger.error(
+            f"No configuration found for vcs instance {repository_runtime.vcs_instance_name}, "
+            f"unable to scan {repository_runtime.project_key}/{repository_runtime.repository_name}"
+        )
```

### Comparing `resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/cli.py` & `resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 from urllib.parse import urlparse
 
 # Third Party
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 # First Party
 from vcs_scanner.common import get_rule_pack_version_from_file, initialise_logs
-from vcs_scanner.constants import CLI_VCS_AZURE, CLI_VCS_BITBUCKET, CLI_VCS_LOCAL_SCAN, LOG_FILE_PATH_CLI
+from vcs_scanner.constants import (
+    CLI_VCS_AZURE,
+    CLI_VCS_BITBUCKET,
+    CLI_VCS_LOCAL_SCAN,
+    LOG_FILE_PATH_CLI,
+)
 from vcs_scanner.helpers.env_default import EnvDefault
 from vcs_scanner.model import RepositoryRuntime
 from vcs_scanner.output_modules.rws_api_writer import RESTAPIWriter
 from vcs_scanner.output_modules.stdout_writer import STDOUTWriter
 from vcs_scanner.secret_scanners.secret_scanner import SecretScanner
 
 logger_config = initialise_logs(LOG_FILE_PATH_CLI)
@@ -36,91 +41,184 @@
 def create_cli_argparser() -> ArgumentParser:
     """
         Create ArgumentParser for CLI arguments
     :return: ArgumentParser.
         ArgumentParser instance with all arguments as expected for RESC
     """
     parser_common = ArgumentParser(add_help=False)
-    parser_common.add_argument("--gitleaks-path", type=pathlib.Path, action=EnvDefault, envvar="RESC_GITLEAKS_PATH",
-                               required=True, help="Path to the gitleaks binary. "
-                                                   "Can also be set via the RESC_GITLEAKS_PATH environment variable")
-    parser_common.add_argument("--gitleaks-rules-path", type=pathlib.Path, action=EnvDefault, required=True,
-                               envvar="RESC_GITLEAKS_RULES_PATH", help="Path to the gitleaks rules file. "
-                                                                       "Can also be set via the "
-                                                                       "RESC_GITLEAKS_RULES_PATH environment variable")
-    parser_common.add_argument("--ignored-blocker-path", type=pathlib.Path, action=EnvDefault, required=False,
-                               envvar="RESC_IGNORED_BLOCKER_PATH", help="Path to the resc-ignore.dsv file. "
-                                                                        "Can also be set via the "
-                                                                        "RESC_IGNORED_BLOCKER_PATH "
-                                                                        "environment variable")
-    parser_common.add_argument("-w", "--exit-code-warn", required=False, action=EnvDefault, default=2, type=int,
-                               envvar="RESC_EXIT_CODE_WARN",
-                               help="Exit code given if CLI encounters findings tagged with Warn, default 2. "
-                                    "Can also be set via the RESC_EXIT_CODE_WARN environment variable")
-    parser_common.add_argument("-b", "--exit-code-block", required=False, action=EnvDefault, default=1, type=int,
-                               envvar="RESC_EXIT_CODE_BLOCK",
-                               help="Exit code given if CLI encounters findings tagged with Block, default 1. "
-                                    "Can also be set via the RESC_EXIT_CODE_BLOCK environment variable")
-    parser_common.add_argument("--include-tags", required=False, action=EnvDefault, type=str,
-                               envvar="RESC_INCLUDE_TAGS",
-                               help="Filter for outputting findings based on specified tags. "
-                                    "Provided as comma separated list. "
-                                    "Can also be set via the RESC_INCLUDE_TAGS environment variable")
-    parser_common.add_argument("--ignore-tags", required=False, action=EnvDefault, type=str,
-                               envvar="RESC_IGNORE_TAGS",
-                               help="Filter for NOT outputting findings based on specified tags. "
-                                    "Provided as comma separated list. "
-                                    "Can also be set via the RESC_IGNORE_TAGS environment variable")
-    parser_common.add_argument("-v", "--verbose", required=False, action="store_true",
-                               help="Enable more verbose logging")
+    parser_common.add_argument(
+        "--gitleaks-path",
+        type=pathlib.Path,
+        action=EnvDefault,
+        envvar="RESC_GITLEAKS_PATH",
+        required=True,
+        help="Path to the gitleaks binary. " "Can also be set via the RESC_GITLEAKS_PATH environment variable",
+    )
+    parser_common.add_argument(
+        "--gitleaks-rules-path",
+        type=pathlib.Path,
+        action=EnvDefault,
+        required=True,
+        envvar="RESC_GITLEAKS_RULES_PATH",
+        help="Path to the gitleaks rules file. "
+        "Can also be set via the "
+        "RESC_GITLEAKS_RULES_PATH environment variable",
+    )
+    parser_common.add_argument(
+        "--ignored-blocker-path",
+        type=pathlib.Path,
+        action=EnvDefault,
+        required=False,
+        envvar="RESC_IGNORED_BLOCKER_PATH",
+        help="Path to the resc-ignore.dsv file. "
+        "Can also be set via the "
+        "RESC_IGNORED_BLOCKER_PATH "
+        "environment variable",
+    )
+    parser_common.add_argument(
+        "-w",
+        "--exit-code-warn",
+        required=False,
+        action=EnvDefault,
+        default=2,
+        type=int,
+        envvar="RESC_EXIT_CODE_WARN",
+        help="Exit code given if CLI encounters findings tagged with Warn, default 2. "
+        "Can also be set via the RESC_EXIT_CODE_WARN environment variable",
+    )
+    parser_common.add_argument(
+        "-b",
+        "--exit-code-block",
+        required=False,
+        action=EnvDefault,
+        default=1,
+        type=int,
+        envvar="RESC_EXIT_CODE_BLOCK",
+        help="Exit code given if CLI encounters findings tagged with Block, default 1. "
+        "Can also be set via the RESC_EXIT_CODE_BLOCK environment variable",
+    )
+    parser_common.add_argument(
+        "--include-tags",
+        required=False,
+        action=EnvDefault,
+        type=str,
+        envvar="RESC_INCLUDE_TAGS",
+        help="Filter for outputting findings based on specified tags. "
+        "Provided as comma separated list. "
+        "Can also be set via the RESC_INCLUDE_TAGS environment variable",
+    )
+    parser_common.add_argument(
+        "--ignore-tags",
+        required=False,
+        action=EnvDefault,
+        type=str,
+        envvar="RESC_IGNORE_TAGS",
+        help="Filter for NOT outputting findings based on specified tags. "
+        "Provided as comma separated list. "
+        "Can also be set via the RESC_IGNORE_TAGS environment variable",
+    )
+    parser_common.add_argument(
+        "-v",
+        "--verbose",
+        required=False,
+        action="store_true",
+        help="Enable more verbose logging",
+    )
 
     repository_common = ArgumentParser(add_help=False)
-    repository_common.add_argument("--repo-name", type=str, required=False, action=EnvDefault, envvar="RESC_REPO_NAME",
-                                   help="The name of the repository. "
-                                        "Can also be set via the RESC_REPO_NAME environment variable")
+    repository_common.add_argument(
+        "--repo-name",
+        type=str,
+        required=False,
+        action=EnvDefault,
+        envvar="RESC_REPO_NAME",
+        help="The name of the repository. " "Can also be set via the RESC_REPO_NAME environment variable",
+    )
     repository_common.add_argument("--force-base-scan", required=False, action="store_true")
 
-    repository_common.add_argument("--rws-url", type=str, required=False, action=EnvDefault, envvar="RESC_RWS_URL",
-                                   help="The URL to the secret tracking service to which the scan results should "
-                                        "be written. "
-                                        "Can also be set via the RESC_RWS_URL environment variable")
+    repository_common.add_argument(
+        "--rws-url",
+        type=str,
+        required=False,
+        action=EnvDefault,
+        envvar="RESC_RWS_URL",
+        help="The URL to the secret tracking service to which the scan results should "
+        "be written. "
+        "Can also be set via the RESC_RWS_URL environment variable",
+    )
 
     parser: ArgumentParser = ArgumentParser()
 
     subparser = parser.add_subparsers(title="command", dest="command", required=True, help="Options dir, repo")
-    directory = subparser.add_parser("dir", description="Scan a directory", help="Scan a directory",
-                                     parents=[parser_common])
+    directory = subparser.add_parser(
+        "dir",
+        description="Scan a directory",
+        help="Scan a directory",
+        parents=[parser_common],
+    )
     repository = subparser.add_parser("repo", description="Scan a Git repository", help="Scan a Git repository")
 
-    directory.add_argument("--dir", type=pathlib.Path, required=True, action=EnvDefault, envvar="RESC_SCAN_PATH",
-                           help="The path to the directory where the scan target. "
-                                "Can also be set via the RESC_SCAN_PATH environment variable")
-
-    repository_subparser = repository.add_subparsers(title="repository_location", dest="repository_location",
-                                                     required=True, help="Options local, remote")
-    repository_local = repository_subparser.add_parser("local", description="Scan a locally already cloned repository",
-                                                       help="Scan a locally already cloned repository",
-                                                       parents=[parser_common, repository_common])
-    repository_remote = repository_subparser.add_parser("remote", description="Scan a remote repository",
-                                                        help="Scan a remote repository",
-                                                        parents=[parser_common, repository_common])
-
-    repository_local.add_argument("--dir", type=pathlib.Path, required=True, action=EnvDefault, envvar="RESC_SCAN_PATH",
-                                  help="The path to the directory where the repo is located. "
-                                       "Can also be set via the RESC_SCAN_PATH environment variable")
-
-    repository_remote.add_argument("--repo-url", type=str, required=True, action=EnvDefault, envvar="RESC_REPO_URL",
-                                   help="url to repository you want to scan. "
-                                        "Can also be set via the RESC_REPO_URL environment variable")
-    repository_remote.add_argument("--username", type=str, required=False,
-                                   action=EnvDefault, envvar="RESC_REPO_USERNAME",
-                                   help="The username used for cloning the repository, "
-                                        "you will be prompted for the password. "
-                                        "Can also be set via the RESC_REPO_USERNAME & RESC_REPO_PASSWORD environment "
-                                        "variable")
+    directory.add_argument(
+        "--dir",
+        type=pathlib.Path,
+        required=True,
+        action=EnvDefault,
+        envvar="RESC_SCAN_PATH",
+        help="The path to the directory where the scan target. "
+        "Can also be set via the RESC_SCAN_PATH environment variable",
+    )
+
+    repository_subparser = repository.add_subparsers(
+        title="repository_location",
+        dest="repository_location",
+        required=True,
+        help="Options local, remote",
+    )
+    repository_local = repository_subparser.add_parser(
+        "local",
+        description="Scan a locally already cloned repository",
+        help="Scan a locally already cloned repository",
+        parents=[parser_common, repository_common],
+    )
+    repository_remote = repository_subparser.add_parser(
+        "remote",
+        description="Scan a remote repository",
+        help="Scan a remote repository",
+        parents=[parser_common, repository_common],
+    )
+
+    repository_local.add_argument(
+        "--dir",
+        type=pathlib.Path,
+        required=True,
+        action=EnvDefault,
+        envvar="RESC_SCAN_PATH",
+        help="The path to the directory where the repo is located. "
+        "Can also be set via the RESC_SCAN_PATH environment variable",
+    )
+
+    repository_remote.add_argument(
+        "--repo-url",
+        type=str,
+        required=True,
+        action=EnvDefault,
+        envvar="RESC_REPO_URL",
+        help="url to repository you want to scan. " "Can also be set via the RESC_REPO_URL environment variable",
+    )
+    repository_remote.add_argument(
+        "--username",
+        type=str,
+        required=False,
+        action=EnvDefault,
+        envvar="RESC_REPO_USERNAME",
+        help="The username used for cloning the repository, "
+        "you will be prompted for the password. "
+        "Can also be set via the RESC_REPO_USERNAME & RESC_REPO_PASSWORD environment "
+        "variable",
+    )
 
     return parser
 
 
 def get_repository_name_from_url(repo_url: str) -> str:
     """
         Get repository name from given URL, taking the last segment of the url as name
@@ -150,16 +248,17 @@
             args.password = os.environ["RESC_REPO_PASSWORD"]
         else:
             args.password = getpass.getpass("Password:")
 
     # Derive the repository name from the directory or url if not provided
     if args.command == "repo" and args.repository_location == "remote" and not args.repo_name:
         args.repo_name = get_repository_name_from_url(args.repo_url)
-    elif args.command == "dir" or \
-            (args.command == "repo" and args.repository_location == "local" and not args.repo_name):
+    elif args.command == "dir" or (
+        args.command == "repo" and args.repository_location == "local" and not args.repo_name
+    ):
         if not os.path.isdir(args.dir.absolute()):
             logger.error(f"The directory {args.dir.absolute()} does not exist")
             valid_arguments = False
         args.repo_name = os.path.split(args.dir.absolute())[1]
 
     # Split the include_tags by comma if supplied
     args.include_tags = args.include_tags.split(",") if args.include_tags else None
@@ -171,15 +270,15 @@
         return False
 
     return args
 
 
 def scan_repository_from_cli():
     """
-        Startup command for the CLI, parsing arguments and starting the process
+    Startup command for the CLI, parsing arguments and starting the process
     """
     parser: ArgumentParser = create_cli_argparser()
     args: Namespace = parser.parse_args()
     args = validate_cli_arguments(args)
 
     if args.verbose:
         logger_config.setLevel(logging.DEBUG)
@@ -208,24 +307,26 @@
     """
     repository = RepositoryRuntime(
         repository_url=FAKE_URL,
         repository_name="local",
         repository_id="local",
         project_key="local",
         vcs_instance_name="vcs_instance_name",
-        latest_commit=FAKE_COMMIT
+        latest_commit=FAKE_COMMIT,
     )
 
-    output_plugin = STDOUTWriter(toml_rule_file_path=args.gitleaks_rules_path,
-                                 exit_code_warn=args.exit_code_warn,
-                                 exit_code_block=args.exit_code_block,
-                                 include_tags=args.include_tags,
-                                 ignore_tags=args.ignore_tags,
-                                 working_dir=args.dir,
-                                 ignore_findings_path=args.ignored_blocker_path)
+    output_plugin = STDOUTWriter(
+        toml_rule_file_path=args.gitleaks_rules_path,
+        exit_code_warn=args.exit_code_warn,
+        exit_code_block=args.exit_code_block,
+        include_tags=args.include_tags,
+        ignore_tags=args.ignore_tags,
+        working_dir=args.dir,
+        ignore_findings_path=args.ignored_blocker_path,
+    )
     with open(args.gitleaks_rules_path, encoding="utf-8") as rule_pack:
         rule_pack_version = get_rule_pack_version_from_file(rule_pack.read())
     if not rule_pack_version:
         rule_pack_version = "0.0.0"
 
     secret_scanner = SecretScanner(
         gitleaks_binary_path=args.gitleaks_path,
@@ -252,32 +353,36 @@
 
     repository = RepositoryRuntime(
         repository_url=args.repo_url,
         repository_name=args.repo_name,
         repository_id=args.repo_name,
         project_key=args.repo_name,
         vcs_instance_name=vcs_name,
-        latest_commit=FAKE_COMMIT
+        latest_commit=FAKE_COMMIT,
     )
 
     if args.rws_url:
-        output_plugin = RESTAPIWriter(rws_url=args.rws_url,
-                                      toml_rule_file_path=args.gitleaks_rules_path,
-                                      include_tags=args.include_tags,
-                                      ignore_tags=args.ignore_tags)
+        output_plugin = RESTAPIWriter(
+            rws_url=args.rws_url,
+            toml_rule_file_path=args.gitleaks_rules_path,
+            include_tags=args.include_tags,
+            ignore_tags=args.ignore_tags,
+        )
         rule_pack_version = output_plugin.download_rule_pack()
 
     else:
-        output_plugin = STDOUTWriter(toml_rule_file_path=args.gitleaks_rules_path,
-                                     exit_code_warn=args.exit_code_warn,
-                                     exit_code_block=args.exit_code_block,
-                                     include_tags=args.include_tags,
-                                     ignore_tags=args.ignore_tags,
-                                     working_dir=args.dir,
-                                     ignore_findings_path=args.ignored_blocker_path)
+        output_plugin = STDOUTWriter(
+            toml_rule_file_path=args.gitleaks_rules_path,
+            exit_code_warn=args.exit_code_warn,
+            exit_code_block=args.exit_code_block,
+            include_tags=args.include_tags,
+            ignore_tags=args.ignore_tags,
+            working_dir=args.dir,
+            ignore_findings_path=args.ignored_blocker_path,
+        )
         with open(args.gitleaks_rules_path, encoding="utf-8") as rule_pack:
             rule_pack_version = get_rule_pack_version_from_file(rule_pack.read())
     if not rule_pack_version:
         rule_pack_version = "0.0.0"
 
     secret_scanner = SecretScanner(
         gitleaks_binary_path=args.gitleaks_path,
@@ -285,15 +390,15 @@
         rule_pack_version=rule_pack_version,
         output_plugin=output_plugin,
         repository=repository.convert_to_repository(vcs_instance_id=1),
         username=args.username,
         personal_access_token=args.password,
         local_path=f"{args.dir.absolute()}",
         force_base_scan=args.force_base_scan,
-        latest_commit="unknown"
+        latest_commit="unknown",
     )
 
     secret_scanner.run_repository_scan()
 
 
 def guess_vcs_provider(repo_url: str) -> VCSProviders:
     """
```

### Comparing `resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/configuration.py` & `resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,9 +79,9 @@
         default=None,
     ),
     EnvironmentVariable(
         RESC_IGNORE_TAGS,
         "Filter for NOT outputting findings based on specified tags. Provided as comma seperated list.",
         required=False,
         default=None,
-    )
+    ),
 ]
```

### Comparing `resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/git_operation.py` & `resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/git_operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 
 # Third Party
 from git import Repo  # noqa: E402
 
 logger = logging.getLogger(__name__)
 
 
-def clone_repository(repository_url: str,
-                     repo_clone_path: str,
-                     username: str = "",
-                     personal_access_token: str = "") -> None:
+def clone_repository(
+    repository_url: str,
+    repo_clone_path: str,
+    username: str = "",
+    personal_access_token: str = "",
+) -> None:
     """
         Clones the given repository
     :param repository_url:
         Repository url to clone
     :param repo_clone_path:
         Path where to clone the repository
     :param username:
```

### Comparing `resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py` & `resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,35 +13,40 @@
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class GitLeaksWrapper:
     SCAN_TMP_DIRECTORY: str = "."
 
-    def __init__(self, rules_filepath: str,
-                 report_filepath: str, repository_path: str,
-                 scan_from: str = None, gitleaks_path: str = "gitleaks",
-                 git_scan: bool = True):
-
+    def __init__(
+        self,
+        rules_filepath: str,
+        report_filepath: str,
+        repository_path: str,
+        scan_from: str = None,
+        gitleaks_path: str = "gitleaks",
+        git_scan: bool = True,
+    ):
         self.rules_filepath = rules_filepath
         self.report_filepath = report_filepath
         self.repository_path = repository_path
         self.scan_from = scan_from
         self.gitleaks_path = gitleaks_path
         self.git_scan = git_scan
 
     def _build_gitleaks_command(self):
-
         # Base scan command
-        command = [f"{self.gitleaks_path}",
-                   "detect",
-                   f"--source={self.repository_path}",
-                   f"--config={self.rules_filepath}",
-                   f"--report-path={self.report_filepath}",
-                   f"--exit-code={LEAKS_FOUND_EXIT_CODE}"]
+        command = [
+            f"{self.gitleaks_path}",
+            "detect",
+            f"--source={self.repository_path}",
+            f"--config={self.rules_filepath}",
+            f"--report-path={self.report_filepath}",
+            f"--exit-code={LEAKS_FOUND_EXIT_CODE}",
+        ]
 
         if not self.git_scan:
             command.append("--no-git")
 
         # Incremental scan command
         if self.scan_from:
             command.append(f"--log-opts={self.scan_from}..")
@@ -52,31 +57,33 @@
         :return: Output.
             If Successful, a list of FindingCreate objects is returned.
             Otherwise, a None object is returned
         """
         try:
             result = subprocess.run(
                 self._build_gitleaks_command(),
-                check=False, stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE
+                check=False,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
             )
 
             exitcode = result.returncode
             if exitcode == NO_LEAKS_FOUND_EXIT_CODE:
                 return []
             if exitcode == LEAKS_FOUND_EXIT_CODE:
                 return self._parse_output(self.report_filepath)
 
             error_output = result.stderr.decode("utf-8")
             logger.error(f"GitLeaks exited with an unexpected code: {exitcode}. Output: {error_output}")
             return None
 
         except subprocess.CalledProcessError as called_process_error:
             logger.error(
-                f"Error encountered while running the gitleaks process: {called_process_error.stdout.decode('utf-8')}")
+                f"Error encountered while running the gitleaks process: {called_process_error.stdout.decode('utf-8')}"
+            )
             return None
         except FileNotFoundError as error:
             logger.error(f"Unable to locate a file: {error}")
             return None
 
     @staticmethod
     def _calculate_permanent_leak_url(leak_url: str, repository: str, commit_id: str) -> str:
@@ -101,16 +108,17 @@
         new_url = new_url.replace(f"/{commit_id}/", f"/{commit_id}#")
 
         return new_url
 
     @staticmethod
     def _is_valid_timestamp(timestamp: str) -> Optional[datetime.datetime]:
         try:
-            converted_timestamp: Optional[datetime.datetime] = \
-                datetime.datetime.strptime(timestamp, "%Y-%m-%dT%H:%M:%S%z")
+            converted_timestamp: Optional[datetime.datetime] = datetime.datetime.strptime(
+                timestamp, "%Y-%m-%dT%H:%M:%S%z"
+            )
         except ValueError:
             converted_timestamp = None
         return converted_timestamp
 
     @classmethod
     def _parse_output(cls, file_path: str) -> List[FindingBase]:
         """
@@ -123,21 +131,23 @@
             results = json.load(report_file)
 
         for result in results:
             commit_timestamp = cls._is_valid_timestamp(result["Date"])
             if not commit_timestamp:
                 logger.debug(f"{result['Date']} has an unexpected date format. Expected ISO 8601")
                 commit_timestamp = datetime.datetime.now()
-            finding = FindingBase(file_path=result["File"],
-                                  line_number=result["StartLine"],
-                                  column_start=result["StartColumn"],
-                                  column_end=result["EndColumn"],
-                                  email=result["Email"],
-                                  author=result["Author"],
-                                  commit_id=result["Commit"],
-                                  commit_message=result["Message"],
-                                  commit_timestamp=commit_timestamp,
-                                  rule_name=result["RuleID"])
+            finding = FindingBase(
+                file_path=result["File"],
+                line_number=result["StartLine"],
+                column_start=result["StartColumn"],
+                column_end=result["EndColumn"],
+                email=result["Email"],
+                author=result["Author"],
+                commit_id=result["Commit"],
+                commit_message=result["Message"],
+                commit_timestamp=commit_timestamp,
+                rule_name=result["RuleID"],
+            )
 
             findings.append(finding)
 
         return findings
```

### Comparing `resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/secret_scanner.py` & `resc_vcs_scanner-3.1.0/src/vcs_scanner/secret_scanners/secret_scanner.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,28 +25,28 @@
 LEAKS_FOUND_EXIT_CODE = 42
 NO_LEAKS_FOUND_EXIT_CODE = 0
 
 logger = logging.getLogger(__name__)
 
 
 class SecretScanner(RESCWorker):  # pylint: disable=R0902
-
-    def __init__(self,
-                 gitleaks_binary_path: str,
-                 gitleaks_rules_path: str,
-                 rule_pack_version: str,
-                 output_plugin: OutputModule,
-                 repository: Repository,
-                 username: str,
-                 personal_access_token: str,
-                 scan_tmp_directory: str = ".",
-                 local_path: str = None,
-                 force_base_scan: bool = False,
-                 latest_commit: str = None):
-
+    def __init__(
+        self,
+        gitleaks_binary_path: str,
+        gitleaks_rules_path: str,
+        rule_pack_version: str,
+        output_plugin: OutputModule,
+        repository: Repository,
+        username: str,
+        personal_access_token: str,
+        scan_tmp_directory: str = ".",
+        local_path: str = None,
+        force_base_scan: bool = False,
+        latest_commit: str = None,
+    ):
         self.gitleaks_rules_path: str = gitleaks_rules_path
         self.gitleaks_binary_path: str = gitleaks_binary_path
         self.rule_pack_version: str = rule_pack_version
         self._output_module: OutputModule = output_plugin
         self._scan_tmp_directory: str = scan_tmp_directory
         self.repository: Repository = repository
         self.username: str = username
@@ -57,99 +57,123 @@
         if self.local_path:
             self.repo_display_name = self.local_path.replace(".", "_").replace("/", "_")
         else:
             self.repo_display_name = self.repository.repository_url
 
     def clone_repo(self) -> str:
         repo_clone_path = f"{self._scan_tmp_directory}/{self.repository.repository_name}"
-        clone_repository(self.repository.repository_url, repo_clone_path, username=self.username,
-                         personal_access_token=self.personal_access_token)
+        clone_repository(
+            self.repository.repository_url,
+            repo_clone_path,
+            username=self.username,
+            personal_access_token=self.personal_access_token,
+        )
         return repo_clone_path
 
     def run_repository_scan(self) -> None:
         if not self.latest_commit:
             # There is no latest commit for this repository, assuming that its empty
-            logger.info(f"Skipping scanning of {self.repository.project_key}/{self.repository.repository_name} "
-                        f"there are no commits")
+            logger.info(
+                f"Skipping scanning of {self.repository.project_key}/{self.repository.repository_name} "
+                f"there are no commits"
+            )
             return
         logger.info(
             f"Started task for scanning {self.repository.repository_name} using "
-            f"rule pack version: {self.rule_pack_version}")
+            f"rule pack version: {self.rule_pack_version}"
+        )
 
         # Insert in to repository table
         created_repository = self._output_module.write_repository(self.repository)
         if not created_repository:
-            logger.error(f"Error processing "
-                         f"{self.repository.repository_name}."
-                         f" Error details: unable to create repository: {created_repository}")
+            logger.error(
+                f"Error processing "
+                f"{self.repository.repository_name}."
+                f" Error details: unable to create repository: {created_repository}"
+            )
             return
 
         logger.info(f"Scanning repository {self.repository.project_key}/{self.repository.repository_name}")
 
         # Get last scanned commit for the repository
         last_scan_for_repository = self._output_module.get_last_scan_for_repository(repository=created_repository)
         last_scanned_commit = last_scan_for_repository.last_scanned_commit if last_scan_for_repository else None
-        scan_type_to_run = self.determine_scan_type(latest_commit=self.latest_commit,
-                                                    last_scan_for_repository=last_scan_for_repository)
+        scan_type_to_run = self.determine_scan_type(
+            latest_commit=self.latest_commit,
+            last_scan_for_repository=last_scan_for_repository,
+        )
 
         if scan_type_to_run:
             # Insert in to scan table
             scan_timestamp_start = datetime.utcnow()
             created_scan = self._output_module.write_scan(
-                scan_type_to_run, self.latest_commit,
-                scan_timestamp_start.isoformat(), created_repository,
-                rule_pack=self.rule_pack_version)
+                scan_type_to_run,
+                self.latest_commit,
+                scan_timestamp_start.isoformat(),
+                created_repository,
+                rule_pack=self.rule_pack_version,
+            )
             if not created_scan:
-                logger.error(f"Error processing {self.repository.project_key}/{self.repository.repository_name} "
-                             f"Error details: unable to create scan object")
+                logger.error(
+                    f"Error processing {self.repository.project_key}/{self.repository.repository_name} "
+                    f"Error details: unable to create scan object"
+                )
                 return
 
             # Clone and run scan upon the repository
             if not self.local_path:
                 repo_clone_path: str = self.clone_repo()
             else:
                 repo_clone_path = self.local_path
 
             findings = self.scan_repo(scan_type_to_run, last_scanned_commit, repo_clone_path)
             scan_timestamp_end = datetime.utcnow()
-            logger.info(f"Running {scan_type_to_run} scan on repository "
-                        f"{self.repository.project_key}/{self.repository.repository_name}"
-                        f" took {scan_timestamp_end - scan_timestamp_start} ms.")
+            logger.info(
+                f"Running {scan_type_to_run} scan on repository "
+                f"{self.repository.project_key}/{self.repository.repository_name}"
+                f" took {scan_timestamp_end - scan_timestamp_start} ms."
+            )
 
             if findings:
                 logger.info(f"Scan completed: {len(findings)} findings were found.")
-                self._output_module.write_findings(repository_id=created_repository.id_, scan_id=created_scan.id_,
-                                                   scan_findings=findings)
+                self._output_module.write_findings(
+                    repository_id=created_repository.id_,
+                    scan_id=created_scan.id_,
+                    scan_findings=findings,
+                )
             else:
-                logger.info("No findings registered in "
-                            f"{self.repository.project_key}/{self.repository.repository_name}")
+                logger.info(
+                    "No findings registered in " f"{self.repository.project_key}/{self.repository.repository_name}"
+                )
         else:
-            logger.info(f"Skipped {scan_type_to_run} scanning on repository: "
-                        f"{self.repository.project_key}/{self.repository.repository_name} no new commits found.")
+            logger.info(
+                f"Skipped {scan_type_to_run} scanning on repository: "
+                f"{self.repository.project_key}/{self.repository.repository_name} no new commits found."
+            )
 
     def run_directory_scan(self) -> None:
         """
-            Scan the given non-git directory, set in the self.local_path variable
+        Scan the given non-git directory, set in the self.local_path variable
         """
         logger.info(f"Started task for scanning {self.local_path} using rule pack version: {self.rule_pack_version}")
 
         scan_timestamp_start = datetime.utcnow()
         findings = self.scan_directory(self.local_path)
         scan_timestamp_end = datetime.utcnow()
         logger.info(f"Running local scan on {self.local_path} took {scan_timestamp_end - scan_timestamp_start} ms.")
 
         if findings:
             logger.info(f"Scan completed: {len(findings)} findings were found.")
             self._output_module.write_findings(repository_id=0, scan_id=0, scan_findings=findings)
         else:
             logger.info(f"No findings registered in {self.local_path}.")
 
-    def scan_repo(self, scan_type_to_run: str, last_scanned_commit: str, repo_clone_path: str) \
-            -> Optional[List[FindingBase]]:
-
+    def scan_repo(
+        self, scan_type_to_run: str, last_scanned_commit: str, repo_clone_path: str
+    ) -> Optional[List[FindingBase]]:
         """
             Clone and scan the given repository
         :param repo_clone_path:
             Directory path where the repository has already been cloned
         :param scan_type_to_run:
             Type of scan to run (Base or Incremental)
         :param last_scanned_commit:
@@ -161,38 +185,39 @@
 
         logger.debug(f"Started scanning {self.repo_display_name}")
         if not self.local_path:
             report_filepath = f"{self._scan_tmp_directory}/{repo_clone_path}_{str(uuid.uuid4().hex)}.json"
         else:
             report_filepath = f"{self.local_path}/{self.repo_display_name}_{str(uuid.uuid4().hex)}.json"
         try:
-
             if scan_type_to_run == ScanType.BASE:
                 scan_from = None
             elif scan_type_to_run == ScanType.INCREMENTAL and last_scanned_commit:
                 scan_from = last_scanned_commit
             else:
                 scan_from = None
 
             gitleaks_command = GitLeaksWrapper(
                 scan_from=scan_from,
                 gitleaks_path=self.gitleaks_binary_path,
                 repository_path=repo_clone_path,
                 rules_filepath=self.gitleaks_rules_path,
-                report_filepath=report_filepath)
+                report_filepath=report_filepath,
+            )
 
             before_scan = time.time()
             findings: Optional[List[FindingBase]] = gitleaks_command.start_scan()
             after_scan = time.time()
             scan_duration = int(after_scan - before_scan)
             logger.info(f"scan of repository {repo_clone_path} took {scan_duration} seconds")
             return findings
         except BaseException as error:
-            logger.error(f"An exception occurred while scanning repository {self.repository.repository_url} "
-                         f"error: {error}")
+            logger.error(
+                f"An exception occurred while scanning repository {self.repository.repository_url} " f"error: {error}"
+            )
         finally:
             # Make sure the tempfile and repo cloned path removed
             logger.debug(f"Cleaning up the temporary report: {report_filepath}")
             if os.path.exists(report_filepath):
                 os.remove(report_filepath)
             if repo_clone_path and not self.local_path and os.path.exists(repo_clone_path):
                 logger.debug(f"Cleaning up the repository cloned directory: {repo_clone_path}")
@@ -215,15 +240,15 @@
         try:
             gitleaks_command = GitLeaksWrapper(
                 scan_from=None,
                 gitleaks_path=self.gitleaks_binary_path,
                 repository_path=directory_path,
                 rules_filepath=self.gitleaks_rules_path,
                 report_filepath=report_filepath,
-                git_scan=False
+                git_scan=False,
             )
 
             before_scan = time.time()
             findings: Optional[List[FindingBase]] = gitleaks_command.start_scan()
             after_scan = time.time()
             scan_duration = int(after_scan - before_scan)
             logger.info(f"scan of repository {directory_path} took {scan_duration} seconds")
```

### Comparing `resc_vcs_scanner-3.0.1/src/vcs_scanner/static/logging.ini` & `resc_vcs_scanner-3.1.0/src/vcs_scanner/static/logging.ini`

 * *Files identical despite different names*

