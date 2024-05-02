# Comparing `tmp/sbcli_release-1.0.9.zip` & `tmp/sbcli_release-1.1.0.zip`

## zipinfo {}

```diff
@@ -1,148 +1,148 @@
-Zip file size: 215466 bytes, number of entries: 146
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 01:47 sbcli_release-1.0.9/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 01:47 sbcli_release-1.0.9/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 01:47 sbcli_release-1.0.9/sbcli_release.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 01:47 sbcli_release-1.0.9/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 01:47 sbcli_release-1.0.9/simplyblock_web/
--rw-r--r--  2.0 unx     2269 b- defN 24-May-01 01:46 sbcli_release-1.0.9/setup.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-01 01:46 sbcli_release-1.0.9/README.md
--rw-r--r--  2.0 unx      158 b- defN 24-May-01 01:46 sbcli_release-1.0.9/env_var
--rw-r--r--  2.0 unx       84 b- defN 24-May-01 01:46 sbcli_release-1.0.9/pyproject.toml
--rw-r--r--  2.0 unx       38 b- defN 24-May-01 01:47 sbcli_release-1.0.9/setup.cfg
--rw-r--r--  2.0 unx     1493 b- defN 24-May-01 01:47 sbcli_release-1.0.9/PKG-INFO
--rw-r--r--  2.0 unx    77592 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_cli/main.py
--rw-r--r--  2.0 unx        1 b- defN 24-May-01 01:47 sbcli_release-1.0.9/sbcli_release.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     5212 b- defN 24-May-01 01:47 sbcli_release-1.0.9/sbcli_release.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       49 b- defN 24-May-01 01:47 sbcli_release-1.0.9/sbcli_release.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1493 b- defN 24-May-01 01:47 sbcli_release-1.0.9/sbcli_release.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       73 b- defN 24-May-01 01:47 sbcli_release-1.0.9/sbcli_release.egg-info/requires.txt
--rw-r--r--  2.0 unx       59 b- defN 24-May-01 01:47 sbcli_release-1.0.9/sbcli_release.egg-info/entry_points.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 01:47 sbcli_release-1.0.9/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 01:47 sbcli_release-1.0.9/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 01:47 sbcli_release-1.0.9/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 01:47 sbcli_release-1.0.9/simplyblock_core/models/
--rw-r--r--  2.0 unx    69599 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1485 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3153 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx      279 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx      938 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3416 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     8189 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     7640 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/utils.py
--rw-r--r--  2.0 unx    23423 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx     5112 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    21980 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     7479 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx     2189 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx     3203 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     5462 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx      229 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     5268 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     2410 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5140 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx     7438 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2423 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     4118 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx      837 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2671 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6577 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/services/storage_node_monitor.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 01:47 sbcli_release-1.0.9/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 01:47 sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx      930 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx      152 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx     4977 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx       54 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx     4470 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
--rw-r--r--  2.0 unx      453 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx     1782 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx      311 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx      118 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx      360 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx       43 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1438 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx      311 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/prometheus.yml
--rwxr-xr-x  2.0 unx      657 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx    25433 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1856 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx   106705 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx   799409 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/node-exporter.json
--rw-r--r--  2.0 unx    99758 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    99862 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/pools.json
--rw-r--r--  2.0 unx    13127 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1120 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     3191 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx     1521 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1630 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    10557 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx    10375 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1900 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx    22802 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx    47366 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx    11298 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx     1500 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx      806 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4846 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      917 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx      736 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     1602 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     1228 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     1020 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx     3765 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     4242 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     2565 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx     3766 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     3113 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_core/models/nvme_device.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 01:47 sbcli_release-1.0.9/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 01:47 sbcli_release-1.0.9/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 01:47 sbcli_release-1.0.9/simplyblock_web/blueprints/
--rw-r--r--  2.0 unx      725 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     5098 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx      703 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     1263 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     2513 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      507 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      322 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      434 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      827 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx     1302 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     2876 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5547 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     4795 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5392 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx    10879 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx     8547 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx    11244 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx    12198 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx      975 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     6326 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     7846 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     2940 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     5274 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx     6206 b- defN 24-May-01 01:46 sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_pool.py
-146 files, 1931084 bytes uncompressed, 187664 bytes compressed:  90.3%
+Zip file size: 215504 bytes, number of entries: 146
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/sbcli_release.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/
+-rw-r--r--  2.0 unx     2269 b- defN 24-May-02 16:27 sbcli_release-1.1.0/setup.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-02 16:27 sbcli_release-1.1.0/README.md
+-rw-r--r--  2.0 unx      158 b- defN 24-May-02 16:27 sbcli_release-1.1.0/env_var
+-rw-r--r--  2.0 unx       84 b- defN 24-May-02 16:27 sbcli_release-1.1.0/pyproject.toml
+-rw-r--r--  2.0 unx       38 b- defN 24-May-02 16:27 sbcli_release-1.1.0/setup.cfg
+-rw-r--r--  2.0 unx     1493 b- defN 24-May-02 16:27 sbcli_release-1.1.0/PKG-INFO
+-rw-r--r--  2.0 unx    77592 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_cli/main.py
+-rw-r--r--  2.0 unx        1 b- defN 24-May-02 16:27 sbcli_release-1.1.0/sbcli_release.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     5212 b- defN 24-May-02 16:27 sbcli_release-1.1.0/sbcli_release.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       49 b- defN 24-May-02 16:27 sbcli_release-1.1.0/sbcli_release.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1493 b- defN 24-May-02 16:27 sbcli_release-1.1.0/sbcli_release.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       73 b- defN 24-May-02 16:27 sbcli_release-1.1.0/sbcli_release.egg-info/requires.txt
+-rw-r--r--  2.0 unx       59 b- defN 24-May-02 16:27 sbcli_release-1.1.0/sbcli_release.egg-info/entry_points.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/
+-rw-r--r--  2.0 unx    69747 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1485 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx      279 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx      938 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3416 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8189 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx    23423 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    21980 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     7504 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx      229 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     5268 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     2410 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5140 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx     7438 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx      837 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6577 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/storage_node_monitor.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx      930 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx      152 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx     4977 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx       54 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx     4470 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+-rw-r--r--  2.0 unx      453 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx     1782 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx      311 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx      118 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx       43 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1438 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/prometheus.yml
+-rwxr-xr-x  2.0 unx      657 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx    25433 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1856 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx   106705 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx   799409 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/node-exporter.json
+-rw-r--r--  2.0 unx    99758 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    99862 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/pools.json
+-rw-r--r--  2.0 unx    13127 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     3191 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10557 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx    22802 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx    47366 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx    11298 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx      806 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      917 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx      736 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx     3765 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     3136 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/nvme_device.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/
+-rw-r--r--  2.0 unx      725 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx      703 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     2513 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      507 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      322 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      434 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5547 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     4795 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5392 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx    10879 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx     8547 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx      975 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     7846 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     5274 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_pool.py
+146 files, 1931280 bytes uncompressed, 187702 bytes compressed:  90.3%
```

## zipnote {}

```diff
@@ -1,439 +1,439 @@
-Filename: sbcli_release-1.0.9/
+Filename: sbcli_release-1.1.0/
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_cli/
+Filename: sbcli_release-1.1.0/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_release-1.0.9/sbcli_release.egg-info/
+Filename: sbcli_release-1.1.0/sbcli_release.egg-info/
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/
+Filename: sbcli_release-1.1.0/simplyblock_core/
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/
+Filename: sbcli_release-1.1.0/simplyblock_web/
 Comment: 
 
-Filename: sbcli_release-1.0.9/setup.py
+Filename: sbcli_release-1.1.0/setup.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/README.md
+Filename: sbcli_release-1.1.0/README.md
 Comment: 
 
-Filename: sbcli_release-1.0.9/env_var
+Filename: sbcli_release-1.1.0/env_var
 Comment: 
 
-Filename: sbcli_release-1.0.9/pyproject.toml
+Filename: sbcli_release-1.1.0/pyproject.toml
 Comment: 
 
-Filename: sbcli_release-1.0.9/setup.cfg
+Filename: sbcli_release-1.1.0/setup.cfg
 Comment: 
 
-Filename: sbcli_release-1.0.9/PKG-INFO
+Filename: sbcli_release-1.1.0/PKG-INFO
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_cli/cli.py
+Filename: sbcli_release-1.1.0/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_cli/main.py
+Filename: sbcli_release-1.1.0/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/sbcli_release.egg-info/dependency_links.txt
+Filename: sbcli_release-1.1.0/sbcli_release.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli_release-1.0.9/sbcli_release.egg-info/SOURCES.txt
+Filename: sbcli_release-1.1.0/sbcli_release.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_release-1.0.9/sbcli_release.egg-info/top_level.txt
+Filename: sbcli_release-1.1.0/sbcli_release.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_release-1.0.9/sbcli_release.egg-info/PKG-INFO
+Filename: sbcli_release-1.1.0/sbcli_release.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_release-1.0.9/sbcli_release.egg-info/requires.txt
+Filename: sbcli_release-1.1.0/sbcli_release.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_release-1.0.9/sbcli_release.egg-info/entry_points.txt
+Filename: sbcli_release-1.1.0/sbcli_release.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/
+Filename: sbcli_release-1.1.0/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/
+Filename: sbcli_release-1.1.0/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/storage_node_ops.py
+Filename: sbcli_release-1.1.0/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/constants.py
+Filename: sbcli_release-1.1.0/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_release-1.1.0/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/cnode_client.py
+Filename: sbcli_release-1.1.0/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/shell_utils.py
+Filename: sbcli_release-1.1.0/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/pci_utils.py
+Filename: sbcli_release-1.1.0/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/__init__.py
+Filename: sbcli_release-1.1.0/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/snode_client.py
+Filename: sbcli_release-1.1.0/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/kv_store.py
+Filename: sbcli_release-1.1.0/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/utils.py
+Filename: sbcli_release-1.1.0/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/cluster_ops.py
+Filename: sbcli_release-1.1.0/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/compute_node_ops.py
+Filename: sbcli_release-1.1.0/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/rpc_client.py
+Filename: sbcli_release-1.1.0/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/distr_controller.py
+Filename: sbcli_release-1.1.0/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_release-1.1.0/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_release-1.1.0/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/health_check_service.py
+Filename: sbcli_release-1.1.0/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/service_template.service
+Filename: sbcli_release-1.1.0/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_release-1.1.0/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/remove_service.sh
+Filename: sbcli_release-1.1.0/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_release-1.1.0/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_release-1.1.0/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_release-1.1.0/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_release-1.1.0/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/device_monitor.py
+Filename: sbcli_release-1.1.0/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/__init__.py
+Filename: sbcli_release-1.1.0/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/install_service.sh
+Filename: sbcli_release-1.1.0/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_release-1.1.0/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_release-1.1.0/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_release-1.1.0/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/alerting/
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/__init__.py
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/node-exporter.json
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/node-exporter.json
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/pools.json
+Filename: sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/pools.json
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/device_events.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/__init__.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_release-1.1.0/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/events.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/iface.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/base_model.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/lvol_model.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/compute_node.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/snapshot.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/pool.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/global_settings.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/port_stat.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/storage_node.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/__init__.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/stats.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/cluster.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/caching_node.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_core/models/nvme_device.py
+Filename: sbcli_release-1.1.0/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/static/
+Filename: sbcli_release-1.1.0/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/templates/
+Filename: sbcli_release-1.1.0/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_release-1.1.0/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/node_utils.py
+Filename: sbcli_release-1.1.0/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/snode_app.py
+Filename: sbcli_release-1.1.0/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/app.py
+Filename: sbcli_release-1.1.0/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/auth_middleware.py
+Filename: sbcli_release-1.1.0/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/__init__.py
+Filename: sbcli_release-1.1.0/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/caching_node_app.py
+Filename: sbcli_release-1.1.0/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/utils.py
+Filename: sbcli_release-1.1.0/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/node_webapp.py
+Filename: sbcli_release-1.1.0/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_release-1.1.0/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/static/tst.py
+Filename: sbcli_release-1.1.0/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/static/is_up.py
+Filename: sbcli_release-1.1.0/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/static/delete.py
+Filename: sbcli_release-1.1.0/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/static/deploy.py
+Filename: sbcli_release-1.1.0/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_release-1.1.0/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/static/rpac.yaml
+Filename: sbcli_release-1.1.0/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/static/list_deps.py
+Filename: sbcli_release-1.1.0/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_release-1.1.0/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/csi.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_release-1.0.9/setup.py` & `sbcli_release-1.1.0/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/README.md` & `sbcli_release-1.1.0/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/PKG-INFO` & `sbcli_release-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-release
-Version: 1.0.9
+Version: 1.1.0
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_release-1.0.9/simplyblock_cli/cli.py` & `sbcli_release-1.1.0/simplyblock_cli/cli.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/sbcli_release.egg-info/SOURCES.txt` & `sbcli_release-1.1.0/sbcli_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/sbcli_release.egg-info/PKG-INFO` & `sbcli_release-1.1.0/sbcli_release.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-release
-Version: 1.0.9
+Version: 1.1.0
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_release-1.0.9/simplyblock_core/storage_node_ops.py` & `sbcli_release-1.1.0/simplyblock_core/storage_node_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -823,14 +823,15 @@
 
     snode.remove(db_controller.kv_store)
 
     for lvol in db_controller.get_lvols():
         logger.info(f"Sending cluster map to LVol: {lvol.get_id()}")
         lvol_controller.send_cluster_map(lvol.get_id())
 
+    storage_events.snode_delete(snode)
     logger.info("done")
 
 
 def remove_storage_node(node_id, force_remove=False, force_migrate=False):
     db_controller = DBController()
     snode = db_controller.get_storage_node_by_id(node_id)
     if not snode:
@@ -893,19 +894,20 @@
     try:
         snode_api = SNodeClient(snode.api_endpoint, timeout=20)
         snode_api.spdk_process_kill()
         snode_api.leave_swarm()
     except Exception as e:
         logger.warning(f"Failed to remove SPDK process: {e}")
 
+    old_status = snode.status
     snode.status = StorageNode.STATUS_REMOVED
     snode.write_to_db(db_controller.kv_store)
     logger.info("Sending node event update")
     distr_controller.send_node_status_event(snode.get_id(), snode.status)
-    storage_events.snode_remove(snode)
+    storage_events.snode_status_change(snode, StorageNode.STATUS_REMOVED, old_status)
     logger.info("done")
 
 
 def restart_storage_node(
         node_id,
         spdk_cpu_mask=None,
         spdk_mem=None,
@@ -1088,45 +1090,45 @@
             else:
                 node.remote_devices.append(dev)
             count += 1
         node.write_to_db(kv_store)
         logger.info(f"connected to devices count: {count}")
         time.sleep(3)
 
-    logger.info("Sending cluster map")
-    ret = distr_controller.send_cluster_map_to_node(snode)
-    if not ret:
-        return False, "Failed to send cluster map"
-    time.sleep(3)
+    logger.info("Setting node status to Online")
+    old_status = snode.status
+    snode.status = StorageNode.STATUS_ONLINE
+    snode.write_to_db(kv_store)
+    storage_events.snode_status_change(snode, snode.status, old_status)
 
     logger.info("Sending node event update")
-    distr_controller.send_node_status_event(snode.get_id(), "online")
+    distr_controller.send_node_status_event(snode.get_id(), NVMeDevice.STATUS_ONLINE)
 
     logger.info("Sending devices event updates")
     for dev in snode.nvme_devices:
         if dev.status != NVMeDevice.STATUS_ONLINE:
             logger.debug(f"Device is not online: {dev.get_id()}, status: {dev.status}")
             continue
         distr_controller.send_dev_status_event(dev.cluster_device_order, NVMeDevice.STATUS_ONLINE)
 
+    logger.info("Sending cluster map to current node")
+    ret = distr_controller.send_cluster_map_to_node(snode)
+    if not ret:
+        return False, "Failed to send cluster map"
+    time.sleep(3)
+
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
```

## Comparing `sbcli_release-1.0.9/simplyblock_core/constants.py` & `sbcli_release-1.1.0/simplyblock_core/constants.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/mgmt_node_ops.py` & `sbcli_release-1.1.0/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/cnode_client.py` & `sbcli_release-1.1.0/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/pci_utils.py` & `sbcli_release-1.1.0/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/snode_client.py` & `sbcli_release-1.1.0/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/kv_store.py` & `sbcli_release-1.1.0/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/utils.py` & `sbcli_release-1.1.0/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/cluster_ops.py` & `sbcli_release-1.1.0/simplyblock_core/cluster_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/compute_node_ops.py` & `sbcli_release-1.1.0/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/rpc_client.py` & `sbcli_release-1.1.0/simplyblock_core/rpc_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/distr_controller.py` & `sbcli_release-1.1.0/simplyblock_core/distr_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     map_prob = []
     for snode in snodes:
         dev_map = {}
         dev_w_map = []
         node_w = 0
         for i, dev in enumerate(snode.nvme_devices):
             logger.debug(f"Device: {dev.get_id()}, status: {dev.status}")
-            if dev.status == NVMeDevice.STATUS_JM:
+            if dev.status in [NVMeDevice.STATUS_JM, NVMeDevice.STATUS_NEW]:
                 continue
 
             dev_w = int(dev.size/(1024*1024*1024)) or 1
             node_w += dev_w
             name = None
             if snode.get_id() == target_node.get_id():
                 name = dev.alceml_bdev
```

## Comparing `sbcli_release-1.0.9/simplyblock_core/services/lvol_monitor.py` & `sbcli_release-1.1.0/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/services/caching_node_monitor.py` & `sbcli_release-1.1.0/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/services/health_check_service.py` & `sbcli_release-1.1.0/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_release-1.1.0/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/services/log_agg_service.py` & `sbcli_release-1.1.0/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/services/distr_event_collector.py` & `sbcli_release-1.1.0/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_release-1.1.0/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/services/port_stat_collector.py` & `sbcli_release-1.1.0/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/services/device_monitor.py` & `sbcli_release-1.1.0/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/services/__init__.py` & `sbcli_release-1.1.0/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/services/install_service.sh` & `sbcli_release-1.1.0/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_release-1.1.0/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/services/cap_monitor.py` & `sbcli_release-1.1.0/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/services/storage_node_monitor.py` & `sbcli_release-1.1.0/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_release-1.1.0/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/haproxy.cfg` & `sbcli_release-1.1.0/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_release-1.1.0/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_release-1.1.0/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml` & `sbcli_release-1.1.0/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/__init__.py` & `sbcli_release-1.1.0/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/install_deps.sh` & `sbcli_release-1.1.0/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_release-1.1.0/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_release-1.1.0/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_release-1.1.0/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/devices.json`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/node-exporter.json` & `sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/node-exporter.json`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/scripts/dashboards/pools.json` & `sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/pools.json`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/controllers/device_controller.py` & `sbcli_release-1.1.0/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/controllers/mgmt_events.py` & `sbcli_release-1.1.0/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/controllers/events_controller.py` & `sbcli_release-1.1.0/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/controllers/storage_events.py` & `sbcli_release-1.1.0/simplyblock_core/controllers/storage_events.py`

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

## Comparing `sbcli_release-1.0.9/simplyblock_core/controllers/lvol_events.py` & `sbcli_release-1.1.0/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_release-1.1.0/simplyblock_core/controllers/snapshot_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/controllers/device_events.py` & `sbcli_release-1.1.0/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/controllers/pool_controller.py` & `sbcli_release-1.1.0/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/controllers/cluster_events.py` & `sbcli_release-1.1.0/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_release-1.1.0/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/controllers/snapshot_events.py` & `sbcli_release-1.1.0/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/controllers/lvol_controller.py` & `sbcli_release-1.1.0/simplyblock_core/controllers/lvol_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/controllers/health_controller.py` & `sbcli_release-1.1.0/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/controllers/pool_events.py` & `sbcli_release-1.1.0/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/events.py` & `sbcli_release-1.1.0/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/iface.py` & `sbcli_release-1.1.0/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/base_model.py` & `sbcli_release-1.1.0/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/lvol_model.py` & `sbcli_release-1.1.0/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/compute_node.py` & `sbcli_release-1.1.0/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/snapshot.py` & `sbcli_release-1.1.0/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/pool.py` & `sbcli_release-1.1.0/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/global_settings.py` & `sbcli_release-1.1.0/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/port_stat.py` & `sbcli_release-1.1.0/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/storage_node.py` & `sbcli_release-1.1.0/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/stats.py` & `sbcli_release-1.1.0/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/cluster.py` & `sbcli_release-1.1.0/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/mgmt_node.py` & `sbcli_release-1.1.0/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/caching_node.py` & `sbcli_release-1.1.0/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_core/models/nvme_device.py` & `sbcli_release-1.1.0/simplyblock_core/models/nvme_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from simplyblock_core.models.base_model import BaseModel
 
 
 class NVMeDevice(BaseModel):
 
     STATUS_JM = "JM_DEV"
 
+    STATUS_NEW = "new"
     STATUS_ONLINE = 'online'
     STATUS_UNAVAILABLE = 'unavailable'
     STATUS_REMOVED = 'removed'
     STATUS_FAILED = 'failed'
     STATUS_READONLY = 'read_only'
 
     attributes = {
```

## Comparing `sbcli_release-1.0.9/simplyblock_web/caching_node_app_k8s.py` & `sbcli_release-1.1.0/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/node_utils.py` & `sbcli_release-1.1.0/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/snode_app.py` & `sbcli_release-1.1.0/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/app.py` & `sbcli_release-1.1.0/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/auth_middleware.py` & `sbcli_release-1.1.0/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/caching_node_app.py` & `sbcli_release-1.1.0/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/utils.py` & `sbcli_release-1.1.0/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/node_webapp.py` & `sbcli_release-1.1.0/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/static/delete.py` & `sbcli_release-1.1.0/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/static/deploy.py` & `sbcli_release-1.1.0/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_release-1.1.0/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_release-1.1.0/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/blueprints/snode_ops.py` & `sbcli_release-1.1.0/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/blueprints/csi.py` & `sbcli_release-1.1.0/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_release-1.1.0/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_release-1.1.0/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_device.py` & `sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.0.9/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

