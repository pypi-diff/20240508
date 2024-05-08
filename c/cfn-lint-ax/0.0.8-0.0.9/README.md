# Comparing `tmp/cfn_lint_ax-0.0.8.tar.gz` & `tmp/cfn_lint_ax-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn_lint_ax-0.0.8.tar", last modified: Mon Feb  7 18:06:36 2022, max compression
+gzip compressed data, was "cfn_lint_ax-0.0.9.tar", last modified: Wed Sep 21 20:24:43 2022, max compression
```

## Comparing `cfn_lint_ax-0.0.8.tar` & `cfn_lint_ax-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 18:06:36.963498 cfn_lint_ax-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-02-07 18:06:25.000000 cfn_lint_ax-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-02-07 18:06:36.963498 cfn_lint_ax-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-02-07 18:06:25.000000 cfn_lint_ax-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 18:06:36.959499 cfn_lint_ax-0.0.8/cfn_lint_ax/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-07 18:06:25.000000 cfn_lint_ax-0.0.8/cfn_lint_ax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 18:06:36.963498 cfn_lint_ax-0.0.8/cfn_lint_ax/rules/
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-02-07 18:06:25.000000 cfn_lint_ax-0.0.8/cfn_lint_ax/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-02-07 18:06:25.000000 cfn_lint_ax-0.0.8/cfn_lint_ax/rules/certificate_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     6608 2022-02-07 18:06:25.000000 cfn_lint_ax-0.0.8/cfn_lint_ax/rules/cloud_front.py
--rw-r--r--   0 runner    (1001) docker     (121)     1884 2022-02-07 18:06:25.000000 cfn_lint_ax-0.0.8/cfn_lint_ax/rules/code_build.py
--rw-r--r--   0 runner    (1001) docker     (121)     4295 2022-02-07 18:06:25.000000 cfn_lint_ax-0.0.8/cfn_lint_ax/rules/ecs.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-02-07 18:06:25.000000 cfn_lint_ax-0.0.8/cfn_lint_ax/rules/intrinsic_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     5822 2022-02-07 18:06:25.000000 cfn_lint_ax-0.0.8/cfn_lint_ax/rules/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     2951 2022-02-07 18:06:25.000000 cfn_lint_ax-0.0.8/cfn_lint_ax/rules/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 18:06:36.959499 cfn_lint_ax-0.0.8/cfn_lint_ax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-02-07 18:06:36.000000 cfn_lint_ax-0.0.8/cfn_lint_ax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-02-07 18:06:36.000000 cfn_lint_ax-0.0.8/cfn_lint_ax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 18:06:36.000000 cfn_lint_ax-0.0.8/cfn_lint_ax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-07 18:06:36.000000 cfn_lint_ax-0.0.8/cfn_lint_ax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-07 18:06:36.000000 cfn_lint_ax-0.0.8/cfn_lint_ax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-02-07 18:06:25.000000 cfn_lint_ax-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-07 18:06:36.963498 cfn_lint_ax-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-02-07 18:06:25.000000 cfn_lint_ax-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 20:24:43.270725 cfn_lint_ax-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-09-21 20:24:23.000000 cfn_lint_ax-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-09-21 20:24:43.270725 cfn_lint_ax-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-09-21 20:24:23.000000 cfn_lint_ax-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 20:24:43.270725 cfn_lint_ax-0.0.9/cfn_lint_ax/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 20:24:23.000000 cfn_lint_ax-0.0.9/cfn_lint_ax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 20:24:43.270725 cfn_lint_ax-0.0.9/cfn_lint_ax/rules/
+-rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-09-21 20:24:23.000000 cfn_lint_ax-0.0.9/cfn_lint_ax/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-09-21 20:24:23.000000 cfn_lint_ax-0.0.9/cfn_lint_ax/rules/certificate_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6546 2022-09-21 20:24:23.000000 cfn_lint_ax-0.0.9/cfn_lint_ax/rules/cloud_front.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-09-21 20:24:23.000000 cfn_lint_ax-0.0.9/cfn_lint_ax/rules/code_build.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1741 2022-09-21 20:24:23.000000 cfn_lint_ax-0.0.9/cfn_lint_ax/rules/ecr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4295 2022-09-21 20:24:23.000000 cfn_lint_ax-0.0.9/cfn_lint_ax/rules/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      905 2022-09-21 20:24:23.000000 cfn_lint_ax-0.0.9/cfn_lint_ax/rules/intrinsic_function.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5822 2022-09-21 20:24:23.000000 cfn_lint_ax-0.0.9/cfn_lint_ax/rules/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2951 2022-09-21 20:24:23.000000 cfn_lint_ax-0.0.9/cfn_lint_ax/rules/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 20:24:43.270725 cfn_lint_ax-0.0.9/cfn_lint_ax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-09-21 20:24:43.000000 cfn_lint_ax-0.0.9/cfn_lint_ax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      519 2022-09-21 20:24:43.000000 cfn_lint_ax-0.0.9/cfn_lint_ax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 20:24:43.000000 cfn_lint_ax-0.0.9/cfn_lint_ax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-21 20:24:43.000000 cfn_lint_ax-0.0.9/cfn_lint_ax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-21 20:24:43.000000 cfn_lint_ax-0.0.9/cfn_lint_ax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2022-09-21 20:24:23.000000 cfn_lint_ax-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 20:24:43.270725 cfn_lint_ax-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-09-21 20:24:23.000000 cfn_lint_ax-0.0.9/setup.py
```

### Comparing `cfn_lint_ax-0.0.8/LICENSE` & `cfn_lint_ax-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn_lint_ax-0.0.8/PKG-INFO` & `cfn_lint_ax-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: cfn_lint_ax
-Version: 0.0.8
+Version: 0.0.9
 Summary: Rules for cfn lint.
 Home-page: https://github.com/aexeagmbh/cfn-lint-rules
 Author: AX Semantics
 Author-email: infrastructure@ax-semantics.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aexeagmbh/cfn-lint-rules/issues
 Project-URL: Source, https://github.com/aexeagmbh/cfn-lint-rules
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 cfn-lint-ax
 ===========
 
 [![Testing](https://github.com/aexeagmbh/cfn-lint-rules/actions/workflows/tests.yml/badge.svg)](https://github.com/aexeagmbh/cfn-lint-rules/actions/workflows/tests.yml)
@@ -60,14 +57,15 @@
 ### Functions (E91XX)
 * E9101 UnresolvedObject
 
 ### Parameters (E92XX)
 
 ### Resources (E93XX)
 * I9301 EcsServiceFargatePlatformVersionNotOutdated
+* I9302 EcrRepositoryAutocleanupTag
 * W9301 S3BucketPublicAccess
 * W9302 S3BucketEncryption
 * W9303 CloudfrontDistributionLogging
 * W9304 CloudfrontDistributionComment
 * W9305 CertificateManagerCertificateNameTag
 * W9306 CodeBuildProjectCloudWatchLogs
 * W9307 CloudfrontDistributionResponseHeadersPolicy
@@ -78,9 +76,7 @@
 * E9401 MetadataAxChangesetAutoApprove
 
 ### Outputs (E96XX)
 
 ### Mappings (E97XX)
 
 ### Conditions (E98XX)
-
-
```

### Comparing `cfn_lint_ax-0.0.8/README.md` & `cfn_lint_ax-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 ### Functions (E91XX)
 * E9101 UnresolvedObject
 
 ### Parameters (E92XX)
 
 ### Resources (E93XX)
 * I9301 EcsServiceFargatePlatformVersionNotOutdated
+* I9302 EcrRepositoryAutocleanupTag
 * W9301 S3BucketPublicAccess
 * W9302 S3BucketEncryption
 * W9303 CloudfrontDistributionLogging
 * W9304 CloudfrontDistributionComment
 * W9305 CertificateManagerCertificateNameTag
 * W9306 CodeBuildProjectCloudWatchLogs
 * W9307 CloudfrontDistributionResponseHeadersPolicy
```

### Comparing `cfn_lint_ax-0.0.8/cfn_lint_ax/rules/__init__.py` & `cfn_lint_ax-0.0.9/cfn_lint_ax/rules/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from .certificate_manager import CertificateManagerCertificateNameTag
 from .cloud_front import (
     CloudfrontDistributionComment,
     CloudfrontDistributionLogging,
     CloudfrontDistributionResponseHeadersPolicy,
     CloudfrontResponseHeaderConfigLongHstsMaxAge,
 )
-from .code_build import CodeBuildProjectCloudWatchLogs
+from .code_build import CodeBuildProjectCloudWatchLogs, CodeBuildProjectImage
+from .ecr import EcrRepositoryAutocleanupTag
 from .ecs import (
     EcsServiceDeploymentConfiguration,
     EcsServiceFargatePlatformVersionNotOutdated,
 )
 from .intrinsic_function import IntrinsicFunctionSubUnresolvedObject
 from .metadata import MetadataAxChangesetAutoApprove
 from .s3 import S3BucketEncryption, S3BucketPublicAccess
@@ -17,14 +18,16 @@
 __all__ = [
     "CertificateManagerCertificateNameTag",
     "CloudfrontDistributionComment",
     "CloudfrontDistributionLogging",
     "CloudfrontDistributionResponseHeadersPolicy",
     "CloudfrontResponseHeaderConfigLongHstsMaxAge",
     "CodeBuildProjectCloudWatchLogs",
+    "CodeBuildProjectImage",
+    "EcrRepositoryAutocleanupTag",
     "EcsServiceDeploymentConfiguration",
     "EcsServiceFargatePlatformVersionNotOutdated",
     "IntrinsicFunctionSubUnresolvedObject",
     "MetadataAxChangesetAutoApprove",
     "S3BucketEncryption",
     "S3BucketPublicAccess",
 ]
```

### Comparing `cfn_lint_ax-0.0.8/cfn_lint_ax/rules/certificate_manager.py` & `cfn_lint_ax-0.0.9/cfn_lint_ax/rules/certificate_manager.py`

 * *Files identical despite different names*

### Comparing `cfn_lint_ax-0.0.8/cfn_lint_ax/rules/cloud_front.py` & `cfn_lint_ax-0.0.9/cfn_lint_ax/rules/cloud_front.py`

 * *Files 7% similar despite different names*

```diff
@@ -161,13 +161,12 @@
                 "Resources",
                 resource_name,
                 "ResponseHeadersPolicyConfig",
                 "SecurityHeadersConfig",
                 "StrictTransportSecurity",
                 "Override",
             ]
-            if not strict_transpost_security.get("Override") == True:
+            if strict_transpost_security.get("Override") is not True:
                 message = f"Property {'/'.join(path)} should be true."
                 matches.append(RuleMatch(path, message))
-            strict_transpost_security.get("Override") == True
 
         return matches
```

### Comparing `cfn_lint_ax-0.0.8/cfn_lint_ax/rules/ecs.py` & `cfn_lint_ax-0.0.9/cfn_lint_ax/rules/ecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         resources = cfn.get_resources(["AWS::ECS::Service"])
         for resource_name, resource in resources.items():
             properties = resource.get("Properties", {})
             platform_version = properties.get("PlatformVersion")
             if platform_version is None:
                 continue
 
-            if not platform_version in valid_platform_versions:
+            if platform_version not in valid_platform_versions:
                 path = ["Resources", resource_name, "Properties", "PlatformVersion"]
                 message = f"{'/'.join(path)} {platform_version} is outdated. Set it to one of:  {', '.join(valid_platform_versions)}"
                 matches.append(RuleMatch(path, message))
 
         return matches
```

### Comparing `cfn_lint_ax-0.0.8/cfn_lint_ax/rules/intrinsic_function.py` & `cfn_lint_ax-0.0.9/cfn_lint_ax/rules/intrinsic_function.py`

 * *Files identical despite different names*

### Comparing `cfn_lint_ax-0.0.8/cfn_lint_ax/rules/metadata.py` & `cfn_lint_ax-0.0.9/cfn_lint_ax/rules/metadata.py`

 * *Files identical despite different names*

### Comparing `cfn_lint_ax-0.0.8/cfn_lint_ax/rules/s3.py` & `cfn_lint_ax-0.0.9/cfn_lint_ax/rules/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     def match(self, cfn: Template) -> List[RuleMatch]:
         matches = []
 
         resources = cfn.get_resources(["AWS::S3::Bucket"])
         for resource_name, resource in resources.items():
             properties = resource.get("Properties", {})
-            if not "BucketEncryption" in properties:
+            if "BucketEncryption" not in properties:
                 path = ["Resources", resource_name, "Properties", "BucketEncryption"]
                 message = f"Property {'/'.join(path)} is missing"
                 matches.append(RuleMatch(path, message))
 
         return matches
```

### Comparing `cfn_lint_ax-0.0.8/cfn_lint_ax.egg-info/PKG-INFO` & `cfn_lint_ax-0.0.9/cfn_lint_ax.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: cfn-lint-ax
-Version: 0.0.8
+Version: 0.0.9
 Summary: Rules for cfn lint.
 Home-page: https://github.com/aexeagmbh/cfn-lint-rules
 Author: AX Semantics
 Author-email: infrastructure@ax-semantics.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aexeagmbh/cfn-lint-rules/issues
 Project-URL: Source, https://github.com/aexeagmbh/cfn-lint-rules
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 cfn-lint-ax
 ===========
 
 [![Testing](https://github.com/aexeagmbh/cfn-lint-rules/actions/workflows/tests.yml/badge.svg)](https://github.com/aexeagmbh/cfn-lint-rules/actions/workflows/tests.yml)
@@ -60,14 +57,15 @@
 ### Functions (E91XX)
 * E9101 UnresolvedObject
 
 ### Parameters (E92XX)
 
 ### Resources (E93XX)
 * I9301 EcsServiceFargatePlatformVersionNotOutdated
+* I9302 EcrRepositoryAutocleanupTag
 * W9301 S3BucketPublicAccess
 * W9302 S3BucketEncryption
 * W9303 CloudfrontDistributionLogging
 * W9304 CloudfrontDistributionComment
 * W9305 CertificateManagerCertificateNameTag
 * W9306 CodeBuildProjectCloudWatchLogs
 * W9307 CloudfrontDistributionResponseHeadersPolicy
@@ -78,9 +76,7 @@
 * E9401 MetadataAxChangesetAutoApprove
 
 ### Outputs (E96XX)
 
 ### Mappings (E97XX)
 
 ### Conditions (E98XX)
-
-
```

### Comparing `cfn_lint_ax-0.0.8/pyproject.toml` & `cfn_lint_ax-0.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # See PEP 518 for the spec of this file
 # https://www.python.org/dev/peps/pep-0518/
 
 [tool.black]
 # See https://github.com/ambv/black/blob/master/pyproject.toml
 line-length = 88
-target_version = ['py37', 'py38']
+target_version = ['py39', 'py310']
 
 
 [tool.isort]
 balanced_wrapping = true
 combine_as_imports = true
 default_section = "THIRDPARTY"
 include_trailing_comma = true
@@ -16,19 +16,28 @@
 known_first_party = [
     "rules",
 ]
 line_length = 88
 multi_line_output = 3
 
 
+[tool.pylint."messages control"]
+disable = [
+    "attribute-defined-outside-init",
+    "duplicate-code",
+    "line-too-long",
+    "missing-docstring",
+]
+
+
 [tool.winky]
 target_branch = "winky"
 
 [[tool.winky.pip_compile]]
 file = "./requirements/base.in"
 hashes = true
-python = "3.8"
+python = "3.9"
 
 [[tool.winky.pip_compile]]
 file = "./requirements/dev.in"
 hashes = true
-python = "3.8"
+python = "3.9"
```

### Comparing `cfn_lint_ax-0.0.8/setup.py` & `cfn_lint_ax-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,33 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="cfn_lint_ax",
-    version="0.0.8",
+    version="0.0.9",
     author="AX Semantics",
     author_email="infrastructure@ax-semantics.com",
     description="Rules for cfn lint.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aexeagmbh/cfn-lint-rules",
     project_urls={
         "Bug Tracker": "https://github.com/aexeagmbh/cfn-lint-rules/issues",
         "Source": "https://github.com/aexeagmbh/cfn-lint-rules",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=[
         "cfn_lint_ax",
         "cfn_lint_ax.rules",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     install_requires=["cfn-lint >= 0.56.1"],
 )
```

