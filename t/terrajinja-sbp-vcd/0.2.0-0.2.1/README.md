# Comparing `tmp/terrajinja-sbp-vcd-0.2.0.tar.gz` & `tmp/terrajinja-sbp-vcd-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrajinja-sbp-vcd-0.2.0.tar", last modified: Wed May  8 07:17:01 2024, max compression
+gzip compressed data, was "terrajinja-sbp-vcd-0.2.1.tar", last modified: Wed May  8 09:14:15 2024, max compression
```

## Comparing `terrajinja-sbp-vcd-0.2.0.tar` & `terrajinja-sbp-vcd-0.2.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:17:01.354379 terrajinja-sbp-vcd-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)       80 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/HISTORY.md
--rw-r--r--   0 root         (0) root         (0)     1061 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      336 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    14080 2024-05-08 07:17:01.354379 terrajinja-sbp-vcd-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/Pipfile
--rw-rw-rw-   0 root         (0) root         (0)    13274 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 07:17:01.355379 terrajinja-sbp-vcd-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1353 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:17:01.344379 terrajinja-sbp-vcd-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:17:01.344379 terrajinja-sbp-vcd-0.2.0/src/terrajinja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:17:01.344379 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:17:01.349379 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/data_vcd_catalog_vapp_template.py
--rw-rw-rw-   0 root         (0) root         (0)      702 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/data_vcd_nsxt_alb_edgegateway_service_engine_group.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/data_vcd_vm_placement_policy.py
--rw-rw-rw-   0 root         (0) root         (0)     1388 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     1781 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/network_routed_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     3180 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_alb_pool.py
--rw-rw-rw-   0 root         (0) root         (0)     2218 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_alb_virtual_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2835 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_app_port_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     2860 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_distributed_firewall.py
--rw-rw-rw-   0 root         (0) root         (0)     2447 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_edge_firewall.py
--rw-rw-rw-   0 root         (0) root         (0)     2152 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_edge_loadbalancer.py
--rw-rw-rw-   0 root         (0) root         (0)     2787 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_firewall_rule_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_ip_set.py
--rw-rw-rw-   0 root         (0) root         (0)     8977 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_nat_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     2996 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/rde.py
--rw-rw-rw-   0 root         (0) root         (0)    12827 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/vm.py
--rw-rw-rw-   0 root         (0) root         (0)     1774 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/vm_internal_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:17:01.354379 terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14080 2024-05-08 07:17:01.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1687 2024-05-08 07:17:01.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 07:17:01.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2024-05-08 07:17:01.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-08 07:17:01.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:17:01.353379 terrajinja-sbp-vcd-0.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1426 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_data_vcd_catalog_vapp_template.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_data_vcd_vm_placement_policy.py
--rw-rw-rw-   0 root         (0) root         (0)     3224 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_network_routed_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     1975 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_alb_pool.py
--rw-rw-rw-   0 root         (0) root         (0)     2750 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_app_port_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     4347 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_distributed_firewall.py
--rw-rw-rw-   0 root         (0) root         (0)     4001 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_edge_firewall.py
--rw-rw-rw-   0 root         (0) root         (0)     2520 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_edge_loadbalancer.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_firewall_rule_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4921 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_ip_set.py
--rw-rw-rw-   0 root         (0) root         (0)    28148 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_nat_rule.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_virtual_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1486 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_rde.py
--rw-rw-rw-   0 root         (0) root         (0)     1809 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_vm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:14:15.471830 terrajinja-sbp-vcd-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/HISTORY.md
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-05-08 09:14:14.000000 terrajinja-sbp-vcd-0.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      336 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    14080 2024-05-08 09:14:15.470830 terrajinja-sbp-vcd-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)    13274 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 09:14:15.471830 terrajinja-sbp-vcd-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1353 2024-05-08 09:14:14.000000 terrajinja-sbp-vcd-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:14:15.462830 terrajinja-sbp-vcd-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:14:15.462830 terrajinja-sbp-vcd-0.2.1/src/terrajinja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:14:15.462830 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:14:15.467830 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 09:14:14.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/data_vcd_catalog_vapp_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      702 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/data_vcd_nsxt_alb_edgegateway_service_engine_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/data_vcd_vm_placement_policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/network_routed_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3180 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_alb_pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2218 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_alb_virtual_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2835 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_app_port_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_distributed_firewall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_edge_firewall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2152 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_edge_loadbalancer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_firewall_rule_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_ip_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     8977 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_nat_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     2996 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/rde.py
+-rw-rw-rw-   0 root         (0) root         (0)    12878 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/vm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1774 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/vm_internal_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:14:15.470830 terrajinja-sbp-vcd-0.2.1/src/terrajinja_sbp_vcd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14080 2024-05-08 09:14:15.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja_sbp_vcd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1687 2024-05-08 09:14:15.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja_sbp_vcd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 09:14:15.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja_sbp_vcd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2024-05-08 09:14:15.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja_sbp_vcd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-08 09:14:15.000000 terrajinja-sbp-vcd-0.2.1/src/terrajinja_sbp_vcd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:14:15.470830 terrajinja-sbp-vcd-0.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/tests/test_data_vcd_catalog_vapp_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/tests/test_data_vcd_vm_placement_policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3224 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_network_routed_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1975 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_alb_pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2750 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_app_port_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     4347 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_distributed_firewall.py
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_edge_firewall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_edge_loadbalancer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_firewall_rule_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4921 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_ip_set.py
+-rw-rw-rw-   0 root         (0) root         (0)    28148 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_nat_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_virtual_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_rde.py
+-rw-rw-rw-   0 root         (0) root         (0)     1809 2024-05-08 09:14:13.000000 terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_vm.py
```

### Comparing `terrajinja-sbp-vcd-0.2.0/LICENSE` & `terrajinja-sbp-vcd-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/PKG-INFO` & `terrajinja-sbp-vcd-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrajinja-sbp-vcd
-Version: 0.2.0
+Version: 0.2.1
 Summary: Terrajinja extension for automation using cdktf
 Home-page: https://gitlab/terrajinja
 Author: Terrajinja Team
 Author-email: int-terrajinja@schubergphilis.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `terrajinja-sbp-vcd-0.2.0/README.md` & `terrajinja-sbp-vcd-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/setup.py` & `terrajinja-sbp-vcd-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = [line.strip()
           for line in open('requirements.txt').readlines()
           if line.strip() and not line.startswith('#')]
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
-version = '0.2.0'
+version = '0.2.1'
 name= 'terrajinja-sbp-vcd'
 package_path= name.replace('-', '.')
 
 # only the cli has an entry point
 entry_points=None
 if name=='terrajinja-cli':
     entry_points={
```

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/data_vcd_catalog_vapp_template.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/data_vcd_catalog_vapp_template.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/data_vcd_nsxt_alb_edgegateway_service_engine_group.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/data_vcd_nsxt_alb_edgegateway_service_engine_group.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/data_vcd_vm_placement_policy.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/data_vcd_vm_placement_policy.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/decorators.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/decorators.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/network_routed_v2.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/network_routed_v2.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_alb_pool.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_alb_pool.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_alb_virtual_service.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_alb_virtual_service.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_app_port_profile.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_app_port_profile.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_distributed_firewall.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_distributed_firewall.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_edge_firewall.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_edge_firewall.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_edge_loadbalancer.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_edge_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_firewall_rule_parser.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_firewall_rule_parser.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_ip_set.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_ip_set.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_nat_rule.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/nsxt_nat_rule.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/rde.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/rde.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/vm.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/vm.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,16 +108,17 @@
             chef_encrypted_databag_secret: str = None,
             chef_server_url: str = None,
             chef_environment: str = None,
             chef_validator_name: str = None,
             chef_validator_pem: str = None,
             depends_on_primary: bool = False,
             depends_on: list = None,
-            os_disk_size: str = "",  # empty means no change
+            os_disk_size: str = None,
             os_disk_iops: int = 5000,
+            os_disk_storage_profile: str = "generic",
             disks: list[dict] = None,
             shared_with_everyone: bool = True,
             everyone_access_level: str = "Change",
             **kwargs,
     ):
         """Enhances the original vcd.nsxt_ip_set
             Ensures that only one ip set is created, and validates its use across the deployment
@@ -240,15 +241,15 @@
             if os_disk_size:
                 kwargs['override_template_disk'] = [{
                     'busType': "paravirtual",
                     'sizeInMb': human_read_to_megabyte(os_disk_size),
                     'busNumber': 0,
                     'unitNumber': 0,
                     'iops': os_disk_iops,
-                    'storageProfile': "*",
+                    'storageProfile': os_disk_storage_profile,
                 }]
 
             new_vm = Vm(
                 scope=scope,
                 id_=f'vm_{vm.name}',
                 name=vm.name,
                 computer_name=vm.name,
```

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/vm_internal_disk.py` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja/sbp/vcd/vm_internal_disk.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/PKG-INFO` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja_sbp_vcd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrajinja-sbp-vcd
-Version: 0.2.0
+Version: 0.2.1
 Summary: Terrajinja extension for automation using cdktf
 Home-page: https://gitlab/terrajinja
 Author: Terrajinja Team
 Author-email: int-terrajinja@schubergphilis.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/SOURCES.txt` & `terrajinja-sbp-vcd-0.2.1/src/terrajinja_sbp_vcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/tests/test_data_vcd_catalog_vapp_template.py` & `terrajinja-sbp-vcd-0.2.1/tests/test_data_vcd_catalog_vapp_template.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/tests/test_data_vcd_vm_placement_policy.py` & `terrajinja-sbp-vcd-0.2.1/tests/test_data_vcd_vm_placement_policy.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_network_routed_v2.py` & `terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_network_routed_v2.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_alb_pool.py` & `terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_alb_pool.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_app_port_profile.py` & `terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_app_port_profile.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_distributed_firewall.py` & `terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_distributed_firewall.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_edge_firewall.py` & `terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_edge_firewall.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_edge_loadbalancer.py` & `terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_edge_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_firewall_rule_parser.py` & `terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_firewall_rule_parser.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_ip_set.py` & `terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_ip_set.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_nat_rule.py` & `terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_nat_rule.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_virtual_service.py` & `terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_nsxt_virtual_service.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_rde.py` & `terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_rde.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_vm.py` & `terrajinja-sbp-vcd-0.2.1/tests/test_sbp_vcd_vm.py`

 * *Files identical despite different names*

