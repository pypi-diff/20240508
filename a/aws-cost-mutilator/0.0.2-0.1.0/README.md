# Comparing `tmp/aws-cost-mutilator-0.0.2.tar.gz` & `tmp/aws_cost_mutilator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cost-mutilator-0.0.2.tar", last modified: Sat Dec 10 09:29:50 2022, max compression
+gzip compressed data, was "aws_cost_mutilator-0.1.0.tar", max compression
```

## Comparing `aws-cost-mutilator-0.0.2.tar` & `aws_cost_mutilator-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 09:29:50.558551 aws-cost-mutilator-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2022-12-10 09:29:40.000000 aws-cost-mutilator-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-10 09:29:40.000000 aws-cost-mutilator-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      706 2022-12-10 09:29:50.558551 aws-cost-mutilator-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-10 09:29:40.000000 aws-cost-mutilator-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 09:29:50.558551 aws-cost-mutilator-0.0.2/aws_cost_mutilator/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-10 09:29:40.000000 aws-cost-mutilator-0.0.2/aws_cost_mutilator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2022-12-10 09:29:40.000000 aws-cost-mutilator-0.0.2/aws_cost_mutilator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2022-12-10 09:29:40.000000 aws-cost-mutilator-0.0.2/aws_cost_mutilator/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    10294 2022-12-10 09:29:40.000000 aws-cost-mutilator-0.0.2/aws_cost_mutilator/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 09:29:50.558551 aws-cost-mutilator-0.0.2/aws_cost_mutilator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2022-12-10 09:29:50.000000 aws-cost-mutilator-0.0.2/aws_cost_mutilator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2022-12-10 09:29:50.000000 aws-cost-mutilator-0.0.2/aws_cost_mutilator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-10 09:29:50.000000 aws-cost-mutilator-0.0.2/aws_cost_mutilator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-10 09:29:50.000000 aws-cost-mutilator-0.0.2/aws_cost_mutilator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-10 09:29:50.000000 aws-cost-mutilator-0.0.2/aws_cost_mutilator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-10 09:29:50.000000 aws-cost-mutilator-0.0.2/aws_cost_mutilator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-10 09:29:50.000000 aws-cost-mutilator-0.0.2/aws_cost_mutilator.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-10 09:29:40.000000 aws-cost-mutilator-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-10 09:29:50.558551 aws-cost-mutilator-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2022-12-10 09:29:40.000000 aws-cost-mutilator-0.0.2/setup.py
+-rw-r--r--   0        0        0     1048 2024-05-08 17:12:15.378273 aws_cost_mutilator-0.1.0/LICENSE
+-rw-r--r--   0        0        0      179 2024-05-08 17:12:15.378273 aws_cost_mutilator-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 17:12:15.378273 aws_cost_mutilator-0.1.0/aws_cost_mutilator/__init__.py
+-rw-r--r--   0        0        0     5224 2024-05-08 17:12:15.378273 aws_cost_mutilator-0.1.0/aws_cost_mutilator/__main__.py
+-rw-r--r--   0        0        0     9274 2024-05-08 17:12:15.378273 aws_cost_mutilator-0.1.0/aws_cost_mutilator/lib.py
+-rw-r--r--   0        0        0    10398 2024-05-08 17:12:15.378273 aws_cost_mutilator-0.1.0/aws_cost_mutilator/tests.py
+-rw-r--r--   0        0        0      812 2024-05-08 17:12:15.378273 aws_cost_mutilator-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 aws_cost_mutilator-0.1.0/PKG-INFO
```

### Comparing `aws-cost-mutilator-0.0.2/LICENSE` & `aws_cost_mutilator-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cost-mutilator-0.0.2/PKG-INFO` & `aws_cost_mutilator-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: aws-cost-mutilator
-Version: 0.0.2
-Summary: cli to mutilate aws costs, it's what accounting craves.
+Version: 0.1.0
+Summary: A cli to mutilate aws costs, it's what accounting craves.
 Home-page: https://github.com/skymoore/aws-cost-mutilator
+License: MIT
+Keywords: aws,cloud
 Author: Sky Moore
 Author-email: i@msky.me
+Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: boto3 (>=1.34.99,<2.0.0)
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Project-URL: Repository, https://github.com/skymoore/aws-cost-mutilator
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # AWS Cost Mutilator
 ### It's what accounting craves.  
 
 
 Usage:
 ```
```

### Comparing `aws-cost-mutilator-0.0.2/aws_cost_mutilator/__main__.py` & `aws_cost_mutilator-0.1.0/aws_cost_mutilator/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import click, json
+import click
+import json
 from .lib import (
     get_lbs_no_targets,
     delete_lbs,
     boto_session,
     get_tgs_no_targets_or_lb,
     delete_tgs,
 )
@@ -20,15 +21,15 @@
 def check(region, profile):
     pass
 
 
 @check.command()
 @click.option("--region", help="The AWS region to use")
 @click.option("--profile", help="The AWS profile to use")
-def tgs(region, profile):
+def tgs_(region, profile):
     session = boto_session(region, profile)
     target_groups = get_tgs_no_targets_or_lb(session)
 
     if len(target_groups) == 0:
         print("No target groups without targets or load balancers found!")
         return
 
@@ -37,15 +38,15 @@
     )
     print(json.dumps(target_groups, indent=4))
 
 
 @check.command()
 @click.option("--region", help="The AWS region to use")
 @click.option("--profile", help="The AWS profile to use")
-def lbs(region, profile):
+def lbs_(region, profile):
     # Perform analysis of ELBv2 resources in the specified region and profile
     session = boto_session(region, profile)
     load_balancers = get_lbs_no_targets(session)
 
     total_monthly_cost = load_balancers["total_monthly_cost"]
     del load_balancers["total_monthly_cost"]
     num_lbs_no_targets = len(load_balancers)
```

### Comparing `aws-cost-mutilator-0.0.2/aws_cost_mutilator/lib.py` & `aws_cost_mutilator-0.1.0/aws_cost_mutilator/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import boto3, json
+import boto3
+import json
 from tqdm import tqdm
 from time import sleep
 
 
 def boto_session(region, profile):
     try:
         session = boto3.Session(region_name=region, profile_name=profile)
```

### Comparing `aws-cost-mutilator-0.0.2/aws_cost_mutilator/tests.py` & `aws_cost_mutilator-0.1.0/aws_cost_mutilator/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .lib import *
+from .lib import boto_session, delete_tgs, delete_lbs, disable_lb_deletion_protection
+from .lib import get_tgs_no_targets_or_lb, get_lbs_no_targets
 import boto3
 from moto import mock_elbv2, mock_sts, mock_ec2
 
 
 @mock_sts
 def test_boto_session():
     # Test successful boto session creation
@@ -30,28 +31,24 @@
     expected_response = {"TargetGroups": []}
 
     # Create a mock describe_target_groups method that returns the expected response
     elb_client.describe_target_groups = lambda **kwargs: expected_response
 
     # Test deleting target groups
     session = boto3.Session(region_name="us-west-2", profile_name="default")
-    region = "us-west-2"
-    profile = "default"
     tgs = ["tg-1234567890", "tg-0987654321"]
     dry_run = False
     delete_tgs(session, tgs, dry_run)
 
     # Verify that the target groups were deleted
     response = elb_client.describe_target_groups()
     assert response == expected_response
 
     # Test dry run deleting target groups
     session = boto3.Session(region_name="us-west-2", profile_name="default")
-    region = "us-west-2"
-    profile = "default"
     tgs = ["tg-1234567890", "tg-0987654321"]
     dry_run = True
     delete_tgs(session, tgs, dry_run)
 
     # Verify that the target groups were not deleted
     response = elb_client.describe_target_groups(TargetGroupArns=tgs)
     assert response == expected_response
@@ -66,15 +63,18 @@
         aws_access_key_id="mock_access_key",
         aws_secret_access_key="mock_secret_key",
     )
 
     # Create a mock VPC and a mock subnet
     ec2_client = session.client("ec2")
     vpc_id = ec2_client.create_vpc(CidrBlock="10.0.0.0/16")["Vpc"]["VpcId"]
-    subnet_id = ec2_client.create_subnet(VpcId=vpc_id, CidrBlock="10.0.0.0/24",)[
+    subnet_id = ec2_client.create_subnet(
+        VpcId=vpc_id,
+        CidrBlock="10.0.0.0/24",
+    )[
         "Subnet"
     ]["SubnetId"]
 
     # Create a mock Elastic Load Balancer
     elb_client = session.client("elbv2")
     elb_response = elb_client.create_load_balancer(
         Name="mock-elb",
@@ -142,15 +142,18 @@
         aws_access_key_id="mock_access_key",
         aws_secret_access_key="mock_secret_key",
     )
 
     # Create a mock VPC and a mock subnet
     ec2_client = session.client("ec2")
     vpc_id = ec2_client.create_vpc(CidrBlock="10.0.0.0/16")["Vpc"]["VpcId"]
-    subnet_id = ec2_client.create_subnet(VpcId=vpc_id, CidrBlock="10.0.0.0/24",)[
+    subnet_id = ec2_client.create_subnet(
+        VpcId=vpc_id,
+        CidrBlock="10.0.0.0/24",
+    )[
         "Subnet"
     ]["SubnetId"]
 
     # Create a mock Elastic Load Balancer
     elb_client = session.client("elbv2")
     elb_response = elb_client.create_load_balancer(
         Name="mock-elb",
@@ -186,15 +189,18 @@
         aws_access_key_id="mock_access_key",
         aws_secret_access_key="mock_secret_key",
     )
 
     # Create a mock VPC and a mock subnet
     ec2_client = session.client("ec2")
     vpc_id = ec2_client.create_vpc(CidrBlock="10.0.0.0/16")["Vpc"]["VpcId"]
-    subnet_id = ec2_client.create_subnet(VpcId=vpc_id, CidrBlock="10.0.0.0/24",)[
+    subnet_id = ec2_client.create_subnet(
+        VpcId=vpc_id,
+        CidrBlock="10.0.0.0/24",
+    )[
         "Subnet"
     ]["SubnetId"]
 
     # Create a mock Elastic Load Balancer
     elb_client = session.client("elbv2")
     elb_response = elb_client.create_load_balancer(
         Name="mock-elb",
@@ -299,15 +305,18 @@
         aws_access_key_id="mock_access_key",
         aws_secret_access_key="mock_secret_key",
     )
 
     # Create a mock VPC and a mock subnet
     ec2_client = session.client("ec2")
     vpc_id = ec2_client.create_vpc(CidrBlock="10.0.0.0/16")["Vpc"]["VpcId"]
-    subnet_id = ec2_client.create_subnet(VpcId=vpc_id, CidrBlock="10.0.0.0/24",)[
+    subnet_id = ec2_client.create_subnet(
+        VpcId=vpc_id,
+        CidrBlock="10.0.0.0/24",
+    )[
         "Subnet"
     ]["SubnetId"]
 
     # Create a mock Elastic Load Balancer
     elb_client = session.client("elbv2")
     elb_response = elb_client.create_load_balancer(
         Name="mock-elb",
@@ -322,15 +331,15 @@
         Protocol="HTTP",
         Port=80,
         VpcId=vpc_id,
     )
     tg_arn = tg_response["TargetGroups"][0]["TargetGroupArn"]
 
     # Add the target group to the load balancer
-    listener_arn = elb_client.create_listener(
+    elb_client.create_listener(
         LoadBalancerArn=elb_arn,
         Protocol="HTTP",
         Port=80,
         DefaultActions=[
             {
                 "Type": "forward",
                 "TargetGroupArn": tg_arn,
```

