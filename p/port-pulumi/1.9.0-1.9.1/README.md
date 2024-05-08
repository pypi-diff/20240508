# Comparing `tmp/port_pulumi-1.9.0.tar.gz` & `tmp/port_pulumi-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_pulumi-1.9.0.tar", last modified: Mon Jan 15 15:45:57 2024, max compression
+gzip compressed data, was "port_pulumi-1.9.1.tar", last modified: Sun Jan 21 14:27:02 2024, max compression
```

## Comparing `port_pulumi-1.9.0.tar` & `port_pulumi-1.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:45:57.179651 port_pulumi-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-01-15 15:45:57.179651 port_pulumi-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:45:57.179651 port_pulumi-1.9.0/port_pulumi/
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   131532 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    40529 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/aggregation_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/aggregation_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    34831 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/blueprint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:45:57.179651 port_pulumi-1.9.0/port_pulumi/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    22683 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)   107602 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15511 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/scorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    22651 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/port_pulumi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:45:57.179651 port_pulumi-1.9.0/port_pulumi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-01-15 15:45:57.000000 port_pulumi-1.9.0/port_pulumi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-01-15 15:45:57.000000 port_pulumi-1.9.0/port_pulumi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 15:45:57.000000 port_pulumi-1.9.0/port_pulumi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 15:45:57.000000 port_pulumi-1.9.0/port_pulumi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-15 15:45:57.000000 port_pulumi-1.9.0/port_pulumi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-15 15:45:57.000000 port_pulumi-1.9.0/port_pulumi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-15 15:45:57.179651 port_pulumi-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-01-15 15:45:56.000000 port_pulumi-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 14:27:02.457555 port_pulumi-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-01-21 14:27:02.457555 port_pulumi-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 14:27:02.457555 port_pulumi-1.9.1/port_pulumi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131924 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40529 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/aggregation_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/aggregation_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34831 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/blueprint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 14:27:02.457555 port_pulumi-1.9.1/port_pulumi/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22683 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107846 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15511 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/scorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22651 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 14:27:02.457555 port_pulumi-1.9.1/port_pulumi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/port_pulumi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-21 14:27:02.457555 port_pulumi-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-01-21 14:27:02.000000 port_pulumi-1.9.1/setup.py
```

### Comparing `port_pulumi-1.9.0/PKG-INFO` & `port_pulumi-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port_pulumi
-Version: 1.9.0
+Version: 1.9.1
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `port_pulumi-1.9.0/README.md` & `port_pulumi-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/port_pulumi/__init__.py` & `port_pulumi-1.9.1/port_pulumi/__init__.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/port_pulumi/_inputs.py` & `port_pulumi-1.9.1/port_pulumi/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,26 +83,38 @@
     def __init__(__self__):
         pass
 
 
 @pulumi.input_type
 class ActionApprovalWebhookNotificationArgs:
     def __init__(__self__, *,
-                 url: pulumi.Input[str]):
+                 url: pulumi.Input[str],
+                 format: Optional[pulumi.Input[str]] = None):
         pulumi.set(__self__, "url", url)
+        if format is not None:
+            pulumi.set(__self__, "format", format)
 
     @property
     @pulumi.getter
     def url(self) -> pulumi.Input[str]:
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: pulumi.Input[str]):
         pulumi.set(self, "url", value)
 
+    @property
+    @pulumi.getter
+    def format(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "format")
+
+    @format.setter
+    def format(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "format", value)
+
 
 @pulumi.input_type
 class ActionAzureMethodArgs:
     def __init__(__self__, *,
                  org: pulumi.Input[str],
                  webhook: pulumi.Input[str]):
         pulumi.set(__self__, "org", org)
```

### Comparing `port_pulumi-1.9.0/port_pulumi/_utilities.py` & `port_pulumi-1.9.1/port_pulumi/_utilities.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/port_pulumi/action.py` & `port_pulumi-1.9.1/port_pulumi/action.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/port_pulumi/action_permissions.py` & `port_pulumi-1.9.1/port_pulumi/action_permissions.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/port_pulumi/aggregation_properties.py` & `port_pulumi-1.9.1/port_pulumi/aggregation_properties.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/port_pulumi/aggregation_property.py` & `port_pulumi-1.9.1/port_pulumi/aggregation_property.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/port_pulumi/blueprint.py` & `port_pulumi-1.9.1/port_pulumi/blueprint.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/port_pulumi/config/vars.py` & `port_pulumi-1.9.1/port_pulumi/config/vars.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/port_pulumi/entity.py` & `port_pulumi-1.9.1/port_pulumi/entity.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/port_pulumi/outputs.py` & `port_pulumi-1.9.1/port_pulumi/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,22 +84,30 @@
     def __init__(__self__):
         pass
 
 
 @pulumi.output_type
 class ActionApprovalWebhookNotification(dict):
     def __init__(__self__, *,
-                 url: str):
+                 url: str,
+                 format: Optional[str] = None):
         pulumi.set(__self__, "url", url)
+        if format is not None:
+            pulumi.set(__self__, "format", format)
 
     @property
     @pulumi.getter
     def url(self) -> str:
         return pulumi.get(self, "url")
 
+    @property
+    @pulumi.getter
+    def format(self) -> Optional[str]:
+        return pulumi.get(self, "format")
+
 
 @pulumi.output_type
 class ActionAzureMethod(dict):
     def __init__(__self__, *,
                  org: str,
                  webhook: str):
         pulumi.set(__self__, "org", org)
```

### Comparing `port_pulumi-1.9.0/port_pulumi/provider.py` & `port_pulumi-1.9.1/port_pulumi/provider.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/port_pulumi/scorecard.py` & `port_pulumi-1.9.1/port_pulumi/scorecard.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/port_pulumi/team.py` & `port_pulumi-1.9.1/port_pulumi/team.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/port_pulumi/webhook.py` & `port_pulumi-1.9.1/port_pulumi/webhook.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/port_pulumi.egg-info/PKG-INFO` & `port_pulumi-1.9.1/port_pulumi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-pulumi
-Version: 1.9.0
+Version: 1.9.1
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `port_pulumi-1.9.0/port_pulumi.egg-info/SOURCES.txt` & `port_pulumi-1.9.1/port_pulumi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.9.0/setup.py` & `port_pulumi-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.9.0"
+VERSION = "1.9.1"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "port Pulumi Package - Development Version"
```

