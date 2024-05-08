# Comparing `tmp/sbcli-mig-1.0.9.zip` & `tmp/sbcli_mig-1.0.90.zip`

## zipinfo {}

```diff
@@ -1,146 +1,148 @@
-Zip file size: 177586 bytes, number of entries: 144
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/sbcli_mig.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/
--rw-r--r--  2.0 unx      149 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/env_var
--rw-r--r--  2.0 unx     2251 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/setup.cfg
--rw-r--r--  2.0 unx      730 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/README.md
--rw-r--r--  2.0 unx       84 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/pyproject.toml
--rw-r--r--  2.0 unx     1129 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     2508 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1638 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx      725 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     1263 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/app.py
--rw-r--r--  2.0 unx     5078 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx     1434 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      703 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx      463 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      827 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx      507 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx     1302 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx      434 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      322 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx     1890 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     4795 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx    12129 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx     6206 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx     3103 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx      975 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     5274 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     5317 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     2940 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     6326 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx     7846 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     5547 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx    11244 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx     8585 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx     8169 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx      357 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_cli/main.py
--rw-r--r--  2.0 unx    76175 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx       55 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/sbcli_mig.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/sbcli_mig.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       66 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/sbcli_mig.egg-info/requires.txt
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/sbcli_mig.egg-info/top_level.txt
--rw-r--r--  2.0 unx     5073 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/sbcli_mig.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx     1129 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/sbcli_mig.egg-info/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/
--rw-r--r--  2.0 unx     3193 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     1426 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/constants.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx     3153 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     7626 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/utils.py
--rw-r--r--  2.0 unx    62998 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx      279 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx    24246 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx      938 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx     6262 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx    21361 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     8189 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     5112 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/compute_node_ops.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx      694 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx       43 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1694 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx     1420 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx      152 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     8081 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx      187 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/prometheus.yml
--rw-r--r--  2.0 unx     5305 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/stack_deploy_wait.sh
--rwxr-xr-x  2.0 unx      595 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx      453 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx      311 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx      360 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx     1853 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx     5860 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx    98031 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    98198 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    98086 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    98143 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx     3203 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     4118 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx     2423 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     2189 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx      173 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     4637 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx     3003 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2410 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx      229 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     7218 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2612 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6360 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/storage_node_monitor.py
--rw-r--r--  2.0 unx      837 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     5462 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx     2490 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     5443 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/capacity_collector.py
--rw-r--r--  2.0 unx     4817 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx     1500 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     2193 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/nvme_device.py
--rw-r--r--  2.0 unx     1228 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     3766 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     1020 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx      736 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx      806 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4242 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     3222 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx      917 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx     1602 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     2565 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     4846 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1521 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1900 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx     1961 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx    46469 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx    22847 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx    10781 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1120 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx    13528 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1425 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx     1568 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx     1122 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx    11300 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx    10375 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/pool_controller.py
-144 files, 983388 bytes uncompressed, 151450 bytes compressed:  84.6%
+Zip file size: 214543 bytes, number of entries: 146
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 17:14 sbcli_mig-1.0.90/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 17:14 sbcli_mig-1.0.90/sbcli_mig.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/
+-rw-r--r--  2.0 unx     2286 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/setup.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/README.md
+-rw-r--r--  2.0 unx      163 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/env_var
+-rw-r--r--  2.0 unx       84 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/pyproject.toml
+-rw-r--r--  2.0 unx       38 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/setup.cfg
+-rw-r--r--  2.0 unx     1511 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/PKG-INFO
+-rw-r--r--  2.0 unx    78538 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_cli/main.py
+-rw-r--r--  2.0 unx        1 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/sbcli_mig.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     5188 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/sbcli_mig.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       49 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/sbcli_mig.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1511 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/sbcli_mig.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       79 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/sbcli_mig.egg-info/requires.txt
+-rw-r--r--  2.0 unx       55 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/sbcli_mig.egg-info/entry_points.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/
+-rw-r--r--  2.0 unx    66195 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1515 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     3638 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx      279 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx      938 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8343 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx    24895 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    21493 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     7504 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx      229 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     5268 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     2410 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5140 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx     7439 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx      837 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6577 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/services/storage_node_monitor.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx      930 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx      152 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx     5333 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx       54 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx     4409 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+-rw-r--r--  2.0 unx      453 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx     1782 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx      311 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx      118 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx       43 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1420 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/prometheus.yml
+-rwxr-xr-x  2.0 unx      657 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx    25433 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1856 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx   106705 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx   799409 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/node-exporter.json
+-rw-r--r--  2.0 unx    99758 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    99862 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/pools.json
+-rw-r--r--  2.0 unx    13877 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     3191 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10557 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx    23245 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx    47471 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx    11294 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx      806 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      917 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx      736 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx     3696 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2094 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_core/models/nvme_device.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/
+-rw-r--r--  2.0 unx      725 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx      703 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     2513 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      507 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      322 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      434 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     2905 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5547 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     4883 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5491 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     9573 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx     8547 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx      975 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     8075 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     5947 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-May-08 17:14 sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_pool.py
+146 files, 1930123 bytes uncompressed, 187673 bytes compressed:  90.3%
```

## zipnote {}

```diff
@@ -1,433 +1,439 @@
-Filename: sbcli-mig-1.0.9/
+Filename: sbcli_mig-1.0.90/
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/
+Filename: sbcli_mig-1.0.90/simplyblock_cli/
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_cli/
+Filename: sbcli_mig-1.0.90/sbcli_mig.egg-info/
 Comment: 
 
-Filename: sbcli-mig-1.0.9/sbcli_mig.egg-info/
+Filename: sbcli_mig-1.0.90/simplyblock_core/
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/
+Filename: sbcli_mig-1.0.90/simplyblock_web/
 Comment: 
 
-Filename: sbcli-mig-1.0.9/env_var
+Filename: sbcli_mig-1.0.90/setup.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/setup.py
+Filename: sbcli_mig-1.0.90/README.md
 Comment: 
 
-Filename: sbcli-mig-1.0.9/setup.cfg
+Filename: sbcli_mig-1.0.90/env_var
 Comment: 
 
-Filename: sbcli-mig-1.0.9/README.md
+Filename: sbcli_mig-1.0.90/pyproject.toml
 Comment: 
 
-Filename: sbcli-mig-1.0.9/pyproject.toml
+Filename: sbcli_mig-1.0.90/setup.cfg
 Comment: 
 
-Filename: sbcli-mig-1.0.9/PKG-INFO
+Filename: sbcli_mig-1.0.90/PKG-INFO
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/static/
+Filename: sbcli_mig-1.0.90/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/templates/
+Filename: sbcli_mig-1.0.90/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/
+Filename: sbcli_mig-1.0.90/sbcli_mig.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/__init__.py
+Filename: sbcli_mig-1.0.90/sbcli_mig.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/caching_node_app.py
+Filename: sbcli_mig-1.0.90/sbcli_mig.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/utils.py
+Filename: sbcli_mig-1.0.90/sbcli_mig.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/auth_middleware.py
+Filename: sbcli_mig-1.0.90/sbcli_mig.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_mig-1.0.90/sbcli_mig.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/app.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/node_utils.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/node_webapp.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/snode_app.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_mig-1.0.90/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/static/list_deps.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/static/rpac.yaml
+Filename: sbcli_mig-1.0.90/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/static/delete.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_mig-1.0.90/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/static/deploy.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/static/is_up.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/static/tst.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_mig-1.0.90/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/csi.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_cli/main.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_cli/cli.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/sbcli_mig.egg-info/entry_points.txt
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.9/sbcli_mig.egg-info/dependency_links.txt
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/sbcli_mig.egg-info/requires.txt
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/sbcli_mig.egg-info/top_level.txt
+Filename: sbcli_mig-1.0.90/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/sbcli_mig.egg-info/SOURCES.txt
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli-mig-1.0.9/sbcli_mig.egg-info/PKG-INFO
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/snode_client.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/constants.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/__init__.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/cnode_client.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/utils.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/storage_node_ops.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/shell_utils.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/cluster_ops.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/pci_utils.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/distr_controller.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/rpc_client.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/kv_store.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/compute_node_ops.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/node-exporter.json
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/pools.json
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/__init__.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_mig-1.0.90/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/__init__.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/remove_service.sh
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/service_template.service
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/install_service.sh
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/health_check_service.py
+Filename: sbcli_mig-1.0.90/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/device_monitor.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/capacity_collector.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/events.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/__init__.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/nvme_device.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/global_settings.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/caching_node.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/port_stat.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/snapshot.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/iface.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/stats.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/storage_node.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/compute_node.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/pool.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/cluster.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/base_model.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/models/lvol_model.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/__init__.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/device_events.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_cluster.py
+Comment: 
+
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/node_api_basic.py
+Comment: 
+
+Filename: sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli-mig-1.0.9/setup.py` & `sbcli_mig-1.0.90/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,16 @@
         "foundationdb",
         "requests",
         "typing",
         "prettytable",
         "docker",
         "psutil",
         "py-cpuinfo",
+        "graypy",
+        "boto3",
     ],
     entry_points={
         'console_scripts': [
             f'{COMMAND_NAME}=simplyblock_cli.cli:main',
         ]
     },
     include_package_data=True,
```

## Comparing `sbcli-mig-1.0.9/README.md` & `sbcli_mig-1.0.90/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -2,27 +2,33 @@
 # Simply Block
 [![Docker Image Build](https://github.com/simplyblock-io/sbcli/actions/workflows/docker-image.yml/badge.svg)](https://github.com/simplyblock-io/sbcli/actions/workflows/docker-image.yml)
 
 [![Python Unit Testing](https://github.com/simplyblock-io/sbcli/actions/workflows/python-testing.yml/badge.svg)](https://github.com/simplyblock-io/sbcli/actions/workflows/python-testing.yml)
 
  
 ## Install
+Add the package repo from AWS CodeArtifact using [awscli](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)
+
+```bash
+aws codeartifact login --tool pip --repository sbcli --domain simplyblock --domain-owner 565979732541 --region eu-west-1
+```
+Install package
 ```bash
-pip install sbcli-dev
- ```
+pip install --extra-index-url https://pypi.org/simple sbcli-dev
+```
 
 # Components 
 
 ## Simply Block Core
 Contains core logic and controllers for the simplyblock cluster
 
 ## Simply Block CLI
 Please see this document 
-[README.md](../simplyblock_cli/README.md)
+[README.md](../main/simplyblock_cli/README.md)
 
 
 ## Simply Block Web API
 Please see this document 
-[README.md](../simplyblock_web/README.md)
+[README.md](../main/simplyblock_web/README.md)
```

## Comparing `sbcli-mig-1.0.9/simplyblock_web/caching_node_app.py` & `sbcli_mig-1.0.90/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/utils.py` & `sbcli_mig-1.0.90/simplyblock_web/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             elif size_v == "g":
                 multi = 3
             elif size_v == "t":
                 multi = 4
             else:
                 print(f"Error parsing size: {size_string}")
                 return -1
-            return size_number * math.pow(one_k, multi)
+            return int(size_number * math.pow(one_k, multi))
         else:
             return -1
     except:
         print(f"Error parsing size: {size_string}")
         return -1
```

## Comparing `sbcli-mig-1.0.9/simplyblock_web/auth_middleware.py` & `sbcli_mig-1.0.90/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/caching_node_app_k8s.py` & `sbcli_mig-1.0.90/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/app.py` & `sbcli_mig-1.0.90/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/node_utils.py` & `sbcli_mig-1.0.90/simplyblock_web/node_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         logger.error(err)
         return []
     data = json.loads(out)
     logger.debug("nvme list:")
     logger.debug(data)
 
     devices = []
-    if data and 'Devices' in data:
+    if data and 'Devices' in data and data['Devices']:
         for dev in data['Devices'][0]['Subsystems']:
             if 'Controllers' in dev and dev['Controllers']:
                 controller = dev['Controllers'][0]
                 namespace = None
                 if "Namespaces" in dev and dev['Namespaces']:
                     namespace = dev['Namespaces'][0]
                 elif controller and controller["Namespaces"]:
```

## Comparing `sbcli-mig-1.0.9/simplyblock_web/node_webapp.py` & `sbcli_mig-1.0.90/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/snode_app.py` & `sbcli_mig-1.0.90/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_mig-1.0.90/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/static/delete.py` & `sbcli_mig-1.0.90/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/static/deploy.py` & `sbcli_mig-1.0.90/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_mig-1.0.90/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 apiVersion: apps/v1
 kind: Deployment
 metadata:
   name: spdk-deployment-{{ HOSTNAME }}
+  namespace: {{ NAMESPACE }}
 spec:
   replicas: 1
   selector:
     matchLabels:
       app: spdk-app-{{ HOSTNAME }}
   template:
     metadata:
@@ -27,30 +28,61 @@
             path: /lib/modules
         - name: dev-vol
           hostPath:
             path: /dev
         - name: hugepage
           emptyDir:
             medium: HugePages
+        - name: script-volume
+          emptyDir: {}
+        - name: script-config
+          configMap:
+            name: caching-node-restart-script-cm
+      initContainers:
+        - name: copy-script
+          image: busybox
+          command: ["sh", "-c", "cp /config/restart_script.py /script/restart_script.py"]
+          volumeMounts:
+            - name: script-volume
+              mountPath: /script
+            - name: script-config
+              mountPath: /config
       containers:
       - name: spdk-container
         image: {{ SPDK_IMAGE }}
         imagePullPolicy: "Always"
         command: ["/root/scripts/run_spdk_tgt.sh", "{{ SPDK_CPU_MASK }}", "{{ SPDK_MEM }}"]
+        lifecycle:
+          postStart:
+            exec:
+              command: ["/usr/bin/python3", "/script/restart_script.py"]
+        env:
+          - name: SPDKCSI_SECRET
+            valueFrom:
+              secretKeyRef:
+                name: spdkcsi-secret
+                key: secret.json
+          - name: CLUSTER_CONFIG
+            valueFrom:
+              configMapKeyRef:
+                name: spdkcsi-cm
+                key: config.json
         securityContext:
           privileged: true
         volumeMounts:
         - name: socket-dir
           mountPath: /var/tmp
         - name: host-sys
           mountPath: /sys
         - name: host-modules
           mountPath: /lib/modules
         - name: dev-vol
           mountPath: /dev
+        - name: script-volume
+          mountPath: /script
         resources:
           limits:
             hugepages-2Mi: 2Gi
             memory: 1024Mi
           requests:
             memory: 1024Mi
```

## Comparing `sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_mig-1.0.90/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,18 @@
     if 'spdk_cpu_mask' in data:
         spdk_cpu_mask = data['spdk_cpu_mask']
     spdk_mem = None
     if 'spdk_mem' in data:
         spdk_mem = data['spdk_mem']
     node_cpu_count = os.cpu_count()
 
+    global namespace
+    if 'namespace' in data:
+        namespace = data['namespace']
+
     if spdk_cpu_mask:
         requested_cpu_count = len(format(int(spdk_cpu_mask, 16), 'b'))
         if requested_cpu_count > node_cpu_count:
             return utils.get_response(
                 False,
                 f"The requested cpu count: {requested_cpu_count} "
                 f"is larger than the node's cpu count: {node_cpu_count}")
```

## Comparing `sbcli-mig-1.0.9/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_mig-1.0.90/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,15 @@
         privileged=True,
         network_mode="host",
         log_config=LogConfig(type=LogConfig.types.JOURNALD),
         volumes=[
             '/var/tmp:/var/tmp',
             '/dev:/dev',
             '/lib/modules/:/lib/modules/',
+            '/var/lib/systemd/coredump/:/var/lib/systemd/coredump/',
             '/sys:/sys'],
         # restart_policy={"Name": "on-failure", "MaximumRetryCount": 99}
     )
 
     server_ip = data['server_ip']
     rpc_port = data['rpc_port']
     rpc_username = data['rpc_username']
```

## Comparing `sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_mig-1.0.90/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -141,7 +141,23 @@
         return utils.get_response_error(f"Cluster not found: {uuid}", 404)
     if cluster.status == Cluster.STATUS_INACTIVE:
         return utils.get_response("Cluster already inactive")
 
     data = cluster_ops.get_logs(uuid, is_json=True)
     return utils.get_response(json.loads(data))
 
+
+@bp.route('/cluster/gracefulshutdown/<string:uuid>', methods=['PUT'])
+def cluster_grace_shutdown(uuid):
+    cluster = db_controller.get_cluster_by_id(uuid)
+    if not cluster:
+        return utils.get_response_error(f"Cluster not found: {uuid}", 404)
+    ret = cluster_ops.cluster_grace_shutdown(uuid)
+    return utils.get_response(ret)
+
+@bp.route('/cluster/gracefulstartup/<string:uuid>', methods=['PUT'])
+def cluster_grace_startup(uuid):
+    cluster = db_controller.get_cluster_by_id(uuid)
+    if not cluster:
+        return utils.get_response_error(f"Cluster not found: {uuid}", 404)
+    ret = cluster_ops.cluster_grace_startup(uuid)
+    return utils.get_response(ret)
```

## Comparing `sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 import logging
+import threading
 
 from flask import Blueprint, request
 
 
 from simplyblock_web import utils
 from simplyblock_core import kv_store
 from simplyblock_core.controllers import caching_node_controller
@@ -30,32 +31,37 @@
     node_ip = cl_data['node_ip']
     iface_name = cl_data['iface_name']
 
     data_nics_list = []
     spdk_cpu_mask = None
     spdk_mem = None
     spdk_image = None
+    namespace = None
 
     if 'spdk_cpu_mask' in cl_data:
         spdk_cpu_mask = cl_data['spdk_cpu_mask']
 
     if 'spdk_mem' in cl_data:
         mem = cl_data['spdk_mem']
         spdk_mem = utils.parse_size(mem)
         if spdk_mem < 1 * 1024 * 1024:
             return utils.get_response_error(f"SPDK memory:{mem} must be larger than 1G", 400)
 
-
     if 'spdk_image' in cl_data:
         spdk_image = cl_data['spdk_image']
 
-    ret = caching_node_controller.add_node(
-        cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask, spdk_mem, spdk_image)
+    if 'namespace' in cl_data:
+        namespace = cl_data['namespace']
+
+    t = threading.Thread(
+        target=caching_node_controller.add_node,
+        args=(cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask, spdk_mem, spdk_image, namespace))
+    t.start()
 
-    return utils.get_response(ret)
+    return utils.get_response(True)
 
 
 @bp.route('/cachingnode', methods=['GET'], defaults={'uuid': None})
 @bp.route('/cachingnode/<string:uuid>', methods=['GET'])
 def list_caching_nodes(uuid):
     if uuid:
         node = db_controller.get_caching_node_by_id(uuid)
```

## Comparing `sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_device.py` & `sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_mig-1.0.90/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 # encoding: utf-8
 import logging
 import math
 import os
 import time
+import traceback
 
 import cpuinfo
 import yaml
 from kubernetes import client, config
 from flask import Blueprint
 from flask import request
 from kubernetes.client import ApiException
@@ -20,15 +21,16 @@
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 bp = Blueprint("caching_node_k", __name__, url_prefix="/cnode")
 
 
 node_name = os.environ.get("HOSTNAME")
 deployment_name = f"spdk-deployment-{node_name}"
-namespace = 'default'
+default_namespace = 'default'
+namespace_id_file = '/etc/simplyblock/namespace'
 pod_name = 'spdk-deployment'
 
 
 config.load_incluster_config()
 k8s_apps_v1 = client.AppsV1Api()
 k8s_core_v1 = client.CoreV1Api()
 
@@ -41,14 +43,34 @@
 system_id = ""
 try:
     system_id, _, _ = node_utils.run_command("dmidecode -s system-uuid")
 except:
     pass
 
 
+def get_namespace():
+    if os.path.exists(namespace_id_file):
+        with open(namespace_id_file, 'r') as f:
+            out = f.read()
+            return out
+    return default_namespace
+
+
+def set_namespace(namespace):
+    if not os.path.exists(namespace_id_file):
+        try:
+            os.makedirs(os.path.dirname(namespace_id_file), exist_ok=True)
+        except:
+            logger.error(traceback.format_exc())
+            return False
+    with open(namespace_id_file, "w+") as f:
+        f.write(namespace)
+    return True
+
+
 @bp.route('/scan_devices', methods=['GET'])
 def scan_devices():
     run_health_check = request.args.get('run_health_check', default=False, type=bool)
     out = {
         "nvme_devices": node_utils._get_nvme_devices(),
         "nvme_pcie_list": node_utils._get_nvme_pcie_list(),
         "spdk_devices": node_utils._get_spdk_devices(),
@@ -65,14 +87,19 @@
     if 'spdk_cpu_mask' in data:
         spdk_cpu_mask = data['spdk_cpu_mask']
     spdk_mem = None
     if 'spdk_mem' in data:
         spdk_mem = data['spdk_mem']
     node_cpu_count = os.cpu_count()
 
+    namespace = get_namespace()
+    if 'namespace' in data:
+        namespace = data['namespace']
+        set_namespace(namespace)
+
     if spdk_cpu_mask:
         requested_cpu_count = len(format(int(spdk_cpu_mask, 16), 'b'))
         if requested_cpu_count > node_cpu_count:
             return utils.get_response(
                 False,
                 f"The requested cpu count: {requested_cpu_count} "
                 f"is larger than the node's cpu count: {node_cpu_count}")
@@ -91,66 +118,45 @@
     if _is_pod_up():
         logger.info("SPDK deployment found, removing...")
         spdk_process_kill()
 
     node_name = os.environ.get("HOSTNAME")
     logger.debug(f"deploying caching node spdk on worker: {node_name}")
 
-    env = Environment(loader=FileSystemLoader(os.path.join(TOP_DIR, 'templates')), trim_blocks=True, lstrip_blocks=True)
-    template = env.get_template('deploy_spdk.yaml.j2')
-    values = {
-        'SPDK_IMAGE': spdk_image,
-        'SPDK_CPU_MASK': spdk_cpu_mask,
-        'SPDK_MEM': spdk_mem,
-        'SERVER_IP': data['server_ip'],
-        'RPC_PORT': data['rpc_port'],
-        'RPC_USERNAME': data['rpc_username'],
-        'RPC_PASSWORD': data['rpc_password'],
-        'HOSTNAME': node_name,
-    }
-    dep = yaml.safe_load(template.render(values))
-    resp = k8s_apps_v1.create_namespaced_deployment(body=dep, namespace=namespace)
-    logger.info(f"Deployment created: '{resp.metadata.name}'")
-
-    retries = 20
-    while retries > 0:
-        resp = k8s_core_v1.list_namespaced_pod(namespace)
-        new_pod = None
-        for pod in resp.items:
-            if pod.metadata.name.startswith(pod_name):
-                new_pod = pod
-                break
-
-        if not new_pod:
-            logger.info("Container is not running, waiting...")
-            time.sleep(3)
-            retries -= 1
-            continue
-
-        status = new_pod.status.phase
-        logger.info(f"pod: {pod_name} status: {status}")
-
-        if status == "Running":
-            logger.info(f"Container status: {status}")
-            return utils.get_response(True)
-        else:
-            logger.info("Container is not running, waiting...")
-            time.sleep(3)
-            retries -= 1
+    try:
+        env = Environment(loader=FileSystemLoader(os.path.join(TOP_DIR, 'templates')), trim_blocks=True, lstrip_blocks=True)
+        template = env.get_template('deploy_spdk.yaml.j2')
+        values = {
+            'SPDK_IMAGE': spdk_image,
+            'SPDK_CPU_MASK': spdk_cpu_mask,
+            'SPDK_MEM': spdk_mem,
+            'SERVER_IP': data['server_ip'],
+            'RPC_PORT': data['rpc_port'],
+            'RPC_USERNAME': data['rpc_username'],
+            'RPC_PASSWORD': data['rpc_password'],
+            'HOSTNAME': node_name,
+            'NAMESPACE': namespace,
+        }
+        dep = yaml.safe_load(template.render(values))
+        logger.debug(dep)
+        resp = k8s_apps_v1.create_namespaced_deployment(body=dep, namespace=namespace)
+        msg = f"Deployment created: '{resp.metadata.name}' in namespace '{namespace}"
+        logger.info(msg)
+    except:
+        return utils.get_response(False, f"Deployment failed:\n{traceback.format_exc()}")
 
-    return utils.get_response(
-        False, f"Deployment create max retries reached")
+    return utils.get_response(msg)
 
 
 @bp.route('/spdk_process_kill', methods=['GET'])
 def spdk_process_kill():
 
     try:
+        namespace = get_namespace()
         resp = k8s_apps_v1.delete_namespaced_deployment(deployment_name, namespace)
-
         retries = 20
         while retries > 0:
             resp = k8s_core_v1.list_namespaced_pod(namespace)
             found = False
             for pod in resp.items:
                 if pod.metadata.name.startswith(pod_name):
                     found = True
@@ -165,15 +171,15 @@
     except ApiException as e:
         logger.info(e.body)
 
     return utils.get_response(True)
 
 
 def _is_pod_up():
-    resp = k8s_core_v1.list_namespaced_pod(namespace)
+    resp = k8s_core_v1.list_namespaced_pod(get_namespace())
     for pod in resp.items:
         if pod.metadata.name.startswith(pod_name):
             status = pod.status.phase
             if status == "Running":
                 return True
             else:
                 return False
```

## Comparing `sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_mig-1.0.90/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/blueprints/csi.py` & `sbcli_mig-1.0.90/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_web/blueprints/snode_ops.py` & `sbcli_mig-1.0.90/simplyblock_web/blueprints/snode_ops.py`

 * *Files 10% similar despite different names*

```diff
@@ -113,14 +113,15 @@
         network_mode="host",
         log_config=log_config,
         volumes=[
             '/etc/simplyblock:/etc/simplyblock',
             '/var/tmp:/var/tmp',
             '/dev:/dev',
             '/lib/modules/:/lib/modules/',
+            '/var/lib/systemd/coredump/:/var/lib/systemd/coredump/',
             '/sys:/sys'],
         # restart_policy={"Name": "on-failure", "MaximumRetryCount": 99}
     )
     container2 = node_docker.containers.run(
         constants.SIMPLY_BLOCK_SPDK_CORE_IMAGE,
         "python /root/scripts/spdk_http_proxy.py",
         name="spdk_proxy",
@@ -187,14 +188,35 @@
 
 
 def delete_cluster_id():
     out, _, _ = node_utils.run_command(f"rm -f {cluster_id_file}")
     return out
 
 
+def get_ec2_meta():
+    stream = os.popen('curl -X PUT "http://169.254.169.254/latest/api/token" -H "X-aws-ec2-metadata-token-ttl-seconds: 21600"')
+    token = stream.read()
+    stream = os.popen(f"curl -H \"X-aws-ec2-metadata-token: {token}\" http://169.254.169.254/latest/dynamic/instance-identity/document")
+    out = stream.read()
+    try:
+        data = json.loads(out)
+        return data
+    except:
+        return {}
+
+
+def get_ec2_public_ip():
+    stream = os.popen('curl -X PUT "http://169.254.169.254/latest/api/token" -H "X-aws-ec2-metadata-token-ttl-seconds: 21600"')
+    token = stream.read()
+    stream = os.popen(f"curl -H \"X-aws-ec2-metadata-token: {token}\" http://169.254.169.254/latest/meta-data/public-ipv4")
+    response = stream.read()
+    out = response if "404" not in response else None
+    return out
+
+
 @bp.route('/info', methods=['GET'])
 def get_info():
 
     out = {
         "cluster_id": get_cluster_id(),
 
         "hostname": hostname,
@@ -209,15 +231,19 @@
 
         "nvme_devices": node_utils._get_nvme_devices(),
         "nvme_pcie_list": node_utils._get_nvme_pcie_list(),
 
         "spdk_devices": node_utils._get_spdk_devices(),
         "spdk_pcie_list": node_utils._get_spdk_pcie_list(),
 
-        "network_interface": node_utils.get_nics_data()
+        "network_interface": node_utils.get_nics_data(),
+
+        "ec2_metadata": get_ec2_meta(),
+
+        "ec2_public_ip": get_ec2_public_ip(),
     }
     return utils.get_response(out)
 
 
 @bp.route('/join_swarm', methods=['POST'])
 def join_swarm():
     data = request.get_json()
```

## Comparing `sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_mig-1.0.90/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 #!/usr/bin/env python
 # encoding: utf-8
 
 import logging
 
 from flask import Blueprint
 from flask import request
@@ -90,15 +91,16 @@
         | max_w_mbytes    | Maximum Write Mega Bytes Per Second
         | ha_type         | LVol HA type, can be (single,ha,default=cluster's ha type), Default=default
         | distr_vuid      | Distr bdev virtual unique ID, Default=0 means random
         | distr_ndcs      | Distr bdev number of data chunks per stripe, Default=0 means auto set
         | distr_npcs      | Distr bdev number of parity chunks per stripe, Default=0 means auto set
         | distr_bs        | Distr bdev block size, Default=4096
         | distr_chunk_bs  | Distr bdev chunk block size, Default=4096
-
+        | crypto_key1     | the hex value of key1 to be used for lvol encryption
+        | crypto_key2     | the hex value of key2 to be used for lvol encryption
     """""
 
     cl_data = request.get_json()
     logger.debug(cl_data)
     if 'size' not in cl_data:
         return utils.get_csi_response(None, "missing required param: size", 400)
     if 'name' not in cl_data:
@@ -134,14 +136,16 @@
     ha_type = utils.get_value_or_default(cl_data, "ha_type", "default")
 
     distr_vuid = utils.get_int_value_or_default(cl_data, "distr_vuid", 0)
     distr_ndcs = utils.get_int_value_or_default(cl_data, "distr_ndcs", 0)
     distr_npcs = utils.get_int_value_or_default(cl_data, "distr_npcs", 0)
     distr_bs = utils.get_int_value_or_default(cl_data, "distr_ps", 4096)
     distr_chunk_bs = utils.get_int_value_or_default(cl_data, "distr_chunk_bs", 4096)
+    crypto_key1 = utils.get_value_or_default(cl_data, "crypto_key1", None)
+    crypto_key2 = utils.get_value_or_default(cl_data, "crypto_key2", None)
 
     ret, error = lvol_controller.add_lvol_ha(
         name=name,
         size=size,
         pool_id_or_name=pool.get_id(),
 
         use_comp=compression,
@@ -154,15 +158,17 @@
 
         host_id_or_name=None,
         ha_type=ha_type,
         distr_vuid=distr_vuid,
         distr_ndcs=distr_ndcs,
         distr_npcs=distr_npcs,
         distr_bs=distr_bs,
-        distr_chunk_bs=distr_chunk_bs
+        distr_chunk_bs=distr_chunk_bs,
+        crypto_key1=crypto_key1,
+        crypto_key2=crypto_key2,
     )
 
     return utils.get_csi_response(ret, error)
 
 
 @bp.route('/lvol/<string:uuid>', methods=['PUT'])
 def update_lvol(uuid):
@@ -241,8 +247,7 @@
 def connect_lvol(uuid):
     lvol = db_controller.get_lvol_by_id(uuid)
     if not lvol:
         return utils.get_response_error(f"LVol not found: {uuid}", 404)
 
     ret = lvol_controller.connect_lvol(uuid)
     return utils.get_csi_response(ret)
-
```

## Comparing `sbcli-mig-1.0.9/simplyblock_cli/cli.py` & `sbcli_mig-1.0.90/simplyblock_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,28 +36,33 @@
         # sub_command.add_argument("ifname", help='Management interface name')
         # sub_command.add_argument("--data-nics", help='Data interface names', nargs='+', dest='data_nics')
 
         sub_command = self.add_sub_command(subparser, "add-node", 'Add storage node by ip')
         sub_command.add_argument("cluster_id", help='UUID of the cluster to which the node will belong')
         sub_command.add_argument("node_ip", help='IP of storage node to add')
         sub_command.add_argument("ifname", help='Management interface name')
+        sub_command.add_argument("--jm-pcie", help='JM device address', dest='jm_pcie')
         sub_command.add_argument("--data-nics", help='Data interface names', nargs='+', dest='data_nics')
         sub_command.add_argument("--cpu-mask", help='SPDK app CPU mask, default is all cores found',
                                  dest='spdk_cpu_mask')
         sub_command.add_argument("--memory", help='SPDK huge memory allocation, default is 4G', dest='spdk_mem')
         sub_command.add_argument("--dev-split", help='Split nvme devices by this factor, can be 2 or more',
                                  dest='dev_split', type=int, default=1)
         sub_command.add_argument("--spdk-image", help='SPDK image uri', dest='spdk_image')
         sub_command.add_argument("--spdk-debug", help='Enable spdk debug logs', dest='spdk_debug', required=False, action='store_true')
 
         sub_command.add_argument("--iobuf_small_pool_count", help='bdev_set_options param', dest='small_pool_count',  type=int, default=0)
         sub_command.add_argument("--iobuf_large_pool_count", help='bdev_set_options param', dest='large_pool_count',  type=int, default=0)
         sub_command.add_argument("--iobuf_small_bufsize", help='bdev_set_options param', dest='small_bufsize',  type=int, default=0)
         sub_command.add_argument("--iobuf_large_bufsize", help='bdev_set_options param', dest='large_bufsize',  type=int, default=0)
 
+        # delete storage node
+        sub_command = self.add_sub_command(subparser, "delete", 'Delete storage node obj')
+        sub_command.add_argument("node_id", help='UUID of storage node')
+
         # remove storage node
         sub_command = self.add_sub_command(subparser, "remove", 'Remove storage node')
         sub_command.add_argument("node_id", help='UUID of storage node')
         sub_command.add_argument("--force-remove", help='Force remove all LVols and snapshots',
                                  dest='force_remove', required=False, action='store_true')
         sub_command.add_argument("--force-migrate", help='Force migrate All LVols to other nodes',
                                  dest='force_migrate', required=False, action='store_true')
@@ -301,14 +306,18 @@
         sub_command.add_argument("--cap-crit", help='Capacity critical level in percent, default=90',
                                  type=int, required=False, dest="cap_crit")
         sub_command.add_argument("--prov-cap-warn", help='Capacity warning level in percent, default=180',
                                  type=int, required=False, dest="prov_cap_warn")
         sub_command.add_argument("--prov-cap-crit", help='Capacity critical level in percent, default=190',
                                  type=int, required=False, dest="prov_cap_crit")
         sub_command.add_argument("--ifname", help='Management interface name, default: eth0')
+        sub_command.add_argument("--log-del-interval", help='graylog deletion interval, default: 7d',
+                                 dest='log_del_interval', default='7d')
+        sub_command.add_argument("--metrics-retention-period", help='retention period for prometheus metrics, default: 7d',
+                                 dest='metrics_retention_period', default='7d')
 
         # show cluster list
         sub_command = self.add_sub_command(subparser, 'list', 'Show clusters list')
 
         # # join cluster
         # sub_command = self.add_sub_command(subparser, 'join', 'join cluster')
         # sub_command.add_argument("cluster_ip", help='the cluster IP address')
@@ -372,14 +381,15 @@
         sub_command.add_argument("host-nqn", help='NQN of the host to remove from the allowed hosts list')
 
         sub_command = self.add_sub_command(
             subparser, 'get-capacity', 'Returns the current total available capacity, utilized capacity '
                                        '(in percent and absolute) and provisioned capacity (in percent and absolute) '
                                        'in GB in the cluster.')
         sub_command.add_argument("cluster_id", help='the cluster UUID')
+        sub_command.add_argument("--json", help='Print json output', required=False, action='store_true')
         sub_command.add_argument("--history", help='(XXdYYh), list history records (one for every 15 minutes) '
                                                    'for XX days and YY hours (up to 10 days in total).')
 
         sub_command = self.add_sub_command(
             subparser, 'get-io-stats', 'Returns the io statistics. If --history is not selected, this is a monitor, '
                                        'which updates current statistics records every two seconds '
                                        '(similar to ping):read-iops write-iops total-iops read-mbs write-mbs total-mbs')
@@ -422,14 +432,22 @@
         sub_command = self.add_sub_command(subparser, "check", 'Health check cluster')
         sub_command.add_argument("id", help='cluster UUID')
 
         # update cluster
         sub_command = self.add_sub_command(subparser, "update", 'Update cluster mgmt services')
         sub_command.add_argument("id", help='cluster UUID')
 
+        # graceful-shutdown storage nodes
+        sub_command = self.add_sub_command(subparser, "graceful-shutdown", 'Graceful shutdown of storage nodes')
+        sub_command.add_argument("id", help='cluster UUID')
+
+        # graceful-startup storage nodes
+        sub_command = self.add_sub_command(subparser, "graceful-startup", 'Graceful startup of storage nodes')
+        sub_command.add_argument("id", help='cluster UUID')
+
         # lvol ops
         subparser = self.add_command('lvol', 'LVol commands')
         # add lvol
         sub_command = self.add_sub_command(subparser, 'add', 'Add a new logical volume')
         sub_command.add_argument("name", help='LVol name or id')
         sub_command.add_argument("size", help='LVol size: 10M, 10G, 10(bytes)')
         sub_command.add_argument("pool", help='Pool UUID or name')
@@ -441,14 +459,18 @@
                                  dest='ha_type', choices=["single", "ha", "default"], default='default')
 
         sub_command.add_argument("--compress",
                                  help='Use inline data compression and de-compression on the logical volume',
                                  required=False, action='store_true')
         sub_command.add_argument("--encrypt", help='Use inline data encryption and de-cryption on the logical volume',
                                  required=False, action='store_true')
+        sub_command.add_argument("--crypto-key1", help='the hex value of key1 to be used for lvol encryption',
+                                 dest='crypto_key1', default=None)
+        sub_command.add_argument("--crypto-key2", help='the hex value of key2 to be used for lvol encryption',
+                                 dest='crypto_key2', default=None)
         sub_command.add_argument("--thick", help='Deactivate thin provisioning', required=False, action='store_true')
         sub_command.add_argument("--node-ha",
                                  help='The maximum amount of concurrent node failures accepted without interruption of operations',
                                  required=False, default=1, type=int, choices=[0, 1, 2])
         sub_command.add_argument("--dev-redundancy",
                                  help='{1,2} supported minimal concurrent device failures without data loss',
                                  required=False, action='store_true')
@@ -704,14 +726,15 @@
         sub_command.add_argument("cluster_id", help='UUID of the cluster to which the node will belong')
         sub_command.add_argument("node_ip", help='IP of caching node to add')
         sub_command.add_argument("ifname", help='Management interface name')
         sub_command.add_argument("--cpu-mask", help='SPDK app CPU mask, default is all cores found',
                                  dest='spdk_cpu_mask')
         sub_command.add_argument("--memory", help='SPDK huge memory allocation, default is Max hugepages available', dest='spdk_mem')
         sub_command.add_argument("--spdk-image", help='SPDK image uri', dest='spdk_image')
+        sub_command.add_argument("--namespace", help='k8s namespace to deploy on',)
 
         sub_command = self.add_sub_command(subparser, 'list', 'List Caching nodes')
 
         sub_command = self.add_sub_command(subparser, 'list-lvols', 'List connected lvols')
         sub_command.add_argument("id", help='Caching Node UUID')
 
         sub_command = self.add_sub_command(subparser, 'remove', 'Remove Caching node from the cluster')
@@ -799,23 +822,26 @@
                 if args.spdk_mem:
                     spdk_mem = self.parse_size(args.spdk_mem)
                     if spdk_mem < 1 * 1024 * 1024:
                         return f"SPDK memory:{args.spdk_mem} must be larger than 1G"
 
                 out = storage_ops.add_node(
                     cluster_id, node_ip, ifname, data_nics, spdk_cpu_mask, spdk_mem, dev_split, spdk_image, spdk_debug,
-                    small_pool_count, large_pool_count, small_bufsize, large_bufsize)
+                    small_pool_count, large_pool_count, small_bufsize, large_bufsize, args.jm_pcie)
                 return out
 
             elif sub_command == "list":
                 ret = storage_ops.list_storage_nodes(self.db_store, args.json)
 
             elif sub_command == "remove":
                 ret = storage_ops.remove_storage_node(args.node_id, args.force_remove, args.force_migrate)
 
+            elif sub_command == "delete":
+                ret = storage_ops.delete_storage_node(args.node_id)
+
             elif sub_command == "restart":
                 node_id = args.node_id
 
                 spdk_image = args.spdk_image
                 spdk_debug = args.spdk_debug
 
                 cpu_mask = None
@@ -986,19 +1012,20 @@
                 ret = cluster_ops.suspend_cluster(cluster_id)
             elif sub_command == 'unsuspend':
                 cluster_id = args.cluster_id
                 ret = cluster_ops.unsuspend_cluster(cluster_id)
             elif sub_command == "get-capacity":
                 cluster_id = args.cluster_id
                 history = args.history
-                data = cluster_ops.get_capacity(cluster_id, history)
-                if data:
-                    ret = utils.print_table(data)
+                is_json = args.json
+                data = cluster_ops.get_capacity(cluster_id, history, is_json=is_json)
+                if is_json:
+                    ret = data
                 else:
-                    return False
+                    ret = utils.print_table(data)
 
             elif sub_command == "get-io-stats":
                 data = cluster_ops.get_iostats_history(args.cluster_id, args.history, args.records)
                 if data:
                     ret = utils.print_table(data)
                 else:
                     return False
@@ -1018,14 +1045,18 @@
             elif sub_command == "check":
                 cluster_id = args.id
                 ret = health_controller.check_cluster(cluster_id)
             elif sub_command == "get":
                 ret = cluster_ops.get_cluster(args.id)
             elif sub_command == "update":
                 ret = cluster_ops.update_cluster(args.id)
+            elif sub_command == "graceful-shutdown":
+                ret = cluster_ops.cluster_grace_shutdown(args.id)
+            elif sub_command == "graceful-startup":
+                ret = cluster_ops.cluster_grace_startup(args.id)
             else:
                 self.parser.print_help()
 
         elif args.command == 'compute-node':
             sub_command = args_dict[args.command]
             if sub_command == "add":
                 ret = compute_ops.add_compute_node(self.db_store)
@@ -1067,15 +1098,17 @@
                     args.max_rw_iops,
                     args.max_rw_mbytes,
                     args.max_r_mbytes,
                     args.max_w_mbytes,
                     distr_bs,
                     distr_chunk_bs,
                     with_snapshot=with_snapshot,
-                    max_size=max_size)
+                    max_size=max_size,
+                    crypto_key1=args.crypto_key1,
+                    crypto_key2=args.crypto_key2)
                 if results:
                     ret = results
                 else:
                     ret = error
             elif sub_command == "add-distr":
                 pass
             elif sub_command == "qos-set":
@@ -1234,14 +1267,15 @@
 
             if sub_command == "add-node":
                 cluster_id = args.cluster_id
                 node_ip = args.node_ip
                 ifname = args.ifname
                 data_nics = []
                 spdk_image = args.spdk_image
+                namespace = args.namespace
 
                 spdk_cpu_mask = None
                 if args.spdk_cpu_mask:
                     if self.validate_cpu_mask(args.spdk_cpu_mask):
                         spdk_cpu_mask = args.spdk_cpu_mask
                     else:
                         return f"Invalid cpu mask value: {args.spdk_cpu_mask}"
@@ -1249,15 +1283,15 @@
                 spdk_mem = None
                 if args.spdk_mem:
                     spdk_mem = self.parse_size(args.spdk_mem)
                     if spdk_mem < 1 * 1024 * 1024:
                         return f"SPDK memory:{args.spdk_mem} must be larger than 1G"
 
                 ret = caching_node_controller.add_node(
-                    cluster_id, node_ip, ifname, data_nics, spdk_cpu_mask, spdk_mem, spdk_image)
+                    cluster_id, node_ip, ifname, data_nics, spdk_cpu_mask, spdk_mem, spdk_image, namespace)
 
             if sub_command == "list":
                 #cluster_id
                 ret = caching_node_controller.list_nodes()
             if sub_command == "list-lvols":
                 ret = caching_node_controller.list_lvols(args.id)
             if sub_command == "remove":
@@ -1325,20 +1359,22 @@
         CLI_PASS = args.CLI_PASS
         model_ids = args.model_ids
         cap_warn = args.cap_warn
         cap_crit = args.cap_crit
         prov_cap_warn = args.prov_cap_warn
         prov_cap_crit = args.prov_cap_crit
         ifname = args.ifname
+        log_del_interval = args.log_del_interval
+        metrics_retention_period = args.metrics_retention_period
 
         # TODO: Validate the inputs
         return cluster_ops.create_cluster(
             blk_size, page_size_in_blocks, ha_type, tls,
             auth_hosts_only, CLI_PASS, model_ids, cap_warn, cap_crit, prov_cap_warn, prov_cap_crit,
-            ifname)
+            ifname, log_del_interval, metrics_retention_period)
 
     def cluster_join(self, args):
         cluster_id = args.cluster_id
         cluster_ip = args.cluster_ip
         role = args.role
         ifname = args.ifname
         data_nics = args.data_nics
```

## Comparing `sbcli-mig-1.0.9/sbcli_mig.egg-info/SOURCES.txt` & `sbcli_mig-1.0.90/sbcli_mig.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,32 +59,34 @@
 simplyblock_core/scripts/apply_dashboard.sh
 simplyblock_core/scripts/clean_local_storage_deploy.sh
 simplyblock_core/scripts/config_docker.sh
 simplyblock_core/scripts/datasource.yml
 simplyblock_core/scripts/db_config_double.sh
 simplyblock_core/scripts/db_config_single.sh
 simplyblock_core/scripts/deploy_stack.sh
+simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
 simplyblock_core/scripts/docker-compose-swarm.yml
 simplyblock_core/scripts/haproxy.cfg
 simplyblock_core/scripts/install_deps.sh
 simplyblock_core/scripts/prometheus.yml
 simplyblock_core/scripts/run_ssh.sh
 simplyblock_core/scripts/set_db_config.sh
 simplyblock_core/scripts/stack_deploy_wait.sh
 simplyblock_core/scripts/alerting/alert_resources.yaml
 simplyblock_core/scripts/alerting/alert_rules.yaml
 simplyblock_core/scripts/dashboards/cluster.json
 simplyblock_core/scripts/dashboards/devices.json
 simplyblock_core/scripts/dashboards/lvols.json
+simplyblock_core/scripts/dashboards/node-exporter.json
 simplyblock_core/scripts/dashboards/nodes.json
+simplyblock_core/scripts/dashboards/pools.json
 simplyblock_core/services/__init__.py
 simplyblock_core/services/caching_node_monitor.py
 simplyblock_core/services/cap_monitor.py
 simplyblock_core/services/capacity_and_stats_collector.py
-simplyblock_core/services/capacity_collector.py
 simplyblock_core/services/device_monitor.py
 simplyblock_core/services/distr_event_collector.py
 simplyblock_core/services/health_check_service.py
 simplyblock_core/services/install_service.sh
 simplyblock_core/services/log_agg_service.py
 simplyblock_core/services/lvol_monitor.py
 simplyblock_core/services/lvol_stat_collector.py
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/snode_client.py` & `sbcli_mig-1.0.90/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/constants.py` & `sbcli_mig-1.0.90/simplyblock_core/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,13 +45,16 @@
 }
 
 # To use 75% of hugepages to calculate ssd size to use for the ocf bdev
 CACHING_NODE_MEMORY_FACTOR = 0.75
 
 HEALTH_CHECK_INTERVAL_SEC = 60
 
+GRAYLOG_CHECK_INTERVAL_SEC = 60
 
-SIMPLY_BLOCK_DOCKER_IMAGE = "simplyblock/simplyblock:dev"
-SIMPLY_BLOCK_SPDK_CORE_IMAGE = "hamdykhader/spdk:core"
-SIMPLY_BLOCK_SPDK_ULTRA_IMAGE = "hamdykhader/spdk:main"
+FDB_CHECK_INTERVAL_SEC = 60
+
+SIMPLY_BLOCK_DOCKER_IMAGE = "simplyblock/simplyblock:graceful-shutdown"
+SIMPLY_BLOCK_SPDK_CORE_IMAGE = "simplyblock/spdk-core:latest"
+SIMPLY_BLOCK_SPDK_ULTRA_IMAGE = "simplyblock/spdk:main-latest"
 
 GELF_PORT = 12201
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/cnode_client.py` & `sbcli_mig-1.0.90/simplyblock_core/cnode_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,33 +65,39 @@
 
     def is_live(self):
         return self._request("GET", "")
 
     def info(self):
         return self._request("GET", "cnode/info")
 
-    def spdk_process_start(self, spdk_cpu_mask, spdk_mem, spdk_image, server_ip, rpc_port, rpc_username, rpc_password):
+    def spdk_process_start(
+            self, spdk_cpu_mask, spdk_mem, spdk_image, server_ip, rpc_port, rpc_username, rpc_password, namespace=None):
         params = {
             "spdk_cpu_mask": spdk_cpu_mask,
             "spdk_mem": spdk_mem,
             "spdk_image": spdk_image,
             "server_ip": server_ip,
             "rpc_port": rpc_port,
             "rpc_username": rpc_username,
             "rpc_password": rpc_password,
         }
+        if namespace:
+            params["namespace"] = namespace
         return self._request("POST", "cnode/spdk_process_start", params)
 
     def join_db(self, db_connection):
         params = {"db_connection": db_connection}
         return self._request("POST", "cnode/join_db", params)
 
     def spdk_process_kill(self):
         return self._request("GET", "cnode/spdk_process_kill")
 
+    def spdk_process_is_up(self):
+        return self._request("GET", "cnode/spdk_process_is_up")
+
     def connect_nvme(self, ip, port, nqn):
         params = {
             "ip": ip,
             "port": port,
             "nqn": nqn}
         return self._request("POST", "cnode/nvme_connect", params)
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/mgmt_node_ops.py` & `sbcli_mig-1.0.90/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/utils.py` & `sbcli_mig-1.0.90/simplyblock_core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     if out and ifname in out:
         return out[ifname]['ip']
     return False
 
 
 def print_table(data: list):
     if data:
-        x = PrettyTable(field_names=data[0].keys())
+        x = PrettyTable(field_names=data[0].keys(), max_width=70)
         x.align = 'l'
         for node_data in data:
             row = []
             for key in node_data:
                 row.append(node_data[key])
             x.add_row(row)
         return x.__str__()
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/storage_node_ops.py` & `sbcli_mig-1.0.90/simplyblock_core/storage_node_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 import datetime
 import json
 import logging as log
+import os
 
 import pprint
 
 import time
 import uuid
 
 import docker
@@ -212,35 +213,48 @@
     db_controller = DBController()
 
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password)
 
     for index, nvme in enumerate(snode.nvme_devices):
-        if nvme.status not in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_UNAVAILABLE]:
+        if nvme.status not in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_UNAVAILABLE,
+                               NVMeDevice.STATUS_JM, NVMeDevice.STATUS_READONLY]:
             logger.debug(f"Device is not online or unavailable: {nvme.get_id()}, status: {nvme.status}")
             continue
 
         test_name = f"{nvme.nvme_bdev}_test"
         # create testing bdev
         ret = rpc_client.bdev_passtest_create(test_name, nvme.nvme_bdev)
-
+        if not ret:
+            logger.error(f"Failed to create bdev: {test_name}")
+            return False
         alceml_id = nvme.get_id()
-        node_id_mini = snode.get_id().split("-")[-1]
-        alceml_id_mini = alceml_id.split("-")[-1]
-        alceml_name = f"node_{node_id_mini}_dev_{alceml_id_mini}"
+        alceml_name = device_controller.get_alceml_name(alceml_id)
         logger.info(f"adding {alceml_name}")
         pba_init_mode = 3
         if after_restart:
             pba_init_mode = 2
         ret = rpc_client.bdev_alceml_create(alceml_name, test_name, alceml_id, pba_init_mode=pba_init_mode)
         if not ret:
             logger.error(f"Failed to create alceml bdev: {alceml_name}")
             return False
 
+        # create jm
+        if nvme.jm_bdev:
+            ret = rpc_client.bdev_jm_create(nvme.jm_bdev, alceml_name)
+            if not ret:
+                logger.error(f"Failed to create JM bdev: {snode.nvme_devices[0].jm_bdev}")
+                return False
+            nvme.testing_bdev = test_name
+            nvme.alceml_bdev = alceml_name
+            nvme.io_error = True
+            nvme.status = NVMeDevice.STATUS_JM
+            continue
+
         # add pass through
         pt_name = f"{alceml_name}_PT"
         ret = rpc_client.bdev_PT_NoExcl_create(pt_name, alceml_name)
         if not ret:
             logger.error(f"Failed to create pt noexcl bdev: {pt_name}")
             return False
 
@@ -265,30 +279,26 @@
                 break
         logger.info(f"add {pt_name} to subsystem")
         ret = rpc_client.nvmf_subsystem_add_ns(subsystem_nqn, pt_name)
         if not ret:
             logger.error(f"Failed to add: {pt_name} to the subsystem: {subsystem_nqn}")
             return False
 
-        # create jm
-        if nvme.jm_bdev:
-            ret = rpc_client.bdev_jm_create(nvme.jm_bdev, alceml_name)
-            if not ret:
-                logger.error(f"Failed to create JM bdev: {snode.nvme_devices[0].jm_bdev}")
-                return False
-
         nvme.testing_bdev = test_name
         nvme.alceml_bdev = alceml_name
         nvme.pt_bdev = pt_name
         nvme.nvmf_nqn = subsystem_nqn
         nvme.nvmf_ip = IP
         nvme.nvmf_port = 4420
         nvme.io_error = False
+        old_status = nvme.status
         nvme.status = NVMeDevice.STATUS_ONLINE
-    snode.write_to_db(db_controller.kv_store)
+        device_events.device_status_change(nvme, nvme.status, old_status)
+        snode.write_to_db(db_controller.kv_store)
+
     return True
 
 
 def _connect_to_remote_devs(this_node):
     db_controller = DBController()
 
     rpc_client = RPCClient(
@@ -314,15 +324,15 @@
             dev.remote_bdev = f"{name}n1"
             remote_devices.append(dev)
     return remote_devices
 
 
 def add_node(cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask,
              spdk_mem, dev_split=1, spdk_image=None, spdk_debug=False,
-             small_pool_count=0, large_pool_count=0, small_bufsize=0, large_bufsize=0):
+             small_pool_count=0, large_pool_count=0, small_bufsize=0, large_bufsize=0, jm_device_pcie=None):
     db_controller = DBController()
     kv_store = db_controller.kv_store
 
     cluster = db_controller.get_cluster_by_id(cluster_id)
     if not cluster:
         logger.error("Cluster not found: %s", cluster_id)
         return False
@@ -335,14 +345,49 @@
     node_info, _ = snode_api.info()
     logger.info(f"Node found: {node_info['hostname']}")
     if "cluster_id" in node_info and node_info['cluster_id']:
         if node_info['cluster_id'] != cluster_id:
             logger.error(f"This node is part of another cluster: {node_info['cluster_id']}")
             return False
 
+    ec2_metadata = None
+    if "ec2_metadata" in node_info and node_info['ec2_metadata']:
+        ec2_metadata = node_info['ec2_metadata']
+        """"
+         "ec2_metadata": {
+              "accountId": "565979732541",
+              "architecture": "x86_64",
+              "availabilityZone": "eu-west-1a",
+              "billingProducts": [
+                "bp-6fa54006"
+              ],
+              "devpayProductCodes": null,
+              "imageId": "ami-08e592fbb0f535224",
+              "instanceId": "i-0ba9e766df57bc62c",
+              "instanceType": "m6id.large",
+              "kernelId": null,
+              "marketplaceProductCodes": null,
+              "pendingTime": "2024-03-24T19:39:14Z",
+              "privateIp": "172.31.23.236",
+              "ramdiskId": null,
+              "region": "eu-west-1",
+              "version": "2017-09-30"
+        }
+        """""
+        logger.debug(json.dumps(ec2_metadata,indent=2))
+        logger.info(f"EC2 Instance found: {ec2_metadata['instanceId']}")
+        logger.info(f"EC2 Instance type: {ec2_metadata['instanceType']}")
+        logger.info(f"EC2 Instance privateIp: {ec2_metadata['privateIp']}")
+        logger.info(f"EC2 Instance region: {ec2_metadata['region']}")
+
+        for node in db_controller.get_storage_nodes():
+            if node.ec2_instance_id and node.ec2_instance_id == ec2_metadata['instanceId']:
+                logger.error(f"Node already exists, try remove it first: {ec2_metadata['instanceId']}")
+                return False
+
     # check for memory
     if "memory_details" in node_info and node_info['memory_details']:
         memory_details = node_info['memory_details']
         logger.info("Node Memory info")
         logger.info(f"Total: {utils.humanbytes(memory_details['total'])}")
         logger.info(f"Free: {utils.humanbytes(memory_details['free'])}")
         logger.info(f"Hugepages Total: {utils.humanbytes(memory_details['huge_total'])}")
@@ -370,41 +415,44 @@
     logger.info("Deploying SPDK")
     results, err = snode_api.spdk_process_start(spdk_cpu_mask, spdk_mem, spdk_image, spdk_debug, cluster_ip)
     time.sleep(10)
     if not results:
         logger.error(f"Failed to start spdk: {err}")
         return False
 
-    hostname = node_info['hostname']
-    snode = db_controller.get_storage_node_by_hostname(hostname)
-    if snode:
-        logger.error("Node already exists, try remove it first.")
-        return False
-
     data_nics = []
     names = data_nics_list or [iface_name]
     for nic in names:
         device = node_info['network_interface'][nic]
         data_nics.append(
             IFace({
                 'uuid': str(uuid.uuid4()),
                 'if_name': device['name'],
                 'ip4_address': device['ip'],
                 'status': device['status'],
                 'net_type': device['net_type']}))
 
+    hostname = node_info['hostname']
     rpc_user, rpc_pass = utils.generate_rpc_user_and_pass()
     BASE_NQN = cluster.nqn.split(":")[0]
     subsystem_nqn = f"{BASE_NQN}:{hostname}"
     # creating storage node object
     snode = StorageNode()
     snode.uuid = str(uuid.uuid4())
     snode.status = StorageNode.STATUS_IN_CREATION
     snode.baseboard_sn = node_info['system_id']
     snode.system_uuid = node_info['system_id']
+
+    if ec2_metadata:
+        snode.ec2_metadata = ec2_metadata
+        snode.ec2_instance_id = ec2_metadata['instanceId']
+
+    if "ec2_public_ip" in node_info and node_info['ec2_public_ip']:
+        snode.ec2_public_ip = node_info['ec2_public_ip']
+
     snode.hostname = hostname
     snode.host_nqn = subsystem_nqn
     snode.subsystem = subsystem_nqn
     snode.data_nics = data_nics
     snode.mgmt_ip = node_info['network_interface'][iface_name]['ip']
     snode.rpc_port = constants.RPC_HTTP_PROXY_PORT
     snode.rpc_username = rpc_user
@@ -425,32 +473,47 @@
 
     snode.spdk_cpu_mask = spdk_cpu_mask or ""
     snode.spdk_mem = spdk_mem or 0
     snode.spdk_image = spdk_image or ""
     snode.spdk_debug = spdk_debug or 0
     snode.write_to_db(kv_store)
 
+    snode.iobuf_small_pool_count = small_pool_count or 0
+    snode.iobuf_large_pool_count = large_pool_count or 0
+    snode.iobuf_small_bufsize = small_bufsize or 0
+    snode.iobuf_large_bufsize = large_bufsize or 0
+
+    snode.write_to_db(kv_store)
+
     # creating RPCClient instance
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password)
 
-    small_pool_count = small_pool_count or 0
-    large_pool_count = large_pool_count or 0
-    small_bufsize = small_bufsize or 0
-    large_bufsize = large_bufsize or 0
-    # set bdev options
-    # rpc_client.bdev_set_options(
-    #     bdev_io_pool_size, bdev_io_cache_size, iobuf_small_cache_size, iobuf_large_cache_size)
+    # 1- set iobuf options
+    if (snode.iobuf_small_pool_count or snode.iobuf_large_pool_count or
+            snode.iobuf_small_bufsize or snode.iobuf_large_bufsize):
+        ret = rpc_client.iobuf_set_options(
+            snode.iobuf_small_pool_count, snode.iobuf_large_pool_count,
+            snode.iobuf_small_bufsize, snode.iobuf_large_bufsize)
+        if not ret:
+            logger.error("Failed to set iobuf options")
+            return False
 
-    rpc_client.iobuf_set_options(
-        small_pool_count, large_pool_count, small_bufsize, large_bufsize)
+    # 2- start spdk framework
+    ret = rpc_client.framework_start_init()
+    if not ret:
+        logger.error("Failed to start framework")
+        return False
 
-    # set nvme bdev options
-    rpc_client.bdev_nvme_set_options()
+    # 3- set nvme bdev options
+    ret = rpc_client.bdev_nvme_set_options()
+    if not ret:
+        logger.error("Failed to set nvme options")
+        return False
 
     # get new node info after starting spdk
     node_info, _ = snode_api.info()
     # adding devices
     nvme_devs = addNvmeDevices(cluster, rpc_client, node_info['spdk_pcie_list'], snode)
     if not nvme_devs:
         logger.error("No NVMe devices was found!")
@@ -468,23 +531,27 @@
                 dev_dict['nvme_bdev'] = pt
                 dev_dict['size'] = int(dev.size / dev_split)
                 new_devices.append(NVMeDevice(dev_dict))
         snode.nvme_devices = new_devices
     else:
         snode.nvme_devices = nvme_devs
 
+    jm_index = 0
     # Set device cluster order
     dev_order = get_next_cluster_device_order(db_controller)
     for index, nvme in enumerate(snode.nvme_devices):
         nvme.cluster_device_order = dev_order
         dev_order += 1
+        if jm_device_pcie and nvme.pcie_address == jm_device_pcie:
+            jm_index = index
         device_events.device_create(nvme)
 
     # create jm
-    snode.nvme_devices[0].jm_bdev = f"jm_{snode.get_id()}"
+    logger.info(f"Using device for JM: {snode.nvme_devices[jm_index].get_id()}")
+    snode.nvme_devices[jm_index].jm_bdev = f"jm_{snode.get_id()}"
 
     # save object
     snode.write_to_db(db_controller.kv_store)
 
     # prepare devices
     ret = _prepare_cluster_devices(snode)
     if not ret:
@@ -524,33 +591,24 @@
             if idx >= 0:
                 node.remote_devices[idx] = dev
             else:
                 node.remote_devices.append(dev)
             count += 1
         node.write_to_db(kv_store)
         logger.info(f"connected to devices count: {count}")
+        time.sleep(3)
 
     logger.info("Sending cluster map")
-    snodes = db_controller.get_storage_nodes()
-    for node in snodes:
-        if node.status != node.STATUS_ONLINE:
-            continue
-        logger.info(f"Sending to: {node.get_id()}")
-        rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
-        if node.get_id() == snode.get_id():
-            cluster_map_data = distr_controller.get_distr_cluster_map(snodes, node)
-            cluster_map_data['UUID_node_target'] = node.get_id()
-            ret = rpc_client.distr_send_cluster_map(cluster_map_data)
-        else:
-            cluster_map_data = distr_controller.get_distr_cluster_map([snode], node)
-            cl_map = {
-                "map_cluster": cluster_map_data['map_cluster'],
-                "map_prob": cluster_map_data['map_prob']}
-            ret = rpc_client.distr_add_nodes(cl_map)
-        time.sleep(3)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
+    ret = distr_controller.send_cluster_map_add_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map add node"
+    time.sleep(3)
 
     logger.info("Sending cluster event updates")
     distr_controller.send_node_status_event(snode.get_id(), "online")
 
     for dev in snode.nvme_devices:
         distr_controller.send_dev_status_event(dev.cluster_device_order, "online")
 
@@ -671,42 +729,53 @@
             else:
                 node.remote_devices.append(dev)
             count += 1
         node.write_to_db(kv_store)
         logger.info(f"connected to devices count: {count}")
 
     logger.info("Sending cluster map")
-    snodes = db_controller.get_storage_nodes()
-    for node in snodes:
-        if node.status != node.STATUS_ONLINE:
-            continue
-        logger.info(f"Sending to: {node.get_id()}")
-        rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
-        if node.get_id() == snode.get_id():
-            cluster_map_data = distr_controller.get_distr_cluster_map(snodes, node)
-            cluster_map_data['UUID_node_target'] = node.get_id()
-            ret = rpc_client.distr_send_cluster_map(cluster_map_data)
-        else:
-            cluster_map_data = distr_controller.get_distr_cluster_map([snode], node)
-            cl_map = {
-                "map_cluster": cluster_map_data['map_cluster'],
-                "map_prob": cluster_map_data['map_prob']}
-            ret = rpc_client.distr_add_nodes(cl_map)
-        time.sleep(3)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
+    ret = distr_controller.send_cluster_map_add_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map add node"
+    time.sleep(3)
 
     logger.info("Sending cluster event updates")
     distr_controller.send_node_status_event(snode.get_id(), "online")
 
     for dev in snode.nvme_devices:
         distr_controller.send_dev_status_event(dev.cluster_device_order, "online")
 
     logger.info("Done")
     return "Success"
 
 
+def delete_storage_node(node_id):
+    db_controller = DBController()
+    snode = db_controller.get_storage_node_by_id(node_id)
+    if not snode:
+        logger.error(f"Can not find storage node: {node_id}")
+        return False
+
+    if snode.status != StorageNode.STATUS_REMOVED:
+        logger.error(f"Node must be in removed status")
+        return False
+
+    snode.remove(db_controller.kv_store)
+
+    for lvol in db_controller.get_lvols():
+        logger.info(f"Sending cluster map to LVol: {lvol.get_id()}")
+        lvol_controller.send_cluster_map(lvol.get_id())
+
+    storage_events.snode_delete(snode)
+    logger.info("done")
+
+
 def remove_storage_node(node_id, force_remove=False, force_migrate=False):
     db_controller = DBController()
     snode = db_controller.get_storage_node_by_id(node_id)
     if not snode:
         logger.error(f"Can not find storage node: {node_id}")
         return False
 
@@ -740,20 +809,22 @@
                 snapshot_controller.delete(sn.get_id())
         else:
             logger.error("Snapshots found on the storage node, use --force-remove or --force-migrate")
             return False
 
     if snode.nvme_devices:
         for dev in snode.nvme_devices:
+            if dev.status == NVMeDevice.STATUS_JM:
+                continue
             if dev.status == 'online':
-                distr_controller.send_dev_status_event(dev.cluster_device_order, "unavailable")
-            distr_controller.disconnect_device(dev)
-
-    for lvol in db_controller.get_lvols():
-        lvol_controller.send_cluster_map(lvol.get_id())
+                distr_controller.disconnect_device(dev)
+            old_status = dev.status
+            dev.status = NVMeDevice.STATUS_FAILED
+            distr_controller.send_dev_status_event(dev.cluster_device_order, NVMeDevice.STATUS_FAILED)
+            device_events.device_status_change(dev, NVMeDevice.STATUS_FAILED, old_status)
 
     logger.info("Removing storage node")
 
     logger.debug("Leaving swarm...")
     try:
         node_docker = docker.DockerClient(base_url=f"tcp://{snode.mgmt_ip}:2375", version="auto")
         cluster_docker = utils.get_docker_client(snode.cluster_id)
@@ -764,16 +835,20 @@
     try:
         snode_api = SNodeClient(snode.api_endpoint)
         snode_api.spdk_process_kill()
         snode_api.leave_swarm()
     except Exception as e:
         logger.warning(f"Failed to remove SPDK process: {e}")
 
-    snode.remove(db_controller.kv_store)
-    storage_events.snode_remove(snode)
+    old_status = snode.status
+    snode.status = StorageNode.STATUS_REMOVED
+    snode.write_to_db(db_controller.kv_store)
+    logger.info("Sending node event update")
+    distr_controller.send_node_status_event(snode.get_id(), snode.status)
+    storage_events.snode_status_change(snode, StorageNode.STATUS_REMOVED, old_status)
     logger.info("done")
 
 
 def restart_storage_node(
         node_id,
         spdk_cpu_mask=None,
         spdk_mem=None,
@@ -793,20 +868,24 @@
         return False
 
     if snode.status == StorageNode.STATUS_ONLINE:
         logger.error(f"Can not restart online node: {node_id}")
         return False
 
     logger.info("Setting node state to restarting")
+    old_status = snode.status
     snode.status = StorageNode.STATUS_RESTARTING
     snode.write_to_db(kv_store)
+    logger.info("Sending node event update")
+    distr_controller.send_node_status_event(snode.get_id(), snode.status)
+    storage_events.snode_status_change(snode, snode.status, old_status)
 
     logger.info(f"Restarting Storage node: {snode.mgmt_ip}")
-    snode_api = SNodeClient(snode.api_endpoint)
 
+    snode_api = SNodeClient(snode.api_endpoint)
     node_info, _ = snode_api.info()
     logger.info(f"Node info: {node_info}")
 
     logger.info("Restarting SPDK")
     cpu = snode.spdk_cpu_mask
     if spdk_cpu_mask:
         cpu = spdk_cpu_mask
@@ -829,36 +908,54 @@
     results, err = snode_api.spdk_process_start(cpu, mem, img, spdk_debug, cluster_ip)
 
     if not results:
         logger.error(f"Failed to start spdk: {err}")
         return False
     time.sleep(3)
 
+    if small_pool_count:
+        snode.iobuf_small_pool_count = small_pool_count
+    if large_pool_count:
+        snode.iobuf_large_pool_count = large_pool_count
+    if small_bufsize:
+        snode.iobuf_small_bufsize = small_bufsize
+    if large_bufsize:
+        snode.iobuf_large_bufsize = large_bufsize
+
     snode.write_to_db(db_controller.kv_store)
 
-    cluster = db_controller.get_cluster_by_id(snode.cluster_id)
     # creating RPCClient instance
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password,
         timeout=10 * 60, retry=5)
 
-    small_pool_count = small_pool_count or 0
-    large_pool_count = large_pool_count or 0
-    small_bufsize = small_bufsize or 0
-    large_bufsize = large_bufsize or 0
-    # set bdev options
-    # rpc_client.bdev_set_options(
-    #     bdev_io_pool_size, bdev_io_cache_size, iobuf_small_cache_size, iobuf_large_cache_size)
-    rpc_client.iobuf_set_options(
-        small_pool_count, large_pool_count, small_bufsize, large_bufsize)
+    # 1- set iobuf options
+    if (snode.iobuf_small_pool_count or snode.iobuf_large_pool_count or
+            snode.iobuf_small_bufsize or snode.iobuf_large_bufsize):
+        ret = rpc_client.iobuf_set_options(
+            snode.iobuf_small_pool_count, snode.iobuf_large_pool_count,
+            snode.iobuf_small_bufsize, snode.iobuf_large_bufsize)
+        if not ret:
+            logger.error("Failed to set iobuf options")
+            return False
 
-    # set nvme bdev options
-    rpc_client.bdev_nvme_set_options()
+    # 2- start spdk framework
+    ret = rpc_client.framework_start_init()
+    if not ret:
+        logger.error("Failed to start framework")
+        return False
+
+    # 3- set nvme bdev options
+    ret = rpc_client.bdev_nvme_set_options()
+    if not ret:
+        logger.error("Failed to set nvme options")
+        return False
 
+    cluster = db_controller.get_cluster_by_id(snode.cluster_id)
     node_info, _ = snode_api.info()
     nvme_devs = addNvmeDevices(cluster, rpc_client, node_info['spdk_pcie_list'], snode)
     if not nvme_devs:
         logger.error("No NVMe devices was found!")
         return False
 
     logger.info(f"Devices found: {len(nvme_devs)}")
@@ -870,18 +967,18 @@
     new_devices = []
     active_devices = []
     known_devices_sn = []
     devices_sn = [d.serial_number for d in nvme_devs]
     for db_dev in snode.nvme_devices:
         known_devices_sn.append(db_dev.serial_number)
         if db_dev.serial_number in devices_sn:
-            logger.info(f"Device found: {db_dev.get_id()}")
-            active_devices.append(db_dev)
-            if db_dev.status == NVMeDevice.STATUS_UNAVAILABLE:
+            logger.info(f"Device found: {db_dev.get_id()}, status {db_dev.status}")
+            if db_dev.status != NVMeDevice.STATUS_JM:
                 db_dev.status = NVMeDevice.STATUS_ONLINE
+            active_devices.append(db_dev)
         else:
             logger.info(f"Device not found: {db_dev.get_id()}")
             db_dev.status = NVMeDevice.STATUS_REMOVED
             distr_controller.send_dev_status_event(db_dev.cluster_device_order, "offline")
 
     for dev in nvme_devs:
         if dev.serial_number not in known_devices_sn:
@@ -932,59 +1029,47 @@
             if idx >= 0:
                 node.remote_devices[idx] = dev
             else:
                 node.remote_devices.append(dev)
             count += 1
         node.write_to_db(kv_store)
         logger.info(f"connected to devices count: {count}")
-
-    logger.info("Sending cluster map")
-    snodes = db_controller.get_storage_nodes()
-    for node in snodes:
-        if node.status != node.STATUS_ONLINE:
-            continue
-        logger.info(f"Sending to: {node.get_id()}")
-        rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
-        if node.get_id() == snode.get_id():
-            cluster_map_data = distr_controller.get_distr_cluster_map(snodes, node)
-            cluster_map_data['UUID_node_target'] = node.get_id()
-            ret = rpc_client.distr_send_cluster_map(cluster_map_data)
-        else:
-            cluster_map_data = distr_controller.get_distr_cluster_map([snode], node)
-            cl_map = {
-                "map_cluster": cluster_map_data['map_cluster'],
-                "map_prob": cluster_map_data['map_prob']}
-            ret = rpc_client.distr_add_nodes(cl_map)
         time.sleep(3)
 
+    logger.info("Setting node status to Online")
+    old_status = snode.status
+    snode.status = StorageNode.STATUS_ONLINE
+    snode.write_to_db(kv_store)
+    storage_events.snode_status_change(snode, snode.status, old_status)
+
     logger.info("Sending node event update")
-    distr_controller.send_node_status_event(snode.get_id(), "online")
+    distr_controller.send_node_status_event(snode.get_id(), NVMeDevice.STATUS_ONLINE)
 
     logger.info("Sending devices event updates")
     for dev in snode.nvme_devices:
-        if dev.status != "online":
+        if dev.status != NVMeDevice.STATUS_ONLINE:
             logger.debug(f"Device is not online: {dev.get_id()}, status: {dev.status}")
             continue
-        distr_controller.send_dev_status_event(dev.cluster_device_order, "online")
+        distr_controller.send_dev_status_event(dev.cluster_device_order, NVMeDevice.STATUS_ONLINE)
+
+    logger.info("Sending cluster map to current node")
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
+    time.sleep(3)
 
     for lvol_id in snode.lvols:
         lvol = lvol_controller.recreate_lvol(lvol_id, snode)
         if not lvol:
             logger.error(f"Failed to create LVol: {lvol_id}")
             return False
         lvol.status = lvol.STATUS_ONLINE
         lvol.io_error = False
         lvol.write_to_db(db_controller.kv_store)
 
-    logger.info("Setting node status to Online")
-    old_status = snode.status
-    snode.status = StorageNode.STATUS_ONLINE
-    snode.write_to_db(kv_store)
-
-    storage_events.snode_status_change(snode, snode.status, old_status)
     logger.info("Done")
     return "Success"
 
 
 def list_storage_nodes(kv_store, is_json):
     db_controller = DBController(kv_store)
     nodes = db_controller.get_storage_nodes()
@@ -1000,21 +1085,25 @@
             if dev.status == NVMeDevice.STATUS_ONLINE:
                 online_devices += 1
         data.append({
             "UUID": node.uuid,
             "Hostname": node.hostname,
             "Management IP": node.mgmt_ip,
             "Devices": f"{total_devices}/{online_devices}",
-            "LVOLs": f"{len(node.lvols)}",
-            "Data NICs": "\n".join([d.if_name for d in node.data_nics]),
+            "LVols": f"{len(node.lvols)}",
+            # "Data NICs": "\n".join([d.if_name for d in node.data_nics]),
             "Status": node.status,
             "Health": node.health_check,
 
-            "Updated At": datetime.datetime.strptime(node.updated_at, "%Y-%m-%d %H:%M:%S.%f").strftime(
-                "%H:%M:%S, %d/%m/%Y"),
+            "EC2 ID": node.ec2_instance_id,
+            "EC2 Type": node.ec2_metadata['instanceType'] if node.ec2_metadata else "",
+            "EC2 Ext IP": node.ec2_public_ip,
+
+            # "Updated At": datetime.datetime.strptime(node.updated_at, "%Y-%m-%d %H:%M:%S.%f").strftime(
+            #     "%H:%M:%S, %d/%m/%Y"),
         })
 
     if not data:
         return output
 
     if is_json:
         output = json.dumps(data, indent=2)
@@ -1101,18 +1190,18 @@
     for lvol_id in snode.lvols:
         logger.debug(lvol_id)
         lvol = db_controller.get_lvol_by_id(lvol_id)
         if lvol:
             lvol.status = lvol.STATUS_OFFLINE
             lvol.write_to_db(db_controller.kv_store)
 
-    distr_controller.send_node_status_event(snode.get_id(), "in_shutdown")
     for dev in snode.nvme_devices:
-        if dev.status == NVMeDevice.STATUS_ONLINE:
+        if dev.status in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_READONLY]:
             device_controller.device_set_unavailable(dev.get_id())
+    distr_controller.send_node_status_event(snode.get_id(), "in_shutdown")
 
     # shutdown node
     # make other nodes disconnect from this node
     logger.info("disconnect all other nodes connections to this node")
     for dev in snode.nvme_devices:
         distr_controller.disconnect_device(dev)
 
@@ -1534,22 +1623,27 @@
     return utils.print_table(out)
 
 
 def deploy(ifname):
     if not ifname:
         ifname = "eth0"
 
-    logger.info("Installing dependencies...")
-    ret = scripts.install_deps()
-
     dev_ip = utils.get_iface_ip(ifname)
     if not dev_ip:
         logger.error(f"Error getting interface ip: {ifname}")
         return False
 
+    logger.info("NVMe SSD devices found on node:")
+    stream = os.popen("lspci -Dnn | grep -i nvme")
+    for l in stream.readlines():
+        logger.info(l.strip())
+
+    logger.info("Installing dependencies...")
+    ret = scripts.install_deps()
+
     logger.info(f"Node IP: {dev_ip}")
     ret = scripts.configure_docker(dev_ip)
 
     node_docker = docker.DockerClient(base_url=f"tcp://{dev_ip}:2375", version="auto", timeout=60 * 5)
     # create the api container
     nodes = node_docker.containers.list(all=True)
     for node in nodes:
@@ -1753,8 +1847,8 @@
 
     snode = db_controller.get_storage_node_by_id(node_id)
     if not snode:
         logger.error(f"Can not find storage node: {node_id}")
         return False
 
     data = snode.get_clean_dict()
-    return json.dumps(data, indent=2)
+    return json.dumps(data, indent=2)
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/cluster_ops.py` & `sbcli_mig-1.0.90/simplyblock_core/cluster_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 import math
 import os
 import time
 import uuid
 
 import docker
 import requests
+import boto3
 
 from simplyblock_core import utils, scripts, constants, mgmt_node_ops, storage_node_ops, shell_utils
 from simplyblock_core.controllers import cluster_events, device_controller
 from simplyblock_core.kv_store import DBController
 from simplyblock_core.models.cluster import Cluster
 from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.models.storage_node import StorageNode
 
 logger = logging.getLogger()
-
+ec2 = boto3.resource('ec2')
 
 def _add_graylog_input(cluster_ip, password):
     url = f"http://{cluster_ip}:9000/api/system/inputs"
     payload = json.dumps({
         "title": "spdk log input",
         "type": "org.graylog2.inputs.gelf.udp.GELFUDPInput",
         "configuration": {
@@ -41,43 +42,17 @@
     }
     session = requests.session()
     session.auth = ("admin", password)
     response = session.request("POST", url, headers=headers, data=payload)
     logger.debug(response.text)
     return response.status_code == 201
 
-def _add_graylog_input_tcp(cluster_ip, password):
-    url = f"http://{cluster_ip}:9000/api/system/inputs"
-    payload = json.dumps({
-        "title": "spdk log input",
-        "type": "org.graylog2.inputs.gelf.tcp.GELFTCPInput",
-        "configuration": {
-            "bind_address": "0.0.0.0",
-            "port": 12201,
-            "recv_buffer_size": 262144,
-            "number_worker_threads": 2,
-            "override_source": None,
-            "charset_name": "UTF-8",
-            "decompress_size_limit": 8388608
-        },
-        "global": True
-    })
-    headers = {
-        'X-Requested-By': '',
-        'Content-Type': 'application/json',
-    }
-    session = requests.session()
-    session.auth = ("admin", password)
-    response = session.request("POST", url, headers=headers, data=payload)
-    logger.debug(response.text)
-    return response.status_code == 201
-
 def create_cluster(blk_size, page_size_in_blocks, ha_type, tls,
                    auth_hosts_only, cli_pass, model_ids,
-                   cap_warn, cap_crit, prov_cap_warn, prov_cap_crit, ifname):
+                   cap_warn, cap_crit, prov_cap_warn, prov_cap_crit, ifname, log_del_interval, metrics_retention_period):
     logger.info("Installing dependencies...")
     ret = scripts.install_deps()
     logger.info("Installing dependencies > Done")
 
     if not ifname:
         ifname = "eth0"
 
@@ -129,23 +104,22 @@
         c.cap_crit = cap_crit
     if prov_cap_warn and prov_cap_warn > 0:
         c.prov_cap_warn = prov_cap_warn
     if prov_cap_crit and prov_cap_crit > 0:
         c.prov_cap_crit = prov_cap_crit
 
     logger.info("Deploying swarm stack ...")
-    ret = scripts.deploy_stack(cli_pass, DEV_IP, constants.SIMPLY_BLOCK_DOCKER_IMAGE, c.secret, c.uuid)
+    ret = scripts.deploy_stack(cli_pass, DEV_IP, constants.SIMPLY_BLOCK_DOCKER_IMAGE, c.secret, c.uuid, log_del_interval, metrics_retention_period)
     logger.info("Deploying swarm stack > Done")
 
     logger.info("Configuring DB...")
     out = scripts.set_db_config_single()
     logger.info("Configuring DB > Done")
 
     _add_graylog_input(DEV_IP, c.secret)
-    _add_graylog_input_tcp(DEV_IP, c.secret)
 
     c.status = Cluster.STATUS_ACTIVE
     if ha_type == 'ha':
         c.status = Cluster.STATUS_SUSPENDED
     c.updated_at = int(time.time())
     c.write_to_db(db_controller.kv_store)
 
@@ -520,15 +494,15 @@
             "mgmt nodes": len(mt),
             "storage nodes": len(st),
             "Status": cl.status,
         })
     return utils.print_table(data)
 
 
-def get_capacity(cluster_id, history, records_count=20, parse_sizes=True):
+def get_capacity(cluster_id, history, records_count=20, is_json=False):
     db_controller = DBController()
     cluster = db_controller.get_cluster_by_id(cluster_id)
     if not cluster:
         logger.error(f"Cluster not found {cluster_id}")
         return False
 
     if history:
@@ -539,16 +513,16 @@
     else:
         records_number = 20
 
     records = db_controller.get_cluster_capacity(cluster, records_number)
 
     new_records = utils.process_records(records, records_count)
 
-    if not parse_sizes:
-        return new_records
+    if is_json:
+        return json.dumps(new_records, indent=2)
 
     out = []
     for record in new_records:
         out.append({
             "Date": time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime(record['date'])),
             "Absolut": utils.humanbytes(record['size_total']),
             "Provisioned": utils.humanbytes(record['size_prov']),
@@ -716,7 +690,49 @@
             storage_node_ops.shutdown_storage_node(node.get_id(), force=True)
             time.sleep(3)
         storage_node_ops.restart_storage_node(node.get_id())
 
     logger.info("Done")
     return True
 
+
+def cluster_grace_startup(cl_id):
+    db_controller = DBController()
+    cluster = db_controller.get_cluster_by_id(cl_id)
+    if not cluster:
+        logger.error(f"Cluster not found {cl_id}")
+        return False
+    unsuspend_cluster(cl_id)
+
+    st = db_controller.get_storage_nodes()
+    for node in st:
+        instance = ec2.Instance(node.ec2_instance_id)
+        response = instance.start()
+        logger.info(f"Starting instance: {node.ec2_instance_id}")
+        logger.info(response)
+        time.sleep(10)
+        storage_node_ops.restart_storage_node(node.get_id())
+        time.sleep(5)
+        get_node = db_controller.get_storage_node_by_id(node.get_id())
+        if get_node.status != StorageNode.STATUS_ONLINE:
+            logger.error("failed to restart node")
+    
+    return True
+
+def cluster_grace_shutdown(cl_id):
+    db_controller = DBController()
+    cluster = db_controller.get_cluster_by_id(cl_id)
+    if not cluster:
+        logger.error(f"Cluster not found {cl_id}")
+        return False
+
+    st = db_controller.get_storage_nodes()
+    for node in st:
+        storage_node_ops.suspend_storage_node(node.get_id())
+        storage_node_ops.shutdown_storage_node(node.get_id())
+        instance = ec2.Instance(node.ec2_instance_id)
+        response = instance.stop()
+        logger.info(f"Stopping instance: {node.ec2_instance_id}")
+        logger.info(response)
+
+    suspend_cluster(cl_id)
+    return True
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/pci_utils.py` & `sbcli_mig-1.0.90/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/distr_controller.py` & `sbcli_mig-1.0.90/simplyblock_core/distr_controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding=utf-8
 import datetime
 import logging
 import re
 
+from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core.kv_store import DBController
 
 logger = logging.getLogger()
 
 
 def send_node_status_event(node_id, node_status):
@@ -41,14 +42,16 @@
     snodes = db_controller.get_storage_nodes()
     for node in snodes:
         if node.status != node.STATUS_ONLINE:
             continue
         logger.info(f"Sending to: {node.get_id()}")
         rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
         ret = rpc_client.distr_status_events_update(events)
+        if not ret:
+            logger.warning("Failed to send event update")
 
 
 def disconnect_device(device):
     db_controller = DBController()
     snodes = db_controller.get_storage_nodes()
     for node in snodes:
         if node.status != node.STATUS_ONLINE:
@@ -65,48 +68,44 @@
         node.write_to_db(db_controller.kv_store)
 
 
 def get_distr_cluster_map(snodes, target_node):
     map_cluster = {}
     map_prob = []
     for snode in snodes:
-        if snode.status not in [snode.STATUS_ONLINE, snode.STATUS_RESTARTING]:
-            logger.debug(f"Node is not online: {snode.get_id()}, status: {snode.status}")
-            continue
         dev_map = {}
         dev_w_map = []
         node_w = 0
-
         for i, dev in enumerate(snode.nvme_devices):
-            if dev.status != "online":
-                logger.debug(f"Device is not online: {dev.get_id()}, status: {dev.status}")
+            logger.debug(f"Device: {dev.get_id()}, status: {dev.status}")
+            if dev.status in [NVMeDevice.STATUS_JM, NVMeDevice.STATUS_NEW]:
                 continue
+
             dev_w = int(dev.size/(1024*1024*1024)) or 1
             node_w += dev_w
             name = None
             if snode.get_id() == target_node.get_id():
                 name = dev.alceml_bdev
             else:
                 for dev2 in target_node.remote_devices:
                     if dev2.get_id() == dev.get_id():
                         name = dev2.remote_bdev
                         break
             if not name:
-                continue
+                name = f"remote_{dev.alceml_bdev}n1"
             dev_map[dev.cluster_device_order] = {
                 "UUID": dev.get_id(),
                 "bdev_name": name,
-                "status": "online"}
+                "status": dev.status}
             dev_w_map.append({
                 "weight": dev_w,
                 "id": dev.cluster_device_order})
         map_cluster[snode.get_id()] = {
-                # "availability_group": 0,
-                "status": "online",
-                "devices": dev_map}
+            "status": snode.status,
+            "devices": dev_map}
         map_prob.append({
             "weight": node_w,
             "items": dev_w_map
         })
     cl_map = {
         "name": "",
         "UUID_node_target": "",
@@ -167,8 +166,43 @@
                 else:
                     data["Results"] = "failed"
                     passed = False
             else:
                 data["Results"] = "not found"
                 passed = False
             results.append(data)
-    return results, passed
+    return results, passed
+
+
+def send_cluster_map_to_node(node):
+    db_controller = DBController()
+    snodes = db_controller.get_storage_nodes()
+    rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
+    cluster_map_data = get_distr_cluster_map(snodes, node)
+    cluster_map_data['UUID_node_target'] = node.get_id()
+    ret = rpc_client.distr_send_cluster_map(cluster_map_data)
+    if not ret:
+        logger.error("Failed to send cluster map")
+        logger.info(cluster_map_data)
+        return False
+    return True
+
+
+def send_cluster_map_add_node(snode):
+    db_controller = DBController()
+    snodes = db_controller.get_storage_nodes()
+    for node in snodes:
+        if node.status != node.STATUS_ONLINE:
+            continue
+        logger.info(f"Sending to: {node.get_id()}")
+        rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
+
+        cluster_map_data = get_distr_cluster_map([snode], node)
+        cl_map = {
+            "map_cluster": cluster_map_data['map_cluster'],
+            "map_prob": cluster_map_data['map_prob']}
+        ret = rpc_client.distr_add_nodes(cl_map)
+        if not ret:
+            logger.error("Failed to send cluster map")
+            logger.info(cl_map)
+            return False
+    return True
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/rpc_client.py` & `sbcli_mig-1.0.90/simplyblock_core/rpc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 import json
 
 import requests
 import logging
 
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
@@ -320,14 +321,15 @@
             "base_bdev_name": base_name,
             "name": name,
             "key_name": key_name,
         }
         return self._request("bdev_crypto_create", params)
 
     def lvol_crypto_key_create(self, name, key, key2):
+        # todo: mask the keys so that they don't show up in logs
         params = {
             "cipher": "AES_XTS",
             "key": key,
             "key2": key2,
             "name": name
         }
         return self._request("accel_crypto_key_create", params)
@@ -504,20 +506,20 @@
         params = {
             "pt_name": name
         }
         return self._request("bdev_passtest_delete", params)
 
     def bdev_nvme_set_options(self):
         params = {
-            "action_on_timeout": "abort",
-            "timeout_us": 25000,
+            "bdev_retry_count": 0,
+            "transport_retry_count": 0,
             "ctrlr_loss_timeout_sec": -1,
-            "reconnect_delay_sec": 15,
-            "transport_retry_count": 1,
-            "bdev_retry_count": 1}
+            "fast_io_fail_timeout_sec": 5,
+            "reconnect_delay_sec": 5,
+        }
         return self._request("bdev_nvme_set_options", params)
 
     def bdev_set_options(self, bdev_io_pool_size, bdev_io_cache_size, iobuf_small_cache_size, iobuf_large_cache_size):
         params = {}
         if bdev_io_pool_size > 0:
             params['bdev_io_pool_size'] = bdev_io_pool_size
         if bdev_io_cache_size > 0:
@@ -638,7 +640,9 @@
         params = {"name": name, "vuid": vuid}
         return self._request("alceml_unmap_vuid", params)
 
     def jm_delete(self):
         params = {"name": 0, "vuid": 0}
         return self._request("jm_delete", params)
 
+    def framework_start_init(self):
+        return self._request("framework_start_init")
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/kv_store.py` & `sbcli_mig-1.0.90/simplyblock_core/kv_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,19 @@
             return ret[0]
 
     def get_lvol_by_id(self, id):
         ret = LVol().read_from_db(self.kv_store, id)
         if ret:
             return ret[0]
 
+    def get_lvol_by_name(self, lvol_name):
+        for lvol in self.get_lvols():
+            if lvol.lvol_name == lvol_name:
+                return lvol
+
     def get_mgmt_node_by_id(self, id):
         ret = MgmtNode().read_from_db(self.kv_store, id)
         if ret:
             return ret[0]
 
     def get_mgmt_nodes(self, cluster_id=None):
         return MgmtNode().read_from_db(self.kv_store)
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/compute_node_ops.py` & `sbcli_mig-1.0.90/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/scripts/haproxy.cfg` & `sbcli_mig-1.0.90/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/scripts/__init__.py` & `sbcli_mig-1.0.90/simplyblock_core/scripts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,18 +26,18 @@
     return __run_script(['bash', '-x', os.path.join(DIR_PATH, 'install_deps.sh')])
 
 
 def configure_docker(docker_ip):
     return __run_script(['bash', '-x', os.path.join(DIR_PATH, 'config_docker.sh'), docker_ip])
 
 
-def deploy_stack(cli_pass, dev_ip, image_name, graylog_password, cluster_id):
+def deploy_stack(cli_pass, dev_ip, image_name, graylog_password, cluster_id, log_del_interval, metrics_retention_period):
     pass_hash = hashlib.sha256(graylog_password.encode('utf-8')).hexdigest()
     return __run_script(
-        ['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'deploy_stack.sh'), cli_pass, dev_ip, image_name, pass_hash, graylog_password, cluster_id])
+        ['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'deploy_stack.sh'), cli_pass, dev_ip, image_name, pass_hash, graylog_password, cluster_id, log_del_interval, metrics_retention_period])
 
 def apply_dashboard(grafanaPassword):
     return __run_script(
         ['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'apply_dashboard.sh'), grafanaPassword])
 
 
 def deploy_cleaner():
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/scripts/install_deps.sh` & `sbcli_mig-1.0.90/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_mig-1.0.90/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_mig-1.0.90/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Grafana username
 GF_ADMIN_USER=admin
 
 HOST=0.0.0.0:3000
 
 DASHBOARDS="${TD}/dashboards"
-for dashboard in "${DASHBOARDS}/cluster.json" "${DASHBOARDS}/devices.json" "${DASHBOARDS}/nodes.json" "${DASHBOARDS}/lvols.json"; do
+for dashboard in "${DASHBOARDS}/cluster.json" "${DASHBOARDS}/devices.json" "${DASHBOARDS}/nodes.json" "${DASHBOARDS}/lvols.json" "${DASHBOARDS}/pools.json" "${DASHBOARDS}/node-exporter.json"; do
     echo -e "\nUploading dashboard: ${dashboard}"
     curl -X POST -H "Content-Type: application/json" \
         -d "@${dashboard}" \
         "http://${GF_ADMIN_USER}:${grafanaPassword}@${HOST}/api/dashboards/import"
     echo ""
 done
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_mig-1.0.90/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 policies:
   - orgId: 1
     receiver: grafana-alerts
     group_by: ['grafana_folder', 'alertname']
     routes:
       - receiver: grafana-alerts
         object_matchers:
-          - ['app', '=', 'demo-app']
+          - ['app', '=', 'simplyblock']
 
 contactPoints:
   - orgId: 1
     name: grafana-alerts
     receivers:
       - uid: grafana
         type: slack
         settings:
           username: grafana_bot
-          url: 'https://hooks.slack.com/services/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'
+          url: 'https://hooks.slack.com/services/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'
           title: |
             {{ template "slack.title" . }}
           text: |
             {{ template "slack.message" . }}
 
 templates:
   - orgId: 1
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9931880696614583%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}, 'gridPos': "*

 * *                "{'w': 7, 'y': 1}, 'id': 13, 'targets': {0: {'expr': 'lvol_size_total'}}, 'title': "*

 * *                "'lvol_size_total'}, 2: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}, "*

 * *                "'gridPos': {'w': 7, 'x': 7, 'y': 1}, 'id': 10, 'targets': {0: {'expr': "*

 * *                "'lvol_size_free'}}, 'title': 'lvol_size_free'}, 3: {'fieldConfig': {'defaults': "*

 * *                "{'unit': 'decb […]*

```diff
@@ -20,14 +20,27 @@
         "fiscalYearStartMonth": 0,
         "graphTooltip": 0,
         "id": null,
         "links": [],
         "liveNow": false,
         "panels": [
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 0
+                },
+                "id": 31,
+                "panels": [],
+                "title": "Size",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -73,25 +86,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
+                    "w": 7,
                     "x": 0,
-                    "y": 0
+                    "y": 1
                 },
-                "id": 27,
+                "id": 13,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -103,21 +116,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_write_latency_ticks",
+                        "expr": "lvol_size_total",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_write_latency_ticks",
+                "title": "lvol_size_total",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -165,25 +178,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 0
+                    "w": 7,
+                    "x": 7,
+                    "y": 1
                 },
-                "id": 26,
+                "id": 10,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -195,21 +209,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_write_latency_ps",
+                        "expr": "lvol_size_free",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_write_latency_ps",
+                "title": "lvol_size_free",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -257,25 +271,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 0
+                    "w": 7,
+                    "x": 14,
+                    "y": 1
                 },
-                "id": 25,
+                "id": 14,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -287,21 +302,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_write_io_ps",
+                        "expr": "lvol_size_used",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_write_io_ps",
+                "title": "lvol_size_used",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -349,25 +364,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 0
+                    "w": 7,
+                    "x": 0,
+                    "y": 8
                 },
-                "id": 24,
+                "id": 11,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -379,21 +395,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_write_io",
+                        "expr": "lvol_size_prov",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_write_io",
+                "title": "lvol_size_prov",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -442,25 +458,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 0,
-                    "y": 7
+                    "w": 7,
+                    "x": 7,
+                    "y": 8
                 },
-                "id": 23,
+                "id": 12,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -472,21 +488,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_write_bytes_ps",
+                        "expr": "lvol_size_prov_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_write_bytes_ps",
+                "title": "lvol_size_prov_util",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -535,25 +551,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 7
+                    "w": 7,
+                    "x": 14,
+                    "y": 8
                 },
-                "id": 22,
+                "id": 15,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -565,24 +581,37 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_write_bytes",
+                        "expr": "lvol_size_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_write_bytes",
+                "title": "lvol_size_util",
                 "type": "timeseries"
             },
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 15
+                },
+                "id": 28,
+                "panels": [],
+                "title": "Writes",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -627,25 +656,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 7
+                    "h": 8,
+                    "w": 7,
+                    "x": 0,
+                    "y": 16
                 },
-                "id": 21,
+                "id": 22,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -657,29 +687,28 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_unmap_latency_ticks",
+                        "expr": "lvol_write_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_latency_ticks",
+                "title": "lvol_write_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
-                "description": "",
                 "fieldConfig": {
                     "defaults": {
                         "color": {
                             "mode": "palette-classic"
                         },
                         "custom": {
                             "axisCenteredZero": false,
@@ -725,20 +754,20 @@
                                 }
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 7
+                    "h": 8,
+                    "w": 7,
+                    "x": 7,
+                    "y": 16
                 },
-                "id": 20,
+                "id": 25,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -750,21 +779,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_unmap_latency_ps",
+                        "expr": "lvol_write_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_latency_ps",
+                "title": "write_iops",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -814,48 +843,23 @@
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         }
                     },
-                    "overrides": [
-                        {
-                            "__systemRef": "hideSeriesFrom",
-                            "matcher": {
-                                "id": "byNames",
-                                "options": {
-                                    "mode": "exclude",
-                                    "names": [
-                                        "{__name__=\"lvol_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
-                                    ],
-                                    "prefix": "All except:",
-                                    "readOnly": true
-                                }
-                            },
-                            "properties": [
-                                {
-                                    "id": "custom.hideFrom",
-                                    "value": {
-                                        "legend": false,
-                                        "tooltip": false,
-                                        "viz": true
-                                    }
-                                }
-                            ]
-                        }
-                    ]
+                    "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 0,
-                    "y": 14
+                    "h": 8,
+                    "w": 7,
+                    "x": 14,
+                    "y": 16
                 },
-                "id": 19,
+                "id": 33,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -867,21 +871,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_unmap_io_ps",
+                        "expr": "lvol_write_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_io_ps",
+                "title": "lvol_wite_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -934,20 +938,20 @@
                                 }
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 14
+                    "h": 8,
+                    "w": 7,
+                    "x": 0,
+                    "y": 24
                 },
-                "id": 18,
+                "id": 24,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -959,21 +963,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_unmap_io",
+                        "expr": "lvol_write_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_io",
+                "title": "lvol_write_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1022,25 +1026,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 14
+                    "h": 8,
+                    "w": 7,
+                    "x": 7,
+                    "y": 24
                 },
-                "id": 17,
+                "id": 23,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1052,21 +1056,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_unmap_bytes_ps",
+                        "expr": "lvol_write_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_bytes_ps",
+                "title": "write_speed",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1115,25 +1119,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "ns"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 14
+                    "h": 8,
+                    "w": 7,
+                    "x": 14,
+                    "y": 24
                 },
-                "id": 16,
+                "id": 26,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1145,24 +1149,37 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_unmap_bytes",
+                        "expr": "lvol_write_latency_ps / 1000",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_bytes",
+                "title": "lvol_write_latency_ps",
                 "type": "timeseries"
             },
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 32
+                },
+                "id": 30,
+                "panels": [],
+                "title": "Reads",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -1208,25 +1225,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
+                    "h": 8,
+                    "w": 7,
                     "x": 0,
-                    "y": 21
+                    "y": 33
                 },
-                "id": 15,
+                "id": 1,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1238,21 +1255,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_size_util",
+                        "expr": "lvol_read_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_util",
+                "title": "lvol_read_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1301,25 +1318,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 21
+                    "h": 8,
+                    "w": 7,
+                    "x": 7,
+                    "y": 33
                 },
-                "id": 14,
+                "id": 2,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1331,21 +1348,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_size_used",
+                        "expr": "lvol_read_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_used",
+                "title": "read_speed",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1393,26 +1410,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 21
+                    "h": 8,
+                    "w": 7,
+                    "x": 14,
+                    "y": 33
                 },
-                "id": 13,
+                "id": 5,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1424,21 +1440,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_size_total",
+                        "expr": "lvol_read_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_total",
+                "title": "lvol_read_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1486,26 +1502,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 21
+                    "w": 7,
+                    "x": 0,
+                    "y": 41
                 },
-                "id": 12,
+                "id": 3,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1517,21 +1532,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_size_prov_util",
+                        "expr": "lvol_read_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_prov_util",
+                "title": "lvol_read_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1579,26 +1594,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 0,
-                    "y": 28
+                    "w": 7,
+                    "x": 7,
+                    "y": 41
                 },
-                "id": 11,
+                "id": 4,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1610,21 +1624,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_size_prov",
+                        "expr": "lvol_read_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_prov",
+                "title": "read_iops",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1672,26 +1686,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 28
+                    "w": 7,
+                    "x": 14,
+                    "y": 41
                 },
-                "id": 10,
+                "id": 6,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1703,24 +1716,37 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_size_free",
+                        "expr": "lvol_read_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_free",
+                "title": "lvol_read_latency_ticks",
                 "type": "timeseries"
             },
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 48
+                },
+                "id": 29,
+                "panels": [],
+                "title": "unmap",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -1765,26 +1791,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 28
+                    "w": 7,
+                    "x": 0,
+                    "y": 49
                 },
-                "id": 9,
+                "id": 21,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1796,21 +1821,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_record_start_time",
+                        "expr": "lvol_unmap_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_record_start_time",
+                "title": "lvol_unmap_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1858,25 +1883,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 28
+                    "w": 7,
+                    "x": 7,
+                    "y": 49
                 },
-                "id": 8,
+                "id": 17,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1888,21 +1914,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_record_end_time",
+                        "expr": "lvol_unmap_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_record_end_time",
+                "title": "lvol_unmap_bytes_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1957,19 +1983,19 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 0,
-                    "y": 35
+                    "w": 7,
+                    "x": 14,
+                    "y": 49
                 },
-                "id": 7,
+                "id": 20,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1981,21 +2007,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_record_duration",
+                        "expr": "lvol_unmap_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_record_duration",
+                "title": "lvol_unmap_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2045,23 +2071,48 @@
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         }
                     },
-                    "overrides": []
+                    "overrides": [
+                        {
+                            "__systemRef": "hideSeriesFrom",
+                            "matcher": {
+                                "id": "byNames",
+                                "options": {
+                                    "mode": "exclude",
+                                    "names": [
+                                        "{__name__=\"lvol_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
+                                    ],
+                                    "prefix": "All except:",
+                                    "readOnly": true
+                                }
+                            },
+                            "properties": [
+                                {
+                                    "id": "custom.hideFrom",
+                                    "value": {
+                                        "legend": false,
+                                        "tooltip": false,
+                                        "viz": true
+                                    }
+                                }
+                            ]
+                        }
+                    ]
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 35
+                    "w": 7,
+                    "x": 0,
+                    "y": 56
                 },
-                "id": 6,
+                "id": 19,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2073,21 +2124,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_read_latency_ticks",
+                        "expr": "lvol_unmap_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_read_latency_ticks",
+                "title": "lvol_unmap_io_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2141,19 +2192,19 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 35
+                    "w": 7,
+                    "x": 7,
+                    "y": 56
                 },
-                "id": 5,
+                "id": 18,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2165,21 +2216,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_read_latency_ps",
+                        "expr": "lvol_unmap_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_read_latency_ps",
+                "title": "lvol_unmap_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2227,25 +2278,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 35
+                    "w": 7,
+                    "x": 14,
+                    "y": 56
                 },
-                "id": 4,
+                "id": 16,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2257,24 +2309,37 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_read_io_ps",
+                        "expr": "lvol_unmap_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_read_io_ps",
+                "title": "lvol_unmap_bytes",
                 "type": "timeseries"
             },
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 63
+                },
+                "id": 32,
+                "panels": [],
+                "title": "others",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -2325,19 +2390,19 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
+                    "w": 7,
                     "x": 0,
-                    "y": 42
+                    "y": 64
                 },
-                "id": 3,
+                "id": 8,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2349,28 +2414,29 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_read_io",
+                        "expr": "lvol_record_end_time",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_read_io",
+                "title": "lvol_record_end_time",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
+                "description": "",
                 "fieldConfig": {
                     "defaults": {
                         "color": {
                             "mode": "palette-classic"
                         },
                         "custom": {
                             "axisCenteredZero": false,
@@ -2411,26 +2477,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 42
+                    "w": 7,
+                    "x": 7,
+                    "y": 64
                 },
-                "id": 1,
+                "id": 7,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2442,21 +2507,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_read_bytes",
+                        "expr": "lvol_record_duration",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_read_bytes",
+                "title": "lvol_record_duration",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2505,25 +2570,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
-                    "x": 12,
-                    "y": 42
+                    "x": 14,
+                    "y": 64
                 },
-                "id": 2,
+                "id": 9,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2535,33 +2600,33 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_read_bytes_ps",
+                        "expr": "lvol_record_start_time",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_read_bytes_ps",
+                "title": "lvol_record_start_time",
                 "type": "timeseries"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
         "templating": {
             "list": []
         },
         "time": {
-            "from": "now-6h",
+            "from": "now-1h",
             "to": "now"
         },
         "timepicker": {},
         "timezone": "",
         "title": "LvolsDashboard",
         "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e19",
         "version": 5,
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files 4% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9932025146484376%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}, 'gridPos': "*

 * *                "{'w': 7, 'y': 1}, 'id': 13, 'targets': {0: {'expr': 'cluster_size_total'}}, "*

 * *                "'title': 'cluster_size_total'}, 2: {'fieldConfig': {'defaults': {'unit': "*

 * *                "'decbytes'}}, 'gridPos': {'w': 7, 'x': 7, 'y': 1}, 'id': 10, 'targets': {0: "*

 * *                "{'expr': 'cluster_size_free'}}, 'title': 'cluster_size_free'}, 3: {'fieldConfig': "*

 * *                "{'defaults': {' […]*

```diff
@@ -20,14 +20,27 @@
         "fiscalYearStartMonth": 0,
         "graphTooltip": 0,
         "id": null,
         "links": [],
         "liveNow": false,
         "panels": [
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 0
+                },
+                "id": 31,
+                "panels": [],
+                "title": "Size",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -73,25 +86,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
+                    "w": 7,
                     "x": 0,
-                    "y": 0
+                    "y": 1
                 },
-                "id": 27,
+                "id": 13,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -103,21 +116,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_latency_ticks",
+                        "expr": "cluster_size_total",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_write_latency_ticks",
+                "title": "cluster_size_total",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -165,25 +178,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 0
+                    "w": 7,
+                    "x": 7,
+                    "y": 1
                 },
-                "id": 26,
+                "id": 10,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -195,21 +209,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_latency_ps",
+                        "expr": "cluster_size_free",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_write_latency_ps",
+                "title": "cluster_size_free",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -257,25 +271,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 0
+                    "w": 7,
+                    "x": 14,
+                    "y": 1
                 },
-                "id": 25,
+                "id": 14,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -287,21 +302,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_io_ps",
+                        "expr": "cluster_size_used",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_write_io_ps",
+                "title": "cluster_size_used",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -349,25 +364,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 0
+                    "w": 7,
+                    "x": 0,
+                    "y": 8
                 },
-                "id": 24,
+                "id": 11,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -379,21 +395,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_io",
+                        "expr": "cluster_size_prov",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_write_io",
+                "title": "cluster_size_prov",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -442,25 +458,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 0,
-                    "y": 7
+                    "w": 7,
+                    "x": 7,
+                    "y": 8
                 },
-                "id": 23,
+                "id": 12,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -472,21 +488,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_bytes_ps",
+                        "expr": "cluster_size_prov_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_write_bytes_ps",
+                "title": "cluster_size_prov_util",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -535,25 +551,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 7
+                    "w": 7,
+                    "x": 14,
+                    "y": 8
                 },
-                "id": 22,
+                "id": 15,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -565,24 +581,37 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_write_bytes",
+                        "expr": "cluster_size_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_write_bytes",
+                "title": "cluster_size_util",
                 "type": "timeseries"
             },
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 15
+                },
+                "id": 28,
+                "panels": [],
+                "title": "Writes",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -627,25 +656,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 7
+                    "w": 7,
+                    "x": 0,
+                    "y": 16
                 },
-                "id": 21,
+                "id": 22,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -657,29 +687,28 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_latency_ticks",
+                        "expr": "cluster_write_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_unmap_latency_ticks",
+                "title": "cluster_write_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
-                "description": "",
                 "fieldConfig": {
                     "defaults": {
                         "color": {
                             "mode": "palette-classic"
                         },
                         "custom": {
                             "axisCenteredZero": false,
@@ -720,25 +749,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 7
+                    "w": 7,
+                    "x": 7,
+                    "y": 16
                 },
-                "id": 20,
+                "id": 23,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -750,21 +780,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_latency_ps",
+                        "expr": "cluster_write_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_unmap_latency_ps",
+                "title": "write_speed",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -812,50 +842,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "ns"
                     },
-                    "overrides": [
-                        {
-                            "__systemRef": "hideSeriesFrom",
-                            "matcher": {
-                                "id": "byNames",
-                                "options": {
-                                    "mode": "exclude",
-                                    "names": [
-                                        "{__name__=\"cluster_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
-                                    ],
-                                    "prefix": "All except:",
-                                    "readOnly": true
-                                }
-                            },
-                            "properties": [
-                                {
-                                    "id": "custom.hideFrom",
-                                    "value": {
-                                        "legend": false,
-                                        "tooltip": false,
-                                        "viz": true
-                                    }
-                                }
-                            ]
-                        }
-                    ]
+                    "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 0,
-                    "y": 14
+                    "w": 7,
+                    "x": 14,
+                    "y": 16
                 },
-                "id": 19,
+                "id": 26,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -867,21 +873,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_io_ps",
+                        "expr": "cluster_write_latency_ps / 1000",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_unmap_io_ps",
+                "title": "cluster_write_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -935,19 +941,19 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 14
+                    "w": 7,
+                    "x": 0,
+                    "y": 23
                 },
-                "id": 18,
+                "id": 24,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -959,21 +965,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_io",
+                        "expr": "cluster_write_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_unmap_io",
+                "title": "cluster_write_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1021,26 +1027,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 14
+                    "w": 7,
+                    "x": 7,
+                    "y": 23
                 },
-                "id": 17,
+                "id": 25,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1052,21 +1057,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_bytes_ps",
+                        "expr": "cluster_write_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_unmap_bytes_ps",
+                "title": "write_iops",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1114,26 +1119,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 14
+                    "w": 7,
+                    "x": 14,
+                    "y": 23
                 },
-                "id": 16,
+                "id": 33,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1145,24 +1149,37 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_unmap_bytes",
+                        "expr": "cluster_write_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_unmap_bytes",
+                "title": "cluster_wite_latency_ticks",
                 "type": "timeseries"
             },
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 30
+                },
+                "id": 30,
+                "panels": [],
+                "title": "Reads",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -1208,25 +1225,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
+                    "h": 8,
+                    "w": 7,
                     "x": 0,
-                    "y": 21
+                    "y": 31
                 },
-                "id": 15,
+                "id": 1,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1238,21 +1255,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_util",
+                        "expr": "cluster_read_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_size_util",
+                "title": "cluster_read_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1301,25 +1318,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 21
+                    "h": 8,
+                    "w": 7,
+                    "x": 7,
+                    "y": 31
                 },
-                "id": 14,
+                "id": 2,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1331,21 +1348,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_used",
+                        "expr": "cluster_read_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_size_used",
+                "title": "read_speed",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1393,26 +1410,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 21
+                    "h": 8,
+                    "w": 7,
+                    "x": 14,
+                    "y": 31
                 },
-                "id": 13,
+                "id": 5,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1424,21 +1440,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_total",
+                        "expr": "cluster_read_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_size_total",
+                "title": "cluster_read_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1486,26 +1502,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 21
+                    "w": 7,
+                    "x": 0,
+                    "y": 39
                 },
-                "id": 12,
+                "id": 3,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1517,21 +1532,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_prov_util",
+                        "expr": "cluster_read_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_size_prov_util",
+                "title": "cluster_read_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1579,26 +1594,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 0,
-                    "y": 28
+                    "w": 7,
+                    "x": 7,
+                    "y": 39
                 },
-                "id": 11,
+                "id": 4,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1610,21 +1624,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_prov",
+                        "expr": "cluster_read_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_size_prov",
+                "title": "read_iops",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1672,26 +1686,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 28
+                    "w": 7,
+                    "x": 14,
+                    "y": 39
                 },
-                "id": 10,
+                "id": 6,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1703,24 +1716,37 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_size_free",
+                        "expr": "cluster_read_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_size_free",
+                "title": "cluster_read_latency_ticks",
                 "type": "timeseries"
             },
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 46
+                },
+                "id": 29,
+                "panels": [],
+                "title": "unmap",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -1765,26 +1791,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 28
+                    "w": 7,
+                    "x": 0,
+                    "y": 47
                 },
-                "id": 9,
+                "id": 21,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1796,21 +1821,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_record_start_time",
+                        "expr": "cluster_unmap_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_record_start_time",
+                "title": "cluster_unmap_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1858,25 +1883,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 28
+                    "w": 7,
+                    "x": 7,
+                    "y": 47
                 },
-                "id": 8,
+                "id": 17,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1888,21 +1914,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_record_end_time",
+                        "expr": "cluster_unmap_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_record_end_time",
+                "title": "cluster_unmap_bytes_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1957,19 +1983,19 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 0,
-                    "y": 35
+                    "w": 7,
+                    "x": 14,
+                    "y": 47
                 },
-                "id": 7,
+                "id": 20,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1981,21 +2007,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_record_duration",
+                        "expr": "cluster_unmap_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_record_duration",
+                "title": "cluster_unmap_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2045,23 +2071,48 @@
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         }
                     },
-                    "overrides": []
+                    "overrides": [
+                        {
+                            "__systemRef": "hideSeriesFrom",
+                            "matcher": {
+                                "id": "byNames",
+                                "options": {
+                                    "mode": "exclude",
+                                    "names": [
+                                        "{__name__=\"cluster_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
+                                    ],
+                                    "prefix": "All except:",
+                                    "readOnly": true
+                                }
+                            },
+                            "properties": [
+                                {
+                                    "id": "custom.hideFrom",
+                                    "value": {
+                                        "legend": false,
+                                        "tooltip": false,
+                                        "viz": true
+                                    }
+                                }
+                            ]
+                        }
+                    ]
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 35
+                    "w": 7,
+                    "x": 0,
+                    "y": 54
                 },
-                "id": 6,
+                "id": 19,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2073,21 +2124,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_latency_ticks",
+                        "expr": "cluster_unmap_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_read_latency_ticks",
+                "title": "cluster_unmap_io_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2141,19 +2192,19 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 35
+                    "w": 7,
+                    "x": 7,
+                    "y": 54
                 },
-                "id": 5,
+                "id": 18,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2165,21 +2216,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_latency_ps",
+                        "expr": "cluster_unmap_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_read_latency_ps",
+                "title": "cluster_unmap_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2227,25 +2278,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 35
+                    "w": 7,
+                    "x": 14,
+                    "y": 54
                 },
-                "id": 4,
+                "id": 16,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2257,24 +2309,37 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_io_ps",
+                        "expr": "cluster_unmap_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_read_io_ps",
+                "title": "cluster_unmap_bytes",
                 "type": "timeseries"
             },
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 61
+                },
+                "id": 32,
+                "panels": [],
+                "title": "others",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -2325,19 +2390,19 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
+                    "w": 7,
                     "x": 0,
-                    "y": 42
+                    "y": 62
                 },
-                "id": 3,
+                "id": 8,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2349,28 +2414,29 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_io",
+                        "expr": "cluster_record_end_time",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_read_io",
+                "title": "cluster_record_end_time",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
+                "description": "",
                 "fieldConfig": {
                     "defaults": {
                         "color": {
                             "mode": "palette-classic"
                         },
                         "custom": {
                             "axisCenteredZero": false,
@@ -2411,26 +2477,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 42
+                    "w": 7,
+                    "x": 7,
+                    "y": 62
                 },
-                "id": 1,
+                "id": 7,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2442,21 +2507,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_bytes",
+                        "expr": "cluster_record_duration",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_read_bytes",
+                "title": "cluster_record_duration",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2505,25 +2570,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
-                    "x": 12,
-                    "y": 42
+                    "x": 14,
+                    "y": 62
                 },
-                "id": 2,
+                "id": 9,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2535,33 +2600,33 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "cluster_read_bytes_ps",
+                        "expr": "cluster_record_start_time",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "cluster_read_bytes_ps",
+                "title": "cluster_record_start_time",
                 "type": "timeseries"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
         "templating": {
             "list": []
         },
         "time": {
-            "from": "now-6h",
+            "from": "now-1h",
             "to": "now"
         },
         "timepicker": {},
         "timezone": "",
         "title": "ClusterDashboard",
         "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e39",
         "version": 5,
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9931951904296875%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}, 'gridPos': "*

 * *                "{'w': 7, 'y': 1}, 'id': 13, 'targets': {0: {'expr': 'snode_size_total'}}, "*

 * *                "'title': 'snode_size_total'}, 2: {'fieldConfig': {'defaults': {'unit': "*

 * *                "'decbytes'}}, 'gridPos': {'w': 7, 'x': 7, 'y': 1}, 'id': 10, 'targets': {0: "*

 * *                "{'expr': 'snode_size_free'}}, 'title': 'snode_size_free'}, 3: {'fieldConfig': "*

 * *                "{'defaults': {'unit': ' […]*

```diff
@@ -20,14 +20,27 @@
         "fiscalYearStartMonth": 0,
         "graphTooltip": 0,
         "id": null,
         "links": [],
         "liveNow": false,
         "panels": [
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 0
+                },
+                "id": 31,
+                "panels": [],
+                "title": "Size",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -73,25 +86,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
+                    "w": 7,
                     "x": 0,
-                    "y": 0
+                    "y": 1
                 },
-                "id": 27,
+                "id": 13,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -103,21 +116,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_write_latency_ticks",
+                        "expr": "snode_size_total",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_write_latency_ticks",
+                "title": "snode_size_total",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -165,25 +178,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 0
+                    "w": 7,
+                    "x": 7,
+                    "y": 1
                 },
-                "id": 26,
+                "id": 10,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -195,21 +209,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_write_latency_ps",
+                        "expr": "snode_size_free",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_write_latency_ps",
+                "title": "snode_size_free",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -257,25 +271,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 0
+                    "w": 7,
+                    "x": 14,
+                    "y": 1
                 },
-                "id": 25,
+                "id": 14,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -287,21 +302,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_write_io_ps",
+                        "expr": "snode_size_used",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_write_io_ps",
+                "title": "snode_size_used",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -349,25 +364,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 0
+                    "w": 7,
+                    "x": 0,
+                    "y": 8
                 },
-                "id": 24,
+                "id": 11,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -379,21 +395,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_write_io",
+                        "expr": "snode_size_prov",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_write_io",
+                "title": "snode_size_prov",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -442,25 +458,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 0,
-                    "y": 7
+                    "w": 7,
+                    "x": 7,
+                    "y": 8
                 },
-                "id": 23,
+                "id": 12,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -472,21 +488,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_write_bytes_ps",
+                        "expr": "snode_size_prov_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_write_bytes_ps",
+                "title": "snode_size_prov_util",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -535,25 +551,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 7
+                    "w": 7,
+                    "x": 14,
+                    "y": 8
                 },
-                "id": 22,
+                "id": 15,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -565,24 +581,37 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_write_bytes",
+                        "expr": "snode_size_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_write_bytes",
+                "title": "snode_size_util",
                 "type": "timeseries"
             },
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 15
+                },
+                "id": 28,
+                "panels": [],
+                "title": "Writes",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -627,25 +656,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 7
+                    "w": 7,
+                    "x": 0,
+                    "y": 16
                 },
-                "id": 21,
+                "id": 22,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -657,29 +687,28 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_unmap_latency_ticks",
+                        "expr": "snode_write_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_unmap_latency_ticks",
+                "title": "snode_write_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
-                "description": "",
                 "fieldConfig": {
                     "defaults": {
                         "color": {
                             "mode": "palette-classic"
                         },
                         "custom": {
                             "axisCenteredZero": false,
@@ -720,25 +749,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 7
+                    "w": 7,
+                    "x": 7,
+                    "y": 16
                 },
-                "id": 20,
+                "id": 23,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -750,21 +780,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_unmap_latency_ps",
+                        "expr": "snode_write_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_unmap_latency_ps",
+                "title": "write_speed",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -814,48 +844,23 @@
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         }
                     },
-                    "overrides": [
-                        {
-                            "__systemRef": "hideSeriesFrom",
-                            "matcher": {
-                                "id": "byNames",
-                                "options": {
-                                    "mode": "exclude",
-                                    "names": [
-                                        "{__name__=\"snode_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
-                                    ],
-                                    "prefix": "All except:",
-                                    "readOnly": true
-                                }
-                            },
-                            "properties": [
-                                {
-                                    "id": "custom.hideFrom",
-                                    "value": {
-                                        "legend": false,
-                                        "tooltip": false,
-                                        "viz": true
-                                    }
-                                }
-                            ]
-                        }
-                    ]
+                    "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 0,
-                    "y": 14
+                    "w": 7,
+                    "x": 14,
+                    "y": 16
                 },
-                "id": 19,
+                "id": 33,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -867,21 +872,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_unmap_io_ps",
+                        "expr": "snode_write_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_unmap_io_ps",
+                "title": "snode_wite_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -934,20 +939,20 @@
                                 }
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 14
+                    "h": 8,
+                    "w": 7,
+                    "x": 0,
+                    "y": 23
                 },
-                "id": 18,
+                "id": 24,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -959,21 +964,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_unmap_io",
+                        "expr": "snode_write_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_unmap_io",
+                "title": "snode_write_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1021,26 +1026,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 14
+                    "h": 8,
+                    "w": 7,
+                    "x": 7,
+                    "y": 23
                 },
-                "id": 17,
+                "id": 25,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1052,21 +1056,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_unmap_bytes_ps",
+                        "expr": "snode_write_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_unmap_bytes_ps",
+                "title": "write_iops",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1115,25 +1119,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "ns"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 14
+                    "h": 8,
+                    "w": 7,
+                    "x": 14,
+                    "y": 23
                 },
-                "id": 16,
+                "id": 26,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1145,24 +1149,37 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_unmap_bytes",
+                        "expr": "snode_write_latency_ps / 1000",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_unmap_bytes",
+                "title": "snode_write_latency_ps",
                 "type": "timeseries"
             },
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 31
+                },
+                "id": 30,
+                "panels": [],
+                "title": "Reads",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -1208,25 +1225,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
+                    "h": 8,
+                    "w": 7,
                     "x": 0,
-                    "y": 21
+                    "y": 32
                 },
-                "id": 15,
+                "id": 1,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1238,21 +1255,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_size_util",
+                        "expr": "snode_read_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_size_util",
+                "title": "snode_read_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1301,25 +1318,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 21
+                    "h": 8,
+                    "w": 7,
+                    "x": 7,
+                    "y": 32
                 },
-                "id": 14,
+                "id": 2,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1331,21 +1348,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_size_used",
+                        "expr": "snode_read_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_size_used",
+                "title": "read_speed",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1393,26 +1410,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 21
+                    "h": 8,
+                    "w": 7,
+                    "x": 14,
+                    "y": 32
                 },
-                "id": 13,
+                "id": 5,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1424,21 +1440,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_size_total",
+                        "expr": "snode_read_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_size_total",
+                "title": "snode_read_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1486,26 +1502,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 21
+                    "w": 7,
+                    "x": 0,
+                    "y": 40
                 },
-                "id": 12,
+                "id": 3,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1517,21 +1532,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_size_prov_util",
+                        "expr": "snode_read_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_size_prov_util",
+                "title": "snode_read_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1579,26 +1594,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 0,
-                    "y": 28
+                    "w": 7,
+                    "x": 7,
+                    "y": 40
                 },
-                "id": 11,
+                "id": 4,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1610,21 +1624,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_size_prov",
+                        "expr": "snode_read_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_size_prov",
+                "title": "read_iops",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1672,26 +1686,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 28
+                    "w": 7,
+                    "x": 14,
+                    "y": 40
                 },
-                "id": 10,
+                "id": 6,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1703,24 +1716,37 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_size_free",
+                        "expr": "snode_read_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_size_free",
+                "title": "snode_read_latency_ticks",
                 "type": "timeseries"
             },
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 47
+                },
+                "id": 29,
+                "panels": [],
+                "title": "unmap",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -1765,26 +1791,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 28
+                    "w": 7,
+                    "x": 0,
+                    "y": 48
                 },
-                "id": 9,
+                "id": 21,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1796,21 +1821,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_record_start_time",
+                        "expr": "snode_unmap_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_record_start_time",
+                "title": "snode_unmap_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1858,25 +1883,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 28
+                    "w": 7,
+                    "x": 7,
+                    "y": 48
                 },
-                "id": 8,
+                "id": 17,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1888,21 +1914,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_record_end_time",
+                        "expr": "snode_unmap_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_record_end_time",
+                "title": "snode_unmap_bytes_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1957,19 +1983,19 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 0,
-                    "y": 35
+                    "w": 7,
+                    "x": 14,
+                    "y": 48
                 },
-                "id": 7,
+                "id": 20,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1981,21 +2007,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_record_duration",
+                        "expr": "snode_unmap_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_record_duration",
+                "title": "snode_unmap_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2045,23 +2071,48 @@
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         }
                     },
-                    "overrides": []
+                    "overrides": [
+                        {
+                            "__systemRef": "hideSeriesFrom",
+                            "matcher": {
+                                "id": "byNames",
+                                "options": {
+                                    "mode": "exclude",
+                                    "names": [
+                                        "{__name__=\"snode_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
+                                    ],
+                                    "prefix": "All except:",
+                                    "readOnly": true
+                                }
+                            },
+                            "properties": [
+                                {
+                                    "id": "custom.hideFrom",
+                                    "value": {
+                                        "legend": false,
+                                        "tooltip": false,
+                                        "viz": true
+                                    }
+                                }
+                            ]
+                        }
+                    ]
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 35
+                    "w": 7,
+                    "x": 0,
+                    "y": 55
                 },
-                "id": 6,
+                "id": 19,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2073,21 +2124,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_read_latency_ticks",
+                        "expr": "snode_unmap_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_read_latency_ticks",
+                "title": "snode_unmap_io_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2141,19 +2192,19 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 35
+                    "w": 7,
+                    "x": 7,
+                    "y": 55
                 },
-                "id": 5,
+                "id": 18,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2165,21 +2216,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_read_latency_ps",
+                        "expr": "snode_unmap_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_read_latency_ps",
+                "title": "snode_unmap_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2227,25 +2278,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 35
+                    "w": 7,
+                    "x": 14,
+                    "y": 55
                 },
-                "id": 4,
+                "id": 16,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2257,24 +2309,37 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_read_io_ps",
+                        "expr": "snode_unmap_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_read_io_ps",
+                "title": "snode_unmap_bytes",
                 "type": "timeseries"
             },
             {
+                "collapsed": false,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 62
+                },
+                "id": 32,
+                "panels": [],
+                "title": "others",
+                "type": "row"
+            },
+            {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
                     "defaults": {
                         "color": {
@@ -2325,19 +2390,19 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
+                    "w": 7,
                     "x": 0,
-                    "y": 42
+                    "y": 63
                 },
-                "id": 3,
+                "id": 8,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2349,28 +2414,29 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_read_io",
+                        "expr": "snode_record_end_time",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_read_io",
+                "title": "snode_record_end_time",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
+                "description": "",
                 "fieldConfig": {
                     "defaults": {
                         "color": {
                             "mode": "palette-classic"
                         },
                         "custom": {
                             "axisCenteredZero": false,
@@ -2411,26 +2477,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 42
+                    "w": 7,
+                    "x": 7,
+                    "y": 63
                 },
-                "id": 1,
+                "id": 7,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2442,21 +2507,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_read_bytes",
+                        "expr": "snode_record_duration",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_read_bytes",
+                "title": "snode_record_duration",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2505,25 +2570,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
-                    "x": 12,
-                    "y": 42
+                    "x": 14,
+                    "y": 63
                 },
-                "id": 2,
+                "id": 9,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -2535,33 +2600,33 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "snode_read_bytes_ps",
+                        "expr": "snode_record_start_time",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "snode_read_bytes_ps",
+                "title": "snode_record_start_time",
                 "type": "timeseries"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
         "templating": {
             "list": []
         },
         "time": {
-            "from": "now-6h",
+            "from": "now-1h",
             "to": "now"
         },
         "timepicker": {},
         "timezone": "",
         "title": "NodesDashboard",
         "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e37",
         "version": 5,
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_mig-1.0.90/simplyblock_core/scripts/dashboards/devices.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9919561938832773%*

 * *Differences: {"'dashboard'": "{'panels': {0: {'gridPos': {'h': 1, 'w': 24}, 'id': 31, 'title': 'Size', 'type': "*

 * *                "'row', 'collapsed': False, 'panels': [], delete: ['datasource', 'fieldConfig', "*

 * *                "'options', 'targets']}, 1: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}, "*

 * *                "'gridPos': {'w': 7, 'x': 0, 'y': 1}, 'id': 13, 'targets': {0: {'expr': "*

 * *                "'device_size_total'}}, 'title': 'device_size_total'}, 2: {'fieldConfig': "*

 * *                "{'defaults': {'un […]*

```diff
@@ -20,105 +20,25 @@
         "fiscalYearStartMonth": 0,
         "graphTooltip": 0,
         "id": null,
         "links": [],
         "liveNow": false,
         "panels": [
             {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        },
-                        "unit": "decmbytes"
-                    },
-                    "overrides": []
-                },
+                "collapsed": false,
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
+                    "h": 1,
+                    "w": 24,
                     "x": 0,
                     "y": 0
                 },
-                "id": 27,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "device_write_latency_ticks",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "device_write_latency_ticks",
-                "type": "timeseries"
+                "id": 31,
+                "panels": [],
+                "title": "Size",
+                "type": "row"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
@@ -165,25 +85,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 0
+                    "w": 7,
+                    "x": 0,
+                    "y": 1
                 },
-                "id": 26,
+                "id": 13,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -195,21 +116,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_write_latency_ps",
+                        "expr": "device_size_total",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_write_latency_ps",
+                "title": "device_size_total",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -257,25 +178,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 0
+                    "w": 7,
+                    "x": 7,
+                    "y": 1
                 },
-                "id": 25,
+                "id": 10,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -287,21 +209,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_write_io_ps",
+                        "expr": "device_size_free",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_write_io_ps",
+                "title": "device_size_free",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -349,25 +271,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 0
+                    "w": 8,
+                    "x": 14,
+                    "y": 1
                 },
-                "id": 24,
+                "id": 14,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -379,21 +302,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_write_io",
+                        "expr": "device_size_used",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_write_io",
+                "title": "device_size_used",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -442,25 +365,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
+                    "w": 7,
                     "x": 0,
-                    "y": 7
+                    "y": 8
                 },
-                "id": 23,
+                "id": 11,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -472,21 +395,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_write_bytes_ps",
+                        "expr": "device_size_prov",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_write_bytes_ps",
+                "title": "device_size_prov",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -535,25 +458,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 7
+                    "w": 7,
+                    "x": 7,
+                    "y": 8
                 },
-                "id": 22,
+                "id": 12,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -565,21 +488,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_write_bytes",
+                        "expr": "device_size_prov_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_write_bytes",
+                "title": "device_size_prov_util",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -627,118 +550,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 7
-                },
-                "id": 21,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "device_unmap_latency_ticks",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "device_unmap_latency_ticks",
-                "type": "timeseries"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "description": "",
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
                         },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        }
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 7
+                    "w": 8,
+                    "x": 14,
+                    "y": 8
                 },
-                "id": 20,
+                "id": 15,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -750,139 +581,35 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_unmap_latency_ps",
+                        "expr": "device_size_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_unmap_latency_ps",
+                "title": "device_size_util",
                 "type": "timeseries"
             },
             {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        }
-                    },
-                    "overrides": [
-                        {
-                            "__systemRef": "hideSeriesFrom",
-                            "matcher": {
-                                "id": "byNames",
-                                "options": {
-                                    "mode": "exclude",
-                                    "names": [
-                                        "{__name__=\"device_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
-                                    ],
-                                    "prefix": "All except:",
-                                    "readOnly": true
-                                }
-                            },
-                            "properties": [
-                                {
-                                    "id": "custom.hideFrom",
-                                    "value": {
-                                        "legend": false,
-                                        "tooltip": false,
-                                        "viz": true
-                                    }
-                                }
-                            ]
-                        }
-                    ]
-                },
+                "collapsed": false,
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
+                    "h": 1,
+                    "w": 24,
                     "x": 0,
-                    "y": 14
-                },
-                "id": 19,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
+                    "y": 15
                 },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "device_unmap_io_ps",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "device_unmap_io_ps",
-                "type": "timeseries"
+                "id": 28,
+                "panels": [],
+                "title": "Writes",
+                "type": "row"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
@@ -929,25 +656,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 14
+                    "h": 8,
+                    "w": 7,
+                    "x": 0,
+                    "y": 16
                 },
-                "id": 18,
+                "id": 22,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -959,21 +687,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_unmap_io",
+                        "expr": "device_write_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_unmap_io",
+                "title": "device_write_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1022,25 +750,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 14
+                    "h": 8,
+                    "w": 7,
+                    "x": 7,
+                    "y": 16
                 },
-                "id": 17,
+                "id": 23,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1052,21 +780,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_unmap_bytes_ps",
+                        "expr": "device_write_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_unmap_bytes_ps",
+                "title": "write_speed",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1115,25 +843,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "ns"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 14
+                    "h": 8,
+                    "w": 8,
+                    "x": 14,
+                    "y": 16
                 },
-                "id": 16,
+                "id": 26,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1145,21 +873,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_unmap_bytes",
+                        "expr": "device_write_latency_ps / 1000",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_unmap_bytes",
+                "title": "device_write_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1207,26 +935,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
+                    "h": 8,
+                    "w": 7,
                     "x": 0,
-                    "y": 21
+                    "y": 24
                 },
-                "id": 15,
+                "id": 24,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1238,21 +965,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_size_util",
+                        "expr": "device_write_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_size_util",
+                "title": "device_write_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1300,26 +1027,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 21
+                    "h": 8,
+                    "w": 7,
+                    "x": 7,
+                    "y": 24
                 },
-                "id": 14,
+                "id": 25,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1331,21 +1057,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_size_used",
+                        "expr": "device_write_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_size_used",
+                "title": "write_iops",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1393,26 +1119,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 21
+                    "h": 8,
+                    "w": 8,
+                    "x": 14,
+                    "y": 24
                 },
-                "id": 13,
+                "id": 33,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1424,115 +1149,35 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_size_total",
+                        "expr": "device_write_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_size_total",
+                "title": "device_wite_latency_ticks",
                 "type": "timeseries"
             },
             {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        },
-                        "unit": "decmbytes"
-                    },
-                    "overrides": []
-                },
+                "collapsed": false,
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 21
-                },
-                "id": 12,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 32
                 },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "device_size_prov_util",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "device_size_prov_util",
-                "type": "timeseries"
+                "id": 30,
+                "panels": [],
+                "title": "Reads",
+                "type": "row"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
                 "fieldConfig": {
@@ -1580,25 +1225,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
+                    "h": 8,
+                    "w": 7,
                     "x": 0,
-                    "y": 28
+                    "y": 33
                 },
-                "id": 11,
+                "id": 1,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1610,21 +1255,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_size_prov",
+                        "expr": "device_read_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_size_prov",
+                "title": "device_read_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1673,25 +1318,25 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decmbytes"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 28
+                    "h": 8,
+                    "w": 7,
+                    "x": 7,
+                    "y": 33
                 },
-                "id": 10,
+                "id": 2,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1703,21 +1348,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_size_free",
+                        "expr": "device_read_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_size_free",
+                "title": "read_speed",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1765,26 +1410,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "decmbytes"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 28
+                    "h": 8,
+                    "w": 8,
+                    "x": 14,
+                    "y": 33
                 },
-                "id": 9,
+                "id": 5,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1796,21 +1440,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_record_start_time",
+                        "expr": "device_read_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_record_start_time",
+                "title": "device_read_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1864,19 +1508,19 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 28
+                    "w": 7,
+                    "x": 0,
+                    "y": 41
                 },
-                "id": 8,
+                "id": 3,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1888,29 +1532,28 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_record_end_time",
+                        "expr": "device_read_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_record_end_time",
+                "title": "device_read_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
-                "description": "",
                 "fieldConfig": {
                     "defaults": {
                         "color": {
                             "mode": "palette-classic"
                         },
                         "custom": {
                             "axisCenteredZero": false,
@@ -1957,19 +1600,19 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 0,
-                    "y": 35
+                    "w": 7,
+                    "x": 7,
+                    "y": 41
                 },
-                "id": 7,
+                "id": 4,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1981,21 +1624,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "device_record_duration",
+                        "expr": "device_read_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "device_record_duration",
+                "title": "read_iops",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2049,17 +1692,17 @@
                             ]
                         }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 35
+                    "w": 8,
+                    "x": 14,
+                    "y": 41
                 },
                 "id": 6,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
@@ -2083,485 +1726,909 @@
                         "refId": "A"
                     }
                 ],
                 "title": "device_read_latency_ticks",
                 "type": "timeseries"
             },
             {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
+                "collapsed": true,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 48
                 },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
+                "id": 29,
+                "panels": [
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
                         },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
+                        "fieldConfig": {
+                            "defaults": {
+                                "color": {
+                                    "mode": "palette-classic"
                                 },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        }
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 12,
-                    "y": 35
-                },
-                "id": 5,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
+                                "custom": {
+                                    "axisCenteredZero": false,
+                                    "axisColorMode": "text",
+                                    "axisLabel": "",
+                                    "axisPlacement": "auto",
+                                    "barAlignment": 0,
+                                    "drawStyle": "line",
+                                    "fillOpacity": 0,
+                                    "gradientMode": "none",
+                                    "hideFrom": {
+                                        "legend": false,
+                                        "tooltip": false,
+                                        "viz": false
+                                    },
+                                    "lineInterpolation": "linear",
+                                    "lineWidth": 1,
+                                    "pointSize": 5,
+                                    "scaleDistribution": {
+                                        "type": "linear"
+                                    },
+                                    "showPoints": "auto",
+                                    "spanNulls": false,
+                                    "stacking": {
+                                        "group": "A",
+                                        "mode": "none"
+                                    },
+                                    "thresholdsStyle": {
+                                        "mode": "off"
+                                    }
+                                },
+                                "mappings": [],
+                                "thresholds": {
+                                    "mode": "absolute",
+                                    "steps": [
+                                        {
+                                            "color": "green",
+                                            "value": null
+                                        },
+                                        {
+                                            "color": "red",
+                                            "value": 80
+                                        }
+                                    ]
+                                }
+                            },
+                            "overrides": []
+                        },
+                        "gridPos": {
+                            "h": 7,
+                            "w": 7,
+                            "x": 0,
+                            "y": 48
+                        },
+                        "id": 21,
+                        "options": {
+                            "legend": {
+                                "calcs": [],
+                                "displayMode": "list",
+                                "placement": "bottom",
+                                "showLegend": true
+                            },
+                            "tooltip": {
+                                "mode": "single",
+                                "sort": "none"
+                            }
+                        },
+                        "targets": [
+                            {
+                                "datasource": {
+                                    "type": "prometheus",
+                                    "uid": "PBFA97CFB590B2093"
+                                },
+                                "editorMode": "builder",
+                                "expr": "device_unmap_latency_ticks",
+                                "legendFormat": "__auto",
+                                "range": true,
+                                "refId": "A"
+                            }
+                        ],
+                        "title": "device_unmap_latency_ticks",
+                        "type": "timeseries"
                     },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_read_latency_ps",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "device_read_latency_ps",
-                "type": "timeseries"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
+                        "fieldConfig": {
+                            "defaults": {
+                                "color": {
+                                    "mode": "palette-classic"
+                                },
+                                "custom": {
+                                    "axisCenteredZero": false,
+                                    "axisColorMode": "text",
+                                    "axisLabel": "",
+                                    "axisPlacement": "auto",
+                                    "barAlignment": 0,
+                                    "drawStyle": "line",
+                                    "fillOpacity": 0,
+                                    "gradientMode": "none",
+                                    "hideFrom": {
+                                        "legend": false,
+                                        "tooltip": false,
+                                        "viz": false
+                                    },
+                                    "lineInterpolation": "linear",
+                                    "lineWidth": 1,
+                                    "pointSize": 5,
+                                    "scaleDistribution": {
+                                        "type": "linear"
+                                    },
+                                    "showPoints": "auto",
+                                    "spanNulls": false,
+                                    "stacking": {
+                                        "group": "A",
+                                        "mode": "none"
+                                    },
+                                    "thresholdsStyle": {
+                                        "mode": "off"
+                                    }
                                 },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        }
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 18,
-                    "y": 35
-                },
-                "id": 4,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
+                                "mappings": [],
+                                "thresholds": {
+                                    "mode": "absolute",
+                                    "steps": [
+                                        {
+                                            "color": "green",
+                                            "value": null
+                                        },
+                                        {
+                                            "color": "red",
+                                            "value": 80
+                                        }
+                                    ]
+                                },
+                                "unit": "decbytes"
+                            },
+                            "overrides": []
+                        },
+                        "gridPos": {
+                            "h": 7,
+                            "w": 7,
+                            "x": 7,
+                            "y": 48
+                        },
+                        "id": 17,
+                        "options": {
+                            "legend": {
+                                "calcs": [],
+                                "displayMode": "list",
+                                "placement": "bottom",
+                                "showLegend": true
+                            },
+                            "tooltip": {
+                                "mode": "single",
+                                "sort": "none"
+                            }
+                        },
+                        "targets": [
+                            {
+                                "datasource": {
+                                    "type": "prometheus",
+                                    "uid": "PBFA97CFB590B2093"
+                                },
+                                "editorMode": "builder",
+                                "expr": "device_unmap_bytes_ps",
+                                "legendFormat": "__auto",
+                                "range": true,
+                                "refId": "A"
+                            }
+                        ],
+                        "title": "device_unmap_bytes_ps",
+                        "type": "timeseries"
                     },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_read_io_ps",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "device_read_io_ps",
-                "type": "timeseries"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
+                        "description": "",
+                        "fieldConfig": {
+                            "defaults": {
+                                "color": {
+                                    "mode": "palette-classic"
+                                },
+                                "custom": {
+                                    "axisCenteredZero": false,
+                                    "axisColorMode": "text",
+                                    "axisLabel": "",
+                                    "axisPlacement": "auto",
+                                    "barAlignment": 0,
+                                    "drawStyle": "line",
+                                    "fillOpacity": 0,
+                                    "gradientMode": "none",
+                                    "hideFrom": {
+                                        "legend": false,
+                                        "tooltip": false,
+                                        "viz": false
+                                    },
+                                    "lineInterpolation": "linear",
+                                    "lineWidth": 1,
+                                    "pointSize": 5,
+                                    "scaleDistribution": {
+                                        "type": "linear"
+                                    },
+                                    "showPoints": "auto",
+                                    "spanNulls": false,
+                                    "stacking": {
+                                        "group": "A",
+                                        "mode": "none"
+                                    },
+                                    "thresholdsStyle": {
+                                        "mode": "off"
+                                    }
                                 },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        }
+                                "mappings": [],
+                                "thresholds": {
+                                    "mode": "absolute",
+                                    "steps": [
+                                        {
+                                            "color": "green",
+                                            "value": null
+                                        },
+                                        {
+                                            "color": "red",
+                                            "value": 80
+                                        }
+                                    ]
+                                }
+                            },
+                            "overrides": []
+                        },
+                        "gridPos": {
+                            "h": 7,
+                            "w": 8,
+                            "x": 14,
+                            "y": 48
+                        },
+                        "id": 20,
+                        "options": {
+                            "legend": {
+                                "calcs": [],
+                                "displayMode": "list",
+                                "placement": "bottom",
+                                "showLegend": true
+                            },
+                            "tooltip": {
+                                "mode": "single",
+                                "sort": "none"
+                            }
+                        },
+                        "targets": [
+                            {
+                                "datasource": {
+                                    "type": "prometheus",
+                                    "uid": "PBFA97CFB590B2093"
+                                },
+                                "editorMode": "builder",
+                                "expr": "device_unmap_latency_ps",
+                                "legendFormat": "__auto",
+                                "range": true,
+                                "refId": "A"
+                            }
+                        ],
+                        "title": "device_unmap_latency_ps",
+                        "type": "timeseries"
                     },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 0,
-                    "y": 42
-                },
-                "id": 3,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_read_io",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "device_read_io",
-                "type": "timeseries"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
+                        "fieldConfig": {
+                            "defaults": {
+                                "color": {
+                                    "mode": "palette-classic"
+                                },
+                                "custom": {
+                                    "axisCenteredZero": false,
+                                    "axisColorMode": "text",
+                                    "axisLabel": "",
+                                    "axisPlacement": "auto",
+                                    "barAlignment": 0,
+                                    "drawStyle": "line",
+                                    "fillOpacity": 0,
+                                    "gradientMode": "none",
+                                    "hideFrom": {
+                                        "legend": false,
+                                        "tooltip": false,
+                                        "viz": false
+                                    },
+                                    "lineInterpolation": "linear",
+                                    "lineWidth": 1,
+                                    "pointSize": 5,
+                                    "scaleDistribution": {
+                                        "type": "linear"
+                                    },
+                                    "showPoints": "auto",
+                                    "spanNulls": false,
+                                    "stacking": {
+                                        "group": "A",
+                                        "mode": "none"
+                                    },
+                                    "thresholdsStyle": {
+                                        "mode": "off"
+                                    }
                                 },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        },
-                        "unit": "decmbytes"
+                                "mappings": [],
+                                "thresholds": {
+                                    "mode": "absolute",
+                                    "steps": [
+                                        {
+                                            "color": "green",
+                                            "value": null
+                                        },
+                                        {
+                                            "color": "red",
+                                            "value": 80
+                                        }
+                                    ]
+                                }
+                            },
+                            "overrides": [
+                                {
+                                    "__systemRef": "hideSeriesFrom",
+                                    "matcher": {
+                                        "id": "byNames",
+                                        "options": {
+                                            "mode": "exclude",
+                                            "names": [
+                                                "{__name__=\"device_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
+                                            ],
+                                            "prefix": "All except:",
+                                            "readOnly": true
+                                        }
+                                    },
+                                    "properties": [
+                                        {
+                                            "id": "custom.hideFrom",
+                                            "value": {
+                                                "legend": false,
+                                                "tooltip": false,
+                                                "viz": true
+                                            }
+                                        }
+                                    ]
+                                }
+                            ]
+                        },
+                        "gridPos": {
+                            "h": 7,
+                            "w": 7,
+                            "x": 0,
+                            "y": 55
+                        },
+                        "id": 19,
+                        "options": {
+                            "legend": {
+                                "calcs": [],
+                                "displayMode": "list",
+                                "placement": "bottom",
+                                "showLegend": true
+                            },
+                            "tooltip": {
+                                "mode": "single",
+                                "sort": "none"
+                            }
+                        },
+                        "targets": [
+                            {
+                                "datasource": {
+                                    "type": "prometheus",
+                                    "uid": "PBFA97CFB590B2093"
+                                },
+                                "editorMode": "builder",
+                                "expr": "device_unmap_io_ps",
+                                "legendFormat": "__auto",
+                                "range": true,
+                                "refId": "A"
+                            }
+                        ],
+                        "title": "device_unmap_io_ps",
+                        "type": "timeseries"
                     },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 6,
-                    "x": 6,
-                    "y": 42
-                },
-                "id": 1,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
+                        },
+                        "fieldConfig": {
+                            "defaults": {
+                                "color": {
+                                    "mode": "palette-classic"
+                                },
+                                "custom": {
+                                    "axisCenteredZero": false,
+                                    "axisColorMode": "text",
+                                    "axisLabel": "",
+                                    "axisPlacement": "auto",
+                                    "barAlignment": 0,
+                                    "drawStyle": "line",
+                                    "fillOpacity": 0,
+                                    "gradientMode": "none",
+                                    "hideFrom": {
+                                        "legend": false,
+                                        "tooltip": false,
+                                        "viz": false
+                                    },
+                                    "lineInterpolation": "linear",
+                                    "lineWidth": 1,
+                                    "pointSize": 5,
+                                    "scaleDistribution": {
+                                        "type": "linear"
+                                    },
+                                    "showPoints": "auto",
+                                    "spanNulls": false,
+                                    "stacking": {
+                                        "group": "A",
+                                        "mode": "none"
+                                    },
+                                    "thresholdsStyle": {
+                                        "mode": "off"
+                                    }
+                                },
+                                "mappings": [],
+                                "thresholds": {
+                                    "mode": "absolute",
+                                    "steps": [
+                                        {
+                                            "color": "green",
+                                            "value": null
+                                        },
+                                        {
+                                            "color": "red",
+                                            "value": 80
+                                        }
+                                    ]
+                                }
+                            },
+                            "overrides": []
+                        },
+                        "gridPos": {
+                            "h": 7,
+                            "w": 7,
+                            "x": 7,
+                            "y": 55
+                        },
+                        "id": 18,
+                        "options": {
+                            "legend": {
+                                "calcs": [],
+                                "displayMode": "list",
+                                "placement": "bottom",
+                                "showLegend": true
+                            },
+                            "tooltip": {
+                                "mode": "single",
+                                "sort": "none"
+                            }
+                        },
+                        "targets": [
+                            {
+                                "datasource": {
+                                    "type": "prometheus",
+                                    "uid": "PBFA97CFB590B2093"
+                                },
+                                "editorMode": "builder",
+                                "expr": "device_unmap_io",
+                                "legendFormat": "__auto",
+                                "range": true,
+                                "refId": "A"
+                            }
+                        ],
+                        "title": "device_unmap_io",
+                        "type": "timeseries"
                     },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_read_bytes",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
+                        "fieldConfig": {
+                            "defaults": {
+                                "color": {
+                                    "mode": "palette-classic"
+                                },
+                                "custom": {
+                                    "axisCenteredZero": false,
+                                    "axisColorMode": "text",
+                                    "axisLabel": "",
+                                    "axisPlacement": "auto",
+                                    "barAlignment": 0,
+                                    "drawStyle": "line",
+                                    "fillOpacity": 0,
+                                    "gradientMode": "none",
+                                    "hideFrom": {
+                                        "legend": false,
+                                        "tooltip": false,
+                                        "viz": false
+                                    },
+                                    "lineInterpolation": "linear",
+                                    "lineWidth": 1,
+                                    "pointSize": 5,
+                                    "scaleDistribution": {
+                                        "type": "linear"
+                                    },
+                                    "showPoints": "auto",
+                                    "spanNulls": false,
+                                    "stacking": {
+                                        "group": "A",
+                                        "mode": "none"
+                                    },
+                                    "thresholdsStyle": {
+                                        "mode": "off"
+                                    }
+                                },
+                                "mappings": [],
+                                "thresholds": {
+                                    "mode": "absolute",
+                                    "steps": [
+                                        {
+                                            "color": "green",
+                                            "value": null
+                                        },
+                                        {
+                                            "color": "red",
+                                            "value": 80
+                                        }
+                                    ]
+                                },
+                                "unit": "decbytes"
+                            },
+                            "overrides": []
+                        },
+                        "gridPos": {
+                            "h": 7,
+                            "w": 8,
+                            "x": 14,
+                            "y": 55
+                        },
+                        "id": 16,
+                        "options": {
+                            "legend": {
+                                "calcs": [],
+                                "displayMode": "list",
+                                "placement": "bottom",
+                                "showLegend": true
+                            },
+                            "tooltip": {
+                                "mode": "single",
+                                "sort": "none"
+                            }
+                        },
+                        "targets": [
+                            {
+                                "datasource": {
+                                    "type": "prometheus",
+                                    "uid": "PBFA97CFB590B2093"
+                                },
+                                "editorMode": "builder",
+                                "expr": "device_unmap_bytes",
+                                "legendFormat": "__auto",
+                                "range": true,
+                                "refId": "A"
+                            }
+                        ],
+                        "title": "device_unmap_bytes",
+                        "type": "timeseries"
                     }
                 ],
-                "title": "device_read_bytes",
-                "type": "timeseries"
+                "title": "unmap",
+                "type": "row"
             },
             {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
+                "collapsed": true,
+                "gridPos": {
+                    "h": 1,
+                    "w": 24,
+                    "x": 0,
+                    "y": 49
                 },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
+                "id": 32,
+                "panels": [
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
                         },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
+                        "fieldConfig": {
+                            "defaults": {
+                                "color": {
+                                    "mode": "palette-classic"
                                 },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        },
-                        "unit": "decmbytes"
+                                "custom": {
+                                    "axisCenteredZero": false,
+                                    "axisColorMode": "text",
+                                    "axisLabel": "",
+                                    "axisPlacement": "auto",
+                                    "barAlignment": 0,
+                                    "drawStyle": "line",
+                                    "fillOpacity": 0,
+                                    "gradientMode": "none",
+                                    "hideFrom": {
+                                        "legend": false,
+                                        "tooltip": false,
+                                        "viz": false
+                                    },
+                                    "lineInterpolation": "linear",
+                                    "lineWidth": 1,
+                                    "pointSize": 5,
+                                    "scaleDistribution": {
+                                        "type": "linear"
+                                    },
+                                    "showPoints": "auto",
+                                    "spanNulls": false,
+                                    "stacking": {
+                                        "group": "A",
+                                        "mode": "none"
+                                    },
+                                    "thresholdsStyle": {
+                                        "mode": "off"
+                                    }
+                                },
+                                "mappings": [],
+                                "thresholds": {
+                                    "mode": "absolute",
+                                    "steps": [
+                                        {
+                                            "color": "green",
+                                            "value": null
+                                        },
+                                        {
+                                            "color": "red",
+                                            "value": 80
+                                        }
+                                    ]
+                                }
+                            },
+                            "overrides": []
+                        },
+                        "gridPos": {
+                            "h": 7,
+                            "w": 7,
+                            "x": 0,
+                            "y": 49
+                        },
+                        "id": 8,
+                        "options": {
+                            "legend": {
+                                "calcs": [],
+                                "displayMode": "list",
+                                "placement": "bottom",
+                                "showLegend": true
+                            },
+                            "tooltip": {
+                                "mode": "single",
+                                "sort": "none"
+                            }
+                        },
+                        "targets": [
+                            {
+                                "datasource": {
+                                    "type": "prometheus",
+                                    "uid": "PBFA97CFB590B2093"
+                                },
+                                "editorMode": "builder",
+                                "expr": "device_record_end_time",
+                                "legendFormat": "__auto",
+                                "range": true,
+                                "refId": "A"
+                            }
+                        ],
+                        "title": "device_record_end_time",
+                        "type": "timeseries"
                     },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 12,
-                    "y": 42
-                },
-                "id": 2,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
+                        },
+                        "description": "",
+                        "fieldConfig": {
+                            "defaults": {
+                                "color": {
+                                    "mode": "palette-classic"
+                                },
+                                "custom": {
+                                    "axisCenteredZero": false,
+                                    "axisColorMode": "text",
+                                    "axisLabel": "",
+                                    "axisPlacement": "auto",
+                                    "barAlignment": 0,
+                                    "drawStyle": "line",
+                                    "fillOpacity": 0,
+                                    "gradientMode": "none",
+                                    "hideFrom": {
+                                        "legend": false,
+                                        "tooltip": false,
+                                        "viz": false
+                                    },
+                                    "lineInterpolation": "linear",
+                                    "lineWidth": 1,
+                                    "pointSize": 5,
+                                    "scaleDistribution": {
+                                        "type": "linear"
+                                    },
+                                    "showPoints": "auto",
+                                    "spanNulls": false,
+                                    "stacking": {
+                                        "group": "A",
+                                        "mode": "none"
+                                    },
+                                    "thresholdsStyle": {
+                                        "mode": "off"
+                                    }
+                                },
+                                "mappings": [],
+                                "thresholds": {
+                                    "mode": "absolute",
+                                    "steps": [
+                                        {
+                                            "color": "green",
+                                            "value": null
+                                        },
+                                        {
+                                            "color": "red",
+                                            "value": 80
+                                        }
+                                    ]
+                                }
+                            },
+                            "overrides": []
+                        },
+                        "gridPos": {
+                            "h": 7,
+                            "w": 7,
+                            "x": 7,
+                            "y": 49
+                        },
+                        "id": 7,
+                        "options": {
+                            "legend": {
+                                "calcs": [],
+                                "displayMode": "list",
+                                "placement": "bottom",
+                                "showLegend": true
+                            },
+                            "tooltip": {
+                                "mode": "single",
+                                "sort": "none"
+                            }
+                        },
+                        "targets": [
+                            {
+                                "datasource": {
+                                    "type": "prometheus",
+                                    "uid": "PBFA97CFB590B2093"
+                                },
+                                "editorMode": "builder",
+                                "expr": "device_record_duration",
+                                "legendFormat": "__auto",
+                                "range": true,
+                                "refId": "A"
+                            }
+                        ],
+                        "title": "device_record_duration",
+                        "type": "timeseries"
                     },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "editorMode": "builder",
-                        "expr": "device_read_bytes_ps",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
+                        "fieldConfig": {
+                            "defaults": {
+                                "color": {
+                                    "mode": "palette-classic"
+                                },
+                                "custom": {
+                                    "axisCenteredZero": false,
+                                    "axisColorMode": "text",
+                                    "axisLabel": "",
+                                    "axisPlacement": "auto",
+                                    "barAlignment": 0,
+                                    "drawStyle": "line",
+                                    "fillOpacity": 0,
+                                    "gradientMode": "none",
+                                    "hideFrom": {
+                                        "legend": false,
+                                        "tooltip": false,
+                                        "viz": false
+                                    },
+                                    "lineInterpolation": "linear",
+                                    "lineWidth": 1,
+                                    "pointSize": 5,
+                                    "scaleDistribution": {
+                                        "type": "linear"
+                                    },
+                                    "showPoints": "auto",
+                                    "spanNulls": false,
+                                    "stacking": {
+                                        "group": "A",
+                                        "mode": "none"
+                                    },
+                                    "thresholdsStyle": {
+                                        "mode": "off"
+                                    }
+                                },
+                                "mappings": [],
+                                "thresholds": {
+                                    "mode": "absolute",
+                                    "steps": [
+                                        {
+                                            "color": "green",
+                                            "value": null
+                                        },
+                                        {
+                                            "color": "red",
+                                            "value": 80
+                                        }
+                                    ]
+                                },
+                                "unit": "decbytes"
+                            },
+                            "overrides": []
+                        },
+                        "gridPos": {
+                            "h": 7,
+                            "w": 8,
+                            "x": 14,
+                            "y": 49
+                        },
+                        "id": 9,
+                        "options": {
+                            "legend": {
+                                "calcs": [],
+                                "displayMode": "list",
+                                "placement": "bottom",
+                                "showLegend": true
+                            },
+                            "tooltip": {
+                                "mode": "single",
+                                "sort": "none"
+                            }
+                        },
+                        "targets": [
+                            {
+                                "datasource": {
+                                    "type": "prometheus",
+                                    "uid": "PBFA97CFB590B2093"
+                                },
+                                "editorMode": "builder",
+                                "expr": "device_record_start_time",
+                                "legendFormat": "__auto",
+                                "range": true,
+                                "refId": "A"
+                            }
+                        ],
+                        "title": "device_record_start_time",
+                        "type": "timeseries"
                     }
                 ],
-                "title": "device_read_bytes_ps",
-                "type": "timeseries"
+                "title": "others",
+                "type": "row"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
         "templating": {
             "list": []
         },
         "time": {
-            "from": "now-6h",
+            "from": "now-1h",
             "to": "now"
         },
         "timepicker": {},
         "timezone": "",
         "title": "DevicesDashboard",
         "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e38",
         "version": 5,
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/services/caching_node_monitor.py` & `sbcli_mig-1.0.90/simplyblock_core/services/caching_node_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 
 from simplyblock_core import constants, kv_store
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core.models.caching_node import CachingNode
 
 # Import the GELF logger
-from graypy import GELFTCPHandler
+from graypy import GELFUDPHandler
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 
 # get DB controller
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/services/__init__.py` & `sbcli_mig-1.0.90/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/services/port_stat_collector.py` & `sbcli_mig-1.0.90/simplyblock_core/services/port_stat_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import psutil
 
 
 from simplyblock_core import constants, kv_store, utils
 from simplyblock_core.models.port_stat import PortStat
 
 # Import the GELF logger
-from graypy import GELFTCPHandler
+from graypy import GELFUDPHandler
 
 def update_port_stats(snode, nic, stats):
     now = int(time.time())
     data = {
         "uuid": nic.get_id(),
         "node_id": snode.get_id(),
         "date": now,
@@ -39,15 +39,15 @@
     stat_obj.write_to_db(db_controller.kv_store)
     return
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/services/lvol_monitor.py` & `sbcli_mig-1.0.90/simplyblock_core/services/lvol_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import datetime
 
 from simplyblock_core import constants, kv_store
 from simplyblock_core.models.lvol_model import LVol
 from simplyblock_core.controllers import health_controller, lvol_events
 
 # Import the GELF logger
-from graypy import GELFTCPHandler
+from graypy import GELFUDPHandler
 
 def set_lvol_status(lvol, status):
     if lvol.status != status:
         lvol = db_controller.get_lvol_by_id(lvol.get_id())
         old_status = lvol.status
         lvol.status = status
         lvol.write_to_db(db_store)
@@ -32,15 +32,15 @@
     lvol.write_to_db(db_store)
     lvol_events.lvol_health_check_change(lvol, lvol.health_check, old_status, caused_by="monitor")
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_store = kv_store.KVStore()
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/services/distr_event_collector.py` & `sbcli_mig-1.0.90/simplyblock_core/services/distr_event_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 
 
 from simplyblock_core import constants, kv_store, utils, rpc_client
 from simplyblock_core.controllers import events_controller, device_controller, lvol_events
 from simplyblock_core.models.lvol_model import LVol
 
 # Import the GELF logger
-from graypy import GELFTCPHandler
+from graypy import GELFUDPHandler
+
+from simplyblock_core.models.nvme_device import NVMeDevice
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
@@ -32,38 +34,43 @@
         storage_id = event.storage_id
 
         nodes = db_controller.get_storage_nodes()
         device_id = None
         for node in nodes:
             for dev in node.nvme_devices:
                 if dev.cluster_device_order == storage_id:
-                    if dev.status != "online":
+                    if dev.status not in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_READONLY]:
                         logger.info(f"The storage device is not online, skipping. status: {dev.status}")
                         event.status = 'skipped'
                         return
 
+                    # if node.get_id() != node_id:
+                    #     logger.info(f"The storage device is remote, skipping")
+                    #     event.status = 'skipped-remote'
+                    #     return
+
                     device_id = dev.get_id()
                     break
 
         if not device_id:
             logger.info(f"Device not found!, storage id: {storage_id} from node: {node_id}")
             event.status = 'device_not_found'
             return
 
         if event.message == 'SPDK_BDEV_EVENT_REMOVE':
             logger.info(f"Removing storage id: {storage_id} from node: {node_id}")
             device_controller.device_remove(device_id)
-        elif event.message == 'error_write':
+        elif event.message in ['error_write', 'error_unmap']:
             logger.info(f"Setting device to read-only")
-            device_controller.device_set_read_only(device_id)
             device_controller.device_set_io_error(device_id, True)
+            device_controller.device_set_read_only(device_id)
         else:
             logger.info(f"Setting device to unavailable")
-            device_controller.device_set_unavailable(device_id)
             device_controller.device_set_io_error(device_id, True)
+            device_controller.device_set_unavailable(device_id)
 
         event.status = 'processed'
 
 
 def process_lvol_event(event):
     if event.message in ["error_open", 'error_read', "error_write", "error_unmap"]:
         vuid = event.object_dict['vuid']
@@ -80,15 +87,18 @@
             lvol.io_error = True
             if lvol.status == LVol.STATUS_ONLINE:
                 logger.info("Setting LVol to offline")
                 old_status = lvol.status
                 lvol.status = LVol.STATUS_OFFLINE
                 lvol.write_to_db(db_controller.kv_store)
                 lvol_events.lvol_status_change(lvol, lvol.status, old_status, caused_by="monitor")
-            event.status = 'processed'
+                lvol_events.lvol_io_error_change(lvol, True, False, caused_by="monitor")
+                event.status = 'processed'
+            else:
+                event.status = 'skipped'
     else:
         logger.error(f"Unknown LVol event message: {event.message}")
         event.status = "event_unknown"
 
 
 def process_event(event_id):
     event = db_controller.get_events(event_id)[0]
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_mig-1.0.90/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 
 from simplyblock_core import constants, kv_store, utils
 from simplyblock_core.controllers import mgmt_events
 from simplyblock_core.models.mgmt_node import MgmtNode
 
 # Import the GELF logger
-from graypy import GELFTCPHandler
+from graypy import GELFUDPHandler
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 
 # get DB controller
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/services/log_agg_service.py` & `sbcli_mig-1.0.90/simplyblock_core/services/log_agg_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import time
 import sys
 
 from simplyblock_core import constants, kv_store, utils
 from simplyblock_core.models.stats import DeviceStatObject, NodeStatObject, ClusterStatObject
 
 # Import the GELF logger
-from graypy import GELFTCPHandler
+from graypy import GELFUDPHandler
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_mig-1.0.90/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # coding=utf-8
 import logging
 
 import time
 import sys
 
 from simplyblock_core import constants, kv_store, utils
+from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core.models.stats import DeviceStatObject, NodeStatObject, ClusterStatObject
 
 # Import the GELF logger
-from graypy import GELFTCPHandler
+from graypy import GELFUDPHandler
 
 last_object_record = {}
 
 
 def add_device_stats(cl, device, capacity_dict, stats_dict):
     now = int(time.time())
     data = {
@@ -83,42 +84,43 @@
     stat_obj = DeviceStatObject(data=data)
     stat_obj.write_to_db(db_controller.kv_store)
     last_object_record[device.get_id()] = stat_obj
     return stat_obj
 
 
 def add_node_stats(node, records):
-    if not records:
-        return False
-    records_sum = utils.sum_records(records)
-
-    size_total = records_sum.size_total
-    size_used = records_sum.size_used
+    size_used = 0
+    size_total = 0
+    data = {}
+    if records:
+        records_sum = utils.sum_records(records)
+        size_total = records_sum.size_total
+        size_used = records_sum.size_used
+        data.update(records_sum.get_clean_dict())
 
     size_prov = 0
     for lvol_id in node.lvols:
         lvol = db_controller.get_lvol_by_id(lvol_id)
         if lvol:
             size_prov += lvol.size
+
     size_util = 0
     size_prov_util = 0
     if size_total > 0:
         size_util = int((size_used / size_total) * 100)
         size_prov_util = int((size_prov / size_total) * 100)
 
-    data = records_sum.get_clean_dict()
     data.update({
         "cluster_id": cl.get_id(),
         "uuid": node.get_id(),
         "date": int(time.time()),
-
         "size_util": size_util,
         "size_prov": size_prov,
-        "size_prov_util": size_prov_util })
-
+        "size_prov_util": size_prov_util
+    })
     stat_obj = NodeStatObject(data=data)
     stat_obj.write_to_db(db_controller.kv_store)
     return stat_obj
 
 
 def add_cluster_stats(cl, records):
 
@@ -147,15 +149,15 @@
     stat_obj.write_to_db(db_controller.kv_store)
     return stat_obj
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
@@ -183,21 +185,22 @@
                 node.mgmt_ip, node.rpc_port,
                 node.rpc_username, node.rpc_password,
                 timeout=3, retry=2)
 
             devices_records = []
             for device in node.nvme_devices:
                 logger.info("Getting device stats: %s", device.uuid)
-                if device.status != 'online':
-                    logger.info("Device is not online, skipping")
+                if device.status not in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_READONLY]:
+                    logger.info(f"Device is skipped: {device.get_id()} status: {device.status}")
                     continue
                 capacity_dict = rpc_client.alceml_get_capacity(device.alceml_bdev)
                 stats_dict = rpc_client.get_device_stats(device.alloc_bdev)
                 record = add_device_stats(cl, device, capacity_dict, stats_dict)
-                devices_records.append(record)
+                if record:
+                    devices_records.append(record)
 
             node_record = add_node_stats(node, devices_records)
             node_records.append(node_record)
 
         add_cluster_stats(cl, node_records)
 
     time.sleep(constants.DEV_STAT_COLLECTOR_INTERVAL_SEC)
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/services/cap_monitor.py` & `sbcli_mig-1.0.90/simplyblock_core/services/cap_monitor.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 
 
 from simplyblock_core import kv_store, constants, cluster_ops
 from simplyblock_core.controllers import cluster_events
 from simplyblock_core.models.cluster import Cluster
 
 # Import the GELF logger
-from graypy import GELFTCPHandler
+from graypy import GELFUDPHandler
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
+### script to test connection once connection is ascertain
 # get DB controller
 db_controller = kv_store.DBController()
 
 logger.info("Starting capacity monitoring service...")
 while True:
     clusters = db_controller.get_clusters()
     for cl in clusters:
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/services/storage_node_monitor.py` & `sbcli_mig-1.0.90/simplyblock_core/services/storage_node_monitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import os
 
 import time
 import sys
 from datetime import datetime
 
 
-from simplyblock_core import constants, kv_store, cluster_ops
+from simplyblock_core import constants, kv_store, cluster_ops, storage_node_ops, distr_controller
 from simplyblock_core.controllers import storage_events, health_controller
 from simplyblock_core.models.cluster import Cluster
 from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.models.storage_node import StorageNode
 
 # Import the GELF logger
-from graypy import GELFTCPHandler
+from graypy import GELFUDPHandler
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 
 # get DB controller
@@ -62,18 +62,14 @@
 
     logger.debug(f"online_nodes: {online_nodes}")
     logger.debug(f"offline_nodes: {offline_nodes}")
     logger.debug(f"affected_nodes: {affected_nodes}")
     logger.debug(f"online_devices: {online_devices}")
     logger.debug(f"offline_devices: {offline_devices}")
 
-    # if less than 3 online nodes then suspend
-    if affected_nodes > 2:
-        return Cluster.STATUS_SUSPENDED
-
     # if more than two affected modes then cluster is suspended
     if affected_nodes > 2:
         return Cluster.STATUS_SUSPENDED
 
     # if any device goes offline then cluster is degraded
     if offline_devices > 0:
         return Cluster.STATUS_DEGRADED
@@ -116,14 +112,18 @@
         #         distr_controller.send_dev_status_event(dev.cluster_device_order, "online")
 
         old_status = snode.status
         snode.status = StorageNode.STATUS_ONLINE
         snode.updated_at = str(datetime.now())
         snode.write_to_db(db_store)
         storage_events.snode_status_change(snode, snode.status, old_status, caused_by="monitor")
+        distr_controller.send_node_status_event(snode.get_id(), StorageNode.STATUS_ONLINE)
+
+        logger.info("Connecting to remote devices")
+        storage_node_ops._connect_to_remote_devs(snode)
 
 
 def set_node_offline(node):
     if node.status == StorageNode.STATUS_ONLINE:
         snode = db_controller.get_storage_node_by_id(node.get_id())
         # for dev in snode.nvme_devices:
         #     if dev.status == 'online':
@@ -131,14 +131,15 @@
         #         distr_controller.send_dev_status_event(dev.cluster_device_order, "unavailable")
 
         old_status = snode.status
         snode.status = StorageNode.STATUS_UNREACHABLE
         snode.updated_at = str(datetime.now())
         snode.write_to_db(db_store)
         storage_events.snode_status_change(snode, snode.status, old_status, caused_by="monitor")
+        distr_controller.send_node_status_event(snode.get_id(), StorageNode.STATUS_UNREACHABLE)
 
 
 logger.info("Starting node monitor")
 
 while True:
     # get storage nodes
     nodes = db_controller.get_storage_nodes()
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/services/install_service.sh` & `sbcli_mig-1.0.90/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/services/health_check_service.py` & `sbcli_mig-1.0.90/simplyblock_core/services/health_check_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from simplyblock_core.controllers import health_controller, storage_events, device_events
 from simplyblock_core.models.storage_node import StorageNode
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core import constants, kv_store
 
 # Import the GELF logger
-from graypy import GELFTCPHandler
+from graypy import GELFUDPHandler
 
 def set_node_health_check(snode, health_check_status):
     snode = db_controller.get_storage_node_by_id(snode.get_id())
     if snode.health_check == health_check_status:
         return
     old_status = snode.health_check
     snode.health_check = health_check_status
@@ -39,15 +39,15 @@
                     device_events.device_health_check_change(
                         dev, dev.health_check, old_status, caused_by="monitor")
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_store = kv_store.KVStore()
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/services/device_monitor.py` & `sbcli_mig-1.0.90/simplyblock_core/services/device_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 from simplyblock_core import constants, kv_store, storage_node_ops
 from simplyblock_core.controllers import health_controller,  device_controller
 from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.models.storage_node import StorageNode
 
 # Import the GELF logger
-from graypy import GELFTCPHandler
+from graypy import GELFUDPHandler
+
 
 def set_dev_status(device, status):
     node = db_controller.get_storage_node_by_id(device.node_id)
     if node.status != StorageNode.STATUS_ONLINE:
         logger.error(f"Node is not online, {node.get_id()}, status: {node.status}, "
                      f"skipping device status change")
         return
@@ -28,15 +29,15 @@
             break
     return
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_store = kv_store.KVStore()
@@ -56,13 +57,13 @@
                 continue
             if dev.io_error:
                 logger.debug(f"Skipping Device check because of io_error {dev.get_id()}")
                 continue
 
             ret = health_controller.check_device(dev.get_id())
             logger.info(f"Device: {dev.get_id()}, is healthy: {ret}")
-            if ret:
-                set_dev_status(dev, NVMeDevice.STATUS_ONLINE)
-            else:
-                set_dev_status(dev, NVMeDevice.STATUS_UNAVAILABLE)
+            # if ret:
+            #     set_dev_status(dev, NVMeDevice.STATUS_ONLINE)
+            # else:
+            #     set_dev_status(dev, NVMeDevice.STATUS_UNAVAILABLE)
 
     time.sleep(constants.DEV_MONITOR_INTERVAL_SEC)
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_mig-1.0.90/simplyblock_core/services/lvol_stat_collector.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import logging
 
 import time
 import sys
 
 
 from simplyblock_core import constants, kv_store, utils
+from simplyblock_core.controllers import lvol_events
 from simplyblock_core.models.stats import LVolStatObject, PoolStatObject
 from simplyblock_core.rpc_client import RPCClient
 
 # Import the GELF logger
-from graypy import GELFTCPHandler
+from graypy import GELFUDPHandler
 
 last_object_record = {}
 
 
 def add_lvol_stats(pool, lvol, stats_dict):
     now = int(time.time())
     data = {
@@ -55,14 +56,21 @@
                 data['write_io_ps'] = int((data['write_io'] - last_record['write_io']) / time_diff)
                 data['write_latency_ps'] = int((data['write_latency_ticks'] - last_record['write_latency_ticks']) / time_diff)
 
                 data['unmap_bytes_ps'] = int((data['unmap_bytes'] - last_record['unmap_bytes']) / time_diff)
                 data['unmap_io_ps'] = int((data['unmap_io'] - last_record['unmap_io']) / time_diff)
                 data['unmap_latency_ps'] = int((data['unmap_latency_ticks'] - last_record['unmap_latency_ticks']) / time_diff)
 
+                if data['read_io_ps'] > 0 and data['write_io_ps'] > 0 and lvol.io_error:
+                    # set lvol io error to false
+                    lvol = db_controller.get_lvol_by_id(lvol.get_id())
+                    lvol.io_error = False
+                    lvol.write_to_db(db_store)
+                    lvol_events.lvol_io_error_change(lvol, False, True, caused_by="monitor")
+
         else:
             logger.warning("last record not found")
     else:
         logger.error("Error getting stats")
 
     stat_obj = LVolStatObject(data=data)
     stat_obj.write_to_db(db_controller.kv_store)
@@ -88,15 +96,15 @@
     stat_obj.write_to_db(db_controller.kv_store)
     return stat_obj
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_store = kv_store.KVStore()
@@ -115,17 +123,17 @@
                 lvols.append(lvol)
 
         if not lvols:
             logger.error("LVols list is empty")
 
         stat_records = []
         for lvol in lvols:
-            if lvol.status != lvol.STATUS_ONLINE:
-                logger.warning(f"LVol in not online, id: {lvol.get_id()}, status: {lvol.status}")
-                continue
+            # if lvol.status != lvol.STATUS_ONLINE:
+            #     logger.warning(f"LVol in not online, id: {lvol.get_id()}, status: {lvol.status}")
+            #     continue
             snode = db_controller.get_storage_node_by_hostname(lvol.hostname)
             rpc_client = RPCClient(
                 snode.mgmt_ip, snode.rpc_port,
                 snode.rpc_username, snode.rpc_password,
                 timeout=3, retry=2)
 
             logger.info("Getting lVol stats: %s", lvol.uuid)
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/events.py` & `sbcli_mig-1.0.90/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/nvme_device.py` & `sbcli_mig-1.0.90/simplyblock_core/models/nvme_device.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 from typing import List
 
 from simplyblock_core.models.base_model import BaseModel
 
 
 class NVMeDevice(BaseModel):
 
+    STATUS_JM = "JM_DEV"
+
+    STATUS_NEW = "new"
     STATUS_ONLINE = 'online'
-    STATUS_AVAILABLE = 'available'
     STATUS_UNAVAILABLE = 'unavailable'
-    STATUS_READONLY = 'read_only'
-    STATUS_OVERLOADED = 'overloaded'
-    STATUS_FAILED = 'failed'
     STATUS_REMOVED = 'removed'
-    STATUS_RESETTING = 'resetting'
-    STATUS_UNRECOGNIZED = 'unrecognized'
+    STATUS_FAILED = 'failed'
+    STATUS_READONLY = 'read_only'
 
     attributes = {
         "uuid": {"type": str, 'default': ""},
         "device_name": {"type": str, 'default': ""},
         "status": {"type": str, 'default': ""},
         "sequential_number": {"type": int, 'default': 0},
         "partitions_count": {"type": int, 'default': 0},
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/global_settings.py` & `sbcli_mig-1.0.90/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/caching_node.py` & `sbcli_mig-1.0.90/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/port_stat.py` & `sbcli_mig-1.0.90/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/snapshot.py` & `sbcli_mig-1.0.90/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/iface.py` & `sbcli_mig-1.0.90/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/stats.py` & `sbcli_mig-1.0.90/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/storage_node.py` & `sbcli_mig-1.0.90/simplyblock_core/models/storage_node.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 
 
 class StorageNode(BaseModel):
 
     STATUS_ONLINE = 'online'
     STATUS_OFFLINE = 'offline'
     STATUS_SUSPENDED = 'suspended'
-    STATUS_IN_CREATION = 'in_creation'
     STATUS_IN_SHUTDOWN = 'in_shutdown'
-    STATUS_RESTARTING = 'restarting'
-    STATUS_UNREACHABLE = 'unreachable'
     STATUS_REMOVED = 'removed'
+    STATUS_RESTARTING = 'in_restart'
+
+    STATUS_IN_CREATION = 'in_restart'  # 'in_creation'
+    STATUS_UNREACHABLE = 'offline'  # 'unreachable'
 
     STATUS_CODE_MAP = {
         STATUS_ONLINE: 0,
         STATUS_OFFLINE: 1,
         STATUS_SUSPENDED: 2,
         STATUS_REMOVED: 3,
 
@@ -68,14 +69,25 @@
         "health_check": {"type": bool, "default": True},
 
         # spdk params
         "spdk_cpu_mask": {"type": str, "default": ""},
         "spdk_mem": {"type": int, "default": 0},
         "spdk_image": {"type": str, "default": ""},
         "spdk_debug": {"type": bool, "default": False},
+
+        "ec2_metadata": {"type": dict, "default": {}},
+        "ec2_instance_id": {"type": str, "default": ""},
+        "ec2_public_ip": {"type": str, "default": ""},
+
+        # IO buffer options
+        "iobuf_small_pool_count": {"type": int, "default": 0},
+        "iobuf_large_pool_count": {"type": int, "default": 0},
+        "iobuf_small_bufsize": {"type": int, "default": 0},
+        "iobuf_large_bufsize": {"type": int, "default": 0},
+
     }
 
     def __init__(self, data=None):
         super(StorageNode, self).__init__()
         self.set_attrs(self.attributes, data)
         self.object_type = "object"
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/compute_node.py` & `sbcli_mig-1.0.90/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/mgmt_node.py` & `sbcli_mig-1.0.90/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/pool.py` & `sbcli_mig-1.0.90/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/cluster.py` & `sbcli_mig-1.0.90/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/base_model.py` & `sbcli_mig-1.0.90/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/models/lvol_model.py` & `sbcli_mig-1.0.90/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/controllers/storage_events.py` & `sbcli_mig-1.0.90/simplyblock_core/controllers/storage_events.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         event=ec.EVENT_OBJ_CREATED,
         db_object=node,
         caused_by=ec.CAUSED_BY_CLI,
         message=f"Storage node created {node.get_id()}",
         node_id=node.get_id())
 
 
-def snode_remove(node):
+def snode_delete(node):
     ec.log_event_cluster(
         cluster_id=node.cluster_id,
         domain=ec.DOMAIN_CLUSTER,
         event=ec.EVENT_OBJ_DELETED,
         db_object=node,
         caused_by=ec.CAUSED_BY_CLI,
         message=f"Storage node deleted {node.get_id()}",
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/controllers/cluster_events.py` & `sbcli_mig-1.0.90/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/controllers/lvol_controller.py` & `sbcli_mig-1.0.90/simplyblock_core/controllers/lvol_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging as lg
 import json
 import string
 import random
 import sys
 import time
 import uuid
+from typing import Tuple
 
 from simplyblock_core import utils, constants, distr_controller
 from simplyblock_core.controllers import snapshot_controller, pool_controller, lvol_events
 from simplyblock_core.kv_store import DBController
 from simplyblock_core.models.cluster import Cluster
 from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.models.pool import Pool
@@ -26,21 +27,20 @@
     def _generate_string(length):
         return ''.join(random.SystemRandom().choice(
             string.ascii_letters + string.digits) for _ in range(length))
 
     return _generate_string(length).encode('utf-8').hex()
 
 
-def _create_crypto_lvol(rpc_client, name, base_name):
+def _create_crypto_lvol(rpc_client, name, base_name, key1, key2):
     key_name = f'key_{name}'
-    key1 = _generate_hex_string(32)
-    key2 = _generate_hex_string(32)
     ret = rpc_client.lvol_crypto_key_create(key_name, key1, key2)
     if not ret:
-        logger.warning("failed to create crypto key")
+        logger.error("failed to create crypto key")
+        return False
     ret = rpc_client.lvol_crypto_create(name, base_name, key_name)
     if not ret:
         logger.error(f"failed to create crypto LVol {name}")
         return False
     return ret
 
 
@@ -290,15 +290,15 @@
 
     lvol_type = 'lvol'
     lvol_bdev = f"LVS_{vuid}/{name}"
     crypto_bdev = ''
     comp_bdev = ''
     top_bdev = lvol_bdev
     if use_crypto is True:
-        crypto_bdev = _create_crypto_lvol(rpc_client, name, lvol_bdev)
+        crypto_bdev = _create_crypto_lvol(rpc_client, name, lvol_bdev, "", "")
         bdev_stack.append({"type": "crypto", "name": crypto_bdev})
         if not crypto_bdev:
             return False, "Error creating crypto bdev"
         lvol_type += ',crypto'
         top_bdev = crypto_bdev
 
     if use_comp is True:
@@ -428,19 +428,48 @@
             node = db_controller.get_storage_node_by_id(node_id)
             print(f"Selected node: {node_id}, {node.hostname}")
             ret.append(node)
         return ret
     else:
         return online_nodes
 
+def is_hex(s: str) -> bool:
+    """
+    given an input checks if the value is hex encoded or not
+    """
+    try:
+        int(s, 16)
+        return True
+    except ValueError:
+        return False
+
+def validate_aes_xts_keys(key1: str, key2: str) -> Tuple[bool, str]:
+    """
+    Key Length: each key should be either 128 or 256 bits long.
+    since hex values of the keys are expected, the key lengths should be either 32 or 64
+    """
+
+    if len(key1) != len(key2):
+        return False, "both the keys should be of the same length"
+
+    if len(key1) not in [32, 64] or len(key2) not in [32, 64]:
+        return False, "each key should be either 16 or 32 bytes long"
+
+    if not is_hex(key1):
+        return False, "please provide hex encoded value for crypto_key1"
+
+    if not is_hex(key2):
+        return False, "please provide hex encoded value for crypto_key2"
+
+    return True, ""
 
 def add_lvol_ha(name, size, host_id_or_name, ha_type, pool_id_or_name, use_comp, use_crypto,
                 distr_vuid, distr_ndcs, distr_npcs,
                 max_rw_iops, max_rw_mbytes, max_r_mbytes, max_w_mbytes,
-                distr_bs=None, distr_chunk_bs=None, with_snapshot=False, max_size=0):
+                distr_bs=None, distr_chunk_bs=None, with_snapshot=False, max_size=0, crypto_key1=None, crypto_key2=None):
 
     logger.info(f"Adding LVol: {name}")
     host_node = None
     if host_id_or_name:
         host_node = db_controller.get_storage_node_by_id(host_id_or_name)
         if not host_node:
             host_node = db_controller.get_storage_node_by_hostname(host_id_or_name)
@@ -524,15 +553,14 @@
         vuid = distr_vuid
 
     if distr_ndcs == 0 and distr_npcs == 0:
         if ha_type == "single":
             distr_ndcs = 4
             distr_npcs = 1
         else:
-
             if dev_count == 3:
                 distr_ndcs = 1
             elif dev_count in [4, 5]:
                 distr_ndcs = 2
             elif dev_count >= 6:
                 distr_ndcs = 4
             distr_npcs = 1
@@ -616,22 +644,31 @@
                 "lvol_name": lvol.top_bdev,
                 "base_bdev": lvol.base_bdev,
                 "label": "label",
                 "desc": "desc"
             }
         })
 
-    if use_crypto is True:
+    if use_crypto:
+        if crypto_key1 == None or crypto_key2 == None:
+            return False, "encryption keys for lvol not provided"
+        else:
+            success, err = validate_aes_xts_keys(crypto_key1, crypto_key2)
+            if not success:
+                return False, err
+
         lvol.crypto_bdev = f"crypto_{lvol.lvol_name}"
         lvol.bdev_stack.append({
             "type": "crypto",
             "name": lvol.crypto_bdev,
             "params": {
                 "name": lvol.crypto_bdev,
-                "base_name": lvol.lvol_bdev
+                "base_name": lvol.base_bdev,
+                "key1": crypto_key1,
+                "key2": crypto_key2,
             }
         })
         lvol.lvol_type += ',crypto'
         lvol.top_bdev = lvol.crypto_bdev
 
     if use_comp is True:
         base_bdev = lvol.lvol_bdev
@@ -709,19 +746,18 @@
         ret = None
 
         if type == "bdev_distr":
             params['jm_names'] = get_jm_names(snode)
             params['ha_comm_addrs'] = ha_comm_addrs
             params['ha_inode_self'] = ha_inode_self
             ret = rpc_client.bdev_distrib_create(**params)
-
-            snodes = db_controller.get_storage_nodes()
-            cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-            cluster_map_data['UUID_node_target'] = snode.get_id()
-            rpc_client.distr_send_cluster_map(cluster_map_data)
+            if ret:
+                ret = distr_controller.send_cluster_map_to_node(snode)
+                if not ret:
+                    return False, "Failed to send cluster map"
 
         elif type == "bmap_init":
             ret = rpc_client.ultra21_lvol_bmap_init(**params)
 
         elif type == "ultra_lvol":
             ret = rpc_client.ultra21_lvol_mount_lvol(**params)
 
@@ -783,18 +819,17 @@
 
     logger.info("Add BDev to subsystem")
     ret = rpc_client.nvmf_subsystem_add_ns(lvol.nqn, lvol.top_bdev, lvol.uuid, lvol.guid)
     if not ret:
         return False, "Failed to add bdev to subsystem"
 
     logger.info("Sending cluster map to LVol")
-    snodes = db_controller.get_storage_nodes()
-    cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-    cluster_map_data['UUID_node_target'] = snode.get_id()
-    ret = rpc_client.distr_send_cluster_map(cluster_map_data)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
 
     spdk_mem_info_after = rpc_client.ultra21_util_get_malloc_stats()
     logger.debug("ultra21_util_get_malloc_stats:")
     logger.debug(spdk_mem_info_after)
 
     diff = {}
     for key in spdk_mem_info_after.keys():
@@ -866,50 +901,54 @@
         if not ret:
             logger.error(f"Failed to delete BDev {name}")
 
         bdev['status'] = 'deleted'
         time.sleep(1)
 
 
-def delete_lvol_from_node(lvol, node_id):
+def delete_lvol_from_node(lvol_id, node_id, clear_data=True):
+    lvol = db_controller.get_lvol_by_id(lvol_id)
     snode = db_controller.get_storage_node_by_id(node_id)
     logger.debug(f"Deleting LVol:{lvol.get_id()} from node:{snode.get_id()}")
     rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
 
     # 1- remove bdevs
     _remove_bdev_stack(lvol.bdev_stack[::-1], rpc_client)
     lvol.deletion_status = 'bdevs_deleted'
     lvol.write_to_db(db_controller.kv_store)
 
     # 2- remove subsystem
     ret = rpc_client.subsystem_delete(lvol.nqn)
 
     # 3- clear alceml devices
-    for node in db_controller.get_storage_nodes():
-        if node.status == StorageNode.STATUS_ONLINE:
-            rpc_node = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
-            for dev in node.nvme_devices:
-                ret = rpc_node.alceml_unmap_vuid(dev.alceml_bdev, lvol.vuid)
+    if clear_data:
+        for node in db_controller.get_storage_nodes():
+            if node.status == StorageNode.STATUS_ONLINE:
+                rpc_node = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
+                for dev in node.nvme_devices:
+                    ret = rpc_node.alceml_unmap_vuid(dev.alceml_bdev, lvol.vuid)
 
     lvol.deletion_status = 'alceml_unmapped'
     lvol.write_to_db(db_controller.kv_store)
 
     # 4- clear JM
     # ret = rpc_client.alceml_unmap_vuid(name, lvol.vuid)
     # lvol.deletion_status = 'jm_unmapped'
     lvol.write_to_db(db_controller.kv_store)
 
     return True
 
 
-def delete_lvol(uuid, force_delete=False):
-    lvol = db_controller.get_lvol_by_id(uuid)
+def delete_lvol(id_or_name, force_delete=False):
+    lvol = db_controller.get_lvol_by_id(id_or_name)
     if not lvol:
-        logger.error(f"lvol not found: {uuid}")
-        return False
+        lvol = db_controller.get_lvol_by_name(id_or_name)
+        if not lvol:
+            logger.error(f"lvol not found: {id_or_name}")
+            return False
 
     pool = db_controller.get_pool_by_id(lvol.pool_uuid)
     if pool.status == Pool.STATUS_INACTIVE:
         logger.error(f"Pool is disabled")
         return False
 
     logger.debug(lvol)
@@ -920,42 +959,42 @@
         snode.rpc_port,
         snode.rpc_username,
         snode.rpc_password)
 
     # soft delete LVol if it has snapshots
     snaps = db_controller.get_snapshots()
     for snap in snaps:
-        if snap.lvol.get_id() == uuid:
+        if snap.lvol.get_id() == lvol.get_id():
             logger.warning(f"Soft delete LVol that has snapshots. Snapshot:{snap.get_id()}")
             ret = rpc_client.subsystem_delete(lvol.nqn)
             logger.debug(ret)
             lvol.deleted = True
             lvol.write_to_db(db_controller.kv_store)
             return True
 
     # set status
     lvol.status = LVol.STATUS_IN_DELETION
     lvol.write_to_db(db_controller.kv_store)
 
     if lvol.ha_type == 'single':
-        ret = delete_lvol_from_node(lvol, lvol.node_id)
+        ret = delete_lvol_from_node(lvol.get_id(), lvol.node_id)
         if not ret:
             return False
     elif lvol.ha_type == "ha":
         for nodes_id in lvol.nodes:
-            ret = delete_lvol_from_node(lvol, nodes_id)
+            ret = delete_lvol_from_node(lvol.get_id(), nodes_id)
             if not ret:
                 return False
 
     # remove from storage node
-    snode.lvols.remove(uuid)
+    snode.lvols.remove(lvol.get_id())
     snode.write_to_db(db_controller.kv_store)
 
     # remove from pool
-    pool.lvols.remove(uuid)
+    pool.lvols.remove(lvol.get_id())
     pool.write_to_db(db_controller.kv_store)
 
     lvol.remove(db_controller.kv_store)
 
     # if lvol is clone and snapshot is deleted, then delete snapshot
     if lvol.cloned_from_snap:
         snap = db_controller.get_snapshot_by_id(lvol.cloned_from_snap)
@@ -1269,21 +1308,15 @@
     lvol = db_controller.get_lvol_by_id(lvol_id)
     if not lvol:
         logger.error(f"LVol not found: {lvol_id}")
         return False
 
     snode = db_controller.get_storage_node_by_id(lvol.node_id)
     logger.info("Sending cluster map")
-    snodes = db_controller.get_storage_nodes()
-    logger.info(f"Sending to: {snode.get_id()}")
-    rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
-    cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-    cluster_map_data['UUID_node_target'] = snode.get_id()
-    ret = rpc_client.distr_send_cluster_map(cluster_map_data)
-    return ret
+    return distr_controller.send_cluster_map_to_node(snode)
 
 
 def get_cluster_map(lvol_id):
     lvol = db_controller.get_lvol_by_id(lvol_id)
     if not lvol:
         logger.error(f"LVol not found: {lvol_id}")
         return False
@@ -1372,18 +1405,18 @@
             logger.error(f"Node is online!: {src_node.get_id()}, use --force to force move")
             return False
 
     if migrate(lvol_id, node_id):
         if src_node.status == StorageNode.STATUS_ONLINE:
             # delete lvol
             if lvol.ha_type == 'single':
-                delete_lvol_from_node(lvol, lvol.node_id)
+                delete_lvol_from_node(lvol_id, lvol.node_id, clear_data=False)
             elif lvol.ha_type == "ha":
                 for nodes_id in lvol.nodes:
-                    delete_lvol_from_node(lvol, nodes_id)
+                    delete_lvol_from_node(lvol_id, nodes_id, clear_data=False)
 
             # remove from storage node
             src_node.lvols.remove(lvol_id)
             src_node.write_to_db(db_controller.kv_store)
         return True
     else:
         logger.error("Failed to migrate lvol")
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/controllers/pool_events.py` & `sbcli_mig-1.0.90/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_mig-1.0.90/simplyblock_core/controllers/caching_node_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                     'cluster_id': snode.cluster_id,
                     'status': 'online'
                 }))
             sequential_number += device_partitions_count
     return devices
 
 
-def add_node(cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask, spdk_mem, spdk_image=None):
+def add_node(cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask, spdk_mem, spdk_image=None, namespace=None):
     db_controller = DBController()
     kv_store = db_controller.kv_store
 
     cluster = db_controller.get_cluster_by_id(cluster_id)
     if not cluster:
         logger.error("Cluster not found: %s", cluster_id)
         return False
@@ -151,19 +151,34 @@
         #     logger.warning(f"Free hugepages are less than 1G: {utils.humanbytes(huge_free)}")
         if not spdk_mem:
             spdk_mem = memory_details['free']
 
     logger.info(f"Trying to set hugepages for: {utils.humanbytes(spdk_mem)}")
     logger.info("Deploying SPDK")
     results, err = snode_api.spdk_process_start(
-        spdk_cpu_mask, spdk_mem, spdk_image, snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
+        spdk_cpu_mask, spdk_mem, spdk_image, snode.mgmt_ip,
+        snode.rpc_port, snode.rpc_username, snode.rpc_password, namespace)
     if not results:
         logger.error(f"Failed to start spdk: {err}")
         return False
-    time.sleep(5)
+
+    retries = 20
+    while retries > 0:
+        resp, _ = snode_api.spdk_process_is_up()
+        if resp:
+            logger.info(f"Pod is up")
+            break
+        else:
+            logger.info("Pod is not running, waiting...")
+            time.sleep(3)
+            retries -= 1
+
+    if retries == 0:
+        logger.error("Pod is not running, exiting")
+        return False
 
     # creating RPCClient instance
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password,
         timeout=60*5, retry=5)
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_mig-1.0.90/simplyblock_core/controllers/snapshot_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     logger.info(f"Creating snapshot: {snapshot_name} from LVol: {lvol.id}")
     snode = db_controller.get_storage_node_by_id(lvol.node_id)
 
 
 ##############################################################################
     snap_count = 0
     for sn in db_controller.get_snapshots():
-        if sn.lvol_id == lvol_id:
+        if sn.lvol.get_id() == lvol_id:
             snap_count += 1
 
     rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
     spdk_mem_info_before = rpc_client.ultra21_util_get_malloc_stats()
 
     num_blocks = int(lvol.size / lvol.distr_bs)
     new_vuid = utils.get_random_vuid()
@@ -50,18 +50,17 @@
         base_name, new_vuid, lvol.ndcs, lvol.npcs, num_blocks,
         lvol.distr_bs, lvol_controller.get_jm_names(snode), lvol.distr_chunk_bs,
         None, None, lvol.distr_page_size)
     if not ret:
         logger.error("Failed to create Distr bdev")
         return False, "Failed to create Distr bdev"
 
-    snodes = db_controller.get_storage_nodes()
-    cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-    cluster_map_data['UUID_node_target'] = snode.get_id()
-    rpc_client.distr_send_cluster_map(cluster_map_data)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
 
     ret = rpc_client.ultra21_lvol_bmap_init(
         base_name, num_blocks, lvol.distr_bs, int(lvol.distr_page_size / lvol.distr_bs), num_blocks * 10)
     if not ret:
         return False, "Failed to init distr bdev"
 
     logger.info("Creating Snapshot bdev")
@@ -134,22 +133,22 @@
     # creating RPCClient instance
     rpc_client = RPCClient(
         snode.mgmt_ip,
         snode.rpc_port,
         snode.rpc_username,
         snode.rpc_password)
 
-    ret = rpc_client.bdev_distrib_delete(snap.base_bdev)
+    ret = rpc_client.ultra21_lvol_dismount(snap.snap_bdev)
     if not ret:
-        logger.error(f"Failed to delete BDev {snap.base_bdev}")
+        logger.error(f"Failed to delete BDev {snap.snap_bdev}")
         return False
 
-    ret = rpc_client.ultra21_lvol_dismount(snap.snap_bdev)
+    ret = rpc_client.bdev_distrib_delete(snap.base_bdev)
     if not ret:
-        logger.error(f"Failed to delete BDev {snap.snap_bdev}")
+        logger.error(f"Failed to delete BDev {snap.base_bdev}")
         return False
 
     snap.remove(db_controller.kv_store)
 
     base_lvol = db_controller.get_lvol_by_id(snap.lvol.get_id())
     if base_lvol.deleted is True:
         lvol_controller.delete_lvol(base_lvol.get_id())
@@ -229,18 +228,17 @@
         logger.error("Failed to create Distr bdev")
         return False, "Failed to create Distr bdev"
     if ret == "?":
         logger.error(f"Failed to create Distr bdev, ret={ret}")
         # return False
 
     logger.info("Sending cluster map to the lvol")
-    snodes = db_controller.get_storage_nodes()
-    cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
-    cluster_map_data['UUID_node_target'] = snode.get_id()
-    ret = rpc_client.distr_send_cluster_map(cluster_map_data)
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
 
     logger.info("Creating clone bdev")
     block_len = lvol.distr_bs
     page_len = int(lvol.distr_page_size / lvol.distr_bs)
     max_num_blocks = num_blocks * 10
     ret = rpc_client.ultra21_lvol_bmap_init(name, num_blocks, block_len, page_len, max_num_blocks)
     if not ret:
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/controllers/mgmt_events.py` & `sbcli_mig-1.0.90/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/controllers/device_controller.py` & `sbcli_mig-1.0.90/simplyblock_core/controllers/device_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,20 +74,28 @@
     return device_set_state(device_id, NVMeDevice.STATUS_READONLY)
 
 
 def device_set_online(device_id):
     return device_set_state(device_id, NVMeDevice.STATUS_ONLINE)
 
 
+def get_alceml_name(alceml_id):
+    return f"alceml_{alceml_id}"
+
+
 def restart_device(device_id):
     db_controller = DBController()
     dev = db_controller.get_storage_devices(device_id)
     if not dev:
         logger.error("device not found")
 
+    if dev.status != NVMeDevice.STATUS_REMOVED:
+        logger.error("Device must be in removed status")
+        return False
+
     snode = db_controller.get_storage_node_by_id(dev.node_id)
     if not snode:
         logger.error("node not found")
         return False
 
     device_obj = None
     for dev in snode.nvme_devices:
@@ -110,17 +118,15 @@
     # create testing bdev
     ret = rpc_client.bdev_passtest_create(test_name, device_obj.nvme_bdev)
     if not ret:
         logger.error(f"Failed to create bdev: {test_name}")
         return False
 
     alceml_id = device_obj.get_id()
-    node_id_mini = snode.get_id().split("-")[-1]
-    alceml_id_mini = alceml_id.split("-")[-1]
-    alceml_name = f"node_{node_id_mini}_dev_{alceml_id_mini}"
+    alceml_name = get_alceml_name(alceml_id)
     logger.info(f"adding {alceml_name}")
     ret = rpc_client.bdev_alceml_create(alceml_name, test_name, alceml_id, pba_init_mode=2)
     if not ret:
         logger.error(f"Failed to create alceml bdev: {alceml_name}")
         return False
 
     # add pass through
@@ -191,30 +197,29 @@
                 idx = i
                 break
         if idx >= 0:
             node.remote_devices[idx] = device_obj
         else:
             node.remote_devices.append(device_obj)
         node.write_to_db(db_controller.kv_store)
+        time.sleep(3)
 
     logger.info("Sending device event")
     distr_controller.send_dev_status_event(device_obj.cluster_device_order, "online")
     device_events.device_restarted(device_obj)
 
-    for lvol in db_controller.get_lvols():
-        lvol_controller.send_cluster_map(lvol.get_id())
-
     return "Done"
 
 
 def set_device_testing_mode(device_id, mode):
     db_controller = DBController()
     device = db_controller.get_storage_devices(device_id)
     if not device:
         logger.error("device not found")
+        return False
 
     snode = db_controller.get_storage_node_by_id(device.node_id)
     if not snode:
         logger.error("node not found")
         return False
 
     logger.info(f"Set device:{device_id} Test mode:{mode}")
@@ -399,23 +404,31 @@
         logger.error(f"Node not found {device.node_id}")
         return False
 
     if device.status == NVMeDevice.STATUS_REMOVED:
         logger.error(f"Device status: {device.status} is removed")
         return False
 
+    logger.info("Setting device to unavailable")
+    old_status = device.status
+    device.status = NVMeDevice.STATUS_UNAVAILABLE
+    distr_controller.send_dev_status_event(device.cluster_device_order, device.status)
+    snode.write_to_db(db_controller.kv_store)
+    device_events.device_status_change(device, device.status, old_status)
+
     logger.info("Resetting device")
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password)
 
     controller_name = device.nvme_bdev[:-2]
     response = rpc_client.reset_device(controller_name)
     if not response:
         logger.error(f"Failed to reset NVMe BDev {controller_name}")
         return False
 
     device.io_error = False
-    device.status = NVMeDevice.STATUS_ONLINE
     snode.write_to_db(db_controller.kv_store)
+
     device_events.device_reset(device)
+    device_set_online(dev_id)
     return True
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/controllers/lvol_events.py` & `sbcli_mig-1.0.90/simplyblock_core/controllers/lvol_events.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,13 +29,17 @@
 
 
 def lvol_status_change(lvol, new_state, old_status, caused_by=ec.CAUSED_BY_CLI):
     _lvol_event(lvol, f"LVol status changed from: {old_status} to: {new_state}", caused_by, ec.EVENT_STATUS_CHANGE)
 
 
 def lvol_migrate(lvol, old_node, new_node, caused_by=ec.CAUSED_BY_CLI):
-    _lvol_event(lvol, f"LVol migrated from: {old_node}, to {new_node}", caused_by, ec.EVENT_STATUS_CHANGE)
+    _lvol_event(lvol, f"LVol migrated from: {old_node}, \nto {new_node}", caused_by, ec.EVENT_STATUS_CHANGE)
 
 
 def lvol_health_check_change(lvol, new_state, old_status, caused_by=ec.CAUSED_BY_CLI):
     _lvol_event(lvol, f"LVol health check changed from: {old_status} to: {new_state}", caused_by, ec.EVENT_STATUS_CHANGE)
 
+
+def lvol_io_error_change(lvol, new_state, old_status, caused_by=ec.CAUSED_BY_CLI):
+    _lvol_event(lvol, f"LVol IO Error changed from: {old_status} to: {new_state}", caused_by, ec.EVENT_STATUS_CHANGE)
+
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/controllers/device_events.py` & `sbcli_mig-1.0.90/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/controllers/snapshot_events.py` & `sbcli_mig-1.0.90/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.9/simplyblock_core/controllers/health_controller.py` & `sbcli_mig-1.0.90/simplyblock_core/controllers/health_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         logger.error("node not found")
         return False
 
     if snode.status in [StorageNode.STATUS_OFFLINE, StorageNode.STATUS_REMOVED]:
         logger.info(f"Skipping ,node status is {snode.status}")
         return True
 
-    if device.status in [NVMeDevice.STATUS_REMOVED, NVMeDevice.STATUS_UNRECOGNIZED]:
+    if device.status in [NVMeDevice.STATUS_REMOVED, NVMeDevice.STATUS_FAILED]:
         logger.info(f"Skipping ,device status is {device.status}")
         return True
 
     passed = True
     try:
         rpc_client = RPCClient(
             snode.mgmt_ip, snode.rpc_port,
```

## Comparing `sbcli-mig-1.0.9/simplyblock_core/controllers/pool_controller.py` & `sbcli_mig-1.0.90/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

