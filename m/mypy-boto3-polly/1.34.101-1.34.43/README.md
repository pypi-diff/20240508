# Comparing `tmp/mypy_boto3_polly-1.34.101.tar.gz` & `tmp/mypy-boto3-polly-1.34.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_polly-1.34.101.tar", last modified: Wed May  8 19:33:03 2024, max compression
+gzip compressed data, was "mypy-boto3-polly-1.34.43.tar", last modified: Thu Feb 15 20:47:30 2024, max compression
```

## Comparing `mypy_boto3_polly-1.34.101.tar` & `mypy-boto3-polly-1.34.43.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:33:03.288212 mypy_boto3_polly-1.34.101/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12886 2024-05-08 19:33:03.288212 mypy_boto3_polly-1.34.101/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:33:03.288212 mypy_boto3_polly-1.34.101/mypy_boto3_polly/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11435 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:33:03.288212 mypy_boto3_polly-1.34.101/mypy_boto3_polly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12886 2024-05-08 19:33:03.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-08 19:33:03.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:33:03.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:33:03.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 19:33:03.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 19:33:03.000000 mypy_boto3_polly-1.34.101/mypy_boto3_polly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:33:03.288212 mypy_boto3_polly-1.34.101/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-08 19:32:49.000000 mypy_boto3_polly-1.34.101/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 20:47:30.085511 mypy-boto3-polly-1.34.43/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-15 20:46:57.000000 mypy-boto3-polly-1.34.43/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12883 2024-02-15 20:47:30.085511 mypy-boto3-polly-1.34.43/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-02-15 20:46:57.000000 mypy-boto3-polly-1.34.43/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 20:47:30.085511 mypy-boto3-polly-1.34.43/mypy_boto3_polly/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-15 20:46:57.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-15 20:46:57.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-02-15 20:46:57.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-02-15 20:46:57.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11435 2024-02-15 20:46:57.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-02-15 20:46:57.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-02-15 20:46:57.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-02-15 20:46:57.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-02-15 20:46:57.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 20:46:57.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-02-15 20:46:58.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-02-15 20:46:58.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-15 20:46:57.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 20:47:30.085511 mypy-boto3-polly-1.34.43/mypy_boto3_polly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12883 2024-02-15 20:47:30.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-02-15 20:47:30.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 20:47:30.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 20:47:30.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-15 20:47:30.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-15 20:47:30.000000 mypy-boto3-polly-1.34.43/mypy_boto3_polly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 20:47:30.085511 mypy-boto3-polly-1.34.43/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-02-15 20:46:56.000000 mypy-boto3-polly-1.34.43/setup.py
```

### Comparing `mypy_boto3_polly-1.34.101/LICENSE` & `mypy-boto3-polly-1.34.43/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_polly-1.34.101/PKG-INFO` & `mypy-boto3-polly-1.34.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-polly
-Version: 1.34.101
-Summary: Type annotations for boto3.Polly 1.34.101 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.43
+Summary: Type annotations for boto3.Polly 1.34.43 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-polly)](https://pepy.tech/project/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.34.101](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.34.43](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_polly-1.34.101/README.md` & `mypy-boto3-polly-1.34.43/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-polly)](https://pepy.tech/project/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.34.101](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.34.43](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_polly-1.34.101/mypy_boto3_polly/__init__.py` & `mypy-boto3-polly-1.34.43/mypy_boto3_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_polly-1.34.101/mypy_boto3_polly/__init__.pyi` & `mypy-boto3-polly-1.34.43/mypy_boto3_polly/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_polly-1.34.101/mypy_boto3_polly/__main__.py` & `mypy-boto3-polly-1.34.43/mypy_boto3_polly/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Polly 1.34.101\n"
-        "Version:         1.34.101\n"
-        "Builder version: 7.24.0\n"
+        "Type annotations for boto3.Polly 1.34.43\n"
+        "Version:         1.34.43\n"
+        "Builder version: 7.23.1\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.101")
+    print("1.34.43")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_polly-1.34.101/mypy_boto3_polly/client.py` & `mypy-boto3-polly-1.34.43/mypy_boto3_polly/client.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_polly-1.34.101/mypy_boto3_polly/client.pyi` & `mypy-boto3-polly-1.34.43/mypy_boto3_polly/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_polly-1.34.101/mypy_boto3_polly/literals.py` & `mypy-boto3-polly-1.34.43/mypy_boto3_polly/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 DescribeVoicesPaginatorName = Literal["describe_voices"]
-EngineType = Literal["generative", "long-form", "neural", "standard"]
+EngineType = Literal["long-form", "neural", "standard"]
 GenderType = Literal["Female", "Male"]
 LanguageCodeType = Literal[
     "ar-AE",
     "arb",
     "ca-ES",
     "cmn-CN",
     "cy-GB",
@@ -228,15 +228,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -254,15 +253,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -275,26 +273,24 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -355,14 +351,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -491,15 +488,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -543,15 +539,14 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy_boto3_polly-1.34.101/mypy_boto3_polly/literals.pyi` & `mypy-boto3-polly-1.34.43/mypy_boto3_polly/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 DescribeVoicesPaginatorName = Literal["describe_voices"]
-EngineType = Literal["generative", "long-form", "neural", "standard"]
+EngineType = Literal["long-form", "neural", "standard"]
 GenderType = Literal["Female", "Male"]
 LanguageCodeType = Literal[
     "ar-AE",
     "arb",
     "ca-ES",
     "cmn-CN",
     "cy-GB",
@@ -228,15 +228,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -254,15 +253,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -275,26 +273,24 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -355,14 +351,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -491,15 +488,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -543,15 +539,14 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy_boto3_polly-1.34.101/mypy_boto3_polly/paginator.py` & `mypy-boto3-polly-1.34.43/mypy_boto3_polly/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_polly-1.34.101/mypy_boto3_polly/paginator.pyi` & `mypy-boto3-polly-1.34.43/mypy_boto3_polly/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_polly-1.34.101/mypy_boto3_polly/type_defs.py` & `mypy-boto3-polly-1.34.43/mypy_boto3_polly/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,18 +90,18 @@
         "NextToken": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
+        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
-        "HostId": NotRequired[str],
     },
 )
 VoiceTypeDef = TypedDict(
     "VoiceTypeDef",
     {
         "Gender": NotRequired[GenderType],
         "Id": NotRequired[VoiceIdType],
@@ -245,16 +245,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVoicesOutputTypeDef = TypedDict(
     "DescribeVoicesOutputTypeDef",
     {
         "Voices": List[VoiceTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 LexiconDescriptionTypeDef = TypedDict(
     "LexiconDescriptionTypeDef",
     {
         "Name": NotRequired[str],
         "Attributes": NotRequired[LexiconAttributesTypeDef],
@@ -274,27 +274,27 @@
         "SynthesisTask": SynthesisTaskTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListSpeechSynthesisTasksOutputTypeDef = TypedDict(
     "ListSpeechSynthesisTasksOutputTypeDef",
     {
+        "NextToken": str,
         "SynthesisTasks": List[SynthesisTaskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 StartSpeechSynthesisTaskOutputTypeDef = TypedDict(
     "StartSpeechSynthesisTaskOutputTypeDef",
     {
         "SynthesisTask": SynthesisTaskTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListLexiconsOutputTypeDef = TypedDict(
     "ListLexiconsOutputTypeDef",
     {
         "Lexicons": List[LexiconDescriptionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_polly-1.34.101/mypy_boto3_polly/type_defs.pyi` & `mypy-boto3-polly-1.34.43/mypy_boto3_polly/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -90,18 +90,18 @@
         "NextToken": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
+        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
-        "HostId": NotRequired[str],
     },
 )
 VoiceTypeDef = TypedDict(
     "VoiceTypeDef",
     {
         "Gender": NotRequired[GenderType],
         "Id": NotRequired[VoiceIdType],
@@ -245,16 +245,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeVoicesOutputTypeDef = TypedDict(
     "DescribeVoicesOutputTypeDef",
     {
         "Voices": List[VoiceTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 LexiconDescriptionTypeDef = TypedDict(
     "LexiconDescriptionTypeDef",
     {
         "Name": NotRequired[str],
         "Attributes": NotRequired[LexiconAttributesTypeDef],
@@ -274,27 +274,27 @@
         "SynthesisTask": SynthesisTaskTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListSpeechSynthesisTasksOutputTypeDef = TypedDict(
     "ListSpeechSynthesisTasksOutputTypeDef",
     {
+        "NextToken": str,
         "SynthesisTasks": List[SynthesisTaskTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 StartSpeechSynthesisTaskOutputTypeDef = TypedDict(
     "StartSpeechSynthesisTaskOutputTypeDef",
     {
         "SynthesisTask": SynthesisTaskTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListLexiconsOutputTypeDef = TypedDict(
     "ListLexiconsOutputTypeDef",
     {
         "Lexicons": List[LexiconDescriptionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_polly-1.34.101/mypy_boto3_polly.egg-info/PKG-INFO` & `mypy-boto3-polly-1.34.43/mypy_boto3_polly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-polly
-Version: 1.34.101
-Summary: Type annotations for boto3.Polly 1.34.101 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.43
+Summary: Type annotations for boto3.Polly 1.34.43 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-polly)](https://pepy.tech/project/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.34.101](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.34.43](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_polly-1.34.101/mypy_boto3_polly.egg-info/SOURCES.txt` & `mypy-boto3-polly-1.34.43/mypy_boto3_polly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_polly-1.34.101/setup.py` & `mypy-boto3-polly-1.34.43/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-polly",
-    version="1.34.101",
+    version="1.34.43",
     packages=["mypy_boto3_polly"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Polly 1.34.101 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.Polly 1.34.43 service generated with mypy-boto3-builder 7.23.1",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

