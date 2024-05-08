# Comparing `tmp/terrajinja-sbp-vcd-0.1.9.tar.gz` & `tmp/terrajinja-sbp-vcd-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrajinja-sbp-vcd-0.1.9.tar", last modified: Wed Apr 10 19:53:22 2024, max compression
+gzip compressed data, was "terrajinja-sbp-vcd-0.2.0.tar", last modified: Wed May  8 07:17:01 2024, max compression
```

## Comparing `terrajinja-sbp-vcd-0.1.9.tar` & `terrajinja-sbp-vcd-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:53:22.517024 terrajinja-sbp-vcd-0.1.9/
--rw-rw-rw-   0 root         (0) root         (0)       80 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/HISTORY.md
--rw-r--r--   0 root         (0) root         (0)     1061 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      336 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    14080 2024-04-10 19:53:22.516023 terrajinja-sbp-vcd-0.1.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/Pipfile
--rw-rw-rw-   0 root         (0) root         (0)    13274 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 19:53:22.517024 terrajinja-sbp-vcd-0.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1353 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:53:22.507023 terrajinja-sbp-vcd-0.1.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:53:22.507023 terrajinja-sbp-vcd-0.1.9/src/terrajinja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:53:22.507023 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:53:22.513023 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/data_vcd_catalog_vapp_template.py
--rw-rw-rw-   0 root         (0) root         (0)      702 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/data_vcd_nsxt_alb_edgegateway_service_engine_group.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/data_vcd_vm_placement_policy.py
--rw-rw-rw-   0 root         (0) root         (0)     1388 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/network_routed_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     2655 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_alb_pool.py
--rw-rw-rw-   0 root         (0) root         (0)     2163 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_alb_virtual_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2835 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_app_port_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     2860 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_distributed_firewall.py
--rw-rw-rw-   0 root         (0) root         (0)     2447 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_edge_firewall.py
--rw-rw-rw-   0 root         (0) root         (0)     2152 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_edge_loadbalancer.py
--rw-rw-rw-   0 root         (0) root         (0)     2787 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_firewall_rule_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_ip_set.py
--rw-rw-rw-   0 root         (0) root         (0)     8977 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_nat_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     2996 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/rde.py
--rw-rw-rw-   0 root         (0) root         (0)    12351 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/vm.py
--rw-rw-rw-   0 root         (0) root         (0)     1774 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/vm_internal_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:53:22.516023 terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14080 2024-04-10 19:53:22.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1687 2024-04-10 19:53:22.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 19:53:22.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2024-04-10 19:53:22.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-10 19:53:22.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:53:22.516023 terrajinja-sbp-vcd-0.1.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1426 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_data_vcd_catalog_vapp_template.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_data_vcd_vm_placement_policy.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_network_routed_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     2002 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_alb_pool.py
--rw-rw-rw-   0 root         (0) root         (0)     2750 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_app_port_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     4347 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_distributed_firewall.py
--rw-rw-rw-   0 root         (0) root         (0)     4001 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_edge_firewall.py
--rw-rw-rw-   0 root         (0) root         (0)     2520 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_edge_loadbalancer.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_firewall_rule_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4921 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_ip_set.py
--rw-rw-rw-   0 root         (0) root         (0)    28148 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_nat_rule.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_virtual_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1486 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_rde.py
--rw-rw-rw-   0 root         (0) root         (0)      912 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_vm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:17:01.354379 terrajinja-sbp-vcd-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/HISTORY.md
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      336 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    14080 2024-05-08 07:17:01.354379 terrajinja-sbp-vcd-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)    13274 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 07:17:01.355379 terrajinja-sbp-vcd-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1353 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:17:01.344379 terrajinja-sbp-vcd-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:17:01.344379 terrajinja-sbp-vcd-0.2.0/src/terrajinja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:17:01.344379 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:17:01.349379 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/data_vcd_catalog_vapp_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      702 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/data_vcd_nsxt_alb_edgegateway_service_engine_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/data_vcd_vm_placement_policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/network_routed_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3180 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_alb_pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2218 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_alb_virtual_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2835 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_app_port_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_distributed_firewall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_edge_firewall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2152 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_edge_loadbalancer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_firewall_rule_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_ip_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     8977 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_nat_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     2996 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/rde.py
+-rw-rw-rw-   0 root         (0) root         (0)    12827 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/vm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1774 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/vm_internal_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:17:01.354379 terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14080 2024-05-08 07:17:01.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1687 2024-05-08 07:17:01.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 07:17:01.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2024-05-08 07:17:01.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-08 07:17:01.000000 terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:17:01.353379 terrajinja-sbp-vcd-0.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_data_vcd_catalog_vapp_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_data_vcd_vm_placement_policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3224 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_network_routed_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1975 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_alb_pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2750 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_app_port_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     4347 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_distributed_firewall.py
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_edge_firewall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_edge_loadbalancer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_firewall_rule_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4921 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_ip_set.py
+-rw-rw-rw-   0 root         (0) root         (0)    28148 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_nat_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_virtual_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_rde.py
+-rw-rw-rw-   0 root         (0) root         (0)     1809 2024-05-08 07:17:00.000000 terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_vm.py
```

### Comparing `terrajinja-sbp-vcd-0.1.9/LICENSE` & `terrajinja-sbp-vcd-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/PKG-INFO` & `terrajinja-sbp-vcd-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrajinja-sbp-vcd
-Version: 0.1.9
+Version: 0.2.0
 Summary: Terrajinja extension for automation using cdktf
 Home-page: https://gitlab/terrajinja
 Author: Terrajinja Team
 Author-email: int-terrajinja@schubergphilis.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `terrajinja-sbp-vcd-0.1.9/README.md` & `terrajinja-sbp-vcd-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/setup.py` & `terrajinja-sbp-vcd-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = [line.strip()
           for line in open('requirements.txt').readlines()
           if line.strip() and not line.startswith('#')]
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
-version = '0.1.9'
+version = '0.2.0'
 name= 'terrajinja-sbp-vcd'
 package_path= name.replace('-', '.')
 
 # only the cli has an entry point
 entry_points=None
 if name=='terrajinja-cli':
     entry_points={
```

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/data_vcd_catalog_vapp_template.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/data_vcd_catalog_vapp_template.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/data_vcd_nsxt_alb_edgegateway_service_engine_group.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/data_vcd_nsxt_alb_edgegateway_service_engine_group.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/data_vcd_vm_placement_policy.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/data_vcd_vm_placement_policy.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/decorators.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/decorators.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/network_routed_v2.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/network_routed_v2.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,42 +4,46 @@
 
 from terrajinja.imports.vcd.network_routed_v2 import NetworkRoutedV2
 
 
 class SbpVcdNetworkRoutedV2(NetworkRoutedV2):
     """SBP version of vcd.network_routed_v2"""
 
-    def __init__(self, scope: Construct, ns: str, cidr: str, dns: list, **kwargs):
+    def __init__(self, scope: Construct, ns: str, cidr: str, dns: list = None, **kwargs):
         """Enhances the original vcd.network_routed_v2
 
         Args:
             scope (Construct): Cdktf App
             id (str): uniq name of the resource
             result_cache (dict): cache of all collected resource outputs so far
             cidr (str): a cidr block to add, which will be used to calculate static_ip_pool and gateway parameters
             dns (list): a list of ips to the dns servers, will be used to fill the dns1 and dns2 parameters
 
         Original:
             https://registry.terraform.io/providers/vmware/vcd/latest/docs/resources/network_routed_v2
         """
         # prepare arguments for constructs
         cidr_ = IPv4Network(cidr)
-        static_ip_pool = [
+        calculated_static_ip_pool = [
             {
                 "startAddress": str(cidr_.network_address + 2),
                 "endAddress": str(cidr_.broadcast_address - 1),
             }
         ]
-        dns1, dns2 = dns
-        gateway = str(cidr_.network_address + 1)
+        calculated_gateway = str(cidr_.network_address + 1)
+
+        dns1 = kwargs.get('dns1')
+        dns2 = kwargs.get('dns2')
+        if dns:
+            dns1, dns2 = dns
 
         # call the original resource
         super().__init__(
             scope=scope,
             id_=ns,
-            gateway=gateway,
-            prefix_length=cidr_.prefixlen,
+            gateway=kwargs.pop('gateway', calculated_gateway),
+            prefix_length=kwargs.pop('prefix_length', cidr_.prefixlen),
+            static_ip_pool=kwargs.pop('static_ip_pool', calculated_static_ip_pool),
             dns1=dns1,
             dns2=dns2,
-            static_ip_pool=static_ip_pool,
             **kwargs,
         )
```

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_alb_pool.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_alb_pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,41 +41,52 @@
 
 
 @run_once(parameter_match=["destination_address_name", "destination_port"])
 class SbpVcdNsxtAlbPool(NsxtAlbPool):
     """Extends the original class to ensure that it only gets called once"""
 
     def __init__(self, scope: Construct, destination_address_name: str, destination_port: int,
-                 algorithm: str, persistence: str, vip_port: int, destination_address: (list | str),
+                 algorithm: str, persistence: str, vip_port: int, destination_address: list,
                  edge_gateway_id: str, id_=None, **kwargs):
 
         pool = SbpLoadbalancerPool(
             scope=scope,
             destination_address_name=destination_address_name,
             destination_port=destination_port,
             algorithm=algorithm,
             persistence=persistence,
             default_port=vip_port,
             destination_address=destination_address,
             edge_gateway_id=edge_gateway_id
         )
 
+        # destination can be a set of ip, or a link to a resource (e.g. security group/ precreated ip set)
         if isinstance(destination_address, str):
             destination_address = [destination_address]
 
+        # test if destination is an ip or resource
         try:
             IPv4Network(destination_address[0])
             member_group_id = pool.member_group_id
+            default_port = pool.default_port
+            algorithm = pool.algorithm
+            persistence = pool.persistence_profile
         except AddressValueError:
             member_group_id = destination_address[0]
+            default_port = destination_port
+            algorithm = algorithm.upper().replace(' ', '_')
+            persistence = {
+                'type': persistence.upper().replace(' ', '_')
+            }
 
         super().__init__(
             scope=scope,
             id_=pool.name,
             name=pool.name,
-            algorithm=pool.algorithm,
-            persistence_profile=pool.persistence_profile,
-            default_port=pool.default_port,
+            algorithm=algorithm,
+            persistence_profile=persistence,
+            default_port=default_port,
             member_group_id=member_group_id,
             edge_gateway_id=edge_gateway_id,
+            lifecycle={'create_before_destroy': True},
             **kwargs
         )
```

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_alb_virtual_service.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_alb_virtual_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,9 +62,10 @@
             scope=scope,
             id_=service.name,
             name=service.name,
             application_profile_type=service_type,
             pool_id=pool_id,
             virtual_ip_address=virtual_ip_address,
             service_port=service.service_port,
+            lifecycle={'create_before_destroy': True},
             **kwargs
         )
```

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_app_port_profile.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_app_port_profile.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_distributed_firewall.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_distributed_firewall.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_edge_firewall.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_edge_firewall.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_edge_loadbalancer.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_edge_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_firewall_rule_parser.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_firewall_rule_parser.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_ip_set.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_ip_set.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_nat_rule.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/nsxt_nat_rule.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/rde.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/rde.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/vm.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/vm.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,16 @@
             chef_encrypted_databag_secret: str = None,
             chef_server_url: str = None,
             chef_environment: str = None,
             chef_validator_name: str = None,
             chef_validator_pem: str = None,
             depends_on_primary: bool = False,
             depends_on: list = None,
+            os_disk_size: str = "",  # empty means no change
+            os_disk_iops: int = 5000,
             disks: list[dict] = None,
             shared_with_everyone: bool = True,
             everyone_access_level: str = "Change",
             **kwargs,
     ):
         """Enhances the original vcd.nsxt_ip_set
             Ensures that only one ip set is created, and validates its use across the deployment
@@ -231,14 +233,24 @@
             time_sleep_destroy_vm = Sleep(
                 scope=scope,
                 id=f'vm_{vm.name}_destroy_sleep',
                 destroy_duration="30s",
                 depends_on=modified_depends_on,
             )
 
+            if os_disk_size:
+                kwargs['override_template_disk'] = [{
+                    'busType': "paravirtual",
+                    'sizeInMb': human_read_to_megabyte(os_disk_size),
+                    'busNumber': 0,
+                    'unitNumber': 0,
+                    'iops': os_disk_iops,
+                    'storageProfile': "*",
+                }]
+
             new_vm = Vm(
                 scope=scope,
                 id_=f'vm_{vm.name}',
                 name=vm.name,
                 computer_name=vm.name,
                 vapp_template_id=vm_template.id,
                 memory=memory,
```

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/vm_internal_disk.py` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja/sbp/vcd/vm_internal_disk.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/PKG-INFO` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrajinja-sbp-vcd
-Version: 0.1.9
+Version: 0.2.0
 Summary: Terrajinja extension for automation using cdktf
 Home-page: https://gitlab/terrajinja
 Author: Terrajinja Team
 Author-email: int-terrajinja@schubergphilis.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/SOURCES.txt` & `terrajinja-sbp-vcd-0.2.0/src/terrajinja_sbp_vcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/tests/test_data_vcd_catalog_vapp_template.py` & `terrajinja-sbp-vcd-0.2.0/tests/test_data_vcd_catalog_vapp_template.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/tests/test_data_vcd_vm_placement_policy.py` & `terrajinja-sbp-vcd-0.2.0/tests/test_data_vcd_vm_placement_policy.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_network_routed_v2.py` & `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_network_routed_v2.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,14 +26,47 @@
         has_resource_with_properties(synthesized, "vcd_network_routed_v2", {"prefix_length": prefix_length})
         has_resource_with_properties(
             synthesized,
             "vcd_network_routed_v2",
             {"static_ip_pool": static_ip_pool},
         )
 
+    def test_new_var(self, stack):
+        # stack = TerraformStack(Testing.app(), "stack")
+        SbpVcdNetworkRoutedV2(
+            stack,
+            f"route_new_var",
+            cidr='40.40.0.0/16',
+            name="name",
+            edge_gateway_id="id",
+            guest_vlan_allowed=True
+        )
+        synthesized = Testing.synth(stack)
+
+        has_resource(synthesized, "vcd_network_routed_v2")
+        has_resource_with_properties(synthesized, "vcd_network_routed_v2", {"gateway": "40.40.0.1"})
+        has_resource_with_properties(synthesized, "vcd_network_routed_v2", {"guest_vlan_allowed": True})
+
+    def test_override_gateway(self, stack):
+        # stack = TerraformStack(Testing.app(), "stack")
+        SbpVcdNetworkRoutedV2(
+            stack,
+            f"route_override_gateway",
+            cidr='40.40.0.0/16',
+            name="name",
+            edge_gateway_id="id",
+            gateway="10.10.10.10"
+        )
+        synthesized = Testing.synth(stack)
+        print(synthesized)
+
+        has_resource(synthesized, "vcd_network_routed_v2")
+        has_resource_with_properties(synthesized, "vcd_network_routed_v2", {"gateway": "10.10.10.10"})
+
+
     def test_cidr_empty(self, stack):
         with pytest.raises(AddressValueError) as context:
             SbpVcdNetworkRoutedV2(stack, "empty_cidr", "", ["", ""], name="name", edge_gateway_id="id")
 
         assert "Address cannot be empty" == str(context.value)
 
     def test_cidr_invalid(self, stack):
```

### Comparing `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_alb_pool.py` & `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_alb_pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,14 @@
             vip_port=8080
         )
         # We should have gotten a formatted pool name
         assert pool.name_input == 'NAME-8080-POOL'
 
         synthesized = Testing.synth(stack)
         j = json.loads(synthesized)
-        print(synthesized)
 
         has_resource(synthesized, "vcd_nsxt_alb_pool")
         # resource has a link to an other resource instead of ips
         assert j['resource']['vcd_nsxt_alb_pool']['NAME-8080-POOL']['member_group_id'] == "id_to_resource"
 
 
 if __name__ == "__main__":
```

### Comparing `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_app_port_profile.py` & `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_app_port_profile.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_distributed_firewall.py` & `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_distributed_firewall.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_edge_firewall.py` & `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_edge_firewall.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_edge_loadbalancer.py` & `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_edge_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_firewall_rule_parser.py` & `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_firewall_rule_parser.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_ip_set.py` & `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_ip_set.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_nat_rule.py` & `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_nat_rule.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_virtual_service.py` & `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_nsxt_virtual_service.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_rde.py` & `terrajinja-sbp-vcd-0.2.0/tests/test_sbp_vcd_rde.py`

 * *Files identical despite different names*

