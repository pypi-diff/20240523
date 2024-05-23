# Comparing `tmp/sbcli_dev-2.6.9.zip` & `tmp/sbcli_dev-2.7.0.zip`

## zipinfo {}

```diff
@@ -1,148 +1,150 @@
-Zip file size: 213640 bytes, number of entries: 146
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:44 sbcli_dev-2.6.9/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:44 sbcli_dev-2.6.9/sbcli_dev.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/
--rw-r--r--  2.0 unx     1068 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/README.md
--rw-r--r--  2.0 unx       84 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/pyproject.toml
--rw-r--r--  2.0 unx     1489 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/PKG-INFO
--rw-r--r--  2.0 unx      148 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/env_var
--rw-r--r--  2.0 unx       38 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/setup.cfg
--rw-r--r--  2.0 unx     2269 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/setup.py
--rw-r--r--  2.0 unx    78538 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_cli/main.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/templates/
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      703 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx      717 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx     5098 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx     2513 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1263 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/app.py
--rw-r--r--  2.0 unx      725 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx      322 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      827 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx      507 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      434 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     1302 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     6206 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     2940 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     8685 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx     9713 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx    12385 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx     6326 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx     6209 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     8075 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     4883 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5746 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     5491 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx    11244 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx      975 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     2905 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5188 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/sbcli_dev.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       73 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/sbcli_dev.egg-info/requires.txt
--rw-r--r--  2.0 unx     1489 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/sbcli_dev.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       49 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/sbcli_dev.egg-info/top_level.txt
--rw-r--r--  2.0 unx       55 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/sbcli_dev.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/sbcli_dev.egg-info/dependency_links.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/
--rw-r--r--  2.0 unx    24741 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx      938 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3193 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     8343 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     5112 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    22010 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     3153 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     7640 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/utils.py
--rw-r--r--  2.0 unx     7504 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx      279 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx     3638 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx    66443 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1501 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3203 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx      229 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx      837 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     4118 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx     2410 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5462 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx     7439 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     5268 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx     2671 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6577 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/storage_node_monitor.py
--rw-r--r--  2.0 unx     2423 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     5140 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2189 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx    10375 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1521 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx    48950 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx     1630 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    10598 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx     3191 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx    11294 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx    13877 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx    23312 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1900 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx     1120 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     3766 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     2094 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/nvme_device.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx      917 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     1500 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx     1228 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     4846 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      736 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     3696 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx     4242 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     1602 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx      806 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     2565 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1020 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/models/port_stat.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx     1420 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx     1782 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx       43 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx      118 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx      360 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx     5333 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx      152 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/set_db_config.sh
--rwxr-xr-x  2.0 unx      657 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx      311 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/prometheus.yml
--rw-r--r--  2.0 unx      311 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx     4409 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
--rw-r--r--  2.0 unx      930 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx       54 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx      453 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx    25433 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1856 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx    88820 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    88911 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    88776 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    88868 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/pools.json
--rw-r--r--  2.0 unx   799409 b- defN 24-May-23 13:44 sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/node-exporter.json
-146 files, 1882494 bytes uncompressed, 187062 bytes compressed:  90.1%
+Zip file size: 216043 bytes, number of entries: 148
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 15:38 sbcli_dev-2.7.0/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 15:38 sbcli_dev-2.7.0/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 15:38 sbcli_dev-2.7.0/simplyblock_web/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 15:38 sbcli_dev-2.7.0/sbcli_dev.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 15:38 sbcli_dev-2.7.0/simplyblock_core/
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/README.md
+-rw-r--r--  2.0 unx       84 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/pyproject.toml
+-rw-r--r--  2.0 unx     1489 b- defN 24-May-23 15:38 sbcli_dev-2.7.0/PKG-INFO
+-rw-r--r--  2.0 unx      148 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/env_var
+-rw-r--r--  2.0 unx       38 b- defN 24-May-23 15:38 sbcli_dev-2.7.0/setup.cfg
+-rw-r--r--  2.0 unx     2269 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/setup.py
+-rw-r--r--  2.0 unx    78181 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_cli/main.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 15:38 sbcli_dev-2.7.0/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 15:38 sbcli_dev-2.7.0/simplyblock_web/blueprints/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 15:38 sbcli_dev-2.7.0/simplyblock_web/templates/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      703 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx      717 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx     2513 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/app.py
+-rw-r--r--  2.0 unx      725 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx      322 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx      507 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      434 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_pool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     8547 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx     9573 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx     5274 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     8075 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     4883 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5547 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     5491 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx      975 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     2905 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5267 b- defN 24-May-23 15:38 sbcli_dev-2.7.0/sbcli_dev.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       73 b- defN 24-May-23 15:38 sbcli_dev-2.7.0/sbcli_dev.egg-info/requires.txt
+-rw-r--r--  2.0 unx     1489 b- defN 24-May-23 15:38 sbcli_dev-2.7.0/sbcli_dev.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       49 b- defN 24-May-23 15:38 sbcli_dev-2.7.0/sbcli_dev.egg-info/top_level.txt
+-rw-r--r--  2.0 unx       55 b- defN 24-May-23 15:38 sbcli_dev-2.7.0/sbcli_dev.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-23 15:38 sbcli_dev-2.7.0/sbcli_dev.egg-info/dependency_links.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 15:38 sbcli_dev-2.7.0/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 15:38 sbcli_dev-2.7.0/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 15:38 sbcli_dev-2.7.0/simplyblock_core/models/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 15:38 sbcli_dev-2.7.0/simplyblock_core/scripts/
+-rw-r--r--  2.0 unx    24107 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx      938 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8532 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    21493 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx     7504 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx      279 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx     3638 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx    66264 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1514 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/job_tasks.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx      229 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx      837 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     4118 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx     7439 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     3169 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     5268 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6577 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/storage_node_monitor.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     5140 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx    47534 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10557 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx     3191 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx    11294 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx    13916 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx    23245 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2094 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/nvme_device.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx      917 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx      973 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/job_schedule.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      736 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     3696 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx      806 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/models/port_stat.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 15:38 sbcli_dev-2.7.0/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 15:38 sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx     1420 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx     1782 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx       43 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx      118 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx     5611 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx      152 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/set_db_config.sh
+-rwxr-xr-x  2.0 unx      657 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/prometheus.yml
+-rw-r--r--  2.0 unx      311 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx     4409 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+-rw-r--r--  2.0 unx      930 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx       54 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx    25433 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1856 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx    99758 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    99862 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx   106705 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/pools.json
+-rw-r--r--  2.0 unx   799409 b- defN 24-May-23 15:37 sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/node-exporter.json
+148 files, 1934026 bytes uncompressed, 189095 bytes compressed:  90.2%
```

## zipnote {}

```diff
@@ -1,439 +1,445 @@
-Filename: sbcli_dev-2.6.9/
+Filename: sbcli_dev-2.7.0/
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_cli/
+Filename: sbcli_dev-2.7.0/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/
+Filename: sbcli_dev-2.7.0/simplyblock_web/
 Comment: 
 
-Filename: sbcli_dev-2.6.9/sbcli_dev.egg-info/
+Filename: sbcli_dev-2.7.0/sbcli_dev.egg-info/
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/
+Filename: sbcli_dev-2.7.0/simplyblock_core/
 Comment: 
 
-Filename: sbcli_dev-2.6.9/README.md
+Filename: sbcli_dev-2.7.0/README.md
 Comment: 
 
-Filename: sbcli_dev-2.6.9/pyproject.toml
+Filename: sbcli_dev-2.7.0/pyproject.toml
 Comment: 
 
-Filename: sbcli_dev-2.6.9/PKG-INFO
+Filename: sbcli_dev-2.7.0/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.6.9/env_var
+Filename: sbcli_dev-2.7.0/env_var
 Comment: 
 
-Filename: sbcli_dev-2.6.9/setup.cfg
+Filename: sbcli_dev-2.7.0/setup.cfg
 Comment: 
 
-Filename: sbcli_dev-2.6.9/setup.py
+Filename: sbcli_dev-2.7.0/setup.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_cli/cli.py
+Filename: sbcli_dev-2.7.0/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_cli/main.py
+Filename: sbcli_dev-2.7.0/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/static/
+Filename: sbcli_dev-2.7.0/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/templates/
+Filename: sbcli_dev-2.7.0/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/__init__.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/node_webapp.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/snode_app.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/caching_node_app.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/auth_middleware.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/node_utils.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/utils.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/app.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/static/tst.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/static/delete.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_dev-2.7.0/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/static/is_up.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_dev-2.7.0/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/static/rpac.yaml
+Filename: sbcli_dev-2.7.0/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/static/list_deps.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/static/deploy.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/csi.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_dev-2.7.0/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_dev-2.6.9/sbcli_dev.egg-info/SOURCES.txt
+Filename: sbcli_dev-2.7.0/sbcli_dev.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_dev-2.6.9/sbcli_dev.egg-info/requires.txt
+Filename: sbcli_dev-2.7.0/sbcli_dev.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_dev-2.6.9/sbcli_dev.egg-info/PKG-INFO
+Filename: sbcli_dev-2.7.0/sbcli_dev.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.6.9/sbcli_dev.egg-info/top_level.txt
+Filename: sbcli_dev-2.7.0/sbcli_dev.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_dev-2.6.9/sbcli_dev.egg-info/entry_points.txt
+Filename: sbcli_dev-2.7.0/sbcli_dev.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_dev-2.6.9/sbcli_dev.egg-info/dependency_links.txt
+Filename: sbcli_dev-2.7.0/sbcli_dev.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/cluster_ops.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/pci_utils.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/__init__.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/snode_client.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/kv_store.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/compute_node_ops.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/rpc_client.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/utils.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/distr_controller.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/shell_utils.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/cnode_client.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/storage_node_ops.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/constants.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/job_tasks.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/service_template.service
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/install_service.sh
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/__init__.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/health_check_service.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/device_monitor.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/remove_service.sh
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/__init__.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/device_events.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/caching_node.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/nvme_device.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/compute_node.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/__init__.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/events.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/global_settings.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/base_model.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/lvol_model.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/job_schedule.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/snapshot.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/storage_node.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/stats.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/pool.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/iface.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/cluster.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/models/port_stat.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/alerting/
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/
+Filename: sbcli_dev-2.7.0/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/__init__.py
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/pools.json
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/node-exporter.json
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/devices.json
+Comment: 
+
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/pools.json
+Comment: 
+
+Filename: sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/node-exporter.json
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_dev-2.6.9/README.md` & `sbcli_dev-2.7.0/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/PKG-INFO` & `sbcli_dev-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.6.9
+Version: 2.7.0
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.6.9/setup.py` & `sbcli_dev-2.7.0/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_cli/cli.py` & `sbcli_dev-2.7.0/simplyblock_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -432,21 +432,18 @@
         sub_command = self.add_sub_command(subparser, "check", 'Health check cluster')
         sub_command.add_argument("id", help='cluster UUID')
 
         # update cluster
         sub_command = self.add_sub_command(subparser, "update", 'Update cluster mgmt services')
         sub_command.add_argument("id", help='cluster UUID')
 
-        # graceful-shutdown storage nodes
-        sub_command = self.add_sub_command(subparser, "graceful-shutdown", 'Graceful shutdown of storage nodes')
-        sub_command.add_argument("id", help='cluster UUID')
+        # get tasks list
+        sub_command = self.add_sub_command(subparser, "list-tasks", 'List tasks by cluster ID')
+        sub_command.add_argument("cluster_id", help='UUID of the cluster')
 
-        # graceful-startup storage nodes
-        sub_command = self.add_sub_command(subparser, "graceful-startup", 'Graceful startup of storage nodes')
-        sub_command.add_argument("id", help='cluster UUID')
 
         # lvol ops
         subparser = self.add_command('lvol', 'LVol commands')
         # add lvol
         sub_command = self.add_sub_command(subparser, 'add', 'Add a new logical volume')
         sub_command.add_argument("name", help='LVol name or id')
         sub_command.add_argument("size", help='LVol size: 10M, 10G, 10(bytes)')
@@ -1045,18 +1042,18 @@
             elif sub_command == "check":
                 cluster_id = args.id
                 ret = health_controller.check_cluster(cluster_id)
             elif sub_command == "get":
                 ret = cluster_ops.get_cluster(args.id)
             elif sub_command == "update":
                 ret = cluster_ops.update_cluster(args.id)
-            elif sub_command == "graceful-shutdown":
-                ret = cluster_ops.cluster_grace_shutdown(args.id)
-            elif sub_command == "graceful-startup":
-                ret = cluster_ops.cluster_grace_startup(args.id)
+
+            elif sub_command == "list-tasks":
+                ret = cluster_ops.list_tasks(args.cluster_id)
+
             else:
                 self.parser.print_help()
 
         elif args.command == 'compute-node':
             sub_command = args_dict[args.command]
             if sub_command == "add":
                 ret = compute_ops.add_compute_node(self.db_store)
```

## Comparing `sbcli_dev-2.6.9/simplyblock_web/node_webapp.py` & `sbcli_dev-2.7.0/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/snode_app.py` & `sbcli_dev-2.7.0/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/caching_node_app.py` & `sbcli_dev-2.7.0/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/auth_middleware.py` & `sbcli_dev-2.7.0/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/node_utils.py` & `sbcli_dev-2.7.0/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/utils.py` & `sbcli_dev-2.7.0/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/app.py` & `sbcli_dev-2.7.0/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/caching_node_app_k8s.py` & `sbcli_dev-2.7.0/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/static/delete.py` & `sbcli_dev-2.7.0/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_dev-2.7.0/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/static/deploy.py` & `sbcli_dev-2.7.0/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_device.py` & `sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,14 @@
         | distr_vuid      | Distr bdev virtual unique ID, Default=0 means random
         | distr_ndcs      | Distr bdev number of data chunks per stripe, Default=0 means auto set
         | distr_npcs      | Distr bdev number of parity chunks per stripe, Default=0 means auto set
         | distr_bs        | Distr bdev block size, Default=4096
         | distr_chunk_bs  | Distr bdev chunk block size, Default=4096
         | crypto_key1     | the hex value of key1 to be used for lvol encryption
         | crypto_key2     | the hex value of key2 to be used for lvol encryption
-        | host_id         | the hostID on which the lvol is created
     """""
 
     cl_data = request.get_json()
     logger.debug(cl_data)
     if 'size' not in cl_data:
         return utils.get_csi_response(None, "missing required param: size", 400)
     if 'name' not in cl_data:
@@ -139,30 +138,29 @@
     distr_vuid = utils.get_int_value_or_default(cl_data, "distr_vuid", 0)
     distr_ndcs = utils.get_int_value_or_default(cl_data, "distr_ndcs", 0)
     distr_npcs = utils.get_int_value_or_default(cl_data, "distr_npcs", 0)
     distr_bs = utils.get_int_value_or_default(cl_data, "distr_ps", 4096)
     distr_chunk_bs = utils.get_int_value_or_default(cl_data, "distr_chunk_bs", 4096)
     crypto_key1 = utils.get_value_or_default(cl_data, "crypto_key1", None)
     crypto_key2 = utils.get_value_or_default(cl_data, "crypto_key2", None)
-    host_id = utils.get_value_or_default(cl_data, "host_id", None)
 
     ret, error = lvol_controller.add_lvol_ha(
         name=name,
         size=size,
         pool_id_or_name=pool.get_id(),
 
         use_comp=compression,
         use_crypto=encryption,
 
         max_rw_iops=rw_iops,
         max_rw_mbytes=rw_mbytes,
         max_r_mbytes=r_mbytes,
         max_w_mbytes=w_mbytes,
 
-        host_id_or_name=host_id,
+        host_id_or_name=None,
         ha_type=ha_type,
         distr_vuid=distr_vuid,
         distr_ndcs=distr_ndcs,
         distr_npcs=distr_npcs,
         distr_bs=distr_bs,
         distr_chunk_bs=distr_chunk_bs,
         crypto_key1=crypto_key1,
```

## Comparing `sbcli_dev-2.6.9/simplyblock_web/blueprints/snode_ops.py` & `sbcli_dev-2.7.0/simplyblock_web/blueprints/snode_ops.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,24 +27,14 @@
 system_id = ""
 try:
     system_id, _, _ = node_utils.run_command("dmidecode -s system-uuid")
 except:
     pass
 
 
-def get_docker_client():
-    ip = os.getenv("DOCKER_IP")
-    if not ip:
-        for ifname in node_utils.get_nics_data():
-            if ifname in ["eth0", "ens0"]:
-                ip = node_utils.get_nics_data()[ifname]['ip']
-                break
-    return docker.DockerClient(base_url=f"tcp://{ip}:2375", version="auto", timeout=60 * 5)
-
-
 @bp.route('/scan_devices', methods=['GET'])
 def scan_devices():
     run_health_check = request.args.get('run_health_check', default=False, type=bool)
     out = {
         "nvme_devices": node_utils._get_nvme_devices(),
         "nvme_pcie_list": node_utils._get_nvme_pcie_list(),
         "spdk_devices": node_utils._get_spdk_devices(),
@@ -86,15 +76,15 @@
         spdk_cpu_mask = hex(int(math.pow(2, node_cpu_count)) - 1)
 
     if spdk_mem:
         spdk_mem = int(utils.parse_size(spdk_mem) / (1000 * 1000))
     else:
         spdk_mem = 4000
 
-    node_docker = get_docker_client()
+    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
     nodes = node_docker.containers.list(all=True)
     for node in nodes:
         if node.attrs["Name"] in ["/spdk", "/spdk_proxy"]:
             logger.info(f"{node.attrs['Name']} container found, removing...")
             node.stop()
             node.remove(force=True)
             time.sleep(2)
@@ -159,26 +149,26 @@
     return utils.get_response(
         False, f"Container create max retries reached, Container status: {status}, Is Running: {is_running}")
 
 
 @bp.route('/spdk_process_kill', methods=['GET'])
 def spdk_process_kill():
     force = request.args.get('force', default=False, type=bool)
-    node_docker = get_docker_client()
+    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
     for cont in node_docker.containers.list(all=True):
         logger.debug(cont.attrs)
         if cont.attrs['Name'] == "/spdk" or cont.attrs['Name'] == "/spdk_proxy":
             cont.stop()
             cont.remove(force=force)
     return utils.get_response(True)
 
 
 @bp.route('/spdk_process_is_up', methods=['GET'])
 def spdk_process_is_up():
-    node_docker = get_docker_client()
+    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
     for cont in node_docker.containers.list(all=True):
         logger.debug(cont.attrs)
         if cont.attrs['Name'] == "/spdk":
             status = cont.attrs['State']["Status"]
             is_running = cont.attrs['State']["Running"]
             if is_running:
                 return utils.get_response(True)
@@ -199,27 +189,27 @@
 
 def delete_cluster_id():
     out, _, _ = node_utils.run_command(f"rm -f {cluster_id_file}")
     return out
 
 
 def get_ec2_meta():
-    stream = os.popen('curl -X PUT "http://169.254.169.254/latest/api/token" -H "X-aws-ec2-metadata-token-ttl-seconds: 1"')
+    stream = os.popen('curl -X PUT "http://169.254.169.254/latest/api/token" -H "X-aws-ec2-metadata-token-ttl-seconds: 21600"')
     token = stream.read()
     stream = os.popen(f"curl -H \"X-aws-ec2-metadata-token: {token}\" http://169.254.169.254/latest/dynamic/instance-identity/document")
     out = stream.read()
     try:
         data = json.loads(out)
         return data
     except:
         return {}
 
 
 def get_ec2_public_ip():
-    stream = os.popen('curl -X PUT "http://169.254.169.254/latest/api/token" -H "X-aws-ec2-metadata-token-ttl-seconds: 1"')
+    stream = os.popen('curl -X PUT "http://169.254.169.254/latest/api/token" -H "X-aws-ec2-metadata-token-ttl-seconds: 21600"')
     token = stream.read()
     stream = os.popen(f"curl -H \"X-aws-ec2-metadata-token: {token}\" http://169.254.169.254/latest/meta-data/public-ipv4")
     response = stream.read()
     out = response if "404" not in response else None
     return out
 
 
@@ -263,15 +253,15 @@
     db_connection = data['db_connection']
 
     logger.info("Setting DB connection")
     scripts.set_db_config(db_connection)
     set_cluster_id(cluster_id)
 
     logger.info("Joining Swarm")
-    node_docker = get_docker_client()
+    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
     if node_docker.info()["Swarm"]["LocalNodeState"] == "active":
         logger.info("Node is part of another swarm, leaving swarm")
         node_docker.swarm.leave(force=True)
         time.sleep(2)
     node_docker.swarm.join([f"{cluster_ip}:2377"], join_token)
     retries = 10
     while retries > 0:
@@ -294,12 +284,12 @@
     return utils.get_response(True)
 
 
 @bp.route('/leave_swarm', methods=['GET'])
 def leave_swarm():
     delete_cluster_id()
     try:
-        node_docker = get_docker_client()
+        node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
         node_docker.swarm.leave(force=True)
     except:
         pass
     return utils.get_response(True)
```

## Comparing `sbcli_dev-2.6.9/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_dev-2.7.0/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,14 @@
 from simplyblock_core import scripts, constants
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 bp = Blueprint("caching_node", __name__, url_prefix="/cnode")
 
 
-def get_docker_client():
-    ip = os.getenv("DOCKER_IP")
-    if not ip:
-        for ifname in node_utils.get_nics_data():
-            if ifname in ["eth0", "ens0"]:
-                ip = node_utils.get_nics_data()[ifname]['ip']
-                break
-    return docker.DockerClient(base_url=f"tcp://{ip}:2375", version="auto", timeout=60 * 5)
-
-
 def run_command(cmd):
     process = subprocess.Popen(
         cmd.split(), stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     stdout, stderr = process.communicate()
     return stdout.strip().decode("utf-8"), stderr.strip(), process.returncode
 
 
@@ -160,15 +150,15 @@
         spdk_cpu_mask = hex(int(math.pow(2, node_cpu_count)) - 1)
 
     if spdk_mem:
         spdk_mem = int(spdk_mem / (1024 * 1024))
     else:
         spdk_mem = 64096
 
-    node_docker = get_docker_client()
+    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
     nodes = node_docker.containers.list(all=True)
     for node in nodes:
         if node.attrs["Name"] in ["/spdk", "/spdk_proxy"]:
             logger.info(f"{node.attrs['Name']} container found, removing...")
             node.stop()
             node.remove(force=True)
             time.sleep(2)
@@ -234,26 +224,26 @@
     return utils.get_response(
         False, f"Container create max retries reached, Container status: {status}, Is Running: {is_running}")
 
 
 @bp.route('/spdk_process_kill', methods=['GET'])
 def spdk_process_kill():
     force = request.args.get('force', default=False, type=bool)
-    node_docker = get_docker_client()
+    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
     for cont in node_docker.containers.list(all=True):
         logger.debug(cont.attrs)
         if cont.attrs['Name'] == "/spdk" or cont.attrs['Name'] == "/spdk_proxy":
             cont.stop()
             cont.remove(force=force)
     return utils.get_response(True)
 
 
 @bp.route('/spdk_process_is_up', methods=['GET'])
 def spdk_process_is_up():
-    node_docker = get_docker_client()
+    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
     for cont in node_docker.containers.list(all=True):
         logger.debug(cont.attrs)
         if cont.attrs['Name'] == "/spdk":
             status = cont.attrs['State']["Status"]
             is_running = cont.attrs['State']["Running"]
             if is_running:
                 return utils.get_response(True)
@@ -323,15 +313,15 @@
     data = request.get_json()
     db_connection = data['db_connection']
 
     logger.info("Setting DB connection")
     ret = scripts.set_db_config(db_connection)
 
     try:
-        node_docker = get_docker_client()
+        node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
         nodes = node_docker.containers.list(all=True)
         for node in nodes:
             if node.attrs["Name"] == "/spdk_proxy":
                 node_docker.containers.get(node.attrs["Id"]).restart()
                 break
     except:
         pass
```

## Comparing `sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python
 # encoding: utf-8
 import json
 import logging
-import threading
 import time
 import uuid
 
 from flask import Blueprint
 from flask import request
 
 from simplyblock_web import utils
@@ -142,32 +141,7 @@
         return utils.get_response_error(f"Cluster not found: {uuid}", 404)
     if cluster.status == Cluster.STATUS_INACTIVE:
         return utils.get_response("Cluster already inactive")
 
     data = cluster_ops.get_logs(uuid, is_json=True)
     return utils.get_response(json.loads(data))
 
-
-@bp.route('/cluster/gracefulshutdown/<string:uuid>', methods=['PUT'])
-def cluster_grace_shutdown(uuid):
-    cluster = db_controller.get_cluster_by_id(uuid)
-    if not cluster:
-        return utils.get_response_error(f"Cluster not found: {uuid}", 404)
-    t = threading.Thread(
-        target=cluster_ops.cluster_grace_shutdown,
-        args=(uuid,))
-    t.start()
-    # FIXME: Any failure within the thread are not handled
-    return utils.get_response(True)
-
-
-@bp.route('/cluster/gracefulstartup/<string:uuid>', methods=['PUT'])
-def cluster_grace_startup(uuid):
-    cluster = db_controller.get_cluster_by_id(uuid)
-    if not cluster:
-        return utils.get_response_error(f"Cluster not found: {uuid}", 404)
-    t = threading.Thread(
-        target=cluster_ops.cluster_grace_startup,
-        args=(uuid,))
-    t.start()
-    # FIXME: Any failure within the thread are not handled
-    return utils.get_response(True)
```

## Comparing `sbcli_dev-2.6.9/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_dev-2.7.0/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_dev-2.7.0/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_dev-2.7.0/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,32 +6,22 @@
 import time
 
 import docker
 from docker.types import LogConfig
 from flask import Blueprint
 from flask import request
 
-from simplyblock_web import utils, node_utils
+from simplyblock_web import utils
 from simplyblock_core import scripts, constants
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 bp = Blueprint("node_api_caching_docker", __name__, url_prefix="/cnode")
 
 
-def get_docker_client():
-    ip = os.getenv("DOCKER_IP")
-    if not ip:
-        for ifname in node_utils.get_nics_data():
-            if ifname in ["eth0", "ens0"]:
-                ip = node_utils.get_nics_data()[ifname]['ip']
-                break
-    return docker.DockerClient(base_url=f"tcp://{ip}:2375", version="auto", timeout=60 * 5)
-
-
 @bp.route('/spdk_process_start', methods=['POST'])
 def spdk_process_start():
     data = request.get_json()
 
     spdk_cpu_mask = None
     if 'spdk_cpu_mask' in data:
         spdk_cpu_mask = data['spdk_cpu_mask']
@@ -51,15 +41,15 @@
         spdk_cpu_mask = hex(int(math.pow(2, node_cpu_count)) - 1)
 
     if spdk_mem:
         spdk_mem = int(spdk_mem / (1024 * 1024))
     else:
         spdk_mem = 64096
 
-    node_docker = get_docker_client()
+    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
     nodes = node_docker.containers.list(all=True)
     for node in nodes:
         if node.attrs["Name"] in ["/spdk", "/spdk_proxy"]:
             logger.info(f"{node.attrs['Name']} container found, removing...")
             node.stop()
             node.remove(force=True)
             time.sleep(2)
@@ -125,26 +115,26 @@
     return utils.get_response(
         False, f"Container create max retries reached, Container status: {status}, Is Running: {is_running}")
 
 
 @bp.route('/spdk_process_kill', methods=['GET'])
 def spdk_process_kill():
     force = request.args.get('force', default=False, type=bool)
-    node_docker = get_docker_client()
+    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
     for cont in node_docker.containers.list(all=True):
         logger.debug(cont.attrs)
         if cont.attrs['Name'] == "/spdk" or cont.attrs['Name'] == "/spdk_proxy":
             cont.stop()
             cont.remove(force=force)
     return utils.get_response(True)
 
 
 @bp.route('/spdk_process_is_up', methods=['GET'])
 def spdk_process_is_up():
-    node_docker = get_docker_client()
+    node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
     for cont in node_docker.containers.list(all=True):
         logger.debug(cont.attrs)
         if cont.attrs['Name'] == "/spdk":
             status = cont.attrs['State']["Status"]
             is_running = cont.attrs['State']["Running"]
             if is_running:
                 return utils.get_response(True)
@@ -158,15 +148,15 @@
     data = request.get_json()
     db_connection = data['db_connection']
 
     logger.info("Setting DB connection")
     ret = scripts.set_db_config(db_connection)
 
     try:
-        node_docker = get_docker_client()
+        node_docker = docker.DockerClient(base_url='unix://var/run/docker.sock')
         nodes = node_docker.containers.list(all=True)
         for node in nodes:
             if node.attrs["Name"] == "/spdk_proxy":
                 node_docker.containers.get(node.attrs["Id"]).restart()
                 break
     except:
         pass
```

## Comparing `sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_dev-2.7.0/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/blueprints/csi.py` & `sbcli_dev-2.7.0/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_dev-2.7.0/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_dev-2.7.0/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/sbcli_dev.egg-info/SOURCES.txt` & `sbcli_dev-2.7.0/sbcli_dev.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 simplyblock_core/models/base_model.py
 simplyblock_core/models/caching_node.py
 simplyblock_core/models/cluster.py
 simplyblock_core/models/compute_node.py
 simplyblock_core/models/events.py
 simplyblock_core/models/global_settings.py
 simplyblock_core/models/iface.py
+simplyblock_core/models/job_schedule.py
 simplyblock_core/models/lvol_model.py
 simplyblock_core/models/mgmt_node.py
 simplyblock_core/models/nvme_device.py
 simplyblock_core/models/pool.py
 simplyblock_core/models/port_stat.py
 simplyblock_core/models/snapshot.py
 simplyblock_core/models/stats.py
@@ -83,14 +84,15 @@
 simplyblock_core/services/caching_node_monitor.py
 simplyblock_core/services/cap_monitor.py
 simplyblock_core/services/capacity_and_stats_collector.py
 simplyblock_core/services/device_monitor.py
 simplyblock_core/services/distr_event_collector.py
 simplyblock_core/services/health_check_service.py
 simplyblock_core/services/install_service.sh
+simplyblock_core/services/job_tasks.py
 simplyblock_core/services/log_agg_service.py
 simplyblock_core/services/lvol_monitor.py
 simplyblock_core/services/lvol_stat_collector.py
 simplyblock_core/services/mgmt_node_monitor.py
 simplyblock_core/services/port_stat_collector.py
 simplyblock_core/services/remove_service.sh
 simplyblock_core/services/service_template.service
```

## Comparing `sbcli_dev-2.6.9/sbcli_dev.egg-info/PKG-INFO` & `sbcli_dev-2.7.0/sbcli_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.6.9
+Version: 2.7.0
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/cluster_ops.py` & `sbcli_dev-2.7.0/simplyblock_core/cluster_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -690,45 +690,27 @@
             time.sleep(3)
         storage_node_ops.restart_storage_node(node.get_id())
 
     logger.info("Done")
     return True
 
 
-def cluster_grace_startup(cl_id):
+def list_tasks(cluster_id):
     db_controller = DBController()
-    cluster = db_controller.get_cluster_by_id(cl_id)
+    cluster = db_controller.get_cluster_by_id(cluster_id)
     if not cluster:
-        logger.error(f"Cluster not found {cl_id}")
+        logger.error("Cluster not found: %s", cluster_id)
         return False
-    logger.info(f"Unsuspending cluster: {cl_id}")
-    unsuspend_cluster(cl_id)
 
-    st = db_controller.get_storage_nodes()
-    for node in st:
-        logger.info(f"Restarting node: {node.get_id()}")
-        storage_node_ops.restart_storage_node(node.get_id())
-        time.sleep(5)
-        get_node = db_controller.get_storage_node_by_id(node.get_id())
-        if get_node.status != StorageNode.STATUS_ONLINE:
-            logger.error("failed to restart node")
-    
-    return True
-
-
-def cluster_grace_shutdown(cl_id):
-    db_controller = DBController()
-    cluster = db_controller.get_cluster_by_id(cl_id)
-    if not cluster:
-        logger.error(f"Cluster not found {cl_id}")
-        return False
-
-    st = db_controller.get_storage_nodes()
-    for node in st:
-        logger.info(f"Suspending node: {node.get_id()}")
-        storage_node_ops.suspend_storage_node(node.get_id())
-        logger.info(f"Shutting down node: {node.get_id()}")
-        storage_node_ops.shutdown_storage_node(node.get_id())
-       
-    logger.info(f"Suspending cluster: {cl_id}")
-    suspend_cluster(cl_id)
-    return True
+    data = []
+    tasks = db_controller.get_job_tasks(cluster_id)
+    for task in tasks:
+        data.append({
+            "UUID": task.uuid,
+            "Device": task.device_id,
+            "Function": task.function_name,
+            "Retry": task.retry,
+            "Status": task.status,
+            "Result": task.function_result,
+            "Date": time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime(task.date)),
+        })
+    return utils.print_table(data)
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/pci_utils.py` & `sbcli_dev-2.7.0/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/snode_client.py` & `sbcli_dev-2.7.0/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/kv_store.py` & `sbcli_dev-2.7.0/simplyblock_core/kv_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from simplyblock_core import constants
 from simplyblock_core.models.caching_node import CachingNode
 from simplyblock_core.models.cluster import ClusterMap
 
 from simplyblock_core.models.cluster import Cluster
 from simplyblock_core.models.compute_node import ComputeNode
+from simplyblock_core.models.job_schedule import JobSchedule
 from simplyblock_core.models.port_stat import PortStat
 from simplyblock_core.models.events import EventObj
 from simplyblock_core.models.global_settings import GlobalSettings
 from simplyblock_core.models.mgmt_node import MgmtNode
 from simplyblock_core.models.pool import Pool
 from simplyblock_core.models.snapshot import SnapShot
 from simplyblock_core.models.stats import DeviceStatObject, NodeStatObject, ClusterStatObject, LVolStatObject, \
@@ -244,7 +245,10 @@
 
     def get_port_stats(self, node_id, port_id, limit=20):
         stats = PortStat().read_from_db(self.kv_store, id="%s/%s" % (node_id, port_id), limit=limit, reverse=True)
         return stats
 
     def get_events(self, event_id=""):
         return EventObj().read_from_db(self.kv_store, id=event_id)
+
+    def get_job_tasks(self, cluster_id):
+        return JobSchedule().read_from_db(self.kv_store, id=cluster_id, reverse=True)
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/compute_node_ops.py` & `sbcli_dev-2.7.0/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/rpc_client.py` & `sbcli_dev-2.7.0/simplyblock_core/rpc_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,19 +114,15 @@
     def transport_list(self, trtype=None):
         params = None
         if trtype:
             params = {"trtype": trtype}
         return self._request("nvmf_get_transports", params)
 
     def transport_create(self, trtype):
-        params = {
-            "trtype": trtype,
-#            "max_io_qpairs_per_ctrlr": 65000,
-#            "max_queue_depth": 65000,
-        }
+        params = {"trtype": trtype}
         return self._request("nvmf_create_transport", params)
 
     def listeners_list(self, nqn):
         params = {"nqn": nqn}
         return self._request("nvmf_subsystem_get_listeners", params)
 
     def listeners_create(self, nqn, trtype, traddr, trsvcid):
@@ -286,27 +282,20 @@
 
     def get_bdevs(self, name=None):
         params = None
         if name:
             params = {"name": name}
         return self._request("bdev_get_bdevs", params)
 
-    def resize_lvol(self, lvol_bdev, blockcnt):
+    def resize_lvol(self, name, new_size_mb):
         params = {
-            "lvol_bdev": lvol_bdev,
-            "blockcnt": blockcnt
-        }
-        return self._request("ultra21_lvol_set", params)
-
-    def resize_clone(self, clone_bdev, blockcnt):
-        params = {
-            "clone_bdev": clone_bdev,
-            "blockcnt": blockcnt
+            "name": name,
+            "size_in_mib": new_size_mb
         }
-        return self._request("ultra21_lvol_set", params)
+        return self._request("bdev_lvol_resize", params)
 
     def lvol_read_only(self, name):
         params = {"name": name}
         return self._request("bdev_lvol_set_read_only", params)
 
     def lvol_create_snapshot(self, lvol_id, snapshot_name):
         params = {
@@ -634,31 +623,26 @@
         params = {"name": name}
         return self._request("bdev_jm_delete", params)
 
     def ultra21_util_get_malloc_stats(self):
         params = {"socket_id": 0}
         return self._request("ultra21_util_get_malloc_stats", params)
 
-    def ultra21_lvol_mount_clone(self, clone_name, snap_bdev, base_bdev, blockcnt):
+    def ultra21_lvol_mount_clone(self, clone_name, snap_bdev, base_bdev):
         params = {
             "modus": "CLONE",
-            "clone_bdev": clone_name,
+            "lvol_bdev": clone_name,
             "base_bdev": base_bdev,
-            "lvol_bdev": snap_bdev,
-            "blockcnt": blockcnt,
+            "snapshot_bdev": snap_bdev
         }
         return self._request("ultra21_lvol_mount", params)
 
     def alceml_unmap_vuid(self, name, vuid):
         params = {"name": name, "vuid": vuid}
         return self._request("alceml_unmap_vuid", params)
 
     def jm_delete(self):
         params = {"name": 0, "vuid": 0}
         return self._request("jm_delete", params)
 
     def framework_start_init(self):
         return self._request("framework_start_init")
-
-    def bdev_jm_unmap_vuid(self, name, vuid):
-        params = {"name": name, "vuid": vuid}
-        return self._request("bdev_jm_unmap_vuid", params)
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/mgmt_node_ops.py` & `sbcli_dev-2.7.0/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/utils.py` & `sbcli_dev-2.7.0/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/distr_controller.py` & `sbcli_dev-2.7.0/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/cnode_client.py` & `sbcli_dev-2.7.0/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/storage_node_ops.py` & `sbcli_dev-2.7.0/simplyblock_core/storage_node_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
             logger.error(f"Failed to create alceml bdev: {alceml_name}")
             return False
 
         # create jm
         if nvme.jm_bdev:
             ret = rpc_client.bdev_jm_create(nvme.jm_bdev, alceml_name)
             if not ret:
-                logger.error(f"Failed to create JM bdev: {nvme.jm_bdev}")
+                logger.error(f"Failed to create JM bdev: {snode.nvme_devices[0].jm_bdev}")
                 return False
             nvme.testing_bdev = test_name
             nvme.alceml_bdev = alceml_name
             nvme.io_error = True
             nvme.status = NVMeDevice.STATUS_JM
             continue
 
@@ -308,15 +308,15 @@
     remote_devices = []
     # connect to remote devs
     snodes = db_controller.get_storage_nodes()
     for node_index, node in enumerate(snodes):
         if node.get_id() == this_node.get_id() or node.status == node.STATUS_OFFLINE:
             continue
         for index, dev in enumerate(node.nvme_devices):
-            if dev.status != NVMeDevice.STATUS_ONLINE:
+            if dev.status != 'online':
                 logger.debug(f"Device is not online: {dev.get_id()}, status: {dev.status}")
                 continue
             name = f"remote_{dev.alceml_bdev}"
             logger.info(f"Connecting to {name}")
             ret = rpc_client.bdev_nvme_attach_controller_tcp(name, dev.nvmf_nqn, dev.nvmf_ip, dev.nvmf_port)
             if not ret:
                 logger.error(f"Failed to connect to device: {dev.get_id()}")
@@ -575,17 +575,14 @@
     for node_index, node in enumerate(snodes):
         if node.get_id() == snode.get_id() or node.status != StorageNode.STATUS_ONLINE:
             continue
         logger.info(f"Connecting to node: {node.get_id()}")
         rpc_client = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
         count = 0
         for dev in snode.nvme_devices:
-            if dev.status != NVMeDevice.STATUS_ONLINE:
-                logger.debug(f"Device is not online: {dev.get_id()}, status: {dev.status}")
-                continue
             name = f"remote_{dev.alceml_bdev}"
             ret = rpc_client.bdev_nvme_attach_controller_tcp(name, dev.nvmf_nqn, dev.nvmf_ip, dev.nvmf_port)
             if not ret:
                 logger.error(f"Failed to connect to device: {name}")
                 continue
 
             dev.remote_bdev = f"{name}n1"
@@ -1188,18 +1185,21 @@
 
     logger.info("Shutting down node")
     old_status = snode.status
     snode.status = StorageNode.STATUS_IN_SHUTDOWN
     snode.write_to_db(db_controller.kv_store)
     storage_events.snode_status_change(snode, snode.status, old_status)
 
-    logger.debug("Removing LVols")
+    logger.debug("Setting LVols to offline")
     for lvol_id in snode.lvols:
         logger.debug(lvol_id)
-        lvol_controller.delete_lvol_from_node(lvol_id, snode.get_id(), clear_data=False)
+        lvol = db_controller.get_lvol_by_id(lvol_id)
+        if lvol:
+            lvol.status = lvol.STATUS_OFFLINE
+            lvol.write_to_db(db_controller.kv_store)
 
     for dev in snode.nvme_devices:
         if dev.status in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_READONLY]:
             device_controller.device_set_unavailable(dev.get_id())
     distr_controller.send_node_status_event(snode.get_id(), "in_shutdown")
 
     # shutdown node
@@ -1209,15 +1209,14 @@
         distr_controller.disconnect_device(dev)
 
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password)
 
     # delete jm
-    logger.info("Removing JM")
     rpc_client.bdev_jm_delete(f"jm_{snode.get_id()}")
 
     logger.info("Stopping SPDK")
     snode_api = SNodeClient(snode.api_endpoint)
     results, err = snode_api.spdk_process_kill()
 
     distr_controller.send_node_status_event(snode.get_id(), StorageNode.STATUS_OFFLINE)
@@ -1668,18 +1667,15 @@
         volumes=[
             '/etc/foundationdb:/etc/foundationdb',
             '/var/tmp:/var/tmp',
             '/var/run:/var/run',
             '/dev:/dev',
             '/lib/modules/:/lib/modules/',
             '/sys:/sys'],
-        restart_policy={"Name": "always"},
-        environment=[
-            f"DOCKER_IP={dev_ip}"
-        ]
+        restart_policy={"Name": "always"}
     )
     logger.info("Pulling SPDK images")
     logger.debug(constants.SIMPLY_BLOCK_SPDK_CORE_IMAGE)
     logger.debug(constants.SIMPLY_BLOCK_SPDK_ULTRA_IMAGE)
     node_docker.images.pull(constants.SIMPLY_BLOCK_SPDK_CORE_IMAGE)
     node_docker.images.pull(constants.SIMPLY_BLOCK_SPDK_ULTRA_IMAGE)
     return f"{dev_ip}:5000"
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/constants.py` & `sbcli_dev-2.7.0/simplyblock_core/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,12 +49,12 @@
 
 HEALTH_CHECK_INTERVAL_SEC = 60
 
 GRAYLOG_CHECK_INTERVAL_SEC = 60
 
 FDB_CHECK_INTERVAL_SEC = 60
 
-SIMPLY_BLOCK_DOCKER_IMAGE = "simplyblock/simplyblock:dev"
+SIMPLY_BLOCK_DOCKER_IMAGE = "simplyblock/simplyblock:dev-auto-restart"
 SIMPLY_BLOCK_SPDK_CORE_IMAGE = "simplyblock/spdk-core:latest"
 SIMPLY_BLOCK_SPDK_ULTRA_IMAGE = "simplyblock/spdk:main-latest"
 
 GELF_PORT = 12201
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/services/caching_node_monitor.py` & `sbcli_dev-2.7.0/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/services/install_service.sh` & `sbcli_dev-2.7.0/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/services/__init__.py` & `sbcli_dev-2.7.0/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/services/log_agg_service.py` & `sbcli_dev-2.7.0/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/services/health_check_service.py` & `sbcli_dev-2.7.0/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_dev-2.7.0/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/services/device_monitor.py` & `sbcli_dev-2.7.0/simplyblock_core/services/job_tasks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,104 @@
 # coding=utf-8
 import logging
-import os
-
 import time
 import sys
 
 
-from simplyblock_core import constants, kv_store, storage_node_ops
-from simplyblock_core.controllers import health_controller,  device_controller
+from simplyblock_core import constants, kv_store
+from simplyblock_core.controllers import device_controller
+from simplyblock_core.models.job_schedule import JobSchedule
 from simplyblock_core.models.nvme_device import NVMeDevice
-from simplyblock_core.models.storage_node import StorageNode
 
 # Import the GELF logger
 from graypy import GELFUDPHandler
 
+from simplyblock_core.models.storage_node import StorageNode
+
+
+def _get_device(task):
+    node = db_controller.get_storage_node_by_id(task.node_id)
+    for dev in node.nvme_devices:
+        if dev.get_id() == task.device_id:
+            return dev
+
 
-def set_dev_status(device, status):
-    node = db_controller.get_storage_node_by_id(device.node_id)
+def task_runner(task):
+    if task.retry <= 0:
+        task.function_result = "timeout"
+        task.status = JobSchedule.STATUS_DONE
+        task.write_to_db(db_controller.kv_store)
+        return
+
+    node = db_controller.get_storage_node_by_id(task.node_id)
     if node.status != StorageNode.STATUS_ONLINE:
-        logger.error(f"Node is not online, {node.get_id()}, status: {node.status}, "
-                     f"skipping device status change")
+        logger.error(f"Node is not online: {node.get_id()} , skipping task: {task.get_id()}")
+        task.function_result = "Node is offline"
+        task.retry -= 1
+        task.write_to_db(db_controller.kv_store)
         return
 
-    for dev in node.nvme_devices:
-        if dev.get_id() == device.get_id():
-            if dev.status in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_UNAVAILABLE]:
-                device_controller.device_set_state(device.get_id(), status)
-            break
+    device = _get_device(task)
+    if device.status == NVMeDevice.STATUS_ONLINE and device.io_error is False:
+        logger.info(f"Device is online: {device.get_id()}, no restart needed")
+        task.function_result = "skipped because dev is online"
+        task.status = JobSchedule.STATUS_DONE
+        task.write_to_db(db_controller.kv_store)
+        return
+
+    task.status = JobSchedule.STATUS_RUNNING
+    task.write_to_db(db_controller.kv_store)
+
+    # resetting device
+    logger.info(f"Resetting device {device.get_id()}")
+    res = device_controller.reset_storage_device(device.get_id())
+    time.sleep(5)
+    device = _get_device(task)
+    if device.status == NVMeDevice.STATUS_ONLINE and device.io_error is False:
+        logger.info(f"Device is online: {device.get_id()}")
+        task.function_result = "done"
+        task.status = JobSchedule.STATUS_DONE
+        task.write_to_db(db_controller.kv_store)
+        return
+
+    logger.info(f"Restarting device {device.get_id()}")
+    res = device_controller.restart_device(device.get_id(), force=True)
+    time.sleep(5)
+    device = _get_device(task)
+    if device.status == NVMeDevice.STATUS_ONLINE and device.io_error is False:
+        logger.info(f"Device is online: {device.get_id()}")
+        task.function_result = "done"
+        task.status = JobSchedule.STATUS_DONE
+        task.write_to_db(db_controller.kv_store)
+        return
+
+    task.retry -= 1
+    task.write_to_db(db_controller.kv_store)
     return
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
 gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
-db_store = kv_store.KVStore()
 db_controller = kv_store.DBController()
 
-
-logger.info("Starting Device monitor...")
+logger.info("Starting Jobs runner...")
 while True:
-    nodes = db_controller.get_storage_nodes()
-    for node in nodes:
-        if node.status != StorageNode.STATUS_ONLINE:
-            logger.warning(f"Node status is not online, id: {node.get_id()}, status: {node.status}")
-            continue
-        for dev in node.nvme_devices:
-            if dev.status not in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_UNAVAILABLE]:
-                logger.warning(f"Device status is not online or unavailable, id: {dev.get_id()}, status: {dev.status}")
-                continue
-            if dev.io_error:
-                logger.debug(f"Skipping Device check because of io_error {dev.get_id()}")
-                continue
-
-            ret = health_controller.check_device(dev.get_id())
-            logger.info(f"Device: {dev.get_id()}, is healthy: {ret}")
-            # if ret:
-            #     set_dev_status(dev, NVMeDevice.STATUS_ONLINE)
-            # else:
-            #     set_dev_status(dev, NVMeDevice.STATUS_UNAVAILABLE)
 
-    time.sleep(constants.DEV_MONITOR_INTERVAL_SEC)
+    clusters = db_controller.get_clusters()
+    if not clusters:
+        logger.error("No clusters found!")
+    else:
+        for cl in clusters:
+            tasks = db_controller.get_job_tasks(cl.get_id())
+            for task in tasks:
+                if task.status != JobSchedule.STATUS_DONE:
+                    res = task_runner(task)
+
+    time.sleep(5)
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_dev-2.7.0/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/services/cap_monitor.py` & `sbcli_dev-2.7.0/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/services/storage_node_monitor.py` & `sbcli_dev-2.7.0/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/services/port_stat_collector.py` & `sbcli_dev-2.7.0/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/services/distr_event_collector.py` & `sbcli_dev-2.7.0/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_dev-2.7.0/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/services/lvol_monitor.py` & `sbcli_dev-2.7.0/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/controllers/pool_controller.py` & `sbcli_dev-2.7.0/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/controllers/storage_events.py` & `sbcli_dev-2.7.0/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/controllers/lvol_controller.py` & `sbcli_dev-2.7.0/simplyblock_core/controllers/lvol_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -604,30 +604,30 @@
     lvol.distr_bs = distr_bs
     lvol.distr_chunk_bs = distr_chunk_bs
     lvol.distr_page_size = cl.page_size_in_blocks
 
     lvol.base_bdev = f"distr_{lvol.vuid}_{name}"
     lvol.top_bdev = lvol.base_bdev
 
-    if with_snapshot:
-        lvol.bdev_stack.append({
-            "type": "bdev_distr",
+    lvol.bdev_stack.append({
+        "type": "bdev_distr",
+        "name": lvol.base_bdev,
+        "params": {
             "name": lvol.base_bdev,
-            "params": {
-                "name": lvol.base_bdev,
-                "vuid": lvol.vuid,
-                "ndcs": lvol.ndcs,
-                "npcs": lvol.npcs,
-                "num_blocks": int(lvol.max_size / lvol.distr_bs),
-                "block_size": lvol.distr_bs,
-                "chunk_size": lvol.distr_chunk_bs,
-                "pba_page_size": lvol.distr_page_size,
-            }
-        })
+            "vuid": lvol.vuid,
+            "ndcs": lvol.ndcs,
+            "npcs": lvol.npcs,
+            "num_blocks": int(lvol.size / lvol.distr_bs),
+            "block_size": lvol.distr_bs,
+            "chunk_size": lvol.distr_chunk_bs,
+            "pba_page_size":  lvol.distr_page_size,
+        }
+    })
 
+    if with_snapshot:
         lvol.bdev_stack.append({
             "type": "bmap_init",
             "name": lvol.base_bdev,
             "params": {
                 "bdev_name": lvol.base_bdev,
                 "num_blocks": int(lvol.size / lvol.distr_bs),
                 "block_len": lvol.distr_bs,
@@ -643,29 +643,14 @@
             "params": {
                 "lvol_name": lvol.top_bdev,
                 "base_bdev": lvol.base_bdev,
                 "label": "label",
                 "desc": "desc"
             }
         })
-    else:
-        lvol.bdev_stack.append({
-            "type": "bdev_distr",
-            "name": lvol.base_bdev,
-            "params": {
-                "name": lvol.base_bdev,
-                "vuid": lvol.vuid,
-                "ndcs": lvol.ndcs,
-                "npcs": lvol.npcs,
-                "num_blocks": int(lvol.size / lvol.distr_bs),
-                "block_size": lvol.distr_bs,
-                "chunk_size": lvol.distr_chunk_bs,
-                "pba_page_size": lvol.distr_page_size,
-            }
-        })
 
     if use_crypto:
         if crypto_key1 == None or crypto_key2 == None:
             return False, "encryption keys for lvol not provided"
         else:
             success, err = validate_aes_xts_keys(crypto_key1, crypto_key2)
             if not success:
@@ -919,55 +904,41 @@
         bdev['status'] = 'deleted'
         time.sleep(1)
 
 
 def delete_lvol_from_node(lvol_id, node_id, clear_data=True):
     lvol = db_controller.get_lvol_by_id(lvol_id)
     snode = db_controller.get_storage_node_by_id(node_id)
-    logger.info(f"Deleting LVol:{lvol.get_id()} from node:{snode.get_id()}")
+    logger.debug(f"Deleting LVol:{lvol.get_id()} from node:{snode.get_id()}")
     rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
 
-    # 1- remove subsystem
-    logger.info(f"Removing subsystem")
-    ret = rpc_client.subsystem_delete(lvol.nqn)
-
-    # 2- remove bdevs
-    logger.info(f"Removing bdev stack")
+    # 1- remove bdevs
     _remove_bdev_stack(lvol.bdev_stack[::-1], rpc_client)
     lvol.deletion_status = 'bdevs_deleted'
     lvol.write_to_db(db_controller.kv_store)
 
+    # 2- remove subsystem
+    ret = rpc_client.subsystem_delete(lvol.nqn)
+
     # 3- clear alceml devices
     if clear_data:
-        logger.info(f"Clearing Alceml devices")
         for node in db_controller.get_storage_nodes():
             if node.status == StorageNode.STATUS_ONLINE:
                 rpc_node = RPCClient(node.mgmt_ip, node.rpc_port, node.rpc_username, node.rpc_password)
                 for dev in node.nvme_devices:
                     if dev.status != NVMeDevice.STATUS_JM:
                         ret = rpc_node.alceml_unmap_vuid(dev.alceml_bdev, lvol.vuid)
 
-        lvol.deletion_status = 'alceml_unmapped'
-        lvol.write_to_db(db_controller.kv_store)
-
-        # 4- clear JM
-        jm_device = None
-        for dev in snode.nvme_devices:
-            if dev.status == NVMeDevice.STATUS_JM:
-                jm_device = dev
-                break
-        ret = rpc_client.alceml_unmap_vuid(jm_device.alceml_bdev, lvol.vuid)
-        if not ret:
-            logger.error(f"Failed to unmap jm alceml {jm_device.alceml_bdev} with vuid {lvol.vuid}")
-        ret = rpc_client.bdev_jm_unmap_vuid(jm_device.jm_bdev, lvol.vuid)
-        if not ret:
-            logger.error(f"Failed to unmap jm {jm_device.jm_bdev} with vuid {lvol.vuid}")
+    lvol.deletion_status = 'alceml_unmapped'
+    lvol.write_to_db(db_controller.kv_store)
 
-        lvol.deletion_status = 'jm_unmapped'
-        lvol.write_to_db(db_controller.kv_store)
+    # 4- clear JM
+    # ret = rpc_client.alceml_unmap_vuid(name, lvol.vuid)
+    # lvol.deletion_status = 'jm_unmapped'
+    lvol.write_to_db(db_controller.kv_store)
 
     return True
 
 
 def delete_lvol(id_or_name, force_delete=False):
     lvol = db_controller.get_lvol_by_id(id_or_name)
     if not lvol:
@@ -1205,48 +1176,43 @@
         logger.error(f"Pool is disabled")
         return False
 
     if lvol.size >= new_size:
         logger.error(f"New size {new_size} must be higher than the original size {lvol.size}")
         return False
 
-    if lvol.max_size < new_size:
-        logger.error(f"New size {new_size} must be smaller than the max size {lvol.max_size}")
-        return False
-
     logger.info(f"Resizing LVol: {lvol.id}, new size: {lvol.size}")
 
-    snode = db_controller.get_storage_node_by_id(lvol.node_id)
+    # if lvol.pool_uuid:
+    #     pool = db_controller.get_pool_by_id(lvol.pool_uuid)
+    #     if pool:
+    #         print(pool)
+
+    snode = db_controller.get_storage_node_by_hostname(lvol.hostname)
 
     # creating RPCClient instance
     rpc_client = RPCClient(
         snode.mgmt_ip,
         snode.rpc_port,
         snode.rpc_username,
         snode.rpc_password)
 
-    num_blocks = int(new_size / lvol.distr_bs)
-    if lvol.snapshot_name:
-        ret = rpc_client.resize_lvol(lvol.top_bdev, num_blocks)
-        if not ret:
-            logger.error("Error resizing lvol")
-            return False
-    elif lvol.cloned_from_snap:
-        ret = rpc_client.resize_clone(lvol.top_bdev, num_blocks)
-        if not ret:
-            logger.error("Error resizing clone")
-            return False
-    else:
-        logger.error("Can not resize distr")
-        return False
+    # ret = rpc_client.get_bdevs(lvol.lvol_name)
+    # bdev_data = ret[0]
+    # logger.debug(json.dumps(ret, indent=2))
+    # print("is claimed:", bdev_data['claimed'])
+    size_mb = int(new_size / (1024 * 1024))
+    ret = rpc_client.resize_lvol(lvol.lvol_bdev, size_mb)
+    if not ret:
+        return "Error"
 
     lvol.size = new_size
     lvol.write_to_db(db_controller.kv_store)
     logger.info("Done")
-    return True
+    return ret
 
 
 def set_read_only(id):
     lvol = db_controller.get_lvol_by_id(id)
     if not lvol:
         logger.error(f"LVol not found: {id}")
         return False
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/controllers/device_events.py` & `sbcli_dev-2.7.0/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/controllers/lvol_events.py` & `sbcli_dev-2.7.0/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_dev-2.7.0/simplyblock_core/controllers/snapshot_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
     page_len = int(lvol.distr_page_size / lvol.distr_bs)
     max_num_blocks = num_blocks * 10
     ret = rpc_client.ultra21_lvol_bmap_init(name, num_blocks, block_len, page_len, max_num_blocks)
     if not ret:
         return False, "Failed to init distr bdev"
 
     lvol_name = f"clone_{lvol.vuid+2}_{lvol.lvol_name}"
-    ret = rpc_client.ultra21_lvol_mount_clone(lvol_name, snap.snap_bdev, name, num_blocks)
+    ret = rpc_client.ultra21_lvol_mount_clone(lvol_name, snap.snap_bdev, name)
     if not ret:
         return False, "Failed to create clone lvol bdev"
 
     ##############################################################################
 
     lvol_id = str(uuid.uuid4())
     # lvs_name = snap.lvol.lvol_bdev.split("/")[0]
@@ -274,15 +274,14 @@
 
     logger.info(f"add lvol {clone_name} to subsystem")
     ret = rpc_client.nvmf_subsystem_add_ns(subsystem_nqn, top_bdev)
 
     lvol.bdev_stack = bdev_stack
     lvol.uuid = lvol_id
     lvol.lvol_bdev = lvol_name
-    lvol.top_bdev = top_bdev
     lvol.hostname = snode.hostname
     lvol.node_id = snode.get_id()
     lvol.mode = 'read-write'
     lvol.lvol_type = lvol_type
     lvol.cloned_from_snap = snapshot_id
     lvol.nqn = subsystem_nqn
     lvol.pool_uuid = pool.id
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/controllers/snapshot_events.py` & `sbcli_dev-2.7.0/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/controllers/events_controller.py` & `sbcli_dev-2.7.0/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/controllers/health_controller.py` & `sbcli_dev-2.7.0/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/controllers/device_controller.py` & `sbcli_dev-2.7.0/simplyblock_core/controllers/device_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,23 +78,24 @@
     return device_set_state(device_id, NVMeDevice.STATUS_ONLINE)
 
 
 def get_alceml_name(alceml_id):
     return f"alceml_{alceml_id}"
 
 
-def restart_device(device_id):
+def restart_device(device_id, force=False):
     db_controller = DBController()
     dev = db_controller.get_storage_devices(device_id)
     if not dev:
         logger.error("device not found")
 
     if dev.status != NVMeDevice.STATUS_REMOVED:
         logger.error("Device must be in removed status")
-        return False
+        if not force:
+            return False
 
     snode = db_controller.get_storage_node_by_id(dev.node_id)
     if not snode:
         logger.error("node not found")
         return False
 
     device_obj = None
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/controllers/pool_events.py` & `sbcli_dev-2.7.0/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_dev-2.7.0/simplyblock_core/controllers/caching_node_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -574,18 +574,15 @@
         volumes=[
             '/etc/foundationdb:/etc/foundationdb',
             '/var/tmp:/var/tmp',
             '/var/run:/var/run',
             '/dev:/dev',
             '/lib/modules/:/lib/modules/',
             '/sys:/sys'],
-        restart_policy={"Name": "always"},
-        environment=[
-            f"DOCKER_IP={dev_ip}"
-        ]
+        restart_policy={"Name": "always"}
     )
     logger.info("Pulling SPDK images")
     node_docker.images.pull(constants.SIMPLY_BLOCK_SPDK_CORE_IMAGE)
     node_docker.images.pull(constants.SIMPLY_BLOCK_SPDK_ULTRA_IMAGE)
     return f"{dev_ip}:5000"
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/controllers/cluster_events.py` & `sbcli_dev-2.7.0/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/controllers/mgmt_events.py` & `sbcli_dev-2.7.0/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/caching_node.py` & `sbcli_dev-2.7.0/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/nvme_device.py` & `sbcli_dev-2.7.0/simplyblock_core/models/nvme_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/mgmt_node.py` & `sbcli_dev-2.7.0/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/compute_node.py` & `sbcli_dev-2.7.0/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/events.py` & `sbcli_dev-2.7.0/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/global_settings.py` & `sbcli_dev-2.7.0/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/base_model.py` & `sbcli_dev-2.7.0/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/lvol_model.py` & `sbcli_dev-2.7.0/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/snapshot.py` & `sbcli_dev-2.7.0/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/storage_node.py` & `sbcli_dev-2.7.0/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/stats.py` & `sbcli_dev-2.7.0/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/pool.py` & `sbcli_dev-2.7.0/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/iface.py` & `sbcli_dev-2.7.0/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/cluster.py` & `sbcli_dev-2.7.0/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/models/port_stat.py` & `sbcli_dev-2.7.0/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/install_deps.sh` & `sbcli_dev-2.7.0/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/__init__.py` & `sbcli_dev-2.7.0/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/haproxy.cfg` & `sbcli_dev-2.7.0/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_dev-2.7.0/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_dev-2.7.0/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files 1% similar despite different names*

```diff
@@ -185,26 +185,39 @@
     deploy:
       placement:
         constraints: [node.role == manager]
     volumes:
       - "/etc/foundationdb:/etc/foundationdb"
     networks:
       - hostnet
+
   CleanupFDB:
     image: $SIMPLYBLOCK_DOCKER_IMAGE
     environment:
       LOG_DELETION_INTERVAL: "${LOG_DELETION_INTERVAL}"
     command: "python simplyblock_core/workers/cleanup_foundationdb.py"
     deploy:
       placement:
         constraints: [node.role == manager]
     volumes:
       - "/etc/foundationdb:/etc/foundationdb"
     networks:
       - hostnet
+
+  TasksRunner:
+    image: $SIMPLYBLOCK_DOCKER_IMAGE
+    command: "python simplyblock_core/services/job_tasks.py"
+    deploy:
+      placement:
+        constraints: [node.role == manager]
+    volumes:
+      - "/etc/foundationdb:/etc/foundationdb"
+    networks:
+      - hostnet
+
 volumes:
   os_data:
 
 networks:
   hostnet:
     external: true
     name: host
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_dev-2.7.0/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml` & `sbcli_dev-2.7.0/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_dev-2.7.0/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_dev-2.7.0/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_dev-2.7.0/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9984272596571181%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 2: "*

 * *                "{'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 3: {'fieldConfig': "*

 * *                "{'defaults': {'unit': 'decbytes'}}}, 4: {'fieldConfig': {'defaults': {'unit': "*

 * *                "'decbytes'}}}, 5: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 6: "*

 * *                "{'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 8: {'fieldConfig': "*

 * *                "{'defaults': {'unit': 'decbytes'} […]*

```diff
@@ -86,15 +86,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -179,15 +179,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -272,15 +272,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -365,15 +365,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -458,15 +458,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "percent"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -551,15 +551,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "percent"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -657,15 +657,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -750,15 +750,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "binBps"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -1119,15 +1119,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "\u00b5s"
+                        "unit": "ns"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
@@ -1225,15 +1225,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -1318,15 +1318,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "binBps"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
@@ -1410,16 +1410,15 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "\u00b5s"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
@@ -1885,15 +1884,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -1978,16 +1977,15 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "\u00b5s"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -2281,15 +2279,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -2319,14 +2317,305 @@
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "snode_unmap_bytes",
                 "type": "timeseries"
+            },
+            {
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
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
+                                },
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        }
+                    },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 0,
+                    "y": 63
+                },
+                "id": 8,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
+                        },
+                        "editorMode": "builder",
+                        "expr": "snode_record_end_time",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "snode_record_end_time",
+                "type": "timeseries"
+            },
+            {
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "description": "",
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
+                                },
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        }
+                    },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 7,
+                    "y": 63
+                },
+                "id": 7,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
+                        },
+                        "editorMode": "builder",
+                        "expr": "snode_record_duration",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "snode_record_duration",
+                "type": "timeseries"
+            },
+            {
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
+                                },
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        },
+                        "unit": "decbytes"
+                    },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 14,
+                    "y": 63
+                },
+                "id": 9,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
+                        },
+                        "editorMode": "builder",
+                        "expr": "snode_record_start_time",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "snode_record_start_time",
+                "type": "timeseries"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
         "templating": {
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9984272596571181%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 2: "*

 * *                "{'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 3: {'fieldConfig': "*

 * *                "{'defaults': {'unit': 'decbytes'}}}, 4: {'fieldConfig': {'defaults': {'unit': "*

 * *                "'decbytes'}}}, 5: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 6: "*

 * *                "{'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 8: {'fieldConfig': "*

 * *                "{'defaults': {'unit': 'decbytes'} […]*

```diff
@@ -86,15 +86,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -179,15 +179,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -272,15 +272,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -365,15 +365,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -458,15 +458,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "percent"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -551,15 +551,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "percent"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -657,15 +657,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -750,15 +750,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "binBps"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -843,15 +843,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "\u00b5s"
+                        "unit": "ns"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -1225,15 +1225,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -1318,15 +1318,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
@@ -1410,16 +1410,15 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "\u00b5s"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
@@ -1885,15 +1884,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -1978,16 +1977,15 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "\u00b5s"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -2281,15 +2279,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -2319,14 +2317,305 @@
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_unmap_bytes",
                 "type": "timeseries"
+            },
+            {
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
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
+                                },
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        }
+                    },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 0,
+                    "y": 62
+                },
+                "id": 8,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
+                        },
+                        "editorMode": "builder",
+                        "expr": "cluster_record_end_time",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "cluster_record_end_time",
+                "type": "timeseries"
+            },
+            {
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "description": "",
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
+                                },
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        }
+                    },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 7,
+                    "y": 62
+                },
+                "id": 7,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
+                        },
+                        "editorMode": "builder",
+                        "expr": "cluster_record_duration",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "cluster_record_duration",
+                "type": "timeseries"
+            },
+            {
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
+                                },
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        },
+                        "unit": "decbytes"
+                    },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 14,
+                    "y": 62
+                },
+                "id": 9,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
+                        },
+                        "editorMode": "builder",
+                        "expr": "cluster_record_start_time",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "cluster_record_start_time",
+                "type": "timeseries"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
         "templating": {
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files 8% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9984272596571181%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 2: "*

 * *                "{'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 3: {'fieldConfig': "*

 * *                "{'defaults': {'unit': 'decbytes'}}}, 4: {'fieldConfig': {'defaults': {'unit': "*

 * *                "'decbytes'}}}, 5: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 6: "*

 * *                "{'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 8: {'fieldConfig': "*

 * *                "{'defaults': {'unit': 'decbytes'} […]*

```diff
@@ -86,15 +86,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -179,15 +179,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -272,15 +272,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -365,15 +365,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -458,15 +458,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "percent"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -551,15 +551,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "percent"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -657,15 +657,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -1026,15 +1026,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "binBps"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
@@ -1119,15 +1119,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "\u00b5s"
+                        "unit": "ns"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
@@ -1225,15 +1225,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -1318,15 +1318,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "binBps"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
@@ -1410,16 +1410,15 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "\u00b5s"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
@@ -1885,15 +1884,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -1978,16 +1977,15 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "\u00b5s"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -2281,15 +2279,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "binBps"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -2319,14 +2317,305 @@
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "lvol_unmap_bytes",
                 "type": "timeseries"
+            },
+            {
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
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
+                                },
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        }
+                    },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 0,
+                    "y": 64
+                },
+                "id": 8,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
+                        },
+                        "editorMode": "builder",
+                        "expr": "lvol_record_end_time",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "lvol_record_end_time",
+                "type": "timeseries"
+            },
+            {
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "description": "",
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
+                                },
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        }
+                    },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 7,
+                    "y": 64
+                },
+                "id": 7,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
+                        },
+                        "editorMode": "builder",
+                        "expr": "lvol_record_duration",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "lvol_record_duration",
+                "type": "timeseries"
+            },
+            {
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
+                                },
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        },
+                        "unit": "decbytes"
+                    },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 14,
+                    "y": 64
+                },
+                "id": 9,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
+                    {
+                        "datasource": {
+                            "type": "prometheus",
+                            "uid": "PBFA97CFB590B2093"
+                        },
+                        "editorMode": "builder",
+                        "expr": "lvol_record_start_time",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "lvol_record_start_time",
+                "type": "timeseries"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
         "templating": {
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/devices.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.997343982514881%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 2: "*

 * *                "{'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 3: {'fieldConfig': "*

 * *                "{'defaults': {'unit': 'decbytes'}}}, 4: {'fieldConfig': {'defaults': {'unit': "*

 * *                "'decbytes'}}}, 5: {'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 6: "*

 * *                "{'fieldConfig': {'defaults': {'unit': 'decbytes'}}}, 8: {'fieldConfig': "*

 * *                "{'defaults': {'unit': 'decbytes'} […]*

```diff
@@ -86,15 +86,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -179,15 +179,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -272,15 +272,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 8,
                     "x": 14,
@@ -365,15 +365,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -458,15 +458,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "percent"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -551,15 +551,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "percent"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 8,
                     "x": 14,
@@ -657,15 +657,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -750,15 +750,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
@@ -843,15 +843,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "\u00b5s"
+                        "unit": "ns"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 8,
                     "x": 14,
@@ -1225,15 +1225,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "decbytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -1318,15 +1318,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "bytes"
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
@@ -1410,16 +1410,15 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "\u00b5s"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 8,
                     "x": 14,
@@ -1727,606 +1726,898 @@
                         "refId": "A"
                     }
                 ],
                 "title": "device_read_latency_ticks",
                 "type": "timeseries"
             },
             {
-                "collapsed": false,
+                "collapsed": true,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
                     "x": 0,
                     "y": 48
                 },
                 "id": 29,
-                "panels": [],
-                "title": "unmap",
-                "type": "row"
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
-                    "w": 7,
-                    "x": 0,
-                    "y": 49
-                },
-                "id": 21,
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
-                        "unit": "bytes"
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
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 7,
-                    "y": 49
-                },
-                "id": 17,
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
-                        "expr": "device_unmap_bytes_ps",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "device_unmap_bytes_ps",
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
-                        },
-                        "unit": "\u00b5s"
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 8,
-                    "x": 14,
-                    "y": 49
-                },
-                "id": 20,
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
-                        "expr": "device_unmap_latency_ps",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "device_unmap_latency_ps",
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
                                         "legend": false,
                                         "tooltip": false,
-                                        "viz": true
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
                                     }
-                                }
-                            ]
-                        }
-                    ]
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 0,
-                    "y": 56
-                },
-                "id": 19,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
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
-                        "expr": "device_unmap_io_ps",
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
-                "title": "device_unmap_io_ps",
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
-                        }
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 7,
-                    "y": 56
-                },
-                "id": 18,
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
-                        "expr": "device_unmap_io",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "device_unmap_io",
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
-                        },
-                        "unit": "decbytes"
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 8,
-                    "x": 14,
-                    "y": 56
-                },
-                "id": 16,
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
-                        "expr": "device_unmap_bytes",
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
-                "title": "device_unmap_bytes",
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
```

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/pools.json` & `sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/pools.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.6.9/simplyblock_core/scripts/dashboards/node-exporter.json` & `sbcli_dev-2.7.0/simplyblock_core/scripts/dashboards/node-exporter.json`

 * *Files identical despite different names*

