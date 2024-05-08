# Comparing `tmp/nexus_pcv-0.1.5.tar.gz` & `tmp/nexus_pcv-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus_pcv-0.1.5.tar", max compression
+gzip compressed data, was "nexus_pcv-0.1.6.tar", max compression
```

## Comparing `nexus_pcv-0.1.5.tar` & `nexus_pcv-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    16295 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/LICENSE
--rw-r--r--   0        0        0     4292 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/README.md
--rw-r--r--   0        0        0      394 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/__init__.py
--rw-r--r--   0        0        0      169 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/__main__.py
--rw-r--r--   0        0        0     5464 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/apic.py
--rw-r--r--   0        0        0        0 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/cli/__init__.py
--rw-r--r--   0        0        0     2488 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/cli/main.py
--rw-r--r--   0        0        0     4210 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/cli/options.py
--rw-r--r--   0        0        0     5879 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/const.py
--rw-r--r--   0        0        0    11189 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/nae.py
--rw-r--r--   0        0        0     8460 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/ndi.py
--rw-r--r--   0        0        0    10017 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/nexus_pcv/pcv.py
--rw-r--r--   0        0        0     1914 2023-04-17 07:02:38.207021 nexus_pcv-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5430 1970-01-01 00:00:00.000000 nexus_pcv-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4292 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/README.md
+-rw-r--r--   0        0        0      394 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/__main__.py
+-rw-r--r--   0        0        0     5456 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/apic.py
+-rw-r--r--   0        0        0        0 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/cli/__init__.py
+-rw-r--r--   0        0        0     2488 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/cli/main.py
+-rw-r--r--   0        0        0     4210 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/cli/options.py
+-rw-r--r--   0        0        0     5879 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/const.py
+-rw-r--r--   0        0        0    11189 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/nae.py
+-rw-r--r--   0        0        0     8224 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/ndi.py
+-rw-r--r--   0        0        0    10017 2024-05-08 19:37:40.523698 nexus_pcv-0.1.6/nexus_pcv/pcv.py
+-rw-r--r--   0        0        0     1914 2024-05-08 19:37:40.523698 nexus_pcv-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5481 1970-01-01 00:00:00.000000 nexus_pcv-0.1.6/PKG-INFO
```

### Comparing `nexus_pcv-0.1.5/LICENSE` & `nexus_pcv-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.5/README.md` & `nexus_pcv-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.5/nexus_pcv/apic.py` & `nexus_pcv-0.1.6/nexus_pcv/apic.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,22 +72,22 @@
         for child in self.children:
             objs = child.find(dn=dn, cl=cl)
             result.extend(objs)
         return result
 
     def _index_of_last_dn_delimiter(self, dn: str) -> int:
         """Helper function to return index of last delimiter ('/') in DN string"""
-        escaped = False
+        escaped = 0
         index = len(dn) - 1
         for c in reversed(dn):
             if c == "]":
-                escaped = True
+                escaped += 1
             elif c == "[":
-                escaped = False
-            elif c == "/" and not escaped:
+                escaped -= 1
+            elif c == "/" and escaped == 0:
                 return index
             index -= 1
         return -1
 
     def insert(self, obj: Optional["ApicObject"]) -> None:
         """Insert object in correct place in tree according to dn"""
         if obj is None:
```

### Comparing `nexus_pcv-0.1.5/nexus_pcv/cli/main.py` & `nexus_pcv-0.1.6/nexus_pcv/cli/main.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.5/nexus_pcv/cli/options.py` & `nexus_pcv-0.1.6/nexus_pcv/cli/options.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.5/nexus_pcv/const.py` & `nexus_pcv-0.1.6/nexus_pcv/const.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.5/nexus_pcv/nae.py` & `nexus_pcv-0.1.6/nexus_pcv/nae.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.5/nexus_pcv/ndi.py` & `nexus_pcv-0.1.6/nexus_pcv/ndi.py`

 * *Files 6% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         if not self.authenticated:
             err = self._login()
             if err is not None:
                 return err, None
 
         suppress_events_list = suppress_events.split(",")
 
-        url = "{}/epochDelta/insightsGroup/{}/fabric/{}/job/{}/health/view/aggregateTable?category=ADC,CHANGE_ANALYSIS,TENANT_ENDPOINT,TENANT_FORWARDING,TENANT_SECURITY,RESOURCE_UTILIZATION,SYSTEM,COMPLIANCE&epochStatus=EPOCH2_ONLY&severity=EVENT_SEVERITY_CRITICAL,EVENT_SEVERITY_MAJOR,EVENT_SEVERITY_MINOR,EVENT_SEVERITY_WARNING,EVENT_SEVERITY_INFO".format(
+        url = "{}/epochDelta/insightsGroup/{}/fabric/{}/job/{}/health/view/aggregateTable?epochStatus=EPOCH2_ONLY".format(
             self.api_url, group, site, epoch_job_id
         )
         resp = self.session.get(url)
         if resp.status_code != 200:
             logger.error("Get PCV results failed: {}".format(resp.json()))
             return resp, None
```

### Comparing `nexus_pcv-0.1.5/nexus_pcv/pcv.py` & `nexus_pcv-0.1.6/nexus_pcv/pcv.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.5/pyproject.toml` & `nexus_pcv-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 documentation = "https://github.com/netascode/nexus-pcv"
 homepage = "https://github.com/netascode/nexus-pcv"
 license = "LICENSE"
 maintainers = ["Daniel Schmidt <danischm@cisco.com>"]
 name = "nexus-pcv"
 readme = "README.md"
 repository = "https://github.com/netascode/nexus-pcv"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.scripts]
 nexus-pcv = "nexus_pcv.cli.main:main"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 errorhandler = "^2.0.1"
```

### Comparing `nexus_pcv-0.1.5/PKG-INFO` & `nexus_pcv-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-pcv
-Version: 0.1.5
+Version: 0.1.6
 Summary: A CLI tool to perform a pre-change validation on Nexus Dashboard Insights or Network Assurance Engine.
 Home-page: https://github.com/netascode/nexus-pcv
 License: LICENSE
 Author: Daniel Schmidt
 Author-email: danischm@cisco.com
 Maintainer: Daniel Schmidt
 Maintainer-email: danischm@cisco.com
@@ -12,14 +12,15 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: errorhandler (>=2.0.1,<3.0.0)
 Requires-Dist: importlib-metadata (>=2.0.0,<3.0.0) ; python_version < "3.8"
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://github.com/netascode/nexus-pcv
 Project-URL: Repository, https://github.com/netascode/nexus-pcv
```

