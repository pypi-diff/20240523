# Comparing `tmp/sbcli_adr-1.0.0.zip` & `tmp/sbcli_adr-1.0.1.zip`

## zipinfo {}

```diff
@@ -1,150 +1,150 @@
-Zip file size: 215520 bytes, number of entries: 148
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-10 13:18 sbcli_adr-1.0.0/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-10 13:18 sbcli_adr-1.0.0/sbcli_adr.egg-info/
--rw-r--r--  2.0 unx     2269 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/setup.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/README.md
--rw-r--r--  2.0 unx      148 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/env_var
--rw-r--r--  2.0 unx       84 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/pyproject.toml
--rw-r--r--  2.0 unx       38 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/setup.cfg
--rw-r--r--  2.0 unx     1489 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/PKG-INFO
--rw-r--r--  2.0 unx    77873 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_cli/main.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/
--rw-r--r--  2.0 unx    66264 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1501 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3153 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     3638 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx      279 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx      938 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3193 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     8468 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     7640 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/utils.py
--rw-r--r--  2.0 unx    23423 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx     5112 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    21493 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     7504 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx     2189 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx     3203 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     2064 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/job_tasks.py
--rw-r--r--  2.0 unx     5462 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx      229 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     5268 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     2410 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5140 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx     7439 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2423 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     4118 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx      837 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2671 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6577 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/services/storage_node_monitor.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx      930 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx      152 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx     5333 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx       54 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx     4409 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
--rw-r--r--  2.0 unx      453 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx     1782 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx      311 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx      118 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx      360 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx       43 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1420 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx      311 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/prometheus.yml
--rwxr-xr-x  2.0 unx      657 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx    25433 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1856 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx   106705 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx   799409 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/node-exporter.json
--rw-r--r--  2.0 unx    99758 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    99862 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/pools.json
--rw-r--r--  2.0 unx    13877 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1120 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     3191 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx     1521 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1630 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    10557 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx    10375 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1900 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx    23245 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx    47534 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx    11294 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx     1500 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx     1277 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/job_schedule.py
--rw-r--r--  2.0 unx      806 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4846 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      917 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx      736 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     1602 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     1228 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     1020 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx     3696 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     4242 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     2565 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx     3766 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     2094 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_core/models/nvme_device.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/
--rw-r--r--  2.0 unx      725 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     5098 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx      703 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     1263 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     2513 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      507 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      322 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      434 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      827 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx     1302 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     2905 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5547 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     4883 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5491 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     9573 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx     8547 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx    11244 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx    12198 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx      975 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     6326 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     8075 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     2940 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     5274 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx     6206 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx        1 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/sbcli_adr.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     5267 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/sbcli_adr.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       49 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/sbcli_adr.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1489 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/sbcli_adr.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       73 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/sbcli_adr.egg-info/requires.txt
--rw-r--r--  2.0 unx       55 b- defN 24-May-10 13:18 sbcli_adr-1.0.0/sbcli_adr.egg-info/entry_points.txt
-148 files, 1930894 bytes uncompressed, 188572 bytes compressed:  90.2%
+Zip file size: 215992 bytes, number of entries: 148
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:18 sbcli_adr-1.0.1/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:18 sbcli_adr-1.0.1/sbcli_adr.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/README.md
+-rw-r--r--  2.0 unx       84 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/pyproject.toml
+-rw-r--r--  2.0 unx     1489 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/PKG-INFO
+-rw-r--r--  2.0 unx      148 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/env_var
+-rw-r--r--  2.0 unx       38 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/setup.cfg
+-rw-r--r--  2.0 unx     2269 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/setup.py
+-rw-r--r--  2.0 unx    78180 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_cli/main.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/templates/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      703 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx      717 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx     2513 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/app.py
+-rw-r--r--  2.0 unx      725 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx      322 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx      507 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      434 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_pool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     8547 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx     9573 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx     5274 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     8075 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     4883 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5547 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     5491 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx      975 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     2905 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5267 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/sbcli_adr.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       73 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/sbcli_adr.egg-info/requires.txt
+-rw-r--r--  2.0 unx     1489 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/sbcli_adr.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       49 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/sbcli_adr.egg-info/top_level.txt
+-rw-r--r--  2.0 unx       55 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/sbcli_adr.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/sbcli_adr.egg-info/dependency_links.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/
+-rw-r--r--  2.0 unx    23423 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx      938 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8532 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    21493 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx     7504 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx      279 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx     3638 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx    66949 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1501 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3340 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/job_tasks.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx      229 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx      837 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     4118 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx     7439 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     3169 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     5268 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6577 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/storage_node_monitor.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     5140 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx    47534 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10557 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx     3191 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx    11294 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx    13877 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx    23245 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2094 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/nvme_device.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx      917 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx      973 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/job_schedule.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      736 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     3696 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx      806 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/models/port_stat.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx     1420 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx     1782 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx       43 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx      118 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx     5333 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx      152 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/set_db_config.sh
+-rwxr-xr-x  2.0 unx      657 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/prometheus.yml
+-rw-r--r--  2.0 unx      311 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx     4409 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+-rw-r--r--  2.0 unx      930 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx       54 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx    25433 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1856 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx    99758 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    99862 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx   106705 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/pools.json
+-rw-r--r--  2.0 unx   799409 b- defN 24-May-23 13:18 sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/node-exporter.json
+148 files, 1933592 bytes uncompressed, 189044 bytes compressed:  90.2%
```

## zipnote {}

```diff
@@ -1,445 +1,445 @@
-Filename: sbcli_adr-1.0.0/
+Filename: sbcli_adr-1.0.1/
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_cli/
+Filename: sbcli_adr-1.0.1/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/
+Filename: sbcli_adr-1.0.1/simplyblock_web/
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/
+Filename: sbcli_adr-1.0.1/sbcli_adr.egg-info/
 Comment: 
 
-Filename: sbcli_adr-1.0.0/sbcli_adr.egg-info/
+Filename: sbcli_adr-1.0.1/simplyblock_core/
 Comment: 
 
-Filename: sbcli_adr-1.0.0/setup.py
+Filename: sbcli_adr-1.0.1/README.md
 Comment: 
 
-Filename: sbcli_adr-1.0.0/README.md
+Filename: sbcli_adr-1.0.1/pyproject.toml
 Comment: 
 
-Filename: sbcli_adr-1.0.0/env_var
+Filename: sbcli_adr-1.0.1/PKG-INFO
 Comment: 
 
-Filename: sbcli_adr-1.0.0/pyproject.toml
+Filename: sbcli_adr-1.0.1/env_var
 Comment: 
 
-Filename: sbcli_adr-1.0.0/setup.cfg
+Filename: sbcli_adr-1.0.1/setup.cfg
 Comment: 
 
-Filename: sbcli_adr-1.0.0/PKG-INFO
+Filename: sbcli_adr-1.0.1/setup.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_cli/cli.py
+Filename: sbcli_adr-1.0.1/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_cli/main.py
+Filename: sbcli_adr-1.0.1/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/
+Filename: sbcli_adr-1.0.1/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/
+Filename: sbcli_adr-1.0.1/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/
+Filename: sbcli_adr-1.0.1/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/storage_node_ops.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/constants.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/cnode_client.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/shell_utils.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/pci_utils.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/__init__.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/snode_client.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/kv_store.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/utils.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/cluster_ops.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/compute_node_ops.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/rpc_client.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/distr_controller.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/job_tasks.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/health_check_service.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/service_template.service
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/remove_service.sh
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/device_monitor.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/__init__.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/install_service.sh
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/alerting/
+Filename: sbcli_adr-1.0.1/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/
+Filename: sbcli_adr-1.0.1/sbcli_adr.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_adr-1.0.1/sbcli_adr.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_adr-1.0.1/sbcli_adr.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_adr-1.0.1/sbcli_adr.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_adr-1.0.1/sbcli_adr.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_adr-1.0.1/sbcli_adr.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/__init__.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_adr-1.0.1/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_adr-1.0.1/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_adr-1.0.1/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_adr-1.0.1/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_adr-1.0.1/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_adr-1.0.1/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_adr-1.0.1/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_adr-1.0.1/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_adr-1.0.1/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_adr-1.0.1/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/node-exporter.json
+Filename: sbcli_adr-1.0.1/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_adr-1.0.1/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_adr-1.0.1/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_adr-1.0.1/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/pools.json
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/job_tasks.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/device_events.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/__init__.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/events.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/job_schedule.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/iface.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/base_model.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/lvol_model.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/compute_node.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/snapshot.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/pool.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/global_settings.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/port_stat.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/storage_node.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/__init__.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/stats.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/cluster.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/caching_node.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_core/models/nvme_device.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/static/
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/templates/
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/node_utils.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/snode_app.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/app.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/job_schedule.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/auth_middleware.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/__init__.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/caching_node_app.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/utils.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/node_webapp.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/static/tst.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/static/is_up.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/static/delete.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/static/deploy.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/static/rpac.yaml
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/static/list_deps.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/csi.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_adr-1.0.0/sbcli_adr.egg-info/dependency_links.txt
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_adr-1.0.0/sbcli_adr.egg-info/SOURCES.txt
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_adr-1.0.0/sbcli_adr.egg-info/top_level.txt
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_adr-1.0.0/sbcli_adr.egg-info/PKG-INFO
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_adr-1.0.0/sbcli_adr.egg-info/requires.txt
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/pools.json
 Comment: 
 
-Filename: sbcli_adr-1.0.0/sbcli_adr.egg-info/entry_points.txt
+Filename: sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/node-exporter.json
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_adr-1.0.0/setup.py` & `sbcli_adr-1.0.1/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/README.md` & `sbcli_adr-1.0.1/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/PKG-INFO` & `sbcli_adr-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-adr
-Version: 1.0.0
+Version: 1.0.1
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_adr-1.0.0/simplyblock_cli/cli.py` & `sbcli_adr-1.0.1/simplyblock_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,19 @@
         sub_command = self.add_sub_command(subparser, "info", 'Get node information')
         sub_command.add_argument("id", help='Node UUID')
 
         # node info-spdk
         sub_command = self.add_sub_command(subparser, "info-spdk", 'Get SPDK memory information')
         sub_command.add_argument("id", help='Node UUID')
 
+        # get tasks list
+        sub_command = self.add_sub_command(subparser, "list-tasks", 'List tasks by cluster ID')
+        sub_command.add_argument("cluster_id", help='UUID of the cluster')
+
+
         # Initialize cluster parser
         subparser = self.add_command('cluster', 'Cluster commands')
 
         sub_command = self.add_sub_command(subparser, 'create',
                                            'Create an new cluster with this node as mgmt (local run)')
         sub_command.add_argument(
             "--blk_size", help='The block size in bytes', type=int, choices=[512, 4096], default=512)
@@ -976,14 +981,17 @@
 
             elif sub_command == "update":
                 ret = storage_ops.update(args.id, args.key, args.value)
 
             elif sub_command == "get":
                 ret = storage_ops.get(args.id)
 
+            elif sub_command == "list-tasks":
+                ret = storage_ops.list_tasks(args.cluster_id)
+
             else:
                 self.parser.print_help()
 
         elif args.command == 'cluster':
             sub_command = args_dict[args.command]
             if sub_command in ["add-dev-model", "rm-dev-model", "add-host-auth",
                                "rm-host-auth", "set-log-level"]:
```

## Comparing `sbcli_adr-1.0.0/simplyblock_core/storage_node_ops.py` & `sbcli_adr-1.0.1/simplyblock_core/storage_node_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1851,7 +1851,29 @@
     snode = db_controller.get_storage_node_by_id(node_id)
     if not snode:
         logger.error(f"Can not find storage node: {node_id}")
         return False
 
     data = snode.get_clean_dict()
     return json.dumps(data, indent=2)
+
+
+def list_tasks(cluster_id):
+    db_controller = DBController()
+    cluster = db_controller.get_cluster_by_id(cluster_id)
+    if not cluster:
+        logger.error("Cluster not found: %s", cluster_id)
+        return False
+
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

## Comparing `sbcli_adr-1.0.0/simplyblock_core/constants.py` & `sbcli_adr-1.0.1/simplyblock_core/constants.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/mgmt_node_ops.py` & `sbcli_adr-1.0.1/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/cnode_client.py` & `sbcli_adr-1.0.1/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/pci_utils.py` & `sbcli_adr-1.0.1/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/snode_client.py` & `sbcli_adr-1.0.1/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/kv_store.py` & `sbcli_adr-1.0.1/simplyblock_core/kv_store.py`

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
@@ -246,8 +247,8 @@
         stats = PortStat().read_from_db(self.kv_store, id="%s/%s" % (node_id, port_id), limit=limit, reverse=True)
         return stats
 
     def get_events(self, event_id=""):
         return EventObj().read_from_db(self.kv_store, id=event_id)
 
     def get_job_tasks(self, cluster_id):
-        return EventObj().read_from_db(self.kv_store, id=cluster_id, reverse=True)
+        return JobSchedule().read_from_db(self.kv_store, id=cluster_id, reverse=True)
```

## Comparing `sbcli_adr-1.0.0/simplyblock_core/utils.py` & `sbcli_adr-1.0.1/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/cluster_ops.py` & `sbcli_adr-1.0.1/simplyblock_core/cluster_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/compute_node_ops.py` & `sbcli_adr-1.0.1/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/rpc_client.py` & `sbcli_adr-1.0.1/simplyblock_core/rpc_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/distr_controller.py` & `sbcli_adr-1.0.1/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/services/lvol_monitor.py` & `sbcli_adr-1.0.1/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/services/caching_node_monitor.py` & `sbcli_adr-1.0.1/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/services/job_tasks.py` & `sbcli_adr-1.0.1/simplyblock_core/services/port_stat_collector.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,20 @@
 import time
 import sys
 
 import psutil
 
 
 from simplyblock_core import constants, kv_store, utils
-from simplyblock_core.models.job_schedule import JobSchedule
 from simplyblock_core.models.port_stat import PortStat
 
 # Import the GELF logger
 from graypy import GELFUDPHandler
 
-
-def task_runner(task):
+def update_port_stats(snode, nic, stats):
     now = int(time.time())
     data = {
         "uuid": nic.get_id(),
         "node_id": snode.get_id(),
         "date": now,
         "bytes_sent": stats.bytes_sent,
         "bytes_received": stats.bytes_recv,
@@ -50,21 +48,30 @@
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
 
-logger.info("Starting Jobs runner...")
+hostname = utils.get_hostname()
+logger.info("Starting port stats collector...")
 while True:
+    time.sleep(constants.PROT_STAT_COLLECTOR_INTERVAL_SEC)
 
-    clusters = db_controller.get_clusters()
-    if not clusters:
-        logger.error("No clusters found!")
-    else:
-        for cl in clusters:
-            tasks = db_controller.get_job_tasks(cl.get_id())
-            for task in tasks:
-                if task.status == JobSchedule.STATUS_NEW:
-                    res = task_runner(task)
+    snode = db_controller.get_storage_node_by_hostname(hostname)
+    if not snode:
+        logger.error("This node is not part of the cluster, hostname: %s" % hostname)
+        continue
+
+    if not snode.data_nics:
+        logger.error("No Data Ports found in node: %s", snode.get_id())
+        continue
+
+    io_stats = psutil.net_io_counters(pernic=True)
+    for nic in snode.data_nics:
+        logger.info("Getting port stats: %s", nic.get_id())
+        if nic.if_name in io_stats:
+            stats = io_stats[nic.if_name]
+            update_port_stats(snode, nic, stats)
+        else:
+            logger.error("Error getting port stats: %s", nic.get_id())
 
-    time.sleep(3)
```

## Comparing `sbcli_adr-1.0.0/simplyblock_core/services/health_check_service.py` & `sbcli_adr-1.0.1/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_adr-1.0.1/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/services/log_agg_service.py` & `sbcli_adr-1.0.1/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/services/distr_event_collector.py` & `sbcli_adr-1.0.1/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_adr-1.0.1/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/services/device_monitor.py` & `sbcli_adr-1.0.1/simplyblock_core/services/job_tasks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,101 @@
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
+
+def task_runner(task):
+    if task.retry <= 0:
+        task.function_result = "timeout"
+        task.status = JobSchedule.STATUS_DONE
+        task.write_to_db(db_controller.kv_store)
+        return
 
-def set_dev_status(device, status):
-    node = db_controller.get_storage_node_by_id(device.node_id)
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
+    res = device_controller.restart_device(device.get_id())
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
+                if task.status == JobSchedule.STATUS_NEW:
+                    res = task_runner(task)
+
+    time.sleep(5)
```

## Comparing `sbcli_adr-1.0.0/simplyblock_core/services/__init__.py` & `sbcli_adr-1.0.1/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/services/install_service.sh` & `sbcli_adr-1.0.1/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_adr-1.0.1/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/services/cap_monitor.py` & `sbcli_adr-1.0.1/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/services/storage_node_monitor.py` & `sbcli_adr-1.0.1/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_adr-1.0.1/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/haproxy.cfg` & `sbcli_adr-1.0.1/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_adr-1.0.1/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_adr-1.0.1/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml` & `sbcli_adr-1.0.1/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/__init__.py` & `sbcli_adr-1.0.1/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/install_deps.sh` & `sbcli_adr-1.0.1/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_adr-1.0.1/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_adr-1.0.1/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_adr-1.0.1/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/devices.json`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/node-exporter.json` & `sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/node-exporter.json`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/scripts/dashboards/pools.json` & `sbcli_adr-1.0.1/simplyblock_core/scripts/dashboards/pools.json`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/controllers/device_controller.py` & `sbcli_adr-1.0.1/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/controllers/mgmt_events.py` & `sbcli_adr-1.0.1/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/controllers/events_controller.py` & `sbcli_adr-1.0.1/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/controllers/storage_events.py` & `sbcli_adr-1.0.1/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/controllers/lvol_events.py` & `sbcli_adr-1.0.1/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_adr-1.0.1/simplyblock_core/controllers/snapshot_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/controllers/device_events.py` & `sbcli_adr-1.0.1/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/controllers/pool_controller.py` & `sbcli_adr-1.0.1/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/controllers/cluster_events.py` & `sbcli_adr-1.0.1/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_adr-1.0.1/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/controllers/snapshot_events.py` & `sbcli_adr-1.0.1/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/controllers/lvol_controller.py` & `sbcli_adr-1.0.1/simplyblock_core/controllers/lvol_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/controllers/health_controller.py` & `sbcli_adr-1.0.1/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/controllers/pool_events.py` & `sbcli_adr-1.0.1/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/events.py` & `sbcli_adr-1.0.1/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/job_schedule.py` & `sbcli_adr-1.0.1/simplyblock_core/models/nvme_device.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,60 @@
 # coding=utf-8
+from typing import List
+
 from simplyblock_core.models.base_model import BaseModel
 
 
-class JobSchedule(BaseModel):
+class NVMeDevice(BaseModel):
+
+    STATUS_JM = "JM_DEV"
 
-    STATUS_NEW = 'new'
-    STATUS_RUNNING = 'running'
-    STATUS_DONE = 'done'
+    STATUS_NEW = "new"
+    STATUS_ONLINE = 'online'
+    STATUS_UNAVAILABLE = 'unavailable'
+    STATUS_REMOVED = 'removed'
+    STATUS_FAILED = 'failed'
+    STATUS_READONLY = 'read_only'
 
     attributes = {
         "uuid": {"type": str, 'default': ""},
-        "cluster_uuid": {"type": str, 'default': ""},
-        "node_id": {"type": str, 'default': ""},
-        "date": {"type": int, 'default': 0},
-
-        "function_name": {"type": str, 'default': ""},
-        "function_params": {"type": dict, 'default': {}},
-
+        "device_name": {"type": str, 'default': ""},
         "status": {"type": str, 'default': ""},
+        "sequential_number": {"type": int, 'default': 0},
+        "partitions_count": {"type": int, 'default': 0},
+        "capacity": {"type": int, 'default': -1},
+        "size": {"type": int, 'default': -1},
+        "pcie_address": {"type": str, 'default': ""},
+        "model_id": {"type": str, 'default': ""},
+        "serial_number": {"type": str, 'default': ""},
+        "overload_percentage": {"type": int, 'default': 0},
+        "nvme_bdev": {"type": str, 'default': ""},
+        "alloc_bdev": {"type": str, 'default': ""},
+        "alceml_bdev": {"type": str, 'default': ""},
+        "node_id": {"type": str, 'default': ""},
+        "pt_bdev": {"type": str, 'default': ""},
+        "nvmf_nqn": {"type": str, 'default': ""},
+        "nvmf_ip": {"type": str, 'default': ""},
+        "nvmf_port": {"type": int, 'default': 0},
+        "remote_bdev": {"type": str, 'default': ""},
+        "testing_bdev": {"type": str, 'default': ""},
+        "jm_bdev": {"type": str, 'default': ""},
+        "cluster_device_order": {"type": int, 'default': 0},
+        "health_check": {"type": bool, "default": True},
+        "cluster_id": {"type": str, 'default': ""},
 
+        "bdev_stack": {"type": List, 'default': []},
 
-        "event": {"type": str, 'default': ""},
-        "domain": {"type": str, 'default': ""},
-        "object_name": {"type": str, 'default': ""},
-        "object_dict": {"type": dict, 'default': {}},
-        "caused_by": {"type": str, 'default': ""},
-        "message": {"type": str, 'default': ""},
-        "storage_id": {"type": int, 'default': -1},
-        "vuid": {"type": int, 'default': -1},
-        "meta_data": {"type": str, 'default': ""},
-
+        "io_error": {"type": bool, 'default': False},
 
     }
 
     def __init__(self, data=None):
-        super(JobSchedule, self).__init__()
+        super(NVMeDevice, self).__init__()
         self.set_attrs(self.attributes, data)
         self.object_type = "object"
 
     def get_id(self):
-        return "%s/%s/%s" % (self.cluster_uuid, self.date, self.uuid)
+        return self.uuid
+
+    def get_capacity_percentage(self):
+        return ((self.size - self.capacity) / self.size) * 100
```

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/iface.py` & `sbcli_adr-1.0.1/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/base_model.py` & `sbcli_adr-1.0.1/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/lvol_model.py` & `sbcli_adr-1.0.1/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/compute_node.py` & `sbcli_adr-1.0.1/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/snapshot.py` & `sbcli_adr-1.0.1/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/pool.py` & `sbcli_adr-1.0.1/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/global_settings.py` & `sbcli_adr-1.0.1/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/port_stat.py` & `sbcli_adr-1.0.1/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/storage_node.py` & `sbcli_adr-1.0.1/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/stats.py` & `sbcli_adr-1.0.1/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/cluster.py` & `sbcli_adr-1.0.1/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/mgmt_node.py` & `sbcli_adr-1.0.1/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_core/models/caching_node.py` & `sbcli_adr-1.0.1/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/caching_node_app_k8s.py` & `sbcli_adr-1.0.1/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/node_utils.py` & `sbcli_adr-1.0.1/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/snode_app.py` & `sbcli_adr-1.0.1/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/app.py` & `sbcli_adr-1.0.1/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/auth_middleware.py` & `sbcli_adr-1.0.1/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/caching_node_app.py` & `sbcli_adr-1.0.1/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/utils.py` & `sbcli_adr-1.0.1/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/node_webapp.py` & `sbcli_adr-1.0.1/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/static/delete.py` & `sbcli_adr-1.0.1/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/static/deploy.py` & `sbcli_adr-1.0.1/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_adr-1.0.1/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_adr-1.0.1/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_adr-1.0.1/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_adr-1.0.1/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/blueprints/snode_ops.py` & `sbcli_adr-1.0.1/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/blueprints/csi.py` & `sbcli_adr-1.0.1/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_adr-1.0.1/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_adr-1.0.1/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_device.py` & `sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_adr-1.0.1/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_adr-1.0.1/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/sbcli_adr.egg-info/SOURCES.txt` & `sbcli_adr-1.0.1/sbcli_adr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli_adr-1.0.0/sbcli_adr.egg-info/PKG-INFO` & `sbcli_adr-1.0.1/sbcli_adr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-adr
-Version: 1.0.0
+Version: 1.0.1
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

