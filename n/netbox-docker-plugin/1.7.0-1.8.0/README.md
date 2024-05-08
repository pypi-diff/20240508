# Comparing `tmp/netbox_docker_plugin-1.7.0.tar.gz` & `tmp/netbox_docker_plugin-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_docker_plugin-1.7.0.tar", last modified: Fri May  3 13:50:54 2024, max compression
+gzip compressed data, was "netbox_docker_plugin-1.8.0.tar", last modified: Wed May  8 08:34:16 2024, max compression
```

## Comparing `netbox_docker_plugin-1.7.0.tar` & `netbox_docker_plugin-1.8.0.tar`

### file list

```diff
@@ -1,133 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.591849 netbox_docker_plugin-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-03 13:50:54.591849 netbox_docker_plugin-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.571849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.571849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15422 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.575849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/network_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.579849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0002_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0003_image_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0004_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0005_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0011_host_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0012_host_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0014_container_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0016_alter_env_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0017_network_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0020_container_hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0021_registry_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0023_delete_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0025_alter_image_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0026_image_digest.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0027_container_restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0028_mount_and_bind_read_only.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.583849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/models/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/models/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/models/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/models/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/models/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/models/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.567849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.583849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/templates/netbox_docker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.583849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/templatetags/host.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.583849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.583849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/container/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/container/test_container_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/container/test_container_operation_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/container/test_container_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/container/test_container_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.583849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/host/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/host/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/host/test_host_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/host/test_host_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/host/test_replace_password.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.583849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/image/test_image_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/image/test_image_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.587849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/network/test_network_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/network/test_network_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.587849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/registry/test_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/registry/test_registry_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.587849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/volume/test_volume_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/volume/test_volume_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.587849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.587849 netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/label.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/network_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:50:54.591849 netbox_docker_plugin-1.7.0/netbox_docker_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-03 13:50:54.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-03 13:50:54.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 13:50:54.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 13:50:54.000000 netbox_docker_plugin-1.7.0/netbox_docker_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-03 13:50:48.000000 netbox_docker_plugin-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 13:50:54.591849 netbox_docker_plugin-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.892270 netbox_docker_plugin-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-08 08:34:16.892270 netbox_docker_plugin-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.872270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.876270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15422 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.876270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/network_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.880270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0002_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0003_image_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0004_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0005_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0011_host_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0012_host_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0014_container_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0016_alter_env_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0017_network_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0020_container_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0021_registry_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0023_delete_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0025_alter_image_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0026_image_digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0027_container_restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0028_mount_and_bind_read_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0029_alter_container_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.884270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/models/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/models/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/models/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/models/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.868270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.884270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/templates/netbox_docker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.884270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/templatetags/host.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.884270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.884270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/container/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/container/test_container_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/container/test_container_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/container/test_container_operation_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/container/test_container_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/container/test_container_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.888270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/host/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/host/test_host_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/host/test_host_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/host/test_replace_password.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.888270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/image/test_image_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/image/test_image_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.888270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/network/test_network_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/network/test_network_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.888270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/registry/test_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/registry/test_registry_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.888270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/volume/test_volume_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/volume/test_volume_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.888270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.892270 netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/network_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:34:16.892270 netbox_docker_plugin-1.8.0/netbox_docker_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-08 08:34:16.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-08 08:34:16.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:34:16.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 08:34:16.000000 netbox_docker_plugin-1.8.0/netbox_docker_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-08 08:34:11.000000 netbox_docker_plugin-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:34:16.892270 netbox_docker_plugin-1.8.0/setup.cfg
```

### Comparing `netbox_docker_plugin-1.7.0/LICENSE` & `netbox_docker_plugin-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/PKG-INFO` & `netbox_docker_plugin-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: netbox-docker-plugin
-Version: 1.7.0
+Version: 1.8.0
 Summary: Manage Docker with Netbox & style.
-Author-email: Vincent Simonin <vincent@saashup.com>
+Author-email: Vincent Simonin <vincent@saashup.com>, David Delassus <david.jose.delassus@gmail.com>
 Project-URL: Homepage, https://github.com/SaaShup/netbox-docker-plugin
 Project-URL: Bug Tracker, https://github.com/SaaShup/netbox-docker-plugin/issues
 Keywords: netbox,netbox-plugin,docker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `netbox_docker_plugin-1.7.0/README.md` & `netbox_docker_plugin-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/__init__.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 
 class NetBoxDockerConfig(PluginConfig):
     """Plugin Config Class"""
 
     name = "netbox_docker_plugin"
     verbose_name = " NetBox Docker Plugin"
     description = "Manage Docker"
-    version = "1.7.0"
+    version = "1.8.0"
     base_url = "docker"
-    author= "Vincent Simonin"
-    author_email= "vincent@saashup.com"
+    author= "Vincent Simonin <vincent@saashup.com>, David Delassus <david.jose.delassus@gmail.com>"
+    author_email= "vincent@saashup.com, david.jose.delassus@gmail.com"
 
     def ready(self):
+        from . import signals # pylint: disable=unused-import, import-outside-toplevel
+
         post_migrate.connect(create_webhook)
 
         super().ready()
 
 
 # pylint: disable=C0103
 config = NetBoxDockerConfig
```

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/api/serializers.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/api/views.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/filtersets.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/bind.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/bind.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/container.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/container.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,19 +10,15 @@
     NetBoxModelForm,
     NetBoxModelImportForm,
     NetBoxModelFilterSetForm,
     NetBoxModelBulkEditForm,
 )
 from ..models.volume import Volume
 from ..models.host import Host
-from ..models.container import (
-    Container,
-    ContainerStateChoices,
-    ContainerRestartPolicyChoices,
-)
+from ..models.container import Container, ContainerRestartPolicyChoices
 from ..models.image import Image
 
 
 class ContainerForm(NetBoxModelForm):
     """Container form definition class"""
 
     host = DynamicModelChoiceField(
@@ -40,24 +36,22 @@
 
         model = Container
         fields = (
             "host",
             "image",
             "name",
             "hostname",
-            "state",
             "restart_policy",
             "tags",
         )
         labels = {
             "name": "Name",
             "host": "Host",
             "image": "Image",
             "hostname": "Hostname",
-            "state": "State",
             "restart_policy": "Restart Policy",
         }
 
 
 class ContainerFilterForm(NetBoxModelFilterSetForm):
     """Container filter form definition class"""
 
@@ -75,33 +69,23 @@
         label="Host",
     )
     image_id = DynamicModelMultipleChoiceField(
         queryset=Image.objects.all(),
         required=False,
         label="Image",
     )
-    state = forms.ChoiceField(
-        label="State", choices=ContainerStateChoices, required=False
-    )
     restart_policy = forms.ChoiceField(
         label="Restart Policy", choices=ContainerRestartPolicyChoices, required=False
     )
     tag = TagFilterField(model)
 
 
 class ContainerImportForm(NetBoxModelImportForm):
     """Container importation form definition class"""
 
-    state = forms.ChoiceField(
-        label="State",
-        choices=ContainerStateChoices,
-        required=False,
-        help_text="Container State. Can be `created`, `restarting`, "
-        + "`running`, `paused`, `exited` or `dead`.",
-    )
     restart_policy = forms.ChoiceField(
         label="Restart Policy",
         choices=ContainerRestartPolicyChoices,
         required=False,
         help_text="Container restart policy. Can be `no`, `on-failure`, "
         + "`always`, `unless-stopped`.",
     )
@@ -110,43 +94,37 @@
         """Container importation form definition Meta class"""
 
         model = Container
         fields = (
             "name",
             "host",
             "image",
-            "state",
             "hostname",
         )
         labels = {
             "name": "Unique container name",
             "host": "Host identifier",
             "image": "Image identifier",
         }
 
 
 class ContainerBulkEditForm(NetBoxModelBulkEditForm):
     """Container bulk edit form definition class"""
 
-    state = forms.ChoiceField(
-        label="State",
-        choices=ContainerStateChoices,
-        required=True,
-    )
     restart_policy = forms.ChoiceField(
         label="Restart Policy",
         choices=ContainerRestartPolicyChoices,
         required=True,
     )
     hostname = forms.CharField(
         label="Hostname", max_length=256, min_length=1, required=False
     )
 
     model = Container
-    fieldsets = (("General", ("state", "restart_policy", "hostname")),)
+    fieldsets = (("General", ("restart_policy", "hostname")),)
 
 
 class ContainerOperationForm(NetBoxModelForm):
     """Container Operation form definition class"""
 
     class Meta:
         """Container form definition Meta class"""
```

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/env.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/env.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/host.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/host.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/image.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/label.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/label.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/mount.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/mount.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/network.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/network_setting.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/network_setting.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/port.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/port.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/registry.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/registry.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/forms/volume.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/forms/volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0001_initial.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0002_image.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0002_image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0003_image_size.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0003_image_size.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0004_volume.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0004_volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0005_network.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0005_network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0011_host_token.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0011_host_token.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0012_host_state.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0012_host_state.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0013_host_netbox_url.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0016_alter_env_value.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0016_alter_env_value.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0020_container_hostname.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0020_container_hostname.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0021_registry_and_more.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0021_registry_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0023_delete_hosts.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0023_delete_hosts.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0025_alter_image_version.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0025_alter_image_version.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0026_image_digest.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0026_image_digest.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/0028_mount_and_bind_read_only.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/0028_mount_and_bind_read_only.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/migrations/__init__.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/models/container.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/models/container.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,25 +12,25 @@
     MinValueValidator,
     MaxValueValidator,
 )
 from utilities.choices import ChoiceSet
 from utilities.querysets import RestrictedQuerySet
 from netbox.models import NetBoxModel
 from .image import Image
-from .host import Host
+from .host import Host, HostStateChoices
 from .network import Network
 from .volume import Volume
 
 
 class ContainerStateChoices(ChoiceSet):
     """Container state choices definition class"""
 
     key = "Container.state"
 
-    DEFAULT_VALUE = "created"
+    DEFAULT_VALUE = "none"
 
     CHOICES = [
         ("created", "Created", "dark"),
         ("restarting", "Restarting", "blue"),
         ("running", "Running", "blue"),
         ("paused", "Paused", "blue"),
         ("exited", "Exited", "blue"),
@@ -129,14 +129,47 @@
     )
     restart_policy = models.CharField(
         max_length=32,
         choices=ContainerRestartPolicyChoices,
         default=ContainerRestartPolicyChoices.DEFAULT_VALUE,
     )
 
+    @property
+    def can_create(self) -> bool:
+        """ Check if the container can be created """
+        return self.state == "none"
+
+    @property
+    def can_start(self) -> bool:
+        """ Check if the container can be started """
+        return self.state in ["created", "exited", "dead"]
+
+    @property
+    def can_stop(self) -> bool:
+        """ Check if the container can be stopped """
+        return self.state in ["running"]
+
+    @property
+    def can_restart(self) -> bool:
+        """ Check if the container can be restarted """
+        return self.state in ["running"]
+
+    @property
+    def can_recreate(self) -> bool:
+        """ Check if the container can be recreated """
+        return self.state in ["created", "running", "exited", "dead"]
+
+    @property
+    def can_delete(self) -> bool:
+        """ Check if the container can be deleted """
+        return (
+            self.host.state == HostStateChoices.STATE_DELETED
+            or self.state in ["created", "paused", "exited", "dead"]
+        )
+
     class Meta:
         """Image Model Meta Class"""
 
         ordering = ("name",)
         constraints = (
             models.UniqueConstraint(
                 Lower("name"), "host", name="%(app_label)s_%(class)s_unique_name_host"
```

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/models/host.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/models/host.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/models/image.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/models/image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/models/network.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/models/network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/models/registry.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/models/registry.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/models/volume.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/models/volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/navigation.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tables.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/templates/netbox_docker_plugin/container.html`

 * *Files 4% similar despite different names*

```diff
@@ -2,39 +2,63 @@
 
 {% load plugins %}
 
 {% block extra_controls %}
 <form action="{% url 'plugins:netbox_docker_plugin:container_operation' pk=object.id operation='start' %}" method="post">
   {% csrf_token %}
   <input type="hidden" name="operation" value="start">
-  <button type="submit" class="btn btn-sm btn-success">
+  <button
+    type="submit"
+    class="btn btn-sm btn-success"
+    {% if not object.can_start %}
+    disabled
+    {% endif %}
+  >
     <i class="mdi mdi-play"></i> Start
   </button>
 </form>
 
 <form action="{% url 'plugins:netbox_docker_plugin:container_operation' pk=object.id operation='stop' %}" method="post">
   {% csrf_token %}
   <input type="hidden" name="operation" value="stop">
-  <button type="submit" class="btn btn-sm btn-danger">
+  <button
+    type="submit"
+    class="btn btn-sm btn-danger"
+    {% if not object.can_stop %}
+    disabled
+    {% endif %}
+  >
     <i class="mdi mdi-stop"></i> Stop
   </button>
 </form>
 
 <form action="{% url 'plugins:netbox_docker_plugin:container_operation' pk=object.id operation='restart' %}" method="post">
   {% csrf_token %}
   <input type="hidden" name="operation" value="restart">
-  <button type="submit" class="btn btn-sm btn-light">
+  <button
+    type="submit"
+    class="btn btn-sm btn-light"
+    {% if not object.can_restart %}
+    disabled
+    {% endif %}
+  >
     <i class="mdi mdi-restart"></i> Restart
   </button>
 </form>
 
 <form action="{% url 'plugins:netbox_docker_plugin:container_operation' pk=object.id operation='recreate' %}" method="post">
   {% csrf_token %}
   <input type="hidden" name="operation" value="recreate">
-  <button type="submit" class="btn btn-sm btn-dark">
+  <button
+    type="submit"
+    class="btn btn-sm btn-dark"
+    {% if not object.can_recreate %}
+    disabled
+    {% endif %}
+  >
     <i class="mdi mdi-autorenew"></i> Recreate
   </button>
 </form>
 {% endblock %}
 
 {% block content %}
 <div class="row mb-3">
```

#### html2text {}

```diff
@@ -1,13 +1,17 @@
 {% extends 'generic/object.html' %} {% load plugins %} {% block extra_controls
 %}
-{% csrf_token %} Start
-{% csrf_token %} Stop
-{% csrf_token %} Restart
-{% csrf_token %} Recreate
+{% csrf_token %}
+% if not object.can_start %} disabled {% endif %} > Start
+{% csrf_token %}
+% if not object.can_stop %} disabled {% endif %} > Stop
+{% csrf_token %}
+% if not object.can_restart %} disabled {% endif %} > Restart
+{% csrf_token %}
+% if not object.can_recreate %} disabled {% endif %} > Recreate
 {% endblock %} {% block content %}
 **** CCOONNTTAAIINNEERR ****
 HHoosstt           _{_{_ _o_b_j_e_c_t_._h_o_s_t_ _}_}
 IImmaaggee          _{_{_ _o_b_j_e_c_t_._i_m_a_g_e_ _}_}
 NNaammee           {{ object.name }}
 CCoonnttaaiinneerrIIDD    {{ object.ContainerID|placeholder }}
 HHoossttnnaammee       {{ object.hostname|placeholder }}
```

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/templates/netbox_docker_plugin/host.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/templates/netbox_docker_plugin/image.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/templates/netbox_docker_plugin/network.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/base.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/base.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/container/test_container_api.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/container/test_container_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=R0801
 """Container Test Case"""
 
 from utilities.testing import APIViewTestCases
 from netbox_docker_plugin.models.container import Container
 from netbox_docker_plugin.models.host import Host
 from netbox_docker_plugin.models.network import Network
 from netbox_docker_plugin.models.image import Image
@@ -60,17 +61,35 @@
         network1 = Network.objects.create(host=host1, name="network1")
         network2 = Network.objects.create(host=host2, name="network2")
 
         volume1 = Volume.objects.create(host=host1, name="volume1")
         volume2 = Volume.objects.create(host=host1, name="volume2")
         volume3 = Volume.objects.create(host=host2, name="volume3")
 
-        Container.objects.create(host=host1, image=image1, name="container1")
-        Container.objects.create(host=host1, image=image1, name="container2")
-        Container.objects.create(host=host2, image=image2, name="container3")
+        Container.objects.create(
+            host=host1,
+            image=image1,
+            name="container1",
+            operation="none",
+            state="created",
+        )
+        Container.objects.create(
+            host=host1,
+            image=image1,
+            name="container2",
+            operation="none",
+            state="created",
+        )
+        Container.objects.create(
+            host=host2,
+            image=image2,
+            name="container3",
+            operation="none",
+            state="created",
+        )
 
         cls.create_data = [
             {
                 "host": host1.pk,
                 "image": image1.pk,
                 "name": "container5",
                 "ports": [
```

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/container/test_container_operation_view.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/container/test_container_operation_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=R0801
 """Container operation Views Test Case"""
 
 from django.urls import reverse
 from django.test import override_settings
 from django.contrib.contenttypes.models import ContentType
 from utilities.testing import ModelViewTestCase
 from utilities.testing.utils import disable_warnings, post_data
@@ -18,15 +19,15 @@
 class ContainerViewsTestCase(BaseModelViewTestCase, ModelViewTestCase):
     """Container operation Views Test Case Class"""
 
     model = Container
 
     def test_operation_start_object_without_permission(self):
         """Test operation start object without permission"""
-        instance = self._get_queryset().first()
+        instance = self._get_queryset().exclude(state="running").first()
 
         # Try GET without permission
         with disable_warnings("django.request"):
             self.assertHttpStatus(self.client.get(self._get_url("edit", instance)), 403)
 
         # Try POST without permission
         request = {
@@ -38,15 +39,15 @@
         }
         with disable_warnings("django.request"):
             self.assertHttpStatus(self.client.post(**request), 403)
 
     @override_settings(EXEMPT_VIEW_PERMISSIONS=["*"])
     def test_operation_start_object_with_permission(self):
         """Test operation start object with permission""" """  """
-        instance = self._get_queryset().first()
+        instance = self._get_queryset().exclude(state="running").first()
 
         # Assign model-level permission
         obj_perm = ObjectPermission(name="Test permission", actions=["change"])
         obj_perm.save()
         # pylint: disable=E1101
         obj_perm.users.add(self.user)
         # pylint: disable=E1101
@@ -74,15 +75,15 @@
         self.assertEqual(len(objectchanges), 1)
         self.assertEqual(
             objectchanges[0].action, ObjectChangeActionChoices.ACTION_UPDATE
         )
 
     def test_operation_stop_object_without_permission(self):
         """Test operation stop object without permission"""
-        instance = self._get_queryset().first()
+        instance = self._get_queryset().filter(state="running").first()
 
         # Try GET without permission
         with disable_warnings("django.request"):
             self.assertHttpStatus(self.client.get(self._get_url("edit", instance)), 403)
 
         # Try POST without permission
         request = {
@@ -94,15 +95,15 @@
         }
         with disable_warnings("django.request"):
             self.assertHttpStatus(self.client.post(**request), 403)
 
     @override_settings(EXEMPT_VIEW_PERMISSIONS=["*"])
     def test_operation_stop_object_with_permission(self):
         """Test operation stop object with permission""" """  """
-        instance = self._get_queryset().first()
+        instance = self._get_queryset().filter(state="running").first()
 
         # Assign model-level permission
         obj_perm = ObjectPermission(name="Test permission", actions=["change"])
         obj_perm.save()
         # pylint: disable=E1101
         obj_perm.users.add(self.user)
         # pylint: disable=E1101
@@ -130,15 +131,15 @@
         self.assertEqual(len(objectchanges), 1)
         self.assertEqual(
             objectchanges[0].action, ObjectChangeActionChoices.ACTION_UPDATE
         )
 
     def test_operation_restart_object_without_permission(self):
         """Test operation restart object without permission"""
-        instance = self._get_queryset().first()
+        instance = self._get_queryset().filter(state="running").first()
 
         # Try GET without permission
         with disable_warnings("django.request"):
             self.assertHttpStatus(self.client.get(self._get_url("edit", instance)), 403)
 
         # Try POST without permission
         request = {
@@ -150,15 +151,15 @@
         }
         with disable_warnings("django.request"):
             self.assertHttpStatus(self.client.post(**request), 403)
 
     @override_settings(EXEMPT_VIEW_PERMISSIONS=["*"])
     def test_operation_restart_object_with_permission(self):
         """Test operation restart object with permission""" """  """
-        instance = self._get_queryset().first()
+        instance = self._get_queryset().filter(state="running").first()
 
         # Assign model-level permission
         obj_perm = ObjectPermission(name="Test permission", actions=["change"])
         obj_perm.save()
         # pylint: disable=E1101
         obj_perm.users.add(self.user)
         # pylint: disable=E1101
@@ -255,11 +256,35 @@
         registry2 = Registry.objects.create(
             host=host2, name="registry2", serveraddress="http://localhost:8082"
         )
 
         image1 = Image.objects.create(host=host1, name="image1", registry=registry1)
         image2 = Image.objects.create(host=host2, name="image2", registry=registry2)
 
-        Container.objects.create(host=host1, image=image1, name="container1")
-        Container.objects.create(host=host1, image=image1, name="container2")
-        Container.objects.create(host=host2, image=image2, name="container3")
-        Container.objects.create(host=host2, image=image2, name="container4")
+        Container.objects.create(
+            host=host1,
+            image=image1,
+            name="container1",
+            operation="none",
+            state="created",
+        )
+        Container.objects.create(
+            host=host1,
+            image=image1,
+            name="container2",
+            operation="none",
+            state="created",
+        )
+        Container.objects.create(
+            host=host2,
+            image=image2,
+            name="container3",
+            operation="none",
+            state="created",
+        )
+        Container.objects.create(
+            host=host2,
+            image=image2,
+            name="container4",
+            operation="none",
+            state="running",
+        )
```

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/container/test_container_validation.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/container/test_container_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,34 +19,40 @@
     def test_that_container_is_created(self):
         """Test that Container object is created"""
 
         container = Container.objects.create(
             host=self.objects["host1"],
             image=self.objects["image1"],
             name="container1",
+            operation="none",
+            state="created",
         )
 
         self.assertTrue(isinstance(container.id, int))
 
         container = Container.objects.create(
             host=self.objects["host2"],
             image=self.objects["image2"],
             name="container2",
+            operation="none",
+            state="created",
         )
 
         self.assertTrue(isinstance(container.id, int))
 
     def test_that_container_image_must_be_on_the_same_host(self):
         """Test that Container image must be on the same host"""
 
         with self.assertRaises(ValidationError) as cm:
             container = Container(
                 host=self.objects["host1"],
                 image=self.objects["image2"],
                 name="container2",
+                operation="none",
+                state="created",
             )
             container.clean()
 
         self.assertEqual(
             cm.exception.messages,
             ["Image image2:latest does not belong to host host1."],
         )
@@ -59,14 +65,16 @@
         """Test that volume mounted must be on the same container host"""
 
         with self.assertRaises(ValidationError) as cm:
             container = Container(
                 host=self.objects["host1"],
                 image=self.objects["image1"],
                 name="container3",
+                operation="none",
+                state="created",
             )
 
             mount = Mount(
                 container=container, volume=self.objects["volume2"], source="/data"
             )
 
             mount.clean()
@@ -84,14 +92,16 @@
         """Test that network settings must be on the same container host"""
 
         with self.assertRaises(ValidationError) as cm:
             container = Container(
                 host=self.objects["host1"],
                 image=self.objects["image1"],
                 name="container3",
+                operation="none",
+                state="created",
             )
 
             network_setting = NetworkSetting(
                 container=container, network=self.objects["network2"]
             )
 
             network_setting.clean()
```

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/container/test_container_views.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/container/test_container_views.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=R0801
 """Container Views Test Case"""
 
 from utilities.testing import ViewTestCases
 from netbox_docker_plugin.tests.base import BaseModelViewTestCase
 from netbox_docker_plugin.models.host import Host
 from netbox_docker_plugin.models.container import Container
 from netbox_docker_plugin.models.image import Image
@@ -27,39 +28,59 @@
             host=host2, name="registry2", serveraddress="http://localhost:8082"
         )
 
         image1 = Image.objects.create(host=host1, name="image1", registry=registry1)
         image2 = Image.objects.create(host=host2, name="image2", registry=registry2)
 
         container1 = Container.objects.create(
-            host=host1, image=image1, name="container1", restart_policy="always"
+            host=host1,
+            image=image1,
+            name="container1",
+            restart_policy="always",
+            operation="none",
+            state="created",
         )
         container2 = Container.objects.create(
-            host=host1, image=image1, name="container2"
+            host=host1,
+            image=image1,
+            name="container2",
+            operation="none",
+            state="created",
+        )
+        Container.objects.create(
+            host=host2,
+            image=image2,
+            name="container3",
+            operation="none",
+            state="created",
+        )
+        Container.objects.create(
+            host=host2,
+            image=image2,
+            name="container4",
+            operation="none",
+            state="created",
         )
-        Container.objects.create(host=host2, image=image2, name="container3")
-        Container.objects.create(host=host2, image=image2, name="container4")
 
         cls.form_data = {
             "name": "container5",
             "host": host1.pk,
             "image": image1.pk,
-            "state": "created",
             "restart_policy": "unless-stopped",
         }
 
         cls.csv_data = (
             "name,host,image,hostname",
             f"container6,{host1.pk},{image1.pk},",
             f"container7,{host2.pk},{image2.pk},container7",
         )
 
         cls.bulk_edit_data = {
-            "state": "running",
+            "hostname": "h",
             "restart_policy": "always",
         }
 
         cls.csv_update_data = (
-            "id,name,host,image,state,hostname,restart_policy",
-            f"{container1.pk},container1,{host1.pk},{image1.pk},paused,,on-failure",
-            f"{container2.pk},container2,{host1.pk},{image1.pk},running,container2,unless-stopped",
+            "id,name,host,image,hostname,restart_policy",
+            f"{container1.pk},container1,{host1.pk},{image1.pk},,on-failure",
+            f"{container2.pk},container2,{host1.pk},{image1.pk},container2,unless-stopped",
         )
```

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/host/test_host_api.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/host/test_host_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/host/test_host_views.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/host/test_host_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/host/test_replace_password.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/host/test_replace_password.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/image/test_image_api.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/image/test_image_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/image/test_image_views.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/image/test_image_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/network/test_network_api.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/network/test_network_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/network/test_network_views.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/network/test_network_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/registry/test_registry_api.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/registry/test_registry_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/registry/test_registry_views.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/registry/test_registry_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/test_init.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/volume/test_volume_api.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/volume/test_volume_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/tests/volume/test_volume_views.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/tests/volume/test_volume_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/urls.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/utilities/__init__.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/bind.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/bind.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/container.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/container.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/env.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/env.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/host.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/host.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/image.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/label.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/label.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/mount.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/mount.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/network.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/network_setting.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/network_setting.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/port.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/port.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/registry.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/registry.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin/views/volume.py` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin/views/volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin.egg-info/PKG-INFO` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: netbox-docker-plugin
-Version: 1.7.0
+Version: 1.8.0
 Summary: Manage Docker with Netbox & style.
-Author-email: Vincent Simonin <vincent@saashup.com>
+Author-email: Vincent Simonin <vincent@saashup.com>, David Delassus <david.jose.delassus@gmail.com>
 Project-URL: Homepage, https://github.com/SaaShup/netbox-docker-plugin
 Project-URL: Bug Tracker, https://github.com/SaaShup/netbox-docker-plugin/issues
 Keywords: netbox,netbox-plugin,docker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `netbox_docker_plugin-1.7.0/netbox_docker_plugin.egg-info/SOURCES.txt` & `netbox_docker_plugin-1.8.0/netbox_docker_plugin.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 netbox_docker_plugin/__init__.py
 netbox_docker_plugin/filtersets.py
 netbox_docker_plugin/navigation.py
+netbox_docker_plugin/signals.py
 netbox_docker_plugin/tables.py
 netbox_docker_plugin/urls.py
 netbox_docker_plugin.egg-info/PKG-INFO
 netbox_docker_plugin.egg-info/SOURCES.txt
 netbox_docker_plugin.egg-info/dependency_links.txt
 netbox_docker_plugin.egg-info/top_level.txt
 netbox_docker_plugin/api/__init__.py
@@ -52,14 +53,15 @@
 netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
 netbox_docker_plugin/migrations/0023_delete_hosts.py
 netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
 netbox_docker_plugin/migrations/0025_alter_image_version.py
 netbox_docker_plugin/migrations/0026_image_digest.py
 netbox_docker_plugin/migrations/0027_container_restart_policy.py
 netbox_docker_plugin/migrations/0028_mount_and_bind_read_only.py
+netbox_docker_plugin/migrations/0029_alter_container_state.py
 netbox_docker_plugin/migrations/__init__.py
 netbox_docker_plugin/models/__init__.py
 netbox_docker_plugin/models/container.py
 netbox_docker_plugin/models/host.py
 netbox_docker_plugin/models/image.py
 netbox_docker_plugin/models/network.py
 netbox_docker_plugin/models/registry.py
@@ -72,14 +74,15 @@
 netbox_docker_plugin/templates/netbox_docker_plugin/volume.html
 netbox_docker_plugin/templatetags/__init__.py
 netbox_docker_plugin/templatetags/host.py
 netbox_docker_plugin/tests/__init__.py
 netbox_docker_plugin/tests/base.py
 netbox_docker_plugin/tests/test_init.py
 netbox_docker_plugin/tests/container/__init__.py
+netbox_docker_plugin/tests/container/test_container_actions.py
 netbox_docker_plugin/tests/container/test_container_api.py
 netbox_docker_plugin/tests/container/test_container_operation_view.py
 netbox_docker_plugin/tests/container/test_container_validation.py
 netbox_docker_plugin/tests/container/test_container_views.py
 netbox_docker_plugin/tests/host/__init__.py
 netbox_docker_plugin/tests/host/test_host_api.py
 netbox_docker_plugin/tests/host/test_host_views.py
```

