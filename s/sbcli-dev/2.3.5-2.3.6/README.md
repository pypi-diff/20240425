# Comparing `tmp/sbcli_dev-2.3.5.zip` & `tmp/sbcli_dev-2.3.6.zip`

## zipinfo {}

```diff
@@ -1,146 +1,146 @@
-Zip file size: 182218 bytes, number of entries: 144
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 14:56 sbcli_dev-2.3.5/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 14:56 sbcli_dev-2.3.5/sbcli_dev.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/
--rw-r--r--  2.0 unx     2251 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/setup.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/README.md
--rw-r--r--  2.0 unx      148 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/env_var
--rw-r--r--  2.0 unx       84 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/pyproject.toml
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/setup.cfg
--rw-r--r--  2.0 unx     1467 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/PKG-INFO
--rw-r--r--  2.0 unx    77199 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_cli/main.py
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/sbcli_dev.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     5072 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/sbcli_dev.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/sbcli_dev.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1467 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/sbcli_dev.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       66 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/sbcli_dev.egg-info/requires.txt
--rw-r--r--  2.0 unx       55 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/sbcli_dev.egg-info/entry_points.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/
--rw-r--r--  2.0 unx    64978 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1440 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3153 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx      279 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx      938 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3193 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     8189 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     7640 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/utils.py
--rw-r--r--  2.0 unx    23335 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx     5112 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    21493 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     7401 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx     2189 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx     3203 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     5462 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx      229 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     5262 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     2410 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5123 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx     7439 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2423 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     2499 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     4118 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx      837 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2671 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6577 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/services/storage_node_monitor.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx      694 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx      152 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx     8081 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx      453 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx     1694 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx      311 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx      360 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx       43 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1420 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx      187 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/prometheus.yml
--rwxr-xr-x  2.0 unx      622 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx     5860 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1853 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx    98143 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx    98086 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    98031 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    98198 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    98031 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/pools.json
--rw-r--r--  2.0 unx    13922 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1120 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     1961 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx     1521 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1630 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    10557 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx    10375 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1900 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx    22847 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx    47339 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx    11294 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx     1500 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx      806 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4846 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      917 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx      736 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     1602 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     1228 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     1020 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx     3421 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     4242 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     2565 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx     3766 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     2071 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_core/models/nvme_device.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/
--rw-r--r--  2.0 unx      725 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     5098 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx      703 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     1263 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     2513 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1434 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      507 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      322 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      434 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      827 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx     1302 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     2876 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5547 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     4795 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5317 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     9573 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx     8547 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx    11244 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx    12198 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx      975 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     6326 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     7846 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     2940 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     5274 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     3103 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx     6206 b- defN 24-Apr-24 14:56 sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_pool.py
-144 files, 1085606 bytes uncompressed, 156084 bytes compressed:  85.6%
+Zip file size: 183601 bytes, number of entries: 144
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:22 sbcli_dev-2.3.6/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:22 sbcli_dev-2.3.6/sbcli_dev.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/
+-rw-r--r--  2.0 unx     2251 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/setup.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/README.md
+-rw-r--r--  2.0 unx      148 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/env_var
+-rw-r--r--  2.0 unx       84 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/pyproject.toml
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/setup.cfg
+-rw-r--r--  2.0 unx     1467 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/PKG-INFO
+-rw-r--r--  2.0 unx    77199 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_cli/main.py
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/sbcli_dev.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     5072 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/sbcli_dev.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/sbcli_dev.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1467 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/sbcli_dev.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/sbcli_dev.egg-info/requires.txt
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/sbcli_dev.egg-info/entry_points.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/
+-rw-r--r--  2.0 unx    65054 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1440 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx      279 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8189 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx    23335 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    21493 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     7401 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx      229 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     5262 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     2410 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5140 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx     7439 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx      837 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6577 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/services/storage_node_monitor.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx     8081 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx     1694 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx      311 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1420 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx      187 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/prometheus.yml
+-rwxr-xr-x  2.0 unx      622 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx     5860 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1853 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx   106705 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    99758 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    99862 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/pools.json
+-rw-r--r--  2.0 unx    13922 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     1961 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10557 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx    22847 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx    47339 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx    11294 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx      806 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx     3421 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_core/models/nvme_device.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/
+-rw-r--r--  2.0 unx      725 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx      703 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     2513 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      322 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      434 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      827 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5547 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     4795 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5317 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     9573 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx     8547 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx      975 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     7846 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     5274 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-Apr-25 15:22 sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_pool.py
+144 files, 1100949 bytes uncompressed, 157467 bytes compressed:  85.7%
```

## zipnote {}

```diff
@@ -1,433 +1,433 @@
-Filename: sbcli_dev-2.3.5/
+Filename: sbcli_dev-2.3.6/
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_cli/
+Filename: sbcli_dev-2.3.6/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_dev-2.3.5/sbcli_dev.egg-info/
+Filename: sbcli_dev-2.3.6/sbcli_dev.egg-info/
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/
+Filename: sbcli_dev-2.3.6/simplyblock_core/
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/
+Filename: sbcli_dev-2.3.6/simplyblock_web/
 Comment: 
 
-Filename: sbcli_dev-2.3.5/setup.py
+Filename: sbcli_dev-2.3.6/setup.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/README.md
+Filename: sbcli_dev-2.3.6/README.md
 Comment: 
 
-Filename: sbcli_dev-2.3.5/env_var
+Filename: sbcli_dev-2.3.6/env_var
 Comment: 
 
-Filename: sbcli_dev-2.3.5/pyproject.toml
+Filename: sbcli_dev-2.3.6/pyproject.toml
 Comment: 
 
-Filename: sbcli_dev-2.3.5/setup.cfg
+Filename: sbcli_dev-2.3.6/setup.cfg
 Comment: 
 
-Filename: sbcli_dev-2.3.5/PKG-INFO
+Filename: sbcli_dev-2.3.6/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_cli/cli.py
+Filename: sbcli_dev-2.3.6/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_cli/main.py
+Filename: sbcli_dev-2.3.6/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/sbcli_dev.egg-info/dependency_links.txt
+Filename: sbcli_dev-2.3.6/sbcli_dev.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli_dev-2.3.5/sbcli_dev.egg-info/SOURCES.txt
+Filename: sbcli_dev-2.3.6/sbcli_dev.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_dev-2.3.5/sbcli_dev.egg-info/top_level.txt
+Filename: sbcli_dev-2.3.6/sbcli_dev.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_dev-2.3.5/sbcli_dev.egg-info/PKG-INFO
+Filename: sbcli_dev-2.3.6/sbcli_dev.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.3.5/sbcli_dev.egg-info/requires.txt
+Filename: sbcli_dev-2.3.6/sbcli_dev.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_dev-2.3.5/sbcli_dev.egg-info/entry_points.txt
+Filename: sbcli_dev-2.3.6/sbcli_dev.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/storage_node_ops.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/constants.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/cnode_client.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/shell_utils.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/pci_utils.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/__init__.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/snode_client.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/kv_store.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/utils.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/cluster_ops.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/compute_node_ops.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/rpc_client.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/distr_controller.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/health_check_service.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/service_template.service
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/remove_service.sh
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/device_monitor.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/__init__.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/install_service.sh
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/alerting/
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/__init__.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/pools.json
+Filename: sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/pools.json
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/device_events.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/__init__.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/events.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/iface.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/base_model.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/lvol_model.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/compute_node.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/snapshot.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/pool.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/global_settings.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/port_stat.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/storage_node.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/__init__.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/stats.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/cluster.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/caching_node.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_core/models/nvme_device.py
+Filename: sbcli_dev-2.3.6/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/static/
+Filename: sbcli_dev-2.3.6/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/templates/
+Filename: sbcli_dev-2.3.6/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/node_utils.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/snode_app.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/app.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/auth_middleware.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/__init__.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/caching_node_app.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/utils.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/node_webapp.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_dev-2.3.6/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/static/tst.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/static/is_up.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/static/delete.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/static/deploy.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_dev-2.3.6/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/static/rpac.yaml
+Filename: sbcli_dev-2.3.6/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/static/list_deps.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_dev-2.3.6/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/csi.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_dev-2.3.5/setup.py` & `sbcli_dev-2.3.6/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/README.md` & `sbcli_dev-2.3.6/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/PKG-INFO` & `sbcli_dev-2.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.3.5
+Version: 2.3.6
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.3.5/simplyblock_cli/cli.py` & `sbcli_dev-2.3.6/simplyblock_cli/cli.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/sbcli_dev.egg-info/SOURCES.txt` & `sbcli_dev-2.3.6/sbcli_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/sbcli_dev.egg-info/PKG-INFO` & `sbcli_dev-2.3.6/sbcli_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.3.5
+Version: 2.3.6
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.3.5/simplyblock_core/storage_node_ops.py` & `sbcli_dev-2.3.6/simplyblock_core/storage_node_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -797,14 +797,16 @@
                 snapshot_controller.delete(sn.get_id())
         else:
             logger.error("Snapshots found on the storage node, use --force-remove or --force-migrate")
             return False
 
     if snode.nvme_devices:
         for dev in snode.nvme_devices:
+            if dev.status == NVMeDevice.STATUS_JM:
+                continue
             if dev.status == 'online':
                 distr_controller.disconnect_device(dev)
             old_status = dev.status
             dev.status = NVMeDevice.STATUS_FAILED
             distr_controller.send_dev_status_event(dev.cluster_device_order, NVMeDevice.STATUS_FAILED)
             device_events.device_status_change(dev, NVMeDevice.STATUS_FAILED, old_status)
```

## Comparing `sbcli_dev-2.3.5/simplyblock_core/constants.py` & `sbcli_dev-2.3.6/simplyblock_core/constants.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/mgmt_node_ops.py` & `sbcli_dev-2.3.6/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/cnode_client.py` & `sbcli_dev-2.3.6/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/pci_utils.py` & `sbcli_dev-2.3.6/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/snode_client.py` & `sbcli_dev-2.3.6/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/kv_store.py` & `sbcli_dev-2.3.6/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/utils.py` & `sbcli_dev-2.3.6/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/cluster_ops.py` & `sbcli_dev-2.3.6/simplyblock_core/cluster_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/compute_node_ops.py` & `sbcli_dev-2.3.6/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/rpc_client.py` & `sbcli_dev-2.3.6/simplyblock_core/rpc_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/distr_controller.py` & `sbcli_dev-2.3.6/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/services/lvol_monitor.py` & `sbcli_dev-2.3.6/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/services/caching_node_monitor.py` & `sbcli_dev-2.3.6/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/services/health_check_service.py` & `sbcli_dev-2.3.6/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_dev-2.3.6/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/services/log_agg_service.py` & `sbcli_dev-2.3.6/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/services/distr_event_collector.py` & `sbcli_dev-2.3.6/simplyblock_core/services/distr_event_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             logger.info(f"Device not found!, storage id: {storage_id} from node: {node_id}")
             event.status = 'device_not_found'
             return
 
         if event.message == 'SPDK_BDEV_EVENT_REMOVE':
             logger.info(f"Removing storage id: {storage_id} from node: {node_id}")
             device_controller.device_remove(device_id)
-        elif event.message == 'error_write':
+        elif event.message in ['error_write', 'error_unmap']:
             logger.info(f"Setting device to read-only")
             device_controller.device_set_io_error(device_id, True)
             device_controller.device_set_read_only(device_id)
         else:
             logger.info(f"Setting device to unavailable")
             device_controller.device_set_io_error(device_id, True)
             device_controller.device_set_unavailable(device_id)
```

## Comparing `sbcli_dev-2.3.5/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_dev-2.3.6/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/services/port_stat_collector.py` & `sbcli_dev-2.3.6/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/services/device_monitor.py` & `sbcli_dev-2.3.6/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/services/__init__.py` & `sbcli_dev-2.3.6/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/services/install_service.sh` & `sbcli_dev-2.3.6/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_dev-2.3.6/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/services/cap_monitor.py` & `sbcli_dev-2.3.6/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/services/storage_node_monitor.py` & `sbcli_dev-2.3.6/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_dev-2.3.6/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/scripts/haproxy.cfg` & `sbcli_dev-2.3.6/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_dev-2.3.6/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_dev-2.3.6/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/scripts/__init__.py` & `sbcli_dev-2.3.6/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/scripts/install_deps.sh` & `sbcli_dev-2.3.6/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_dev-2.3.6/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_dev-2.3.6/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_dev-2.3.6/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/devices.json`

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

## Comparing `sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/nodes.json`

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

## Comparing `sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/lvols.json`

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

## Comparing `sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/cluster.json`

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

## Comparing `sbcli_dev-2.3.5/simplyblock_core/scripts/dashboards/pools.json` & `sbcli_dev-2.3.6/simplyblock_core/scripts/dashboards/pools.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9931863742404514%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}, 'gridPos': "*

 * *                "{'w': 7, 'y': 1}, 'id': 13, 'targets': {0: {'expr': 'pool_size_total'}}, 'title': "*

 * *                "'pool_size_total'}, 2: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}, "*

 * *                "'gridPos': {'w': 7, 'x': 7, 'y': 1}, 'id': 10, 'targets': {0: {'expr': "*

 * *                "'pool_size_free'}}, 'title': 'pool_size_free'}, 3: {'fieldConfig': {'defaults': "*

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
-                        "expr": "pool_write_latency_ticks",
+                        "expr": "pool_size_total",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_latency_ticks",
+                "title": "pool_size_total",
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
-                        "expr": "pool_write_latency_ps",
+                        "expr": "pool_size_free",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_latency_ps",
+                "title": "pool_size_free",
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
-                        "expr": "pool_write_io_ps",
+                        "expr": "pool_size_used",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_io_ps",
+                "title": "pool_size_used",
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
-                        "expr": "pool_write_io",
+                        "expr": "pool_size_prov",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_io",
+                "title": "pool_size_prov",
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
-                        "expr": "pool_write_bytes_ps",
+                        "expr": "pool_size_prov_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_bytes_ps",
+                "title": "pool_size_prov_util",
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
-                        "expr": "pool_write_bytes",
+                        "expr": "pool_size_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_bytes",
+                "title": "pool_size_util",
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
-                        "expr": "pool_unmap_latency_ticks",
+                        "expr": "pool_write_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_latency_ticks",
+                "title": "pool_write_bytes",
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
-                        "expr": "pool_unmap_latency_ps",
+                        "expr": "pool_write_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_latency_ps",
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
-                                        "{__name__=\"pool_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
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
@@ -867,21 +872,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_unmap_io_ps",
+                        "expr": "pool_write_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_io_ps",
+                "title": "pool_wite_latency_ticks",
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
@@ -959,21 +964,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_unmap_io",
+                        "expr": "pool_write_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_io",
+                "title": "pool_write_io",
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
+                    "y": 24
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
-                        "expr": "pool_unmap_bytes_ps",
+                        "expr": "pool_write_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_bytes_ps",
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
-                        "expr": "pool_unmap_bytes",
+                        "expr": "pool_write_latency_ps / 1000",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_bytes",
+                "title": "pool_write_latency_ps",
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
-                        "expr": "pool_size_util",
+                        "expr": "pool_read_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_util",
+                "title": "pool_read_bytes",
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
-                        "expr": "pool_size_used",
+                        "expr": "pool_read_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_used",
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
-                        "expr": "pool_size_total",
+                        "expr": "pool_read_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_total",
+                "title": "pool_read_latency_ps",
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
-                        "expr": "pool_size_prov_util",
+                        "expr": "pool_read_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_prov_util",
+                "title": "pool_read_io",
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
-                        "expr": "pool_size_prov",
+                        "expr": "pool_read_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_prov",
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
-                        "expr": "pool_size_free",
+                        "expr": "pool_read_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_free",
+                "title": "pool_read_latency_ticks",
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
-                        "expr": "pool_record_start_time",
+                        "expr": "pool_unmap_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_record_start_time",
+                "title": "pool_unmap_latency_ticks",
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
-                        "expr": "pool_record_end_time",
+                        "expr": "pool_unmap_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_record_end_time",
+                "title": "pool_unmap_bytes_ps",
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
-                        "expr": "pool_record_duration",
+                        "expr": "pool_unmap_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_record_duration",
+                "title": "pool_unmap_latency_ps",
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
+                                        "{__name__=\"pool_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
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
-                        "expr": "pool_read_latency_ticks",
+                        "expr": "pool_unmap_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_latency_ticks",
+                "title": "pool_unmap_io_ps",
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
-                        "expr": "pool_read_latency_ps",
+                        "expr": "pool_unmap_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_latency_ps",
+                "title": "pool_unmap_io",
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
-                        "expr": "pool_read_io_ps",
+                        "expr": "pool_unmap_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_io_ps",
+                "title": "pool_unmap_bytes",
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
-                        "expr": "pool_read_io",
+                        "expr": "pool_record_end_time",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_io",
+                "title": "pool_record_end_time",
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
-                        "expr": "pool_read_bytes",
+                        "expr": "pool_record_duration",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_bytes",
+                "title": "pool_record_duration",
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
-                        "expr": "pool_read_bytes_ps",
+                        "expr": "pool_record_start_time",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_bytes_ps",
+                "title": "pool_record_start_time",
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
         "title": "PoolsDashboard",
         "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e40",
         "version": 5,
```

## Comparing `sbcli_dev-2.3.5/simplyblock_core/controllers/device_controller.py` & `sbcli_dev-2.3.6/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/controllers/mgmt_events.py` & `sbcli_dev-2.3.6/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/controllers/events_controller.py` & `sbcli_dev-2.3.6/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/controllers/storage_events.py` & `sbcli_dev-2.3.6/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/controllers/lvol_events.py` & `sbcli_dev-2.3.6/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_dev-2.3.6/simplyblock_core/controllers/snapshot_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/controllers/device_events.py` & `sbcli_dev-2.3.6/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/controllers/pool_controller.py` & `sbcli_dev-2.3.6/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/controllers/cluster_events.py` & `sbcli_dev-2.3.6/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_dev-2.3.6/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/controllers/snapshot_events.py` & `sbcli_dev-2.3.6/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/controllers/lvol_controller.py` & `sbcli_dev-2.3.6/simplyblock_core/controllers/lvol_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/controllers/health_controller.py` & `sbcli_dev-2.3.6/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/controllers/pool_events.py` & `sbcli_dev-2.3.6/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/events.py` & `sbcli_dev-2.3.6/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/iface.py` & `sbcli_dev-2.3.6/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/base_model.py` & `sbcli_dev-2.3.6/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/lvol_model.py` & `sbcli_dev-2.3.6/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/compute_node.py` & `sbcli_dev-2.3.6/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/snapshot.py` & `sbcli_dev-2.3.6/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/pool.py` & `sbcli_dev-2.3.6/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/global_settings.py` & `sbcli_dev-2.3.6/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/port_stat.py` & `sbcli_dev-2.3.6/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/storage_node.py` & `sbcli_dev-2.3.6/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/stats.py` & `sbcli_dev-2.3.6/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/cluster.py` & `sbcli_dev-2.3.6/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/mgmt_node.py` & `sbcli_dev-2.3.6/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/caching_node.py` & `sbcli_dev-2.3.6/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_core/models/nvme_device.py` & `sbcli_dev-2.3.6/simplyblock_core/models/nvme_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/caching_node_app_k8s.py` & `sbcli_dev-2.3.6/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/node_utils.py` & `sbcli_dev-2.3.6/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/snode_app.py` & `sbcli_dev-2.3.6/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/app.py` & `sbcli_dev-2.3.6/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/auth_middleware.py` & `sbcli_dev-2.3.6/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/caching_node_app.py` & `sbcli_dev-2.3.6/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/utils.py` & `sbcli_dev-2.3.6/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/node_webapp.py` & `sbcli_dev-2.3.6/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/static/delete.py` & `sbcli_dev-2.3.6/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/static/deploy.py` & `sbcli_dev-2.3.6/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_dev-2.3.6/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_dev-2.3.6/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_dev-2.3.6/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_dev-2.3.6/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/blueprints/snode_ops.py` & `sbcli_dev-2.3.6/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/blueprints/csi.py` & `sbcli_dev-2.3.6/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_dev-2.3.6/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_dev-2.3.6/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_device.py` & `sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_dev-2.3.6/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.3.5/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_dev-2.3.6/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

