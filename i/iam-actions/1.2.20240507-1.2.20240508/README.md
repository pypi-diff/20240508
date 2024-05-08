# Comparing `tmp/iam_actions-1.2.20240507.tar.gz` & `tmp/iam_actions-1.2.20240508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240507.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240508.tar", max compression
```

## Comparing `iam_actions-1.2.20240507.tar` & `iam_actions-1.2.20240508.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-07 02:25:57.948188 iam_actions-1.2.20240507/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-07 02:25:57.948188 iam_actions-1.2.20240507/README.md
--rw-r--r--   0        0        0      228 2024-05-07 02:25:57.948188 iam_actions-1.2.20240507/iam_actions/__init__.py
--rw-r--r--   0        0        0  4826404 2024-05-07 02:28:01.812222 iam_actions-1.2.20240507/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-07 02:25:57.948188 iam_actions-1.2.20240507/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-07 02:25:57.948188 iam_actions-1.2.20240507/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-07 02:25:57.948188 iam_actions-1.2.20240507/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-07 02:25:57.948188 iam_actions-1.2.20240507/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-07 02:25:57.948188 iam_actions-1.2.20240507/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-07 02:25:57.948188 iam_actions-1.2.20240507/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-07 02:25:57.948188 iam_actions-1.2.20240507/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-07 02:25:57.948188 iam_actions-1.2.20240507/iam_actions/generate/services.py
--rw-r--r--   0        0        0   627782 2024-05-07 02:28:01.812222 iam_actions-1.2.20240507/iam_actions/policies.json
--rw-r--r--   0        0        0   209418 2024-05-07 02:28:01.812222 iam_actions-1.2.20240507/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   609172 2024-05-07 02:28:01.812222 iam_actions-1.2.20240507/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-07 02:28:02.516223 iam_actions-1.2.20240507/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240507/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240507/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-08 02:09:35.737366 iam_actions-1.2.20240508/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-08 02:09:35.737366 iam_actions-1.2.20240508/README.md
+-rw-r--r--   0        0        0      228 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4827367 2024-05-08 02:11:21.373174 iam_actions-1.2.20240508/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-08 02:09:35.741366 iam_actions-1.2.20240508/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   628076 2024-05-08 02:11:21.373174 iam_actions-1.2.20240508/iam_actions/policies.json
+-rw-r--r--   0        0        0   209418 2024-05-08 02:11:21.373174 iam_actions-1.2.20240508/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   609432 2024-05-08 02:11:21.373174 iam_actions-1.2.20240508/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-08 02:11:22.033173 iam_actions-1.2.20240508/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240508/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240508/PKG-INFO
```

### Comparing `iam_actions-1.2.20240507/LICENSE` & `iam_actions-1.2.20240508/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240507/README.md` & `iam_actions-1.2.20240508/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240507/iam_actions/actions.json` & `iam_actions-1.2.20240508/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999680461313731%*

 * *Differences: {"'budgets'": "{'ListTagsForResource': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *              "'ListTagsForResource'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *              "AWS'), ('orphan', False), ('resources', [])]), 'UntagResource': "*

 * *              "OrderedDict([('access_level', 'Undocumented'), ('action', 'UntagResource'), "*

 * *              "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', "*

 * *              "False), ('resources', [])]), ' […]*

```diff
@@ -15340,24 +15340,48 @@
             "condition_keys": [],
             "description": "Grants permission to initiate a pending budget action as well as reverse a previously executed budget action",
             "orphan": false,
             "resources": [
                 "budgetAction"
             ]
         },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ModifyBudget": {
             "access_level": "Write",
             "action": "ModifyBudget",
             "condition_keys": [],
             "description": "Grants permission to modify budgets and budget details",
             "orphan": false,
             "resources": [
                 "budget"
             ]
         },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateBudgetAction": {
             "access_level": "Write",
             "action": "UpdateBudgetAction",
             "condition_keys": [],
             "description": "Grants permission to update the details of a specific budget action associated with a budget",
             "orphan": false,
             "resources": [
@@ -109183,15 +109207,16 @@
         },
         "CreateCluster": {
             "access_level": "Write",
             "action": "CreateCluster",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:TagKeys",
+                "memorydb:TLSEnabled"
             ],
             "description": "Grants permissions to create a cluster",
             "orphan": false,
             "resources": [
                 "acl",
                 "parametergroup",
                 "snapshot",
@@ -109235,15 +109260,16 @@
             "resources": []
         },
         "CreateUser": {
             "access_level": "Write",
             "action": "CreateUser",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:TagKeys",
+                "memorydb:UserAuthenticationMode"
             ],
             "description": "Grants permissions to create a new user",
             "orphan": false,
             "resources": []
         },
         "DeleteAcl": {
             "access_level": "Write",
@@ -109602,15 +109628,16 @@
                 "subnetgroup"
             ]
         },
         "UpdateUser": {
             "access_level": "Write",
             "action": "UpdateUser",
             "condition_keys": [
-                "aws:ResourceTag/${TagKey}"
+                "aws:ResourceTag/${TagKey}",
+                "memorydb:UserAuthenticationMode"
             ],
             "description": "Grants permissions to update a user",
             "orphan": false,
             "resources": [
                 "user"
             ]
         }
@@ -164045,14 +164072,22 @@
             "orphan": false,
             "resources": [
                 "parallel-data"
             ]
         }
     },
     "trustedadvisor": {
+        "BatchUpdateRecommendationResourceExclusion": {
+            "access_level": "Undocumented",
+            "action": "BatchUpdateRecommendationResourceExclusion",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateEngagement": {
             "access_level": "Write",
             "action": "CreateEngagement",
             "condition_keys": [],
             "description": "Grants permission to create an engagement",
             "orphan": false,
             "resources": []
```

### Comparing `iam_actions-1.2.20240507/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240508/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240507/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240508/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240507/iam_actions/generate/generate.py` & `iam_actions-1.2.20240508/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240507/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240508/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240507/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240508/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240507/iam_actions/generate/services.py` & `iam_actions-1.2.20240508/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240507/iam_actions/policies.json` & `iam_actions-1.2.20240508/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999730956391542%*

 * *Differences: {"'serviceMap'": "{'AWS Trusted Advisor': {'Actions': {insert: [(0, "*

 * *                 "'BatchUpdateRecommendationResourceExclusion')]}}, 'AWS Budget Service': "*

 * *                 "{'Actions': {insert: [(7, 'ListTagsForResource'), (9, 'TagResource'), (10, "*

 * *                 "'UntagResource')]}, 'conditionKeys': ['aws:RequestTag/${TagKey}', "*

 * *                 "'aws:ResourceTag/${TagKey}', 'aws:TagKeys']}, 'Amazon MemoryDB': "*

 * *                 "{'conditionKeys': {insert: [(3, 'memorydb:TLSEnabled'), (4, "*

 * *     […]*

```diff
@@ -1391,20 +1391,28 @@
                 "CreateBudgetAction",
                 "DeleteBudgetAction",
                 "DescribeBudgetAction",
                 "DescribeBudgetActionHistories",
                 "DescribeBudgetActionsForAccount",
                 "DescribeBudgetActionsForBudget",
                 "ExecuteBudgetAction",
+                "ListTagsForResource",
                 "ModifyBudget",
+                "TagResource",
+                "UntagResource",
                 "UpdateBudgetAction",
                 "ViewBudget"
             ],
             "HasResource": true,
-            "StringPrefix": "budgets"
+            "StringPrefix": "budgets",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
         },
         "AWS BugBust": {
             "ARNFormat": "arn:aws:bugbust:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:bugbust:.+:.+:.+",
             "Actions": [
                 "CreateEvent",
                 "EvaluateProfilingGroups",
@@ -10369,14 +10377,15 @@
                 "aws:TagKeys"
             ]
         },
         "AWS Trusted Advisor": {
             "ARNFormat": "arn:aws:trustedadvisor:${Region}:${Account}:checks/${Category}/${CheckId}",
             "ARNRegex": "^arn:aws:trustedadvisor:.*",
             "Actions": [
+                "BatchUpdateRecommendationResourceExclusion",
                 "CreateEngagement",
                 "CreateEngagementAttachment",
                 "CreateEngagementCommunication",
                 "DeleteNotificationConfigurationForDelegatedAdmin",
                 "DescribeAccount",
                 "DescribeAccountAccess",
                 "DescribeCheckItems",
@@ -17955,15 +17964,17 @@
                 "UpdateUser"
             ],
             "HasResource": true,
             "StringPrefix": "memorydb",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:TagKeys",
+                "memorydb:TLSEnabled",
+                "memorydb:UserAuthenticationMode"
             ]
         },
         "Amazon Message Delivery Service": {
             "Actions": [
                 "AcknowledgeMessage",
                 "DeleteMessage",
                 "FailMessage",
```

### Comparing `iam_actions-1.2.20240507/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240508/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240507/iam_actions/services.json` & `iam_actions-1.2.20240508/iam_actions/services.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998250636132315%*

 * *Differences: {"'budgets'": "{'Actions': {insert: [(7, 'ListTagsForResource'), (9, 'TagResource'), (10, "*

 * *              "'UntagResource')]}, 'ConditionKeys': ['aws:RequestTag/${TagKey}', "*

 * *              "'aws:ResourceTag/${TagKey}', 'aws:TagKeys']}",*

 * * "'memorydb'": "{'ConditionKeys': {insert: [(3, 'memorydb:TLSEnabled'), (4, "*

 * *               "'memorydb:UserAuthenticationMode')]}}",*

 * * "'trustedadvisor'": "{'Actions': {insert: [(0, 'BatchUpdateRecommendationResourceExclusion')]}}"}*

```diff
@@ -2473,19 +2473,26 @@
             "CreateBudgetAction",
             "DeleteBudgetAction",
             "DescribeBudgetAction",
             "DescribeBudgetActionHistories",
             "DescribeBudgetActionsForAccount",
             "DescribeBudgetActionsForBudget",
             "ExecuteBudgetAction",
+            "ListTagsForResource",
             "ModifyBudget",
+            "TagResource",
+            "UntagResource",
             "UpdateBudgetAction",
             "ViewBudget"
         ],
-        "ConditionKeys": [],
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys"
+        ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Budget Service"
         ]
     },
     "bugbust": {
         "ARNFormats": [
@@ -15239,15 +15246,17 @@
             "UpdateParameterGroup",
             "UpdateSubnetGroup",
             "UpdateUser"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
-            "aws:TagKeys"
+            "aws:TagKeys",
+            "memorydb:TLSEnabled",
+            "memorydb:UserAuthenticationMode"
         ],
         "HasResource": true,
         "ServiceNames": [
             "Amazon MemoryDB"
         ]
     },
     "mgh": {
@@ -23100,14 +23109,15 @@
         "ARNFormats": [
             "arn:aws:trustedadvisor:${Region}:${Account}:checks/${Category}/${CheckId}"
         ],
         "ARNRegexes": [
             "^arn:aws:trustedadvisor:.*"
         ],
         "Actions": [
+            "BatchUpdateRecommendationResourceExclusion",
             "CreateEngagement",
             "CreateEngagementAttachment",
             "CreateEngagementCommunication",
             "DeleteNotificationConfigurationForDelegatedAdmin",
             "DescribeAccount",
             "DescribeAccountAccess",
             "DescribeCheckItems",
```

### Comparing `iam_actions-1.2.20240507/pyproject.toml` & `iam_actions-1.2.20240508/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240507"
+version = "1.2.20240508"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240507/setup.py` & `iam_actions-1.2.20240508/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240507',
+    'version': '1.2.20240508',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240507/PKG-INFO` & `iam_actions-1.2.20240508/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240507
+Version: 1.2.20240508
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

