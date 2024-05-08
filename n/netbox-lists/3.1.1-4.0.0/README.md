# Comparing `tmp/netbox_lists-3.1.1.tar.gz` & `tmp/netbox_lists-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_lists-3.1.1.tar", max compression
+gzip compressed data, was "netbox_lists-4.0.0.tar", max compression
```

## Comparing `netbox_lists-3.1.1.tar` & `netbox_lists-4.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11358 2023-08-26 18:00:32.067741 netbox_lists-3.1.1/LICENSE
--rw-r--r--   0        0        0     8818 2023-08-26 18:00:32.067741 netbox_lists-3.1.1/README.md
--rw-r--r--   0        0        0     2481 2023-08-26 18:00:32.071741 netbox_lists-3.1.1/netbox_lists/__init__.py
--rw-r--r--   0        0        0        0 2023-08-26 18:00:32.071741 netbox_lists-3.1.1/netbox_lists/api/__init__.py
--rw-r--r--   0        0        0       95 2023-08-26 18:00:32.071741 netbox_lists-3.1.1/netbox_lists/api/constants.py
--rw-r--r--   0        0        0     1942 2023-08-26 18:00:32.071741 netbox_lists-3.1.1/netbox_lists/api/filtersets.py
--rw-r--r--   0        0        0      547 2023-08-26 18:00:32.071741 netbox_lists-3.1.1/netbox_lists/api/renderers.py
--rw-r--r--   0        0        0     1831 2023-08-26 18:00:32.071741 netbox_lists-3.1.1/netbox_lists/api/serializers.py
--rw-r--r--   0        0        0     1385 2023-08-26 18:00:32.071741 netbox_lists-3.1.1/netbox_lists/api/urls.py
--rw-r--r--   0        0        0     6639 2023-08-26 18:00:32.071741 netbox_lists-3.1.1/netbox_lists/api/utils.py
--rw-r--r--   0        0        0    25851 2023-08-26 18:00:32.071741 netbox_lists-3.1.1/netbox_lists/api/views.py
--rw-r--r--   0        0        0        0 2023-08-26 18:00:32.071741 netbox_lists-3.1.1/netbox_lists/py.typed
--rw-r--r--   0        0        0     1023 2023-08-26 18:00:32.071741 netbox_lists-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     9428 1970-01-01 00:00:00.000000 netbox_lists-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-08 05:17:04.049067 netbox_lists-4.0.0/LICENSE
+-rw-r--r--   0        0        0     8668 2024-05-08 05:17:04.049067 netbox_lists-4.0.0/README.md
+-rw-r--r--   0        0        0     2458 2024-05-08 05:17:04.049067 netbox_lists-4.0.0/netbox_lists/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 05:17:04.049067 netbox_lists-4.0.0/netbox_lists/api/__init__.py
+-rw-r--r--   0        0        0       95 2024-05-08 05:17:04.049067 netbox_lists-4.0.0/netbox_lists/api/constants.py
+-rw-r--r--   0        0        0     1942 2024-05-08 05:17:04.049067 netbox_lists-4.0.0/netbox_lists/api/filtersets.py
+-rw-r--r--   0        0        0      547 2024-05-08 05:17:04.049067 netbox_lists-4.0.0/netbox_lists/api/renderers.py
+-rw-r--r--   0        0        0     1819 2024-05-08 05:17:04.049067 netbox_lists-4.0.0/netbox_lists/api/serializers.py
+-rw-r--r--   0        0        0     1385 2024-05-08 05:17:04.049067 netbox_lists-4.0.0/netbox_lists/api/urls.py
+-rw-r--r--   0        0        0     6619 2024-05-08 05:17:04.049067 netbox_lists-4.0.0/netbox_lists/api/utils.py
+-rw-r--r--   0        0        0    25565 2024-05-08 05:17:04.049067 netbox_lists-4.0.0/netbox_lists/api/views.py
+-rw-r--r--   0        0        0        0 2024-05-08 05:17:04.049067 netbox_lists-4.0.0/netbox_lists/py.typed
+-rw-r--r--   0        0        0     1025 2024-05-08 05:17:04.049067 netbox_lists-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9172 1970-01-01 00:00:00.000000 netbox_lists-4.0.0/PKG-INFO
```

### Comparing `netbox_lists-3.1.1/LICENSE` & `netbox_lists-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_lists-3.1.1/README.md` & `netbox_lists-4.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Lists are returned as JSON arrays or as plain text. This means that firewalls
 can use NetBox as a source for dynamic address lists, such as Palo Alto's External Dynamic Lists, Fortinet's External Block List (Threat Feed) or
 pfSesnse/OPNSense's firewall aliases.
 
 This plugin also features endpoints for devices/VMs/IP addresses compatible with Prometheus' http_sd.
 
-This plugin supports NetBox v3.0, v3.1, v3.2, v3.3, and v3.4.
+This plugin supports NetBox v4.0.
 
 ## Features
 * Supports NetBox's object permissions.
 
 * [Ansible](https://galaxy.ansible.com/devon_mar/nblists) and [Terraform](https://registry.terraform.io/providers/devon-mar/nblists/latest/docs) integrations.
 
 * Prometheus http_sd endpoint for devices/vms.
@@ -63,16 +63,14 @@
         # A list of attributes for the devices-vms-attrs endpoint
         #
         # Attributes will be joined with "__" in the returned object.
         # eg. ("primary_ip", "address") -> primary_ip__address
         "devices_vms_attrs": [
             ("id",),
             ("name",),
-            # `role` will automatically be converted to `device_role` for devices.
-            # Don't use `device_role`.
             ("role", "slug"),
             ("platform", "slug"),
             ("primary_ip", "address"),
             ("tags",),
         ],
         # Tuple/list of attributes to use for Prometheus VM SD target. Defaults are shown.
         #
```

### Comparing `netbox_lists-3.1.1/netbox_lists/__init__.py` & `netbox_lists-4.0.0/netbox_lists/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-__version__ = "3.1.1"
+__version__ = "4.0.0"
 
-from typing import List
 
-from extras.plugins import PluginConfig
+from netbox.plugins import PluginConfig
 
 
 class ListsPluginConfig(PluginConfig):
     name = "netbox_lists"
     verbose_name = "NetBox Lists"
     version = __version__
-    author = "Devon Mar"
+    author = "@devon-mar"
     base_url = "lists"
-    required_settings: List[str] = []
+    required_settings: list[str] = []
     default_settings = {
         "as_cidr": True,
         "service_primary_ips": True,
         "summarize": True,
         "devices_vms_attrs": [
             ("id",),
             ("name",),
```

### Comparing `netbox_lists-3.1.1/netbox_lists/api/filtersets.py` & `netbox_lists-4.0.0/netbox_lists/api/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_lists-3.1.1/netbox_lists/api/renderers.py` & `netbox_lists-4.0.0/netbox_lists/api/renderers.py`

 * *Files identical despite different names*

### Comparing `netbox_lists-3.1.1/netbox_lists/api/serializers.py` & `netbox_lists-4.0.0/netbox_lists/api/serializers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from itertools import chain
-from typing import Dict, Generic, List, TypeVar
+from typing import Generic, TypeVar
 
 from dcim.models import Device
 from django.conf import settings
 from ipam.models import IPAddress
 from rest_framework import serializers
 from utilities.exceptions import AbortRequest
 from virtualization.models import VirtualMachine
@@ -15,15 +15,15 @@
 
 class BasePrometheusSerializer(serializers.Serializer, Generic[T]):
     targets = serializers.SerializerMethodField()
     labels = serializers.SerializerMethodField()
 
     default_target_attr = "name"
 
-    def get_targets(self, device: T) -> List[str]:
+    def get_targets(self, device: T) -> list[str]:
         # Default to default_target_attr
         for attrs in chain(
             settings.PLUGINS_CONFIG["netbox_lists"][
                 f"prometheus_{self.settings_type}_sd_target"
             ],
             ((self.default_target_attr,),),
         ):
@@ -32,15 +32,15 @@
                 return [str(target)]
 
         # This shouldn't happen since default_target_attr should be a required field
         raise AbortRequest(
             f"No target found for {repr(device)}. (this shouldn't happen)"
         )
 
-    def get_labels(self, device: T) -> Dict[str, str]:
+    def get_labels(self, device: T) -> dict[str, str]:
         labels = {
             k: get_attr_str(v, device)
             for k, v in settings.PLUGINS_CONFIG["netbox_lists"][
                 f"prometheus_{self.settings_type}_sd_labels"
             ].items()
         }
```

### Comparing `netbox_lists-3.1.1/netbox_lists/api/urls.py` & `netbox_lists-4.0.0/netbox_lists/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_lists-3.1.1/netbox_lists/api/utils.py` & `netbox_lists-4.0.0/netbox_lists/api/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import itertools
-from typing import Any, Iterable, List, Union
+from typing import Any, Iterable, Optional
 
 from django.conf import settings
 from django.db.models import Q
 from django.db.models.query import QuerySet
 from django_filters import FilterSet
 from django_filters.utils import translate_validation
 from netaddr import cidr_merge, IPNetwork, iprange_to_cidrs
@@ -36,15 +36,15 @@
 
 def set_prefixlen_max(ipn: IPNetwork) -> IPNetwork:
     ipn.prefixlen = 32 if ipn.version == 4 else 128
     return ipn
 
 
 def device_vm_primary_list(
-    qs: QuerySet[Any], family: Union[int, None]
+    qs: QuerySet[Any], family: Optional[int]
 ) -> Iterable[IPNetwork]:
     if family is None:
         queryset = qs.filter(
             Q(primary_ip4__isnull=False) | Q(primary_ip6__isnull=False)
         )
         retindex = -1
     elif family == 4:
@@ -61,18 +61,18 @@
     else:
         return (
             set_prefixlen_max(i) for i in itertools.chain.from_iterable(queryset) if i
         )
 
 
 def services_primary_ips(
-    qs: QuerySet[Any], family: Union[int, None]
+    qs: QuerySet[Any], family: Optional[int]
 ) -> Iterable[IPNetwork]:
     family_filter = Q()
-    values: List[str] = []
+    values: list[str] = []
     if family == 4 or family is None:
         family_filter |= Q(device__primary_ip4__isnull=False) | Q(
             virtual_machine__primary_ip4__isnull=False
         )
         values.extend(
             [
                 "device__primary_ip4__address",
@@ -91,15 +91,15 @@
         )
 
     qs = qs.filter(Q(ipaddresses__isnull=True), family_filter).values_list(*values)
     return (set_prefixlen_max(i) for i in itertools.chain.from_iterable(qs) if i)
 
 
 def services_assigned_ips(
-    qs: QuerySet[Any], family: Union[int, None]
+    qs: QuerySet[Any], family: Optional[int]
 ) -> Iterable[IPNetwork]:
     if family is None:
         family_filter = Q()
     elif family == 4:
         family_filter = Q(ipaddresses__address__family=4)
     else:
         family_filter = Q(ipaddresses__address__family=6)
@@ -108,17 +108,17 @@
         qs.filter(Q(ipaddresses__isnull=False), family_filter)
         .values_list("ipaddresses__address", flat=True)
         .distinct()
     )
 
 
 def get_service_ips(
-    qs: QuerySet[Any], family: Union[int, None], include_primaries: bool
+    qs: QuerySet[Any], family: Optional[int], include_primaries: bool
 ) -> Iterable[IPNetwork]:
-    iterables: List[Iterable[IPNetwork]] = [services_assigned_ips(qs, family)]
+    iterables: list[Iterable[IPNetwork]] = [services_assigned_ips(qs, family)]
 
     if include_primaries is True:
         iterables.append(services_primary_ips(qs, family))
 
     return (set_prefixlen_max(i) for i in itertools.chain.from_iterable(iterables))
 
 
@@ -130,15 +130,15 @@
         return True
     elif val.lower() == "false":
         return False
     else:
         raise ValidationError(f"{param} must be true or false.")
 
 
-def get_family_param(req: Request) -> Union[int, None]:
+def get_family_param(req: Request) -> Optional[int]:
     """
     Raises a ValidationError if family is not '4' or '6'.
     """
     val = req.query_params.get(FAMILY_PARAM_NAME, None)
 
     if val is not None and val not in ["4", "6"]:
         raise ValidationError("Family must be 4 or 6.")
@@ -168,19 +168,19 @@
         return True
     elif val.lower() == "false":
         return False
     else:
         raise ValidationError("summarize must be true or false.")
 
 
-def ip_range_prefixes(start: IPNetwork, end: IPNetwork) -> List[IPNetwork]:
+def ip_range_prefixes(start: IPNetwork, end: IPNetwork) -> list[IPNetwork]:
     return iprange_to_cidrs(start.ip, end.ip)
 
 
-def _json_rep(obj: Any) -> Union[str, int, bool, list, dict, None]:
+def _json_rep(obj: Any) -> str | int | bool | list | dict | None:
     """Return a JSON serializable representation"""
     if isinstance(obj, (str, int, bool)) or obj is None:
         return obj
     elif isinstance(obj, list):
         return [_json_rep(o) for o in obj]
     elif isinstance(obj, dict):
         return {str(k): _json_rep(v) for k, v in obj.items()}
```

### Comparing `netbox_lists-3.1.1/netbox_lists/api/views.py` & `netbox_lists-4.0.0/netbox_lists/api/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import itertools
 import operator
 from functools import reduce
-from typing import Any, Dict, Iterable, List, Optional, Union
+from typing import Any, Iterable, Optional
 
 from dcim.filtersets import DeviceFilterSet
 from dcim.models import Device
 from django.conf import settings
 from django.db.models import Q
 from django_filters.rest_framework import DjangoFilterBackend
 from drf_spectacular.utils import (
@@ -404,15 +404,15 @@
         return (
             param in request.query_params
             or ("all" in request.query_params and not primary)
             or ("all_primary" in request.query_params and primary)
         )
 
     def get_prefixes(
-        self, tag: Tag, family: Union[int, None], request: Request
+        self, tag: Tag, family: Optional[int], request: Request
     ) -> Iterable[IPNetwork]:
         if not self.param_all_any(request, "prefixes"):
             return []
 
         if family == 4:
             family_filter = Q(prefix__family=4)
         elif family == 6:
@@ -423,15 +423,15 @@
             Prefix.objects.restrict(request.user, "view")
             .filter(Q(tags=tag) & family_filter)
             .values_list("prefix", flat=True)
             .distinct()
         )
 
     def get_aggregates(
-        self, tag: Tag, family: Union[int, None], request: Request
+        self, tag: Tag, family: Optional[int], request: Request
     ) -> Iterable[IPNetwork]:
         if not self.param_all_any(request, "aggregates"):
             return []
 
         if family == 4:
             family_filter = Q(prefix__family=4)
         elif family == 6:
@@ -443,15 +443,15 @@
             Aggregate.objects.restrict(request.user, "view")
             .filter(Q(tags=tag) & family_filter)
             .values_list("prefix", flat=True)
             .distinct()
         )
 
     def get_ips(
-        self, tag: Tag, family: Union[int, None], request: Request
+        self, tag: Tag, family: Optional[int], request: Request
     ) -> Iterable[IPNetwork]:
         if family == 4:
             family_filter = Q(address__family=4)
         elif family == 6:
             family_filter = Q(address__family=6)
         else:
             family_filter = Q()
@@ -472,37 +472,37 @@
                 .values_list("address", flat=True)
                 .distinct()
             )
         else:
             return []
 
     def get_services(
-        self, tag: Tag, family: Union[int, None], request: Request
+        self, tag: Tag, family: Optional[int], request: Request
     ) -> Iterable[IPNetwork]:
         if not self.param_all_any(request, "services"):
             return []
 
         return get_service_ips(
             Service.objects.restrict(request.user, "view").filter(tags=tag),
             family,
             get_svc_primary_ips_param("service_primary_ips", request),
         )
 
     def get_devices_primary(
-        self, tag: Tag, family: Union[int, None], request: Request
+        self, tag: Tag, family: Optional[int], request: Request
     ) -> Iterable[IPNetwork]:
         if not self.param_all_primary(request, "devices_primary", True):
             return []
 
         return device_vm_primary_list(
             Device.objects.restrict(request.user, "view").filter(tags=tag), family
         )
 
     def get_vms_primary(
-        self, tag: Tag, family: Union[int, None], request: Request
+        self, tag: Tag, family: Optional[int], request: Request
     ) -> Iterable[IPNetwork]:
         if not self.param_all_primary(request, "vms_primary", True):
             return []
 
         return device_vm_primary_list(
             VirtualMachine.objects.restrict(request.user, "view").filter(tags=tag),
             family,
@@ -672,16 +672,16 @@
     filter_backends = (DjangoFilterBackend,)
     queryset = Device.objects.filter()
 
     def _to_dict(
         self,
         attrs: Iterable[Iterable[str]],
         display_attrs: Iterable[Iterable[str]],
-        device: Union[Device, VirtualMachine],
-    ) -> Dict[str, Any]:
+        device: Device | VirtualMachine,
+    ) -> dict[str, Any]:
         """Convert a device or VM to a dictionary"""
         return {
             "__".join(d_a): get_attr_json(a, device)
             for a, d_a in zip(attrs, display_attrs)
         }
 
     def validate_filters(self):
@@ -719,30 +719,23 @@
         },
     )
     def list(self, request: Request) -> Response:
         self.validate_filters()
 
         attrs = settings.PLUGINS_CONFIG["netbox_lists"]["devices_vms_attrs"]
 
-        device_attrs: List[Iterable[str]] = []
-        for a in attrs:
-            if len(a) > 0 and a[0] == "role":
-                device_attrs.append(("device_role", *a[1:]))
-            else:
-                device_attrs.append(a)
-
         devices = filter_queryset(
             DeviceFilterSet(
                 request.query_params,
                 queryset=Device.objects.restrict(request.user, "view").all(),
             )
         )
         vms = filter_queryset(
             VirtualMachineFilterSet(
                 request.query_params,
                 queryset=VirtualMachine.objects.restrict(request.user, "view").all(),
             )
         )
         return Response(
             [self._to_dict(attrs, attrs, d) for d in vms]
-            + [self._to_dict(device_attrs, attrs, d) for d in devices]
+            + [self._to_dict(attrs, attrs, d) for d in devices]
         )
```

### Comparing `netbox_lists-3.1.1/pyproject.toml` & `netbox_lists-4.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "netbox-lists"
-version = "3.1.1"
+version = "4.0.0"
 description = ""
 authors = ["Devon Mar <devonm@mdmm.ca>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
-netaddr = "^0.8.0"
+python = "^3.10"
+netaddr = ">=0.8,<1.3"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.0"
+pytest = "^8.2"
 flake8 = "^5.0"
-pynetbox = "^7.0.1"
+pynetbox = "^7.2.0"
 requests = "^2.27.1"
 isort = "^5.10.1"
-black = "^22.8.0"
-mypy = "^0.971"
+black = "^24.4.2"
+mypy = "^1.10"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `netbox_lists-3.1.1/PKG-INFO` & `netbox_lists-4.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: netbox-lists
-Version: 3.1.1
+Version: 4.0.0
 Summary: 
 License: Apache-2.0
 Author: Devon Mar
 Author-email: devonm@mdmm.ca
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: netaddr (>=0.8.0,<0.9.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: netaddr (>=0.8,<1.3)
 Description-Content-Type: text/markdown
 
 # netbox-lists
 
 NetBox Lists generates list of IPs and prefixes from NetBox data.
 While this can be accomplished using the existing NetBox API, this plugin
 saves the user from having to manipulate the data to get just the IPs/prefixes. Lists endpoints (mostly) share the same filters as the builtin NetBox endpoints, making querying easy.
 
 Lists are returned as JSON arrays or as plain text. This means that firewalls
 can use NetBox as a source for dynamic address lists, such as Palo Alto's External Dynamic Lists, Fortinet's External Block List (Threat Feed) or
 pfSesnse/OPNSense's firewall aliases.
 
 This plugin also features endpoints for devices/VMs/IP addresses compatible with Prometheus' http_sd.
 
-This plugin supports NetBox v3.0, v3.1, v3.2, v3.3, and v3.4.
+This plugin supports NetBox v4.0.
 
 ## Features
 * Supports NetBox's object permissions.
 
 * [Ansible](https://galaxy.ansible.com/devon_mar/nblists) and [Terraform](https://registry.terraform.io/providers/devon-mar/nblists/latest/docs) integrations.
 
 * Prometheus http_sd endpoint for devices/vms.
@@ -81,16 +79,14 @@
         # A list of attributes for the devices-vms-attrs endpoint
         #
         # Attributes will be joined with "__" in the returned object.
         # eg. ("primary_ip", "address") -> primary_ip__address
         "devices_vms_attrs": [
             ("id",),
             ("name",),
-            # `role` will automatically be converted to `device_role` for devices.
-            # Don't use `device_role`.
             ("role", "slug"),
             ("platform", "slug"),
             ("primary_ip", "address"),
             ("tags",),
         ],
         # Tuple/list of attributes to use for Prometheus VM SD target. Defaults are shown.
         #
```

