# Comparing `tmp/iac_init-0.5.8.tar.gz` & `tmp/iac_init-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.5.8.tar", max compression
+gzip compressed data, was "iac_init-0.5.9.tar", max compression
```

## Comparing `iac_init-0.5.8.tar` & `iac_init-0.5.9.tar`

### file list

```diff
@@ -1,102 +1,103 @@
--rw-r--r--   0        0        0    16295 2024-05-07 04:39:46.483204 iac_init-0.5.8/LICENSE
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.483204 iac_init-0.5.8/README.md
--rw-r--r--   0        0        0      389 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/__main__.py
--rw-r--r--   0        0        0    13292 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/cli/main.py
--rw-r--r--   0        0        0      206 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/cli/options.py
--rw-r--r--   0        0        0     2064 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     2886 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0     1041 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2595 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     7490 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      453 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0      263 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0     3778 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6989 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1370 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.483204 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1557 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/03-node_registration/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/06-fabric_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/07-access_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-07 04:39:46.487205 iac_init-0.5.8/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/09-smart_licensing/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/10-confg_aaa/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/11-config_monitor/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/templates/12-config_backup/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4910 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/utils/functional.py
--rw-r--r--   0        0        0    11463 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/validator.py
--rw-r--r--   0        0        0     5093 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5222 2024-05-07 04:39:46.491205 iac_init-0.5.8/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1636 2024-05-07 04:39:46.491205 iac_init-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-08 13:34:21.406823 iac_init-0.5.9/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.406823 iac_init-0.5.9/README.md
+-rw-r--r--   0        0        0      389 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/__main__.py
+-rw-r--r--   0        0        0    11618 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/cli/main.py
+-rw-r--r--   0        0        0      206 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/cli/options.py
+-rw-r--r--   0        0        0     2064 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     2886 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0     1406 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2595 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     7490 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      453 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0      263 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0      334 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/scripts/thread_tool.py
+-rw-r--r--   0        0        0     3778 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.406823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1557 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/03-node_registration/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/06-fabric_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-08 13:34:21.410823 iac_init-0.5.9/iac_init/templates/07-access_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/09-smart_licensing/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/10-confg_aaa/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/11-config_monitor/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/templates/12-config_backup/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4910 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    11463 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/validator.py
+-rw-r--r--   0        0        0     5093 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5222 2024-05-08 13:34:21.414823 iac_init-0.5.9/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1636 2024-05-08 13:34:21.414823 iac_init-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.5.9/PKG-INFO
```

### Comparing `iac_init-0.5.8/LICENSE` & `iac_init-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/cli/main.py` & `iac_init-0.5.9/iac_init/cli/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # -*- coding: utf-8 -*-
 
 # Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
 
 import os
-import re
 import sys
 import click
 import shutil
-import logging
-import threading
 import errorhandler
 import iac_init.validator
 
 from . import options
 from loguru import logger
-from ansible_runner import run
 from iac_init.conf import settings
 from iac_init.yaml_conf import yaml_writer
-from iac_init.scripts.ansible_tool import run_ansible_playbook
+from iac_init.scripts.thread_tool import MyThread
+from iac_init.scripts.ansible_tool import ansible_deploy_function
 
 error_handler = errorhandler.ErrorHandler()
 ansible_run_result = 1
 
 @click.command(context_settings=dict(help_option_names=["-h", "--help"]))
 @click.version_option(iac_init.__version__)
 @options.yaml_dir_path
@@ -96,65 +93,42 @@
 
             except Exception as e:
                 msg = "Generate working directory fail, detail: {}".format(e)
                 logger.error(msg)
                 exit()
 
             try:
-                def ansible_deploy_function(playbook_name, step_name):
-                    import logging
-                    from logging.handlers import TimedRotatingFileHandler
-
-                    playbook_dir = os.path.join(os.getcwd(), output,
-                                                os.path.basename(settings.TEMPLATE_DIR[int(option) - 1]),
-                                                playbook_name)
-
-                    logger = logging.getLogger(playbook_dir)
-                    logger.setLevel(logging.INFO)
-                    log_formatter = logging.Formatter('%(message)s')
-                    log_file = os.path.join(settings.OUTPUT_BASE_DIR, 'iac_init_log',
-                                                 'iac-init-{}-{}.log'.format(option, step_name))
-                    file_handler = TimedRotatingFileHandler(log_file, when="M", interval=30, backupCount=0)
-                    file_handler.setFormatter(log_formatter)
-                    logger.addHandler(file_handler)
-
-                    def callback(res):
-                        output = re.compile(r'\x1b\[\[?(?:\d{1,2}(?:;\d{0,2})*)?[m|K]').sub('', res['stdout'])
-                        logger.info(output)
-
-                    runner = run(playbook=playbook_dir, inventory=None, verbosity=5,
-                                 quiet=True, event_handler=callback)
-
-                    if runner.status == "successful":
-                        logger.info("Successfully finish Step {}: {}".format(option, step_name.upper()))
-
-                    else:
-                        logger.error("Failed run Step {}: {}".format(option, step_name.upper()))
-                        global ansible_run_result
-                        ansible_run_result = 0
-                        exit()
-
-                thread1 = threading.Thread(target=ansible_deploy_function,
-                                           args=("playbook_apic_init.yaml", settings.ANSIBLE_STEP[3]))
-                thread2 = threading.Thread(target=ansible_deploy_function,
-                                           args=("playbook_aci_switch_init.yaml", settings.ANSIBLE_STEP[4]))
+                playbook_dir_apic = os.path.join(os.getcwd(), output,
+                                            os.path.basename(settings.TEMPLATE_DIR[int(option) - 1]),
+                                            "playbook_apic_init.yaml")
+
+                playbook_dir_switch = os.path.join(os.getcwd(), output,
+                                            os.path.basename(settings.TEMPLATE_DIR[int(option) - 1]),
+                                            "playbook_aci_switch_init.yaml")
+
+
+
+                thread1 = MyThread(target=ansible_deploy_function,
+                                    args=(playbook_dir_apic, settings.ANSIBLE_STEP[3], option, None, False))
+                thread2 = MyThread(target=ansible_deploy_function,
+                                    args=(playbook_dir_switch, settings.ANSIBLE_STEP[4], option, None, False))
 
                 logger.info("Wipe aci fabric start pls wait, check log for detail.")
 
                 thread1.start()
                 thread2.start()
 
                 thread1.join()
                 thread2.join()
 
-                global ansible_run_result
-                if ansible_run_result == 0:
-                    logger.error("Exist iac-init tool Step 1 failed pls check log for detail")
-                else:
+                if thread1.get_result() and thread2.get_result():
                     logger.info("Wipe aci fabric Success proceed.")
+                else:
+                    logger.error("Exist iac-init tool Step 1 failed pls check log for detail")
+                    exit()
 
             except Exception as e:
                 msg = "Run Step 1 wipe aci fabric ansible-playbook failed detail:\nError: {}".format(e)
                 logger.error(msg)
                 exit()
 
         elif int(option) in [2]:
@@ -181,47 +155,26 @@
 
             except Exception as e:
                 msg = "Generate working directory fail, detail: {}".format(e)
                 logger.error(msg)
                 exit()
 
             try:
-                def ansible_deploy_function(playbook_name, step_name):
-                    import logging
-                    from logging.handlers import TimedRotatingFileHandler
-
-                    playbook_dir = os.path.join(os.getcwd(), output,
-                                                os.path.basename(settings.TEMPLATE_DIR[int(option) - 1]),
-                                                playbook_name)
-
-                    logger = logging.getLogger(playbook_dir)
-                    logger.setLevel(logging.INFO)
-                    log_formatter = logging.Formatter('%(message)s')
-                    log_file = os.path.join(settings.OUTPUT_BASE_DIR, 'iac_init_log',
-                                                 'iac-init-{}-{}.log'.format(option, step_name))
-                    file_handler = TimedRotatingFileHandler(log_file, when="M", interval=30, backupCount=0)
-                    file_handler.setFormatter(log_formatter)
-                    logger.addHandler(file_handler)
-
-                    def callback(res):
-                        print(res['stdout'])
-                        output = re.compile(r'\x1b\[\[?(?:\d{1,2}(?:;\d{0,2})*)?[m|K]').sub('', res['stdout'])
-                        logger.info(output)
-
-                    runner = run(playbook=playbook_dir, inventory=None, verbosity=5,
-                                 quiet=True, event_handler=callback)
-
-                    if runner.status == "successful":
-                        logger.info("Successfully finish Step {}: {}".format(option, step_name.upper()))
-
-                    else:
-                        logger.error("Failed run Step {}: {}".format(option, step_name.upper()))
-                        exit()
+                playbook_dir = os.path.join(os.getcwd(), output,
+                                            os.path.basename(settings.TEMPLATE_DIR[int(option) - 1]),
+                                            "playbook_apic_discovery.yaml")
 
-                ansible_deploy_function("playbook_apic_discovery.yaml", settings.ANSIBLE_STEP[5])
+                run_result = ansible_deploy_function(playbook_dir=playbook_dir, step_name=settings.ANSIBLE_STEP[5],
+                                                     option=option, quiet=False)
+                if run_result:
+                    logger.info("Run step 2 APIC discovery ansible-playbook successfully.")
+                else:
+                    msg = "Run Step 2 APIC discovery ansible-playbook failed"
+                    logger.error(msg)
+                    exit()
 
             except Exception as e:
                 msg = "Run Step 2 APIC discovery ansible-playbook fail detail:\nError: {}".format(e)
                 logger.error(msg)
                 exit()
 
         else:
@@ -249,30 +202,38 @@
                 logger.error(msg)
                 exit()
 
             try:
                 inventory_path = os.path.join(os.getcwd(), output,
                                               os.path.basename(settings.TEMPLATE_DIR[int(option) - 1]),
                                               'inventory.yaml')
-                playbook_dir = os.path.join(os.getcwd(), output,
-                                            os.path.basename(settings.TEMPLATE_DIR[int(option) - 1]),
-                                            'aac_ansible')
+                playbook_dir_validate = os.path.join(os.getcwd(), output,
+                                                    os.path.basename(settings.TEMPLATE_DIR[int(option) - 1]),
+                                                    'aac_ansible', "apic_validate.yaml")
+
+                playbook_dir_deploy = os.path.join(os.getcwd(), output,
+                                                    os.path.basename(settings.TEMPLATE_DIR[int(option) - 1]),
+                                                    'aac_ansible', "apic_deploy.yaml")
+
+                playbook_dir_test = os.path.join(os.getcwd(), output,
+                                                    os.path.basename(settings.TEMPLATE_DIR[int(option) - 1]),
+                                                    'aac_ansible', "apic_test.yaml")
 
-                validate_result = run_ansible_playbook(settings.ANSIBLE_STEP[0], option, inventory_path,
-                                                       os.path.join(playbook_dir, "apic_validate.yaml"))
+                validate_result = ansible_deploy_function(playbook_dir=playbook_dir_validate, step_name=settings.ANSIBLE_STEP[0],
+                                                          inventory_path=inventory_path, option=option, quiet=False)
                 if not validate_result:
                     exit()
 
-                deploy_result = run_ansible_playbook(settings.ANSIBLE_STEP[1], option, inventory_path,
-                                                     os.path.join(playbook_dir, "apic_deploy.yaml"))
+                deploy_result = ansible_deploy_function(playbook_dir=playbook_dir_deploy, step_name=settings.ANSIBLE_STEP[1],
+                                                          inventory_path=inventory_path, option=option, quiet=False)
                 if not deploy_result:
                     exit()
 
-                test_result = run_ansible_playbook(settings.ANSIBLE_STEP[2], option, inventory_path,
-                                                   os.path.join(playbook_dir, "apic_test.yaml"))
+                test_result = ansible_deploy_function(playbook_dir=playbook_dir_test, step_name=settings.ANSIBLE_STEP[2],
+                                                          inventory_path=inventory_path, option=option, quiet=False)
                 if not test_result:
                     exit()
 
             except Exception as e:
                 msg = "Run NAC ansible-playbook fail detail:\nError: {}".format(e)
                 logger.error(msg)
                 exit()
```

### Comparing `iac_init-0.5.8/iac_init/conf/__init__.py` & `iac_init-0.5.9/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/conf/global_settings.py` & `iac_init-0.5.9/iac_init/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/scripts/ansible_tool.py` & `iac_init-0.5.9/iac_init/scripts/ansible_tool.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 # -*- coding: utf-8 -*-
 
 # Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
 
-import os
 import re
-from loguru import logger
+import os
 from ansible_runner import run
 from iac_init.conf import settings
 
-def run_ansible_playbook(step: str, option, inventory_path, playbook_path):
-    logger.add(sink=os.path.join(settings.OUTPUT_BASE_DIR, 'iac_init_log', 'iac-init-{}-{}.log'.format(option, step)),
-               enqueue=True, format="{message}")
+def ansible_deploy_function(playbook_dir, step_name, option, inventory_path=None, quiet=True):
+    import logging
+    from logging.handlers import TimedRotatingFileHandler
+
+    logger = logging.getLogger(playbook_dir)
+    logger.setLevel(logging.INFO)
+    log_formatter = logging.Formatter('%(message)s')
+    log_file = os.path.join(settings.OUTPUT_BASE_DIR, 'iac_init_log',
+                            'iac-init-{}-{}.log'.format(option, step_name))
+    file_handler = TimedRotatingFileHandler(log_file, when="M", interval=30, backupCount=0)
+    file_handler.setFormatter(log_formatter)
+    logger.addHandler(file_handler)
 
     def callback(res):
+        if not quiet and 'stdout' in res:
+            print(res['stdout'])
         output = re.compile(r'\x1b\[\[?(?:\d{1,2}(?:;\d{0,2})*)?[m|K]').sub('', res['stdout'])
         logger.info(output)
 
-    runner = run(playbook=playbook_path, inventory=inventory_path, verbosity=5, stdout_callback="debug", quiet=True,
-                 event_handler=callback)
+    runner = run(playbook=playbook_dir, inventory=inventory_path, verbosity=5,
+                 quiet=True, event_handler=callback)
 
     if runner.status == "successful":
-        logger.info("Successfully finish Step {}: {}".format(option, step.upper()))
-        logger.remove()
+        logger.info("Successfully finish Step {}: {}".format(option, step_name.upper()))
         return True
+
     else:
-        logger.error("Failed run Step {}: {}".format(option, step.upper()))
-        logger.remove()
-        return False
+        logger.error("Failed run Step {}: {}".format(option, step_name.upper()))
+        return False
```

### Comparing `iac_init-0.5.8/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.5.9/iac_init/scripts/apic_connecton_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.5.9/iac_init/scripts/cimc_precheck_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.5.9/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.5.9/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.5.9/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.5.9/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.5.9/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/utils/functional.py` & `iac_init-0.5.9/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/validator.py` & `iac_init-0.5.9/iac_init/validator.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/yaml_conf/yaml.py` & `iac_init-0.5.9/iac_init/yaml_conf/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.5.9/iac_init/yaml_conf/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.5.8/pyproject.toml` & `iac_init-0.5.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.5.8"
+version = "0.5.9"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.5.8/PKG-INFO` & `iac_init-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.5.8
+Version: 0.5.9
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

