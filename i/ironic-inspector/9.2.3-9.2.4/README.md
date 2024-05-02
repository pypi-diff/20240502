# Comparing `tmp/ironic-inspector-9.2.3.tar.gz` & `tmp/ironic-inspector-9.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ironic-inspector-9.2.3.tar", last modified: Mon Jun 15 09:51:41 2020, max compression
+gzip compressed data, was "dist/ironic-inspector-9.2.4.tar", last modified: Mon Feb  1 18:37:09 2021, max compression
```

## Comparing `ironic-inspector-9.2.3.tar` & `ironic-inspector-9.2.4.tar`

### file list

```diff
@@ -1,415 +1,418 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/ironic_inspector.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/ironic_inspector.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/ironic_inspector.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/ironic_inspector.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2679 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/ironic_inspector.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/ironic_inspector.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18031 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/ironic_inspector.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3236 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/ironic_inspector.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/ironic_inspector.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3269 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/bindep.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47485 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/LICENSE
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/introspection-api-v1-introspection-management.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2047 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/introspection-api-versions.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2709 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/introspection-api-v1-introspection.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6634 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7841 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/api-ref/source/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/samples/api-v1-get-introspections-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/samples/api-v1-get-introspection-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/samples/api-v1-create-rule-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/samples/api-v1-get-rules-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/samples/api-v1-common-node-uuid.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1517 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/samples/api-v1-continue-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      653 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/samples/api-v1-create-rule-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/samples/api-v1-get-rule-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/samples/api-v1-common-rule-uuid.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/samples/api-v1-root-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/samples/api-root-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2508 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/samples/api-v1-data-introspection-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1644 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/introspection-api-v1-continue.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2756 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/api-ref/source/introspection-api-v1-rules.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      969 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/rootwrap.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2679 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic-inspector.8
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/ironic_inspector/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/ironic_inspector/migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/migrations/script.py.mako
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2470 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/migrations/env.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/ironic_inspector/migrations/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/migrations/versions/e169a4a81d88_add_invert_field_to_rule_condition.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/migrations/versions/2970d2d44edc_add_manage_boot_to_nodes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1868 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/migrations/versions/578f84f38d_inital_db_schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1339 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/migrations/versions/bf8dec16023c_add_introspection_data_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3136 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/migrations/versions/882b2d84cb1b_attribute_constraints_relaxing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/migrations/versions/d2e48801c8ef_introducing_node_state_attribute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/migrations/versions/d588418040d_add_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1358 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/migrations/versions/18440d0834af_introducing_the_aborting_state.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2709 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/migrations/versions/d00d6e3f38c4_change_created_finished_at_type.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/ironic_inspector/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1991 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conf/dnsmasq_pxe_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1505 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conf/swift.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4210 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conf/default.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1129 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conf/coordination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conf/pxe_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1080 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conf/pci_devices.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conf/discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conf/service_catalog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conf/iptables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conf/ironic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5707 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conf/processing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1567 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3352 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conf/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conf/capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6849 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/introspect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17119 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1723 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/wsgi_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/ironic_inspector/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/cmd/conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1124 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/cmd/wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4465 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/cmd/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/cmd/all.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3058 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/cmd/dbsync.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/alembic.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7889 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/ironic_inspector/conductor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conductor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7618 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/conductor/manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/ironic_inspector/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2729 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/common/locking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5346 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/common/swift.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14392 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/common/lldp_parsers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4770 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/common/coordination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1867 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/common/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/common/service_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2076 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/common/rpc_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10601 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/common/ironic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/common/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/common/rpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2797 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/common/keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10500 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/common/lldp_tlvs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15896 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/process.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/ironic_inspector/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6132 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/plugins/rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2730 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/plugins/pci_devices.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13899 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/plugins/standard.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3095 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/plugins/discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4500 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/plugins/raid_device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4447 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/plugins/introspection_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3236 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/plugins/lldp_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4138 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/plugins/extra_hardware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6451 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/plugins/local_link_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1381 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/plugins/example.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8352 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/plugins/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2741 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/plugins/capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2506 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/api_tools.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/ironic_inspector/pxe_filter/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1991 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/pxe_filter/interface.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9334 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/pxe_filter/iptables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7133 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/pxe_filter/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/pxe_filter/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11643 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/pxe_filter/dnsmasq.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/ironic_inspector/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31763 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/functional.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8333 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12163 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_common_ironic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3563 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_locking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1369 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/policy_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4722 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_api_tools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5108 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_coordination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22203 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13411 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_lldp_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6725 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32538 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21879 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5084 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_extra_hardware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2987 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3050 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3175 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_introspection_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26643 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_introspect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20574 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_dnsmasq_pxe_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5380 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_swift.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3420 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9455 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_local_link_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6346 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22809 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_standard.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4835 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_raid_device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3292 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_wsgi_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    57571 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_node_cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4965 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_pci_devices.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11505 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_pxe_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33392 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_process.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20881 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_migrations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17843 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_iptables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11806 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_rules.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/ironic_inspector/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/ironic_inspector/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/ironic_inspector/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25122 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/locale/en_GB/LC_MESSAGES/ironic_inspector.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38506 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/node_cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7120 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4632 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/introspection_state.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6647 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14902 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/ironic_inspector/main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13616 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/CONTRIBUTING.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5752 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/Makefile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1775 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/contributor/jobs-description.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17730 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12393 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/user/http-api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16165 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/user/usage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6328 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/user/troubleshooting.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3557 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/user/workflow.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/.gitignore
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/configuration/sample-policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/configuration/ironic-inspector.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/configuration/policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/configuration/sample-config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3494 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/doc/source/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16969 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/images/states.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4944 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/admin/dnsmasq-pxe-filter.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1491 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/doc/source/admin/upgrade.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1990 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/tools/test-setup.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/tools/policy-generator.conf
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3208 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/tools/states_to_dot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8360 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/tools/bandit.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/tools/config-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4754 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4421 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/AUTHORS
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/active-node-not-in-cache-b2d7b77603f02a66.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/ramdisk-logs-on-all-failures-24da41edf3a98400.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/introspection-data-db-store-0586292de05cbfd7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/add-support-for-listing-all-introspection-statuses-2a3d4379c3854894.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/reset-interfaces-ff78d50b9f05d47d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/cpu-memory-cfdc72b625780871.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/validate-ipv6-address-fda29c929754352e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/nested-value-formatting-e04f187475e5e475.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/rollback-removal-a03a989e2e9f776b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/support-microversion-latest-dcf9598c5218e979.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/split-services-99873ff27ef2d89b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/rollback-formatting-7d61c9af2600d42f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/deprecate-ssl-opts-40ce8f4618c786ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/no-root_device_hint-0e7676d481d503bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/flask-debug-6d2dcc2b482324dc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/contains-matches-ee28958b08995494.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/add-lldp-plugin-4645596cb8b39fd3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/swift-max-retries-dfaecb74bd3aba9a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/migrations-autogenerate-4303fd496c3c2757.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/fix-periodic-tasks-configuration-edd167f0146e60b5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/fix-wrong-provision-state-name-150c91c48d471bf9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/missing-pxe-mac-d9329dab85513460.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/compact-debug-logging-b15dd9bbdd3ce27a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/firewall-rerun-f2d0f64cca2698ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/allow-periodics-shutdown-inspector-ac28ea5ba3224279.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/abort-introspection-ae5cb5a9fbacd2ac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/deprecated-ironic-1751ceec6295917d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/patch-head-backslash-24bcdd03ba254bf2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/stein-prelude-42f0d90bf2c6a1a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/edeploy-typeerror-6486e31923d91666.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/size-hint-ea2a264468e1fcb7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/persistent-boot-207b32257a97451e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/dnsmasq-pxe-filter-37928d3fdb1e8ec3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/names-82d9f84153a228ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/introspection-state-03538fac198882b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/active_states_timeout-3e3ab110870483ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/reapply-introspection-5edbbfaf498dbd12.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      439 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/status-removal-fa1d9a98ffad9f60.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1778 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/policy-engine-c44828e3131e6c62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/bmc-logging-deprecation-4ca046a64fac6f11.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/periodics-18bf7fb57777c043.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/lookup-all-macs-eead528c0b764ad7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/futurist-557fcd18d4eaf1c1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/continue-http-500-62f33d425aade9d7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/stop-when-setbootdev-failed-68d84fec0843bdc8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/add-support-for-long-running-ramdisk-ffee3c177c56cebb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/active-introspection-949f4a50c9d5218a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/change_started_finished_at_type_to_datetime-c5617e598350970c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/trailing-slashes-93c2466b71829ec1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/ironic-lib-hints-20412a1c7fa796e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/add-node-state-to-introspection-api-response-85fb7f4e72ae386a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/empty-ipmi-address-2-4d57c34aec7d14e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/node-locking-4d135ca5b93524b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/trait-actions-eec05cbb6a944619.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/fix_llc_hook_bugs-efeea008c2f792eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/ksadapters-abc9edc63cafa405.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/infiniband-support-960d6846e326dec4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/custom-ramdisk-log-name-dac06822c38657e7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/remove-opt-group-firewall-96266983e476c29e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/less-iptables-calls-759e89d103df504c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/ipa-inventory-0a1e8d644da850ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/mdns-a5f4034257139e31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/logs-collector-logging-356e56cd70a04a2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/deprecated-options-removal-ocata-a44dadf3bcf8d6fc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/extend-rules-9a9d38701e970611.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/no-logs-stored-data-6db52934c7f9a91a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/empty-ipmi-address-5b5ca186a066ed32.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/remove-deprecated-conf-opts-361ab0bb342f0e7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/processing-logging-e2d27bbac95a7213.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/manage-boot-2ae986f87098576b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/enroll-nodes-with-bmc-v6address-ba224f4a8a151c53.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/no-rollback-e15bc7fee0134545.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/handle-patch-port-failure-9a8b85749104506f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/no-fail-on-power-off-enroll-node-e40854f6def397b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/fix-pxe-filter-get-blacklist-2dde59d51c1d010f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/manage-boot-power-off-d8ed644f11659c38.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/unmanaged-result-4de3788e7820e3c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/update-default-ironic-api-stein-b3b01ec542fa8f15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/remove-opt-keep-node-status-7d6b96f1a6e498a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/remove-store-data-location-e68462ff6ba257e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/empty-condition-abc707b771be6be3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/pgsql-imperative-enum-dda76f150a205d0a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/fix_node_uuid_for_manual_inspection-2fa3f11343cab417.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/post-introspection-data-9cdd39a3de446e92.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/support-ip6tables-ce30f614de502adb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/add-disabled-option-to-add-ports-f8c6c9b3e6797652.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/multiattribute_node_lookup-17e219ba8d3e5eb0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/story-2002166-371315335fd8e62d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/Reapply_update_started_at-8af8cf254cdf8cde.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/fix-crash-when-use-postgresql-ac6c708f48f55c83.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/fix-llc-switch-id-not-mac-e2de3adc0945ee70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/fix-CalledProcessError-on-startup-28d9dbed85a81542.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/pxe-enabled-cbc3287ebe3fcd49.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/firewall-refactoring-17e8ad764f2cde8d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/fix_llc_port_assume-4ea47d26501bddc3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/pxe-filter-dnsmasq-manage-deleted-ironic-macs-4bb766efad8c6d02.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/UUID-started_at-finished_at-in-the-status-API-7860312102923938.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/deprecate-root-device-hint-909d389b7efed5da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/unset_property_instrospectionrules-78d64b8b7643e40d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/check-formatted-value-from-nonstring-3d851cb42ce3a0ac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/unmanaged-delay-d39871e1346d9448.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/deprecate-store-data-location-037eaab9cd326646.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/find-node-input-filtering-e8ea529252e80739.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/prelude-10.0.0-773ef7f14a5dfdf5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/dnsmask-pxe-filter-rootwrap-systemctl-099964ad39d38b4c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/fix-deadlock-during-cleanup-bcb6b517ef299791.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/log-info-not-found-cache-error-afbc87e80305ca5c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/deprecate-rollback-dea95ac515d3189b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/processing-data-type-check-7c914339d3ab15ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/sighup-support-e6eaec034d963108.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/preprocessing-error-01e55b4db20fb7fc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/fix-extra-hardware-process-c0635a972de37b0a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/fix-mysql-6b79049fe96edae4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/set-node-to-error-when-swift-failure-3e919ecbf9db6401.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/ipv6-bmc-address-start-inspection-7a72794f25eb9f19.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/enroll-hook-d8c32eba70848210.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/port-creation-plugin-c0405ec646b1051d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/introspection-delay-drivers-deprecation-1d0c25b112fbd4da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/deprecate-setting-ipmi-creds-1581ddc63b273811.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/short_circuit_port_update_for_manual_inspection-5dc296df9d409c69.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/keystoneauth-plugins-aab6cbe1d0e884bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/add-lldp-plugin-dependency-c323412654f71b3e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/remove_filter_logging-1a80419083c42bc6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/swift-deprecations-d7680b867fae7f3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/pxe-filter-dnsmasq-not-known-hosts-filter-76ae5bd7a8db6f75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/ipmi-credentials-removal-0021f89424fbf7a3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/drop-maintenance-a9a87a9a2af051ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/db-status-consistency-enhancements-f97fbaccfc81a60b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/port-list-retry-745d1cf41780e961.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/add-lldp-basic-plugin-98aebcf43e60931b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/loopback-bmc-e60d64fe74bdf142.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/sphinx-docs-4d0a5886261e57bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/keystone-noauth-9ba5ad9884c6273c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/remove-policy-json-b4746d64c1511023.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/cors-5f345c65da7f5c99.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/is-empty-missing-a590d580cb62761d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/remove-deprecated-ssl-opt-f6e6bd841f2c1061.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/pci_devices-plugin-5b93196e0e973155.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/extra-hardware-swift-aeebf299b9605bb0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/rules-invert-2585173a11db3c31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/migrate-introspection-data-bcd692c9ad3f22d7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/hook-deps-83a867c7af0300e4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/tempest_plugin_removal-91a01f5950f543e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/Inspector_rules_API_does_not_return_all_attributes-98a9765726c405d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/discovery-default-driver-94f990bb0676369b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/rpc-backends-0e7405aa1c7723a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/no-downgrade-migrations-514bf872d9f944ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/disable-dhcp-c86a3a0ee2696ee0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/ipa-support-7eea800306829a49.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/capabilities-15cc2268d661f0a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/no-old-ramdisk-095b05e1245131d8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/fix-rules-endpoint-response-d60984c40d927c1f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/add_node-with-version_id-24f51e5888480aa0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/local_gb-250bd415684a7855.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/googbye-patches-args-071532024b9260bd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/notes/optional-root-disk-9b972f504b2e6262.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/queens.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/ocata.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    63827 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9355 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/liberty.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/releasenotes/source/pike.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/rootwrap.d/ironic-inspector.filters
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/devstack/settings
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23294 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2437 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/devstack/example.local.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/devstack/upgrade/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1540 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/devstack/upgrade/resources.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3263 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/devstack/upgrade/upgrade.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/devstack/upgrade/settings
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      690 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/devstack/upgrade/shutdown.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:40.000000 ironic-inspector-9.2.3/playbooks/legacy/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/playbooks/legacy/ironic-inspector-grenade-dsvm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/playbooks/legacy/ironic-inspector-grenade-dsvm/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5464 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/playbooks/legacy/ironic-inspector-grenade-dsvm/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2396 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:41.000000 ironic-inspector-9.2.3/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1086 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3064 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/zuul.d/ironic-inspector-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/zuul.d/legacy-ironic-inspector-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2020-06-15 09:50:21.000000 ironic-inspector-9.2.3/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.155723 ironic-inspector-9.2.4/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4421 2021-02-01 18:37:08.000000 ironic-inspector-9.2.4/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13616 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47696 2021-02-01 18:37:08.000000 ironic-inspector-9.2.4/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2679 2021-02-01 18:37:09.155723 ironic-inspector-9.2.4/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.079727 ironic-inspector-9.2.4/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.087726 ironic-inspector-9.2.4/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7841 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1644 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/introspection-api-v1-continue.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/introspection-api-v1-introspection-management.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2709 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/introspection-api-v1-introspection.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2756 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/introspection-api-v1-rules.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2047 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/introspection-api-versions.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6634 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/parameters.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.087726 ironic-inspector-9.2.4/api-ref/source/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/samples/api-root-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/samples/api-v1-common-node-uuid.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/samples/api-v1-common-rule-uuid.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1517 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/samples/api-v1-continue-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      653 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/samples/api-v1-create-rule-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/samples/api-v1-create-rule-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2508 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/samples/api-v1-data-introspection-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/samples/api-v1-get-introspection-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/samples/api-v1-get-introspections-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/samples/api-v1-get-rule-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/samples/api-v1-get-rules-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/api-ref/source/samples/api-v1-root-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.091726 ironic-inspector-9.2.4/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2437 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/devstack/example.local.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23294 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.091726 ironic-inspector-9.2.4/devstack/upgrade/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1540 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/devstack/upgrade/resources.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/devstack/upgrade/settings
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      690 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/devstack/upgrade/shutdown.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3263 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/devstack/upgrade/upgrade.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.091726 ironic-inspector-9.2.4/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5752 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/Makefile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.091726 ironic-inspector-9.2.4/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/.gitignore
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.091726 ironic-inspector-9.2.4/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4944 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/admin/dnsmasq-pxe-filter.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1491 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/admin/upgrade.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3494 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.091726 ironic-inspector-9.2.4/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/configuration/ironic-inspector.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/configuration/policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/configuration/sample-config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/configuration/sample-policy.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.091726 ironic-inspector-9.2.4/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1775 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/contributor/jobs-description.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.091726 ironic-inspector-9.2.4/doc/source/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16969 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/images/states.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.095726 ironic-inspector-9.2.4/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17730 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.095726 ironic-inspector-9.2.4/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12393 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/user/http-api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6328 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/user/troubleshooting.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16165 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/user/usage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3557 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/doc/source/user/workflow.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic-inspector.8
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.099726 ironic-inspector-9.2.4/ironic_inspector/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/alembic.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2506 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/api_tools.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.099726 ironic-inspector-9.2.4/ironic_inspector/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/cmd/all.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/cmd/conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3058 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/cmd/dbsync.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4465 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/cmd/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1124 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/cmd/wsgi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.103726 ironic-inspector-9.2.4/ironic_inspector/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1867 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/common/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4770 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/common/coordination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/common/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10601 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/common/ironic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2797 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/common/keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14392 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/common/lldp_parsers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10500 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/common/lldp_tlvs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2729 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/common/locking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/common/rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2076 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/common/rpc_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/common/service_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5346 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/common/swift.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.103726 ironic-inspector-9.2.4/ironic_inspector/conductor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conductor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7618 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conductor/manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.107725 ironic-inspector-9.2.4/ironic_inspector/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1567 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conf/capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1129 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conf/coordination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4210 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conf/default.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conf/discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1991 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conf/dnsmasq_pxe_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conf/iptables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conf/ironic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3352 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conf/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1080 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conf/pci_devices.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5707 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conf/processing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conf/pxe_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conf/service_catalog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1505 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/conf/swift.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6647 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6849 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/introspect.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4632 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/introspection_state.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.079727 ironic-inspector-9.2.4/ironic_inspector/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.079727 ironic-inspector-9.2.4/ironic_inspector/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.107725 ironic-inspector-9.2.4/ironic_inspector/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25122 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/locale/en_GB/LC_MESSAGES/ironic_inspector.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14902 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/main.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.107725 ironic-inspector-9.2.4/ironic_inspector/migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2470 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/migrations/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/migrations/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.107725 ironic-inspector-9.2.4/ironic_inspector/migrations/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1358 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/migrations/versions/18440d0834af_introducing_the_aborting_state.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/migrations/versions/2970d2d44edc_add_manage_boot_to_nodes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1868 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/migrations/versions/578f84f38d_inital_db_schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3181 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/migrations/versions/882b2d84cb1b_attribute_constraints_relaxing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1339 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/migrations/versions/bf8dec16023c_add_introspection_data_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3016 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/migrations/versions/d00d6e3f38c4_change_created_finished_at_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/migrations/versions/d2e48801c8ef_introducing_node_state_attribute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/migrations/versions/d588418040d_add_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/migrations/versions/e169a4a81d88_add_invert_field_to_rule_condition.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38506 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/node_cache.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.111725 ironic-inspector-9.2.4/ironic_inspector/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8352 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/plugins/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2741 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/plugins/capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3095 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/plugins/discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1381 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/plugins/example.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4138 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/plugins/extra_hardware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4447 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/plugins/introspection_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3236 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/plugins/lldp_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6451 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/plugins/local_link_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2730 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/plugins/pci_devices.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4500 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/plugins/raid_device.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6132 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/plugins/rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14166 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/plugins/standard.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7120 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15896 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/process.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.111725 ironic-inspector-9.2.4/ironic_inspector/pxe_filter/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/pxe_filter/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7133 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/pxe_filter/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11643 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/pxe_filter/dnsmasq.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1991 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/pxe_filter/interface.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9334 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/pxe_filter/iptables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17119 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/rules.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.111725 ironic-inspector-9.2.4/ironic_inspector/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8333 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31763 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/functional.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.119725 ironic-inspector-9.2.4/ironic_inspector/test/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1369 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/policy_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4722 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_api_tools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12163 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_common_ironic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5108 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_coordination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3050 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20574 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_dnsmasq_pxe_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26643 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_introspect.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17843 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_iptables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3563 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_locking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32538 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22203 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20881 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_migrations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57571 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_node_cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3420 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2987 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6725 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5084 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_extra_hardware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3175 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_introspection_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13411 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_lldp_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9455 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_local_link_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4965 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_pci_devices.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4835 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_raid_device.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11806 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22247 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_standard.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33392 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_process.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11505 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_pxe_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21879 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5380 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_swift.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6346 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3292 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/test/unit/test_wsgi_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7889 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1723 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/ironic_inspector/wsgi_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.099726 ironic-inspector-9.2.4/ironic_inspector.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2679 2021-02-01 18:37:08.000000 ironic-inspector-9.2.4/ironic_inspector.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18208 2021-02-01 18:37:09.000000 ironic-inspector-9.2.4/ironic_inspector.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-02-01 18:37:08.000000 ironic-inspector-9.2.4/ironic_inspector.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3236 2021-02-01 18:37:08.000000 ironic-inspector-9.2.4/ironic_inspector.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-02-01 18:37:08.000000 ironic-inspector-9.2.4/ironic_inspector.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-02-01 18:37:08.000000 ironic-inspector-9.2.4/ironic_inspector.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2021-02-01 18:37:08.000000 ironic-inspector-9.2.4/ironic_inspector.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-02-01 18:37:08.000000 ironic-inspector-9.2.4/ironic_inspector.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2396 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.079727 ironic-inspector-9.2.4/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.079727 ironic-inspector-9.2.4/playbooks/legacy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.119725 ironic-inspector-9.2.4/playbooks/legacy/ironic-inspector-grenade-dsvm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/playbooks/legacy/ironic-inspector-grenade-dsvm/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5464 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/playbooks/legacy/ironic-inspector-grenade-dsvm/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.079727 ironic-inspector-9.2.4/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.151723 ironic-inspector-9.2.4/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/Inspector_rules_API_does_not_return_all_attributes-98a9765726c405d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/Reapply_update_started_at-8af8cf254cdf8cde.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/UUID-started_at-finished_at-in-the-status-API-7860312102923938.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/abort-introspection-ae5cb5a9fbacd2ac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/accept-link-local-address-1fbb9cbdc3f980bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/active-introspection-949f4a50c9d5218a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/active-node-not-in-cache-b2d7b77603f02a66.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/active_states_timeout-3e3ab110870483ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/add-disabled-option-to-add-ports-f8c6c9b3e6797652.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/add-lldp-basic-plugin-98aebcf43e60931b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/add-lldp-plugin-4645596cb8b39fd3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/add-lldp-plugin-dependency-c323412654f71b3e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/add-node-state-to-introspection-api-response-85fb7f4e72ae386a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/add-support-for-listing-all-introspection-statuses-2a3d4379c3854894.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/add-support-for-long-running-ramdisk-ffee3c177c56cebb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/add_node-with-version_id-24f51e5888480aa0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/allow-periodics-shutdown-inspector-ac28ea5ba3224279.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/bmc-logging-deprecation-4ca046a64fac6f11.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/capabilities-15cc2268d661f0a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/change_started_finished_at_type_to_datetime-c5617e598350970c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/check-formatted-value-from-nonstring-3d851cb42ce3a0ac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/compact-debug-logging-b15dd9bbdd3ce27a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/contains-matches-ee28958b08995494.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/continue-http-500-62f33d425aade9d7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/cors-5f345c65da7f5c99.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/cpu-memory-cfdc72b625780871.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/custom-ramdisk-log-name-dac06822c38657e7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/db-status-consistency-enhancements-f97fbaccfc81a60b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/deprecate-rollback-dea95ac515d3189b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/deprecate-root-device-hint-909d389b7efed5da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/deprecate-setting-ipmi-creds-1581ddc63b273811.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/deprecate-ssl-opts-40ce8f4618c786ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/deprecate-store-data-location-037eaab9cd326646.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/deprecated-ironic-1751ceec6295917d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/deprecated-options-removal-ocata-a44dadf3bcf8d6fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/disable-dhcp-c86a3a0ee2696ee0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/discovery-default-driver-94f990bb0676369b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/dnsmask-pxe-filter-rootwrap-systemctl-099964ad39d38b4c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/dnsmasq-pxe-filter-37928d3fdb1e8ec3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/drop-maintenance-a9a87a9a2af051ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/edeploy-typeerror-6486e31923d91666.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/empty-condition-abc707b771be6be3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/empty-ipmi-address-2-4d57c34aec7d14e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/empty-ipmi-address-5b5ca186a066ed32.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/enroll-hook-d8c32eba70848210.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/enroll-nodes-with-bmc-v6address-ba224f4a8a151c53.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/extend-rules-9a9d38701e970611.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/extra-hardware-swift-aeebf299b9605bb0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/find-node-input-filtering-e8ea529252e80739.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/firewall-refactoring-17e8ad764f2cde8d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/firewall-rerun-f2d0f64cca2698ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/fix-CalledProcessError-on-startup-28d9dbed85a81542.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/fix-crash-when-use-postgresql-ac6c708f48f55c83.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/fix-deadlock-during-cleanup-bcb6b517ef299791.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/fix-extra-hardware-process-c0635a972de37b0a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/fix-llc-switch-id-not-mac-e2de3adc0945ee70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/fix-mysql-6b79049fe96edae4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/fix-periodic-tasks-configuration-edd167f0146e60b5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/fix-pxe-filter-get-blacklist-2dde59d51c1d010f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/fix-rules-endpoint-response-d60984c40d927c1f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/fix-wrong-provision-state-name-150c91c48d471bf9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/fix_llc_hook_bugs-efeea008c2f792eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/fix_llc_port_assume-4ea47d26501bddc3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/fix_node_uuid_for_manual_inspection-2fa3f11343cab417.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/flask-debug-6d2dcc2b482324dc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/futurist-557fcd18d4eaf1c1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/googbye-patches-args-071532024b9260bd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/handle-patch-port-failure-9a8b85749104506f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/hook-deps-83a867c7af0300e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/infiniband-support-960d6846e326dec4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/introspection-data-db-store-0586292de05cbfd7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/introspection-delay-drivers-deprecation-1d0c25b112fbd4da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/introspection-state-03538fac198882b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/ipa-inventory-0a1e8d644da850ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/ipa-support-7eea800306829a49.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/ipmi-credentials-removal-0021f89424fbf7a3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/ipv6-bmc-address-start-inspection-7a72794f25eb9f19.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/ironic-lib-hints-20412a1c7fa796e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/is-empty-missing-a590d580cb62761d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/keystone-noauth-9ba5ad9884c6273c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/keystoneauth-plugins-aab6cbe1d0e884bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/ksadapters-abc9edc63cafa405.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/less-iptables-calls-759e89d103df504c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/local_gb-250bd415684a7855.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/log-info-not-found-cache-error-afbc87e80305ca5c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/logs-collector-logging-356e56cd70a04a2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/lookup-all-macs-eead528c0b764ad7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/loopback-bmc-e60d64fe74bdf142.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/manage-boot-2ae986f87098576b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/manage-boot-power-off-d8ed644f11659c38.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/mdns-a5f4034257139e31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/migrate-introspection-data-bcd692c9ad3f22d7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/migrations-1.3.20-0d337d000bd0a7e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/migrations-autogenerate-4303fd496c3c2757.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/missing-pxe-mac-d9329dab85513460.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      584 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/multiattribute_node_lookup-17e219ba8d3e5eb0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/names-82d9f84153a228ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/nested-value-formatting-e04f187475e5e475.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/no-downgrade-migrations-514bf872d9f944ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/no-fail-on-power-off-enroll-node-e40854f6def397b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/no-logs-stored-data-6db52934c7f9a91a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/no-old-ramdisk-095b05e1245131d8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/no-rollback-e15bc7fee0134545.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/no-root_device_hint-0e7676d481d503bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/node-locking-4d135ca5b93524b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/optional-root-disk-9b972f504b2e6262.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/patch-head-backslash-24bcdd03ba254bf2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/pci_devices-plugin-5b93196e0e973155.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/periodics-18bf7fb57777c043.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/persistent-boot-207b32257a97451e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/pgsql-imperative-enum-dda76f150a205d0a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1778 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/policy-engine-c44828e3131e6c62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/port-creation-plugin-c0405ec646b1051d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/port-list-retry-745d1cf41780e961.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/post-introspection-data-9cdd39a3de446e92.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/prelude-10.0.0-773ef7f14a5dfdf5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/preprocessing-error-01e55b4db20fb7fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/processing-data-type-check-7c914339d3ab15ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/processing-logging-e2d27bbac95a7213.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/pxe-enabled-cbc3287ebe3fcd49.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/pxe-filter-dnsmasq-manage-deleted-ironic-macs-4bb766efad8c6d02.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/pxe-filter-dnsmasq-not-known-hosts-filter-76ae5bd7a8db6f75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/ramdisk-logs-on-all-failures-24da41edf3a98400.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/reapply-introspection-5edbbfaf498dbd12.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/remove-deprecated-conf-opts-361ab0bb342f0e7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/remove-deprecated-ssl-opt-f6e6bd841f2c1061.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/remove-opt-group-firewall-96266983e476c29e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/remove-opt-keep-node-status-7d6b96f1a6e498a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/remove-policy-json-b4746d64c1511023.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/remove-store-data-location-e68462ff6ba257e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/remove_filter_logging-1a80419083c42bc6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/reset-interfaces-ff78d50b9f05d47d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/rollback-formatting-7d61c9af2600d42f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/rollback-removal-a03a989e2e9f776b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/rpc-backends-0e7405aa1c7723a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/rules-invert-2585173a11db3c31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/set-node-to-error-when-swift-failure-3e919ecbf9db6401.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/short_circuit_port_update_for_manual_inspection-5dc296df9d409c69.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/sighup-support-e6eaec034d963108.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/size-hint-ea2a264468e1fcb7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/sphinx-docs-4d0a5886261e57bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/split-services-99873ff27ef2d89b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      439 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/status-removal-fa1d9a98ffad9f60.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/stein-prelude-42f0d90bf2c6a1a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/stop-when-setbootdev-failed-68d84fec0843bdc8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/story-2002166-371315335fd8e62d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/support-ip6tables-ce30f614de502adb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/support-microversion-latest-dcf9598c5218e979.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/swift-deprecations-d7680b867fae7f3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/swift-max-retries-dfaecb74bd3aba9a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/tempest_plugin_removal-91a01f5950f543e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/trailing-slashes-93c2466b71829ec1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/trait-actions-eec05cbb6a944619.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/unmanaged-delay-d39871e1346d9448.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/unmanaged-result-4de3788e7820e3c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/unset_property_instrospectionrules-78d64b8b7643e40d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/update-default-ironic-api-stein-b3b01ec542fa8f15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/validate-ipv6-address-fda29c929754352e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/notes/zero-size-55c4b4f2b9e8384d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.151723 ironic-inspector-9.2.4/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.151723 ironic-inspector-9.2.4/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.151723 ironic-inspector-9.2.4/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9355 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/liberty.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.083726 ironic-inspector-9.2.4/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.083726 ironic-inspector-9.2.4/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.151723 ironic-inspector-9.2.4/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    63827 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.083726 ironic-inspector-9.2.4/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.151723 ironic-inspector-9.2.4/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      969 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/rootwrap.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.151723 ironic-inspector-9.2.4/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/rootwrap.d/ironic-inspector.filters
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4754 2021-02-01 18:37:09.155723 ironic-inspector-9.2.4/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.155723 ironic-inspector-9.2.4/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8360 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/tools/bandit.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/tools/config-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/tools/policy-generator.conf
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3208 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/tools/states_to_dot.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1990 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/tools/test-setup.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3269 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 18:37:09.155723 ironic-inspector-9.2.4/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3064 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/zuul.d/ironic-inspector-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/zuul.d/legacy-ironic-inspector-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1055 2021-02-01 18:36:34.000000 ironic-inspector-9.2.4/zuul.d/project.yaml
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ironic-inspector-9.2.3/ironic_inspector.egg-info/requires.txt` & `ironic-inspector-9.2.4/ironic_inspector.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-automaton>=1.9.0
-alembic>=0.8.10
 Babel!=2.4.0,>=2.3.4
+Flask!=0.11,>=0.10
+SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8,>=1.0.10
+alembic>=0.8.10
+automaton>=1.9.0
 construct<2.9,>=2.8.10
 eventlet!=0.18.3,!=0.20.1,>=0.18.2
-Flask!=0.11,>=0.10
 futurist>=1.2.0
 ironic-lib>=2.17.0
 jsonpath-rw<2.0,>=1.2.0
 jsonschema>=2.6.0
 keystoneauth1>=3.4.0
 keystonemiddleware>=4.18.0
 netaddr>=0.7.18
-pbr!=2.1.0,>=2.0.0
-python-ironicclient!=2.5.2,!=2.7.1,!=3.0.0,>=2.3.0
-pytz>=2013.6
 openstacksdk>=0.30.0
 oslo.concurrency>=3.26.0
 oslo.config>=5.2.0
 oslo.context>=2.19.2
 oslo.db>=4.27.0
 oslo.i18n>=3.15.3
 oslo.log>=3.36.0
 oslo.messaging>=5.32.0
 oslo.middleware>=3.31.0
 oslo.policy>=1.30.0
 oslo.rootwrap>=5.8.0
 oslo.serialization!=2.19.1,>=2.18.0
 oslo.service!=1.28.1,>=1.24.0
 oslo.utils>=3.33.0
+pbr!=2.1.0,>=2.0.0
+python-ironicclient!=2.5.2,!=2.7.1,!=3.0.0,>=2.3.0
+pytz>=2013.6
 retrying!=1.3.0,>=1.2.3
 six>=1.10.0
 stevedore>=1.20.0
-SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8,>=1.0.10
 tooz>=1.64.0
```

### Comparing `ironic-inspector-9.2.3/ironic_inspector.egg-info/PKG-INFO` & `ironic-inspector-9.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ironic-inspector
-Version: 9.2.3
+Version: 9.2.4
 Summary: Hardware introspection for OpenStack Bare Metal
 Home-page: https://docs.openstack.org/ironic-inspector/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: ===============================================
         Hardware introspection for OpenStack Bare Metal
```

### Comparing `ironic-inspector-9.2.3/ironic_inspector.egg-info/SOURCES.txt` & `ironic-inspector-9.2.4/ironic_inspector.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
 playbooks/legacy/ironic-inspector-grenade-dsvm/post.yaml
 playbooks/legacy/ironic-inspector-grenade-dsvm/run.yaml
 releasenotes/notes/.placeholder
 releasenotes/notes/Inspector_rules_API_does_not_return_all_attributes-98a9765726c405d5.yaml
 releasenotes/notes/Reapply_update_started_at-8af8cf254cdf8cde.yaml
 releasenotes/notes/UUID-started_at-finished_at-in-the-status-API-7860312102923938.yaml
 releasenotes/notes/abort-introspection-ae5cb5a9fbacd2ac.yaml
+releasenotes/notes/accept-link-local-address-1fbb9cbdc3f980bb.yaml
 releasenotes/notes/active-introspection-949f4a50c9d5218a.yaml
 releasenotes/notes/active-node-not-in-cache-b2d7b77603f02a66.yaml
 releasenotes/notes/active_states_timeout-3e3ab110870483ec.yaml
 releasenotes/notes/add-disabled-option-to-add-ports-f8c6c9b3e6797652.yaml
 releasenotes/notes/add-lldp-basic-plugin-98aebcf43e60931b.yaml
 releasenotes/notes/add-lldp-plugin-4645596cb8b39fd3.yaml
 releasenotes/notes/add-lldp-plugin-dependency-c323412654f71b3e.yaml
@@ -274,14 +275,15 @@
 releasenotes/notes/logs-collector-logging-356e56cd70a04a2b.yaml
 releasenotes/notes/lookup-all-macs-eead528c0b764ad7.yaml
 releasenotes/notes/loopback-bmc-e60d64fe74bdf142.yaml
 releasenotes/notes/manage-boot-2ae986f87098576b.yaml
 releasenotes/notes/manage-boot-power-off-d8ed644f11659c38.yaml
 releasenotes/notes/mdns-a5f4034257139e31.yaml
 releasenotes/notes/migrate-introspection-data-bcd692c9ad3f22d7.yaml
+releasenotes/notes/migrations-1.3.20-0d337d000bd0a7e0.yaml
 releasenotes/notes/migrations-autogenerate-4303fd496c3c2757.yaml
 releasenotes/notes/missing-pxe-mac-d9329dab85513460.yaml
 releasenotes/notes/multiattribute_node_lookup-17e219ba8d3e5eb0.yaml
 releasenotes/notes/names-82d9f84153a228ec.yaml
 releasenotes/notes/nested-value-formatting-e04f187475e5e475.yaml
 releasenotes/notes/no-downgrade-migrations-514bf872d9f944ed.yaml
 releasenotes/notes/no-fail-on-power-off-enroll-node-e40854f6def397b8.yaml
@@ -339,14 +341,15 @@
 releasenotes/notes/trailing-slashes-93c2466b71829ec1.yaml
 releasenotes/notes/trait-actions-eec05cbb6a944619.yaml
 releasenotes/notes/unmanaged-delay-d39871e1346d9448.yaml
 releasenotes/notes/unmanaged-result-4de3788e7820e3c5.yaml
 releasenotes/notes/unset_property_instrospectionrules-78d64b8b7643e40d.yaml
 releasenotes/notes/update-default-ironic-api-stein-b3b01ec542fa8f15.yaml
 releasenotes/notes/validate-ipv6-address-fda29c929754352e.yaml
+releasenotes/notes/zero-size-55c4b4f2b9e8384d.yaml
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/liberty.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
```

### Comparing `ironic-inspector-9.2.3/ironic_inspector.egg-info/entry_points.txt` & `ironic-inspector-9.2.4/ironic_inspector.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/tox.ini` & `ironic-inspector-9.2.4/tox.ini`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ChangeLog` & `ironic-inspector-9.2.4/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+9.2.4
+-----
+
+* Fix database migrations and disable the non-standalone job
+* Do not try to set local\_gb to -1 when the matched root device size is 0
+* Accept IPv6 link local address during interface validation
+
 9.2.3
 -----
 
 * Treat endpoints with trailing slashes the same way as without them
 * Stop running a periodic task for the noop PXE filter
 
 9.2.2
```

### Comparing `ironic-inspector-9.2.3/LICENSE` & `ironic-inspector-9.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/introspection-api-v1-introspection-management.inc` & `ironic-inspector-9.2.4/api-ref/source/introspection-api-v1-introspection-management.inc`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/introspection-api-versions.inc` & `ironic-inspector-9.2.4/api-ref/source/introspection-api-versions.inc`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/introspection-api-v1-introspection.inc` & `ironic-inspector-9.2.4/api-ref/source/introspection-api-v1-introspection.inc`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/parameters.yaml` & `ironic-inspector-9.2.4/api-ref/source/parameters.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/conf.py` & `ironic-inspector-9.2.4/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/samples/api-v1-get-introspections-response.json` & `ironic-inspector-9.2.4/api-ref/source/samples/api-v1-get-introspections-response.json`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/samples/api-v1-create-rule-response.json` & `ironic-inspector-9.2.4/api-ref/source/samples/api-v1-create-rule-response.json`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/samples/api-v1-get-rules-response.json` & `ironic-inspector-9.2.4/api-ref/source/samples/api-v1-get-rules-response.json`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/samples/api-v1-continue-request.json` & `ironic-inspector-9.2.4/api-ref/source/samples/api-v1-continue-request.json`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/samples/api-v1-create-rule-request.json` & `ironic-inspector-9.2.4/api-ref/source/samples/api-v1-create-rule-request.json`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/samples/api-v1-get-rule-response.json` & `ironic-inspector-9.2.4/api-ref/source/samples/api-v1-get-rule-response.json`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/samples/api-v1-root-response.json` & `ironic-inspector-9.2.4/api-ref/source/samples/api-v1-root-response.json`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/samples/api-v1-data-introspection-response.json` & `ironic-inspector-9.2.4/api-ref/source/samples/api-v1-data-introspection-response.json`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/introspection-api-v1-continue.inc` & `ironic-inspector-9.2.4/api-ref/source/introspection-api-v1-continue.inc`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/api-ref/source/introspection-api-v1-rules.inc` & `ironic-inspector-9.2.4/api-ref/source/introspection-api-v1-rules.inc`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/setup.py` & `ironic-inspector-9.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/rootwrap.conf` & `ironic-inspector-9.2.4/rootwrap.conf`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/PKG-INFO` & `ironic-inspector-9.2.4/ironic_inspector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ironic-inspector
-Version: 9.2.3
+Version: 9.2.4
 Summary: Hardware introspection for OpenStack Bare Metal
 Home-page: https://docs.openstack.org/ironic-inspector/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: ===============================================
         Hardware introspection for OpenStack Bare Metal
```

### Comparing `ironic-inspector-9.2.3/ironic-inspector.8` & `ironic-inspector-9.2.4/ironic-inspector.8`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/migrations/script.py.mako` & `ironic-inspector-9.2.4/ironic_inspector/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/migrations/env.py` & `ironic-inspector-9.2.4/ironic_inspector/migrations/env.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/migrations/versions/e169a4a81d88_add_invert_field_to_rule_condition.py` & `ironic-inspector-9.2.4/ironic_inspector/migrations/versions/e169a4a81d88_add_invert_field_to_rule_condition.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/migrations/versions/2970d2d44edc_add_manage_boot_to_nodes.py` & `ironic-inspector-9.2.4/ironic_inspector/migrations/versions/2970d2d44edc_add_manage_boot_to_nodes.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/migrations/versions/578f84f38d_inital_db_schema.py` & `ironic-inspector-9.2.4/ironic_inspector/migrations/versions/578f84f38d_inital_db_schema.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/migrations/versions/bf8dec16023c_add_introspection_data_table.py` & `ironic-inspector-9.2.4/ironic_inspector/migrations/versions/bf8dec16023c_add_introspection_data_table.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/migrations/versions/882b2d84cb1b_attribute_constraints_relaxing.py` & `ironic-inspector-9.2.4/ironic_inspector/migrations/versions/882b2d84cb1b_attribute_constraints_relaxing.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,16 @@
                  if meta['name'] == NAME}.pop()
     value_type = {meta.get('type') for meta in columns_meta
                   if meta['name'] == VALUE}.pop()
 
     node_uuid_column = sa.Column(NODE_UUID, sa.String(36))
     op.add_column(ATTRIBUTES, node_uuid_column)
 
-    attributes = sa.table(ATTRIBUTES, node_uuid_column,
+    attributes = sa.table(ATTRIBUTES,
+                          sa.Column(NODE_UUID, sa.String(36)),
                           sa.Column(UUID, sa.String(36)))
 
     with op.batch_alter_table(ATTRIBUTES,
                               naming_convention=naming_convention) as batch_op:
         batch_op.drop_constraint(fk_constraint, type_='foreignkey')
 
     rows = connection.execute(sa.select([attributes.c.uuid,
```

### Comparing `ironic-inspector-9.2.3/ironic_inspector/migrations/versions/d2e48801c8ef_introducing_node_state_attribute.py` & `ironic-inspector-9.2.4/ironic_inspector/migrations/versions/d2e48801c8ef_introducing_node_state_attribute.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/migrations/versions/d588418040d_add_rules.py` & `ironic-inspector-9.2.4/ironic_inspector/migrations/versions/d588418040d_add_rules.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/migrations/versions/18440d0834af_introducing_the_aborting_state.py` & `ironic-inspector-9.2.4/ironic_inspector/migrations/versions/18440d0834af_introducing_the_aborting_state.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/migrations/versions/d00d6e3f38c4_change_created_finished_at_type.py` & `ironic-inspector-9.2.4/ironic_inspector/migrations/versions/d00d6e3f38c4_change_created_finished_at_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,25 +28,30 @@
 revision = 'd00d6e3f38c4'
 down_revision = 'd2e48801c8ef'
 branch_labels = None
 depends_on = None
 
 
 def upgrade():
-    started_at = sa.Column('started_at', sa.types.Float, nullable=True)
-    finished_at = sa.Column('finished_at', sa.types.Float, nullable=True)
     temp_started_at = sa.Column("temp_started_at", sa.types.DateTime,
                                 nullable=True)
     temp_finished_at = sa.Column("temp_finished_at", sa.types.DateTime,
                                  nullable=True)
-    uuid = sa.Column("uuid", sa.String(36), primary_key=True)
 
     op.add_column("nodes", temp_started_at)
     op.add_column("nodes", temp_finished_at)
 
+    uuid = sa.Column("uuid", sa.String(36), primary_key=True)
+    started_at = sa.Column('started_at', sa.types.Float, nullable=True)
+    finished_at = sa.Column('finished_at', sa.types.Float, nullable=True)
+    # NOTE(dtantsur): do not reuse the column objects from add_column
+    temp_started_at = sa.Column("temp_started_at", sa.types.DateTime,
+                                nullable=True)
+    temp_finished_at = sa.Column("temp_finished_at", sa.types.DateTime,
+                                 nullable=True)
     t = sa.table('nodes', started_at, finished_at,
                  temp_started_at, temp_finished_at, uuid)
 
     conn = op.get_bind()
     rows = conn.execute(sa.select([t.c.started_at, t.c.finished_at, t.c.uuid]))
     for row in rows:
         temp_started = datetime.datetime.utcfromtimestamp(row['started_at'])
```

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conf/dnsmasq_pxe_filter.py` & `ironic-inspector-9.2.4/ironic_inspector/conf/dnsmasq_pxe_filter.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conf/swift.py` & `ironic-inspector-9.2.4/ironic_inspector/conf/swift.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conf/default.py` & `ironic-inspector-9.2.4/ironic_inspector/conf/default.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conf/coordination.py` & `ironic-inspector-9.2.4/ironic_inspector/conf/coordination.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conf/pxe_filter.py` & `ironic-inspector-9.2.4/ironic_inspector/conf/pxe_filter.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conf/pci_devices.py` & `ironic-inspector-9.2.4/ironic_inspector/conf/pci_devices.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conf/discovery.py` & `ironic-inspector-9.2.4/ironic_inspector/conf/discovery.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conf/service_catalog.py` & `ironic-inspector-9.2.4/ironic_inspector/conf/service_catalog.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conf/iptables.py` & `ironic-inspector-9.2.4/ironic_inspector/conf/iptables.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conf/ironic.py` & `ironic-inspector-9.2.4/ironic_inspector/conf/ironic.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conf/processing.py` & `ironic-inspector-9.2.4/ironic_inspector/conf/processing.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conf/__init__.py` & `ironic-inspector-9.2.4/ironic_inspector/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conf/opts.py` & `ironic-inspector-9.2.4/ironic_inspector/conf/opts.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conf/capabilities.py` & `ironic-inspector-9.2.4/ironic_inspector/conf/capabilities.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/introspect.py` & `ironic-inspector-9.2.4/ironic_inspector/introspect.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/rules.py` & `ironic-inspector-9.2.4/ironic_inspector/rules.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/wsgi_service.py` & `ironic-inspector-9.2.4/ironic_inspector/wsgi_service.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/cmd/conductor.py` & `ironic-inspector-9.2.4/ironic_inspector/cmd/conductor.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/cmd/wsgi.py` & `ironic-inspector-9.2.4/ironic_inspector/cmd/wsgi.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/cmd/migration.py` & `ironic-inspector-9.2.4/ironic_inspector/cmd/migration.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/cmd/all.py` & `ironic-inspector-9.2.4/ironic_inspector/cmd/all.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/cmd/dbsync.py` & `ironic-inspector-9.2.4/ironic_inspector/cmd/dbsync.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/alembic.ini` & `ironic-inspector-9.2.4/ironic_inspector/alembic.ini`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/utils.py` & `ironic-inspector-9.2.4/ironic_inspector/utils.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/conductor/manager.py` & `ironic-inspector-9.2.4/ironic_inspector/conductor/manager.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/common/locking.py` & `ironic-inspector-9.2.4/ironic_inspector/common/locking.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/common/swift.py` & `ironic-inspector-9.2.4/ironic_inspector/common/swift.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/common/lldp_parsers.py` & `ironic-inspector-9.2.4/ironic_inspector/common/lldp_parsers.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/common/coordination.py` & `ironic-inspector-9.2.4/ironic_inspector/common/coordination.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/common/context.py` & `ironic-inspector-9.2.4/ironic_inspector/common/context.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/common/service_utils.py` & `ironic-inspector-9.2.4/ironic_inspector/common/service_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/common/rpc_service.py` & `ironic-inspector-9.2.4/ironic_inspector/common/rpc_service.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/common/ironic.py` & `ironic-inspector-9.2.4/ironic_inspector/common/ironic.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/common/i18n.py` & `ironic-inspector-9.2.4/ironic_inspector/common/i18n.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/common/rpc.py` & `ironic-inspector-9.2.4/ironic_inspector/common/rpc.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/common/keystone.py` & `ironic-inspector-9.2.4/ironic_inspector/common/keystone.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/common/lldp_tlvs.py` & `ironic-inspector-9.2.4/ironic_inspector/common/lldp_tlvs.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/process.py` & `ironic-inspector-9.2.4/ironic_inspector/process.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/plugins/rules.py` & `ironic-inspector-9.2.4/ironic_inspector/plugins/rules.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/plugins/pci_devices.py` & `ironic-inspector-9.2.4/ironic_inspector/plugins/pci_devices.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/plugins/standard.py` & `ironic-inspector-9.2.4/ironic_inspector/plugins/standard.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,19 +73,25 @@
                                         node_info=node_info)
         self._process_root_device_hints(introspection_data, node_info,
                                         inventory)
 
         root_disk = introspection_data.get('root_disk')
         if root_disk:
             local_gb = root_disk['size'] // units.Gi
-            if CONF.processing.disk_partitioning_spacing:
-                local_gb -= 1
-            LOG.info('Root disk %(disk)s, local_gb %(local_gb)s GiB',
-                     {'disk': root_disk, 'local_gb': local_gb},
-                     node_info=node_info, data=introspection_data)
+            if not local_gb:
+                LOG.warning('The requested root disk is too small (smaller '
+                            'than 1 GiB) or its size cannot be detected: %s',
+                            root_disk,
+                            node_info=node_info, data=introspection_data)
+            else:
+                if CONF.processing.disk_partitioning_spacing:
+                    local_gb -= 1
+                LOG.info('Root disk %(disk)s, local_gb %(local_gb)s GiB',
+                         {'disk': root_disk, 'local_gb': local_gb},
+                         node_info=node_info, data=introspection_data)
         else:
             local_gb = 0
             LOG.info('No root device found, assuming a diskless node',
                      node_info=node_info, data=introspection_data)
 
         introspection_data['local_gb'] = local_gb
         if (CONF.processing.overwrite_existing or not
@@ -217,16 +223,15 @@
                 LOG.debug('Skipping local interface %s', name, data=data)
                 continue
 
             if CONF.processing.add_ports == 'pxe' and pxe_mac and not pxe:
                 LOG.debug('Skipping interface %s as it was not PXE booting',
                           name, data=data)
                 continue
-            elif CONF.processing.add_ports != 'all' and (
-                        not ip or netaddr.IPAddress(ip).is_link_local()):
+            elif CONF.processing.add_ports != 'all' and not ip:
                 LOG.debug('Skipping interface %s as it did not have '
                           'an IP address assigned during the ramdisk run',
                           name, data=data)
                 continue
 
             result[name] = iface
```

### Comparing `ironic-inspector-9.2.3/ironic_inspector/plugins/discovery.py` & `ironic-inspector-9.2.4/ironic_inspector/plugins/discovery.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/plugins/raid_device.py` & `ironic-inspector-9.2.4/ironic_inspector/plugins/raid_device.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/plugins/introspection_data.py` & `ironic-inspector-9.2.4/ironic_inspector/plugins/introspection_data.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/plugins/lldp_basic.py` & `ironic-inspector-9.2.4/ironic_inspector/plugins/lldp_basic.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/plugins/extra_hardware.py` & `ironic-inspector-9.2.4/ironic_inspector/plugins/extra_hardware.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/plugins/local_link_connection.py` & `ironic-inspector-9.2.4/ironic_inspector/plugins/local_link_connection.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/plugins/example.py` & `ironic-inspector-9.2.4/ironic_inspector/plugins/example.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/plugins/base.py` & `ironic-inspector-9.2.4/ironic_inspector/plugins/base.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/plugins/capabilities.py` & `ironic-inspector-9.2.4/ironic_inspector/plugins/capabilities.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/api_tools.py` & `ironic-inspector-9.2.4/ironic_inspector/api_tools.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/pxe_filter/interface.py` & `ironic-inspector-9.2.4/ironic_inspector/pxe_filter/interface.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/pxe_filter/iptables.py` & `ironic-inspector-9.2.4/ironic_inspector/pxe_filter/iptables.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/pxe_filter/base.py` & `ironic-inspector-9.2.4/ironic_inspector/pxe_filter/base.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/pxe_filter/dnsmasq.py` & `ironic-inspector-9.2.4/ironic_inspector/pxe_filter/dnsmasq.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/functional.py` & `ironic-inspector-9.2.4/ironic_inspector/test/functional.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/base.py` & `ironic-inspector-9.2.4/ironic_inspector/test/base.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_common_ironic.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_common_ironic.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_locking.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_locking.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/policy_fixture.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/policy_fixture.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_keystone.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_keystone.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_api_tools.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_api_tools.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_coordination.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_coordination.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_manager.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_manager.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_lldp_basic.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_lldp_basic.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_discovery.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_discovery.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_main.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_main.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_rules.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_rules.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_extra_hardware.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_extra_hardware.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_capabilities.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_capabilities.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_db.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_db.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_introspection_data.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_introspection_data.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_introspect.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_introspect.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_dnsmasq_pxe_filter.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_dnsmasq_pxe_filter.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_swift.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_swift.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_base.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_base.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_local_link_connection.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_local_link_connection.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_utils.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_standard.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_standard.py`

 * *Files 5% similar despite different names*

```diff
@@ -218,33 +218,14 @@
             # malformed MAC provided
             {'name': 'em4', 'mac_address': 'foobar',
              'ipv4_address': '2.2.2.2'},
         ]
         self.assertRaisesRegex(utils.Error, 'No suitable interfaces found',
                                self.hook.before_processing, self.data)
 
-    def test_skipped_interfaces_with_local_address(self):
-        CONF.set_override('add_ports', 'active', 'processing')
-        self.inventory['interfaces'] = [
-            # local interface (by IPv4 address)
-            {'name': 'em1', 'mac_address': '22:22:22:22:22:22',
-             'ipv4_address': '127.0.0.1'},
-            # local interface (by IPv6 address)
-            {'name': 'em2', 'mac_address': '33:33:33:33:33:33',
-             'ipv6_address': '::1'},
-            # interface only with local-link address
-            {'name': 'em3', 'mac_address': '44:44:44:44:44:44',
-             'ipv6_address': 'fe80::4644:44ff:fe44:4444'},
-            # interface only with local-link address with suffix
-            {'name': 'em4', 'mac_address': '55:55:55:55:55:55',
-             'ipv6_address': 'fe80::5755:55ff:fe55:5555%em4'},
-        ]
-        self.assertRaisesRegex(utils.Error, 'No suitable interfaces found',
-                               self.hook.before_processing, self.data)
-
     def test_interfaces_with_ipv6_addresses_only(self):
         CONF.set_override('add_ports', 'all', 'processing')
         self.inventory['interfaces'] = [
             # loopback interface (by IPv6 address)
             {'name': 'em2', 'mac_address': '33:33:33:33:33:33',
              'ipv6_address': '::1'},
             # interface with local-link address
@@ -378,14 +359,15 @@
         self.hook = std_plugins.RootDiskSelectionHook()
         self.inventory['disks'] = [
             {'model': 'Model 1', 'size': 20 * units.Gi, 'name': '/dev/sdb'},
             {'model': 'Model 2', 'size': 5 * units.Gi, 'name': '/dev/sda'},
             {'model': 'Model 3', 'size': 10 * units.Gi, 'name': '/dev/sdc'},
             {'model': 'Model 4', 'size': 4 * units.Gi, 'name': '/dev/sdd'},
             {'model': 'Too Small', 'size': 1 * units.Gi, 'name': '/dev/sde'},
+            {'model': 'Floppy', 'size': 0, 'name': '/dev/sdf'},
         ]
         self.matched = self.inventory['disks'][2].copy()
         self.node_info = mock.Mock(spec=node_cache.NodeInfo,
                                    _state='foo',
                                    uuid=self.uuid,
                                    **{'node.return_value': self.node})
 
@@ -449,14 +431,23 @@
 
         self.hook.before_update(self.data, self.node_info)
 
         self.assertEqual(self.matched, self.data['root_disk'])
         self.assertEqual(10, self.data['local_gb'])
         self.node_info.update_properties.assert_called_once_with(local_gb='10')
 
+    def test_zero_size(self):
+        self.node.properties['root_device'] = {'name': '/dev/sdf'}
+
+        self.hook.before_update(self.data, self.node_info)
+
+        self.assertEqual(self.inventory['disks'][5], self.data['root_disk'])
+        self.assertEqual(0, self.data['local_gb'])
+        self.node_info.update_properties.assert_called_once_with(local_gb='0')
+
     def test_all_match(self):
         self.node.properties['root_device'] = {'size': 10,
                                                'model': 'Model 3'}
 
         self.hook.before_update(self.data, self.node_info)
 
         self.assertEqual(self.matched, self.data['root_disk'])
```

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_raid_device.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_raid_device.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_wsgi_service.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_wsgi_service.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_node_cache.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_node_cache.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_pci_devices.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_pci_devices.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_pxe_filter.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_pxe_filter.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_process.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_process.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_migrations.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_migrations.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_iptables.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_iptables.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/test/unit/test_plugins_rules.py` & `ironic-inspector-9.2.4/ironic_inspector/test/unit/test_plugins_rules.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/locale/en_GB/LC_MESSAGES/ironic_inspector.po` & `ironic-inspector-9.2.4/ironic_inspector/locale/en_GB/LC_MESSAGES/ironic_inspector.po`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/node_cache.py` & `ironic-inspector-9.2.4/ironic_inspector/node_cache.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/policy.py` & `ironic-inspector-9.2.4/ironic_inspector/policy.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/introspection_state.py` & `ironic-inspector-9.2.4/ironic_inspector/introspection_state.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/version.py` & `ironic-inspector-9.2.4/ironic_inspector/version.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/db.py` & `ironic-inspector-9.2.4/ironic_inspector/db.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/ironic_inspector/main.py` & `ironic-inspector-9.2.4/ironic_inspector/main.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/test-requirements.txt` & `ironic-inspector-9.2.4/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/CONTRIBUTING.rst` & `ironic-inspector-9.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/doc/Makefile` & `ironic-inspector-9.2.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/doc/source/contributor/jobs-description.rst` & `ironic-inspector-9.2.4/doc/source/contributor/jobs-description.rst`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/doc/source/install/index.rst` & `ironic-inspector-9.2.4/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/doc/source/user/http-api.rst` & `ironic-inspector-9.2.4/doc/source/user/http-api.rst`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/doc/source/user/usage.rst` & `ironic-inspector-9.2.4/doc/source/user/usage.rst`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/doc/source/user/troubleshooting.rst` & `ironic-inspector-9.2.4/doc/source/user/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/doc/source/user/workflow.rst` & `ironic-inspector-9.2.4/doc/source/user/workflow.rst`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/doc/source/configuration/sample-config.rst` & `ironic-inspector-9.2.4/doc/source/configuration/sample-config.rst`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/doc/source/conf.py` & `ironic-inspector-9.2.4/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/doc/source/images/states.svg` & `ironic-inspector-9.2.4/doc/source/images/states.svg`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/doc/source/admin/dnsmasq-pxe-filter.rst` & `ironic-inspector-9.2.4/doc/source/admin/dnsmasq-pxe-filter.rst`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/doc/source/admin/upgrade.rst` & `ironic-inspector-9.2.4/doc/source/admin/upgrade.rst`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/tools/test-setup.sh` & `ironic-inspector-9.2.4/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/tools/states_to_dot.py` & `ironic-inspector-9.2.4/tools/states_to_dot.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/tools/bandit.yml` & `ironic-inspector-9.2.4/tools/bandit.yml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/setup.cfg` & `ironic-inspector-9.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/requirements.txt` & `ironic-inspector-9.2.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/AUTHORS` & `ironic-inspector-9.2.4/AUTHORS`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/ramdisk-logs-on-all-failures-24da41edf3a98400.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/ramdisk-logs-on-all-failures-24da41edf3a98400.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/split-services-99873ff27ef2d89b.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/split-services-99873ff27ef2d89b.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/fix-wrong-provision-state-name-150c91c48d471bf9.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/fix-wrong-provision-state-name-150c91c48d471bf9.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/introspection-state-03538fac198882b6.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/introspection-state-03538fac198882b6.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/policy-engine-c44828e3131e6c62.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/policy-engine-c44828e3131e6c62.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/ksadapters-abc9edc63cafa405.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/ksadapters-abc9edc63cafa405.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/ipa-inventory-0a1e8d644da850ff.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/ipa-inventory-0a1e8d644da850ff.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/multiattribute_node_lookup-17e219ba8d3e5eb0.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/multiattribute_node_lookup-17e219ba8d3e5eb0.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/story-2002166-371315335fd8e62d.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/story-2002166-371315335fd8e62d.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/firewall-refactoring-17e8ad764f2cde8d.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/firewall-refactoring-17e8ad764f2cde8d.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/dnsmask-pxe-filter-rootwrap-systemctl-099964ad39d38b4c.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/dnsmask-pxe-filter-rootwrap-systemctl-099964ad39d38b4c.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/deprecate-setting-ipmi-creds-1581ddc63b273811.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/deprecate-setting-ipmi-creds-1581ddc63b273811.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/keystoneauth-plugins-aab6cbe1d0e884bf.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/keystoneauth-plugins-aab6cbe1d0e884bf.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/pxe-filter-dnsmasq-not-known-hosts-filter-76ae5bd7a8db6f75.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/pxe-filter-dnsmasq-not-known-hosts-filter-76ae5bd7a8db6f75.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/cors-5f345c65da7f5c99.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/cors-5f345c65da7f5c99.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/notes/migrate-introspection-data-bcd692c9ad3f22d7.yaml` & `ironic-inspector-9.2.4/releasenotes/notes/migrate-introspection-data-bcd692c9ad3f22d7.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `ironic-inspector-9.2.4/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `ironic-inspector-9.2.4/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/releasenotes/source/conf.py` & `ironic-inspector-9.2.4/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/rootwrap.d/ironic-inspector.filters` & `ironic-inspector-9.2.4/rootwrap.d/ironic-inspector.filters`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/devstack/plugin.sh` & `ironic-inspector-9.2.4/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/devstack/example.local.conf` & `ironic-inspector-9.2.4/devstack/example.local.conf`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/devstack/upgrade/resources.sh` & `ironic-inspector-9.2.4/devstack/upgrade/resources.sh`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/devstack/upgrade/upgrade.sh` & `ironic-inspector-9.2.4/devstack/upgrade/upgrade.sh`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/devstack/upgrade/shutdown.sh` & `ironic-inspector-9.2.4/devstack/upgrade/shutdown.sh`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/playbooks/legacy/ironic-inspector-grenade-dsvm/run.yaml` & `ironic-inspector-9.2.4/playbooks/legacy/ironic-inspector-grenade-dsvm/run.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/lower-constraints.txt` & `ironic-inspector-9.2.4/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/zuul.d/project.yaml` & `ironic-inspector-9.2.4/zuul.d/project.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -9,24 +9,24 @@
       - release-notes-jobs-python3
     check:
       jobs:
         - ironic-inspector-grenade-dsvm
         - ironic-inspector-tempest
         - ironic-inspector-tempest-discovery
         - ironic-inspector-tempest-python3
-        - ironic-inspector-non-standalone-tempest-python3
+        - ironic-inspector-non-standalone-tempest-python3:
+            voting: false
         - openstack-tox-functional
         - openstack-tox-functional-py36
         - bifrost-integration-tinyipa-ubuntu-xenial
         - ironic-inspector-tox-bandit:
             voting: false
     gate:
       queue: ironic
       jobs:
         - ironic-inspector-grenade-dsvm
         - ironic-inspector-tempest
         - ironic-inspector-tempest-discovery
         - ironic-inspector-tempest-python3
-        - ironic-inspector-non-standalone-tempest-python3
         - openstack-tox-functional
         - openstack-tox-functional-py36
         - bifrost-integration-tinyipa-ubuntu-xenial
```

### Comparing `ironic-inspector-9.2.3/zuul.d/ironic-inspector-jobs.yaml` & `ironic-inspector-9.2.4/zuul.d/ironic-inspector-jobs.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/zuul.d/legacy-ironic-inspector-jobs.yaml` & `ironic-inspector-9.2.4/zuul.d/legacy-ironic-inspector-jobs.yaml`

 * *Files identical despite different names*

### Comparing `ironic-inspector-9.2.3/README.rst` & `ironic-inspector-9.2.4/README.rst`

 * *Files identical despite different names*

