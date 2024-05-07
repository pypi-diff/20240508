# Comparing `tmp/netbox_plugin_prometheus_sd-0.8.0rc1.tar.gz` & `tmp/netbox_plugin_prometheus_sd-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_plugin_prometheus_sd-0.8.0rc1.tar", max compression
+gzip compressed data, was "netbox_plugin_prometheus_sd-1.0.0.tar", max compression
```

## Comparing `netbox_plugin_prometheus_sd-0.8.0rc1.tar` & `netbox_plugin_prometheus_sd-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-12-25 10:29:12.080071 netbox_plugin_prometheus_sd-0.8.0rc1/LICENSE
--rw-r--r--   0        0        0     4905 2023-12-25 10:29:12.080071 netbox_plugin_prometheus_sd-0.8.0rc1/README.md
--rw-r--r--   0        0        0      488 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/__init__.py
--rw-r--r--   0        0        0        0 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/__init__.py
--rw-r--r--   0        0        0     7182 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/serializers.py
--rw-r--r--   0        0        0      381 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/urls.py
--rw-r--r--   0        0        0     5815 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/utils.py
--rw-r--r--   0        0        0     3354 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/views.py
--rw-r--r--   0        0        0       50 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/tests/__init__.py
--rw-r--r--   0        0        0     3514 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/tests/test_api.py
--rwxr-xr-x   0        0        0    13166 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/tests/test_serializers.py
--rw-r--r--   0        0        0     6974 2023-12-25 10:29:12.084071 netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/tests/utils.py
--rw-r--r--   0        0        0      621 2023-12-25 10:29:21.991980 netbox_plugin_prometheus_sd-0.8.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5564 1970-01-01 00:00:00.000000 netbox_plugin_prometheus_sd-0.8.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-07 22:22:07.539324 netbox_plugin_prometheus_sd-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5730 2024-05-07 22:22:07.539324 netbox_plugin_prometheus_sd-1.0.0/README.md
+-rw-r--r--   0        0        0      488 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/__init__.py
+-rw-r--r--   0        0        0     7032 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/serializers.py
+-rw-r--r--   0        0        0      381 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/urls.py
+-rw-r--r--   0        0        0     5992 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/utils.py
+-rw-r--r--   0        0        0     3360 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/views.py
+-rw-r--r--   0        0        0     2031 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/filtersets.py
+-rw-r--r--   0        0        0       50 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/__init__.py
+-rw-r--r--   0        0        0     3535 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/test_api.py
+-rw-r--r--   0        0        0     1304 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/test_filtersets.py
+-rwxr-xr-x   0        0        0    15114 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/test_serializers.py
+-rw-r--r--   0        0        0     7157 2024-05-07 22:22:07.543324 netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/utils.py
+-rw-r--r--   0        0        0      616 2024-05-07 22:22:18.271447 netbox_plugin_prometheus_sd-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6386 1970-01-01 00:00:00.000000 netbox_plugin_prometheus_sd-1.0.0/PKG-INFO
```

### Comparing `netbox_plugin_prometheus_sd-0.8.0rc1/LICENSE` & `netbox_plugin_prometheus_sd-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-0.8.0rc1/README.md` & `netbox_plugin_prometheus_sd-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -43,14 +43,19 @@
 ```
 GET        /api/plugins/prometheus-sd/devices/              Get a list of devices in a prometheus compatible format
 GET        /api/plugins/prometheus-sd/virtual-machines/     Get a list of vms in a prometheus compatible format
 GET        /api/plugins/prometheus-sd/services/             Get a list of services in a prometheus compatible format
 GET        /api/plugins/prometheus-sd/ip-addresses/         Get a list of ip in a prometheus compatible format
 ```
 
+#### Extended services filters
+
+Apart from standard Netbox filters, services endpoint also supports `tenant=<slug>` or `tenant_id=<id>` parameters.
+The lookup is only executed against the `tenant` attribute of the object associated with the service.
+
 ### Config context
 
 The plugin can also discover extra config to inject in the HTTP SD JSON from the config context of the devices/virtual machines.
 If you have a `prometheus-plugin-prometheus-sd` entry in your config context with the following schema it will be automatically picked up:
 
 ```
 prometheus-plugin-prometheus-sd:
@@ -89,21 +94,24 @@
 Netbox content should then be available in the service discovery tab.
 
 ## Development
 
 We use Poetry for dependency management and invoke as task runner.
 As Netbox plugins cannot be tested standalone, we need invoke to start all code embedded in Netbox Docker containers.
 
-All code to run in docker is located under `development`.
+All code to run in docker is located under `develop`.
 To start a virtual env managed by poetry run `poetry shell`.
 All following commands are started inside this environment.
 
 In order to run tests invoke the test steps
 
 ``` bash
+# Build Docker images
+invoke build
+
 # Execute all tests
 invoke tests
 
 # Execute unit tests only
 invoke unittest
 ```
 
@@ -117,7 +125,15 @@
 invoke create-user
 ```
 
 Visit http://localhost:8000 and log in with the new user.
 You can now define Netbox entities and test around.
 
 API endpoints for testing can be found at http://localhost:8000/api/plugins/prometheus-sd/
+
+## Conventional Commits
+
+This repository follows the Conventional Commits specification for versioning and changelog generation.
+Conventional Commits provide a standardized way of writing commit messages to convey semantic meaning
+about the changes made. Each commit message follows a defined format that includes a type,
+an optional scope, and a message. The types typically include features, fixes, documentation, and more.
+By adhering to this convention, we ensure clear and automated versioning, release notes, and changelog generation.
```

### Comparing `netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/serializers.py` & `netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,18 +92,14 @@
             labels["role"] = obj.device_role.name
             labels["role_slug"] = obj.device_role.slug
 
         if hasattr(obj, "device_type") and obj.device_type is not None:
             labels["device_type"] = obj.device_type.model
             labels["device_type_slug"] = obj.device_type.slug
 
-        if hasattr(obj, "site") and obj.site is not None:
-            labels["site"] = obj.site.name
-            labels["site_slug"] = obj.site.slug
-
         labels = labels.get_labels()
 
         # Those shouldn't have the netbox prefix
         utils.extract_prometheus_sd_config(obj, labels)
 
         return labels
```

### Comparing `netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/utils.py` & `netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,19 @@
             labels["cluster_group"] = obj.cluster.group.name
         if obj.cluster.type:
             labels["cluster_type"] = obj.cluster.type.name
         if obj.cluster.site:
             labels["site"] = obj.cluster.site.name
             labels["site_slug"] = obj.cluster.site.slug
 
+    # Has precedence over cluster site
+    if hasattr(obj, "site") and obj.site is not None:
+        labels["site"] = obj.site.name
+        labels["site_slug"] = obj.site.slug
+
 
 def extract_primary_ip(obj, labels: LabelDict):
     if getattr(obj, "primary_ip", None) is not None:
         labels["primary_ip"] = str(IPNetwork(obj.primary_ip.address).ip)
 
     if getattr(obj, "primary_ip4", None) is not None:
         labels["primary_ip4"] = str(IPNetwork(obj.primary_ip4.address).ip)
```

### Comparing `netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/api/views.py` & `netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/api/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,24 +18,25 @@
         from netbox.api.viewsets import NetBoxModelViewSet as NetboxPrometheusSDModelViewSet
     except ImportError: # Netbox < 3.2
         from extras.api.views import CustomFieldModelViewSet as NetboxPrometheusSDModelViewSet
 
 # Filtersets have been renamed, we support both
 # https://github.com/netbox-community/netbox/commit/1024782b9e0abb48f6da65f8248741227d53dbed#diff-d9224204dab475bbe888868c02235b8ef10f07c9201c45c90804d395dc161c40
 try:
-    from ipam.filtersets import IPAddressFilterSet, ServiceFilterSet
+    from ipam.filtersets import IPAddressFilterSet
     from dcim.filtersets import DeviceFilterSet
     from virtualization.filtersets import VirtualMachineFilterSet
 except ImportError:
-    from ipam.filters import IPAddressFilterSet, ServiceFilterSet
+    from ipam.filters import IPAddressFilterSet
     from dcim.filters import DeviceFilterSet
     from virtualization.filters import VirtualMachineFilterSet
 # pylint: enable=ungrouped-imports
 
 
+from ..filtersets import ServiceFilterSet
 from .serializers import (
     PrometheusIPAddressSerializer,
     PrometheusDeviceSerializer,
     PrometheusVirtualMachineSerializer,
     PrometheusServiceSerializer
 )
```

### Comparing `netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/tests/test_api.py` & `netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,59 +37,59 @@
             ContentType.objects.get(app_label="virtualization", model="virtualmachine")
         )
         self.client.force_authenticate(user)
 
     def test_endpoint_device(self):
         """Ensure device endpoint returns a valid response"""
 
-        for i in range(60):
-            utils.build_device_full(f"api-test-{i}.example.com")
+        for i in range(1, 61):
+            utils.build_device_full(f"api-test-{i}.example.com", i)
 
         resp = self.client.get("/api/plugins/prometheus-sd/devices/")
         self.assertEqual(resp.status_code, status.HTTP_200_OK)
         data = json.loads(resp.content)
 
         self.assertIsNotNone(data[0]["targets"])
         self.assertIsNotNone(data[0]["labels"])
         self.assertEqual(len(data), 60)
 
     def test_endpoint_virtual_machine(self):
         """Ensure virtual machine endpoint returns a valid response"""
 
-        for i in range(60):
-            utils.build_vm_full(f"api-test-vm-{i}.example.com")
+        for i in range(1, 61):
+            utils.build_vm_full(f"api-test-vm-{i}.example.com", i)
 
         resp = self.client.get("/api/plugins/prometheus-sd/virtual-machines/")
         self.assertEqual(resp.status_code, status.HTTP_200_OK)
         data = json.loads(resp.content)
 
         self.assertIsNotNone(data[0]["targets"])
         self.assertIsNotNone(data[0]["labels"])
         # Full vm contains two entry in the config context so we have to double the number of vm
         self.assertEqual(len(data), 120)
 
     def test_endpoint_ip_address(self):
         """Ensure ip address endpoint returns a valid response"""
 
-        for i in range(60):
+        for i in range(1, 61):
             utils.build_full_ip(address=f"10.10.10.{i}/24")
 
         resp = self.client.get("/api/plugins/prometheus-sd/ip-addresses/")
         self.assertEqual(resp.status_code, status.HTTP_200_OK)
         data = json.loads(resp.content)
 
         self.assertIsNotNone(data[0]["targets"])
         self.assertIsNotNone(data[0]["labels"])
         self.assertEqual(len(data), 60)
 
     def test_endpoint_service(self):
         """Ensure service endpoint returns a valid response"""
 
-        for i in range(60):
-            utils.build_vm_full(f"api-test-vm-{i}.example.com")
+        for i in range(1, 61):
+            utils.build_vm_full(f"api-test-vm-{i}.example.com", i)
 
         resp = self.client.get("/api/plugins/prometheus-sd/services/")
         self.assertEqual(resp.status_code, status.HTTP_200_OK)
         data = json.loads(resp.content)
 
         self.assertIsNotNone(data[0]["targets"])
         self.assertIsNotNone(data[0]["labels"])
```

### Comparing `netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/tests/test_serializers.py` & `netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/test_serializers.py`

 * *Files 7% similar despite different names*

```diff
@@ -188,14 +188,20 @@
             {"__meta_netbox_primary_ip6": "2001:db8:1701::2"}, data["labels"]
         )
         self.assertDictContainsSubset(
             {"__meta_netbox_oob_ip": "10.0.0.1"}, data["labels"]
         )
         self.assertDictContainsSubset({"__meta_netbox_rack": "R01B01"}, data["labels"])
         self.assertDictContainsSubset(
+            {"__meta_netbox_site": "Site"}, data["labels"]
+        )
+        self.assertDictContainsSubset(
+            {"__meta_netbox_site_slug": "site"}, data["labels"]
+        )
+        self.assertDictContainsSubset(
             {"__meta_netbox_description": "Device Description"}, data["labels"]
         )
         self.assertDictContainsSubset(
             {"__meta_netbox_location": "First Floor"}, data["labels"]
         )
         self.assertDictContainsSubset(
             {"__meta_netbox_location_slug": "first-floor"}, data["labels"]
@@ -262,15 +268,54 @@
         )
         self.assertDictContainsSubset(
             {"__meta_netbox_custom_field_simple": "Foobar 123"}, data["labels"]
         )
 
 
 class PrometheusServiceSerializerTests(TestCase):
-    def test_service_full_to_target(self):
+    def test_device_service_full_to_target(self):
+        device = utils.build_device_full("firewall-full-01")
+        instance = device.services.first()
+        data_list = PrometheusServiceSerializer(many=True, instance=[instance]).data
+
+        self.assertEqual(data_list[0]["targets"], ["ssh"])
+        for data in data_list:
+            self.assertDictContainsSubset({"__meta_netbox_id": str(instance.id)}, data["labels"])
+            self.assertDictContainsSubset(
+                {"__meta_netbox_display": "ssh (TCP/22)"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_ports": "22"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_parent": "firewall-full-01"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_tenant": "Acme Corp."}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_tenant_slug": "acme"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_site": "Site"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_site_slug": "site"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_primary_ip": "2001:db8:1701::2"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_primary_ip4": "192.168.0.1"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_primary_ip6": "2001:db8:1701::2"}, data["labels"]
+            )
+
+    def test_vm_service_full_to_target(self):
         vm = utils.build_vm_full("vm-full-01.example.com")
         instance = vm.services.first()
         data_list = PrometheusServiceSerializer(many=True, instance=[instance]).data
 
         self.assertEqual(data_list[0]["targets"], ["ssh"])
         for data in data_list:
             self.assertDictContainsSubset({"__meta_netbox_id": str(instance.id)}, data["labels"])
```

### Comparing `netbox_plugin_prometheus_sd-0.8.0rc1/netbox_prometheus_sd/tests/utils.py` & `netbox_plugin_prometheus_sd-1.0.0/netbox_prometheus_sd/tests/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         "bool": "True"
     }
 
 def build_minimal_vm(name):
     return VirtualMachine.objects.get_or_create(name=name, cluster=build_cluster())[0]
 
 
-def build_vm_full(name):
+def build_vm_full(name, ip_octet=1):
     # Create the confix context beforehand
     config_context, created = ConfigContext.objects.get_or_create(name="context 1",
         weight=100, data={"prometheus-plugin-prometheus-sd": [
             {"metrics_path": "/not/metrics", "port": 4242, "scheme": "https"},
             {"port": 4243},
         ]
     })
@@ -79,24 +79,24 @@
         )[0]
         config_context.platforms.add(platform)
 
     vm = build_minimal_vm(name=name)
     vm.platform = Platform.objects.get_or_create(
         name="Ubuntu 20.04", slug="ubuntu-20.04"
     )[0]
-    vm.save() # Save the platform so that we can find the config context in test API
 
     vm.tenant = build_tenant()
     vm.custom_field_data = build_custom_fields()
     vm.role = DeviceRole.objects.get_or_create(name="VM", slug="vm", vm_role=True)[0]
-    vm.primary_ip4 = IPAddress.objects.get_or_create(address="192.168.0.1/24")[0]
-    vm.primary_ip6 = IPAddress.objects.get_or_create(address="2001:db8:1701::2/64")[0]
+    vm.primary_ip4 = IPAddress.objects.get_or_create(address=f"192.168.0.{ip_octet}/24")[0]
+    vm.primary_ip6 = IPAddress.objects.get_or_create(address=f"2001:db8:1701::{ip_octet+1}/64")[0]
 
     vm.tags.add("Tag1")
     vm.tags.add("Tag 2")
+    vm.save()
 
     Service.objects.create(virtual_machine=vm, name="ssh", protocol='tcp', ports=[22])
     return vm
 
 
 def build_minimal_device(name):
     role_attr = "role" if hasattr(Device, "role") else "device_role"
@@ -170,31 +170,33 @@
         tag = Tag.objects.create(name='mix valid invalid', slug='mix-valid-invalid')
         config_context.platforms.add(tag)
         device.tags.add(tag)
     device.save()
 
     return device
 
-def build_device_full(name):
+def build_device_full(name, ip_octet=1):
     device = build_minimal_device(name)
     device.location = build_location()
     device.tenant = build_tenant()
     device.description = "Device Description"
     device.custom_field_data = build_custom_fields()
     device.platform = Platform.objects.get_or_create(name="Junos", slug="junos")[0]
-    device.primary_ip4 = IPAddress.objects.get_or_create(address="192.168.0.1/24")[0]
-    device.primary_ip6 = IPAddress.objects.get_or_create(address="2001:db8:1701::2/64")[
-        0
-    ]
-    device.oob_ip = IPAddress.objects.get_or_create(address="10.0.0.1/24")[0]
+    device.primary_ip4 = IPAddress.objects.get_or_create(address=f"192.168.0.{ip_octet}/24")[0]
+    device.primary_ip6 = IPAddress.objects.get_or_create(address=f"2001:db8:1701::{ip_octet+1}/64")[0]
+    device.oob_ip = IPAddress.objects.get_or_create(address=f"10.0.0.{ip_octet}/24")[0]
     device.rack = Rack.objects.get_or_create(
         name="R01B01", site=Site.objects.get_or_create(name="Site", slug="site")[0]
     )[0]
+    device.site = Site.objects.get_or_create(name="Site", slug="site")[0]
     device.tags.add("Tag1")
     device.tags.add("Tag 2")
+    device.save()
+
+    Service.objects.create(device=device, name="ssh", protocol='tcp', ports=[22])
     return device
 
 
 def build_minimal_ip(address):
     return IPAddress.objects.get_or_create(address=address)[0]
 
 
@@ -207,8 +209,10 @@
         group=TenantGroup.objects.get_or_create(name="Federation", slug="federation")[
             0
         ],
     )[0]
     ip.dns_name = dns_name
     ip.tags.add("Tag1")
     ip.tags.add("Tag 2")
+    ip.save()
+
     return ip
```

### Comparing `netbox_plugin_prometheus_sd-0.8.0rc1/pyproject.toml` & `netbox_plugin_prometheus_sd-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "netbox-plugin-prometheus-sd"
-version = "0.8.0-rc1" # placeholder
+version = "1.0.0" # placeholder
 description = "A Netbox plugin to provide Netbox entires to Prometheus HTTP service discovery"
 authors = ["Felix Peters <felix.peters@breuninger.de>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "netbox_prometheus_sd" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-black = "^23.12"
+black = "^24.4"
 invoke = "^2.2.0"
-pylint = "^3.0.3"
+pylint = "^3.1.0"
 pylint-django = "^2.5.5"
-yamllint = "^1.33.0"
+yamllint = "^1.35.1"
 typed-ast = "^1.5.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `netbox_plugin_prometheus_sd-0.8.0rc1/PKG-INFO` & `netbox_plugin_prometheus_sd-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-prometheus-sd
-Version: 0.8.0rc1
+Version: 1.0.0
 Summary: A Netbox plugin to provide Netbox entires to Prometheus HTTP service discovery
 License: MIT
 Author: Felix Peters
 Author-email: felix.peters@breuninger.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -60,14 +60,19 @@
 ```
 GET        /api/plugins/prometheus-sd/devices/              Get a list of devices in a prometheus compatible format
 GET        /api/plugins/prometheus-sd/virtual-machines/     Get a list of vms in a prometheus compatible format
 GET        /api/plugins/prometheus-sd/services/             Get a list of services in a prometheus compatible format
 GET        /api/plugins/prometheus-sd/ip-addresses/         Get a list of ip in a prometheus compatible format
 ```
 
+#### Extended services filters
+
+Apart from standard Netbox filters, services endpoint also supports `tenant=<slug>` or `tenant_id=<id>` parameters.
+The lookup is only executed against the `tenant` attribute of the object associated with the service.
+
 ### Config context
 
 The plugin can also discover extra config to inject in the HTTP SD JSON from the config context of the devices/virtual machines.
 If you have a `prometheus-plugin-prometheus-sd` entry in your config context with the following schema it will be automatically picked up:
 
 ```
 prometheus-plugin-prometheus-sd:
@@ -106,21 +111,24 @@
 Netbox content should then be available in the service discovery tab.
 
 ## Development
 
 We use Poetry for dependency management and invoke as task runner.
 As Netbox plugins cannot be tested standalone, we need invoke to start all code embedded in Netbox Docker containers.
 
-All code to run in docker is located under `development`.
+All code to run in docker is located under `develop`.
 To start a virtual env managed by poetry run `poetry shell`.
 All following commands are started inside this environment.
 
 In order to run tests invoke the test steps
 
 ``` bash
+# Build Docker images
+invoke build
+
 # Execute all tests
 invoke tests
 
 # Execute unit tests only
 invoke unittest
 ```
 
@@ -135,7 +143,15 @@
 ```
 
 Visit http://localhost:8000 and log in with the new user.
 You can now define Netbox entities and test around.
 
 API endpoints for testing can be found at http://localhost:8000/api/plugins/prometheus-sd/
 
+## Conventional Commits
+
+This repository follows the Conventional Commits specification for versioning and changelog generation.
+Conventional Commits provide a standardized way of writing commit messages to convey semantic meaning
+about the changes made. Each commit message follows a defined format that includes a type,
+an optional scope, and a message. The types typically include features, fixes, documentation, and more.
+By adhering to this convention, we ensure clear and automated versioning, release notes, and changelog generation.
+
```

