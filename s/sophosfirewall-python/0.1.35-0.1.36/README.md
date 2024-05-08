# Comparing `tmp/sophosfirewall_python-0.1.35.tar.gz` & `tmp/sophosfirewall_python-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sophosfirewall_python-0.1.35.tar", max compression
+gzip compressed data, was "sophosfirewall_python-0.1.36.tar", max compression
```

## Comparing `sophosfirewall_python-0.1.35.tar` & `sophosfirewall_python-0.1.36.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-03-15 13:38:55.440692 sophosfirewall_python-0.1.35/LICENSE
--rw-r--r--   0        0        0     9124 2024-03-15 13:38:55.440692 sophosfirewall_python-0.1.35/README.md
--rw-r--r--   0        0        0      675 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/pyproject.toml
--rw-r--r--   0        0        0    42848 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/firewallapi.py
--rw-r--r--   0        0        0     1681 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/templates/createfwrule.j2
--rw-r--r--   0        0        0      356 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/templates/createiphost.j2
--rw-r--r--   0        0        0      463 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/templates/createiphostgroup.j2
--rw-r--r--   0        0        0      397 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/templates/createipnetwork.j2
--rw-r--r--   0        0        0      402 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/templates/createiprange.j2
--rw-r--r--   0        0        0      591 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/templates/createservice.j2
--rw-r--r--   0        0        0      406 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/templates/createurlgroup.j2
--rw-r--r--   0        0        0     2210 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/templates/createuser.j2
--rw-r--r--   0        0        0      326 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/templates/updateadminpassword.j2
--rw-r--r--   0        0        0     1432 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/templates/updatebackup.j2
--rw-r--r--   0        0        0      482 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/templates/updateiphostgroup.j2
--rw-r--r--   0        0        0      615 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/templates/updateserviceacl.j2
--rw-r--r--   0        0        0      409 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/templates/updateurlgroup.j2
--rw-r--r--   0        0        0     2231 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/templates/updateuserpassword.j2
--rw-r--r--   0        0        0        0 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/tests/__init__.py
--rw-r--r--   0        0        0    13275 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/tests/functional.py
--rw-r--r--   0        0        0    30393 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/tests/unittests.py
--rw-r--r--   0        0        0      522 2024-03-15 13:38:55.460692 sophosfirewall_python-0.1.35/sophosfirewall_python/urlgroup_example.j2
--rw-r--r--   0        0        0     9733 1970-01-01 00:00:00.000000 sophosfirewall_python-0.1.35/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-08 19:41:34.017393 sophosfirewall_python-0.1.36/LICENSE
+-rw-r--r--   0        0        0     9124 2024-05-08 19:41:34.017393 sophosfirewall_python-0.1.36/README.md
+-rw-r--r--   0        0        0      675 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/pyproject.toml
+-rw-r--r--   0        0        0    46031 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/firewallapi.py
+-rw-r--r--   0        0        0     1681 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createfwrule.j2
+-rw-r--r--   0        0        0      356 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createiphost.j2
+-rw-r--r--   0        0        0      463 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createiphostgroup.j2
+-rw-r--r--   0        0        0      397 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createipnetwork.j2
+-rw-r--r--   0        0        0      402 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createiprange.j2
+-rw-r--r--   0        0        0      713 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createservice.j2
+-rw-r--r--   0        0        0      406 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createurlgroup.j2
+-rw-r--r--   0        0        0     2210 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createuser.j2
+-rw-r--r--   0        0        0      326 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateadminpassword.j2
+-rw-r--r--   0        0        0     1432 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updatebackup.j2
+-rw-r--r--   0        0        0      482 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateiphostgroup.j2
+-rw-r--r--   0        0        0      716 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateservice.j2
+-rw-r--r--   0        0        0      615 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateserviceacl.j2
+-rw-r--r--   0        0        0      409 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateurlgroup.j2
+-rw-r--r--   0        0        0     2231 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateuserpassword.j2
+-rw-r--r--   0        0        0        0 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/tests/__init__.py
+-rw-r--r--   0        0        0    16512 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/tests/functional.py
+-rw-r--r--   0        0        0      103 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/tests/pytest.ini
+-rw-r--r--   0        0        0    30393 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/tests/unittests.py
+-rw-r--r--   0        0        0      522 2024-05-08 19:41:34.037393 sophosfirewall_python-0.1.36/sophosfirewall_python/urlgroup_example.j2
+-rw-r--r--   0        0        0     9733 1970-01-01 00:00:00.000000 sophosfirewall_python-0.1.36/PKG-INFO
```

### Comparing `sophosfirewall_python-0.1.35/LICENSE` & `sophosfirewall_python-0.1.36/LICENSE`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.35/README.md` & `sophosfirewall_python-0.1.36/README.md`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.35/pyproject.toml` & `sophosfirewall_python-0.1.36/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "sophosfirewall-python"
 packages = [
     { include = "sophosfirewall_python" },
 ]
-version = "0.1.35"
+version = "0.1.36"
 description = "Python SDK for Sophos Firewall"
 authors = ["Matt Mullen <matt.mullen@sophos.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 requests = "^2.31.0"
```

### Comparing `sophosfirewall_python-0.1.35/sophosfirewall_python/firewallapi.py` & `sophosfirewall_python-0.1.36/sophosfirewall_python/firewallapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -824,29 +824,30 @@
             "createiprange.j2", template_vars=params, debug=debug
         )
         return resp
 
     def create_service(
         self,
         name: str,
-        port: str,
-        protocol: str,
+        service_list: list[dict],
         debug: bool = False,
     ):
         """Create a TCP or UDP service
 
         Args:
-            name (str): Service name
-            port (str): TCP/UDP port
+        name (str): Service name
+        service_list(list): List of dictionaries containing the below keys for each port/proto pair
+            src_port (str, optional): Source TCP/UDP port. Default=1:65535.
+            dst_port (str): Destination TCP/UDP port
             protocol (str): TCP or UDP
-            debug (bool, optional): Enable debug mode. Defaults to False.
+        debug (bool, optional): Enable debug mode. Defaults to False.
         Returns:
             dict: XML response converted to Python dictionary
         """
-        params = {"name": name, "port": port, "protocol": protocol}
+        params = {"name": name, "service_list": service_list}
         resp = self.submit_template(
             "createservice.j2", template_vars=params, debug=debug
         )
         return resp
 
     def create_ip_hostgroup(
         self,
@@ -1023,14 +1024,83 @@
 
         params = {"name": name, "domain_list": new_domain_list}
         resp = self.submit_template(
             "updateurlgroup.j2", template_vars=params, debug=debug
         )
         return resp
 
+    def update_service(
+        self, name: str, service_list: list[dict], action: str = "add", debug: bool = False
+    ):
+        """Add or remove a service entry to/from a service
+
+        Args:
+            name (str): Service name.
+            service_list (list[dict]): List of dicts containing port/protocol pairs to be added or removed.
+              src_port(str, optional): Source TCP/UDP port range. Default=1:65535.
+              dst_port(str): Destination TCP/UDP port range.
+              protocol(str): TCP or UDP
+            action (str): Options are 'add', 'remove' or 'replace'. Defaults to 'add'.
+            debug (bool, optional): Enable debug mode. Defaults to False.
+
+        Returns:
+            dict: XML response converted to Python dictionary
+        """
+        if not isinstance(service_list, list):
+            raise SophosFirewallInvalidArgument(
+                "The update_service() argument `service_list` must be of type list!"
+            )
+
+        if action:
+            self._validate_arg(
+                arg_name="action",
+                arg_value=action,
+                valid_choices=["add", "remove", "replace"],
+            )
+
+        # Get the existing Service list first
+        resp = self.get_service(name=name)
+        if "ServiceDetail" in resp["Response"]["Services"]["ServiceDetails"]:
+            exist_list = (
+                resp.get("Response").get("Services").get("ServiceDetails").get("ServiceDetail")
+            )
+        else:
+            exist_list = None
+
+        # Add src_port to input if not present
+        for service in service_list:
+            if not "src_port" in service:
+                service["src_port"] = "1:65535"
+        if action == "replace":
+            exist_list = None
+        new_service_list = []
+        if exist_list:
+            if isinstance(exist_list, dict):
+                new_service_list.append({"src_port": exist_list["SourcePort"],
+                                         "dst_port": exist_list["DestinationPort"],
+                                         "protocol": exist_list["Protocol"]})
+            elif isinstance(exist_list, list):
+                for service in exist_list:
+                    new_service_list.append({"src_port": service["SourcePort"],
+                                             "dst_port": service["DestinationPort"],
+                                             "protocol": service["Protocol"]})
+        for service in service_list:
+            if action.lower() == "add" and service not in new_service_list:
+                new_service_list.append(service)
+            elif action.lower() == "remove" and service in new_service_list:
+                new_service_list.remove(service)
+            elif action.lower() == "replace":
+                new_service_list.append(service)
+
+        params = {"name": name, "service_list": new_service_list}
+        resp = self.submit_template(
+            "updateservice.j2", template_vars=params, debug=debug
+        )
+        return resp
+
     def update_ip_hostgroup(
         self,
         name: str,
         host_list: list,
         description: str = None,
         action: str = "add",
         debug: bool = False,
```

### Comparing `sophosfirewall_python-0.1.35/sophosfirewall_python/templates/createfwrule.j2` & `sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createfwrule.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.35/sophosfirewall_python/templates/createservice.j2` & `sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createservice.j2`

 * *Files 19% similar despite different names*

```diff
@@ -4,16 +4,18 @@
         <Password>{{password}}</Password>
     </Login>
     <Set operation="add">
         <Services transactionid="">
             <Name>{{ name }}</Name>
             <Type>TCPorUDP</Type>
             <ServiceDetails>
+            {% for service in service_list %}
                 <ServiceDetail>
-                    <SourcePort>1:65535</SourcePort>
-                    <DestinationPort>{{ port }}</DestinationPort>
-                    <Protocol>{{ protocol }}</Protocol>
+                    <SourcePort>{{ service.get(src_port, '1:65535') }}</SourcePort>
+                    <DestinationPort>{{ service.dst_port }}</DestinationPort>
+                    <Protocol>{{ service.protocol }}</Protocol>
                 </ServiceDetail>
+            {% endfor %}
             </ServiceDetails>
         </Services>
     </Set>
 </Request>
```

### Comparing `sophosfirewall_python-0.1.35/sophosfirewall_python/templates/createuser.j2` & `sophosfirewall_python-0.1.36/sophosfirewall_python/templates/createuser.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.35/sophosfirewall_python/templates/updatebackup.j2` & `sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updatebackup.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.35/sophosfirewall_python/templates/updateserviceacl.j2` & `sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateserviceacl.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.35/sophosfirewall_python/templates/updateuserpassword.j2` & `sophosfirewall_python-0.1.36/sophosfirewall_python/templates/updateuserpassword.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.35/sophosfirewall_python/tests/unittests.py` & `sophosfirewall_python-0.1.36/sophosfirewall_python/tests/unittests.py`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.35/sophosfirewall_python/urlgroup_example.j2` & `sophosfirewall_python-0.1.36/sophosfirewall_python/urlgroup_example.j2`

 * *Files identical despite different names*

### Comparing `sophosfirewall_python-0.1.35/PKG-INFO` & `sophosfirewall_python-0.1.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sophosfirewall-python
-Version: 0.1.35
+Version: 0.1.36
 Summary: Python SDK for Sophos Firewall
 Author: Matt Mullen
 Author-email: matt.mullen@sophos.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

