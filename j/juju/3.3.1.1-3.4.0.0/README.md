# Comparing `tmp/juju-3.3.1.1.tar.gz` & `tmp/juju-3.4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juju-3.3.1.1.tar", last modified: Thu Feb 15 17:30:34 2024, max compression
+gzip compressed data, was "juju-3.4.0.0.tar", last modified: Thu Mar 28 18:08:28 2024, max compression
```

## Comparing `juju-3.3.1.1.tar` & `juju-3.4.0.0.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2024-02-15 17:30:34.295622 juju-3.3.1.1/
--rw-rw-r--   0 caner     (1000) caner     (1000)      155 2024-02-15 16:55:42.000000 juju-3.3.1.1/CONTRIBUTORS
--rw-rw-r--   0 caner     (1000) caner     (1000)    11344 2024-02-15 16:55:42.000000 juju-3.3.1.1/LICENSE
--rw-rw-r--   0 caner     (1000) caner     (1000)      151 2024-02-15 16:55:42.000000 juju-3.3.1.1/MANIFEST.in
--rw-r--r--   0 caner     (1000) caner     (1000)    41785 2024-02-15 17:30:34.291622 juju-3.3.1.1/PKG-INFO
--rw-rw-r--   0 caner     (1000) caner     (1000)     3238 2024-02-15 16:55:42.000000 juju-3.3.1.1/README.rst
-drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2024-02-15 17:30:34.139618 juju-3.3.1.1/docs/
-drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2024-02-15 17:30:34.147619 juju-3.3.1.1/docs/api/
--rw-rw-r--   0 caner     (1000) caner     (1000)      190 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.action.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      206 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.annotation.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      210 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.application.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)     2352 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.client.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      210 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.constraints.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      206 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.controller.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      186 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.delta.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      190 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.errors.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      206 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.exceptions.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      182 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.juju.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      182 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.loop.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      194 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.machine.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      186 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.model.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      202 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.placement.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      198 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.relation.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      178 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.tag.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      182 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.unit.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      186 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/juju.utils.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      575 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/api/modules.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)    37582 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/changelog.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      666 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/index.rst
-drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2024-02-15 17:30:34.151619 juju-3.3.1.1/docs/narrative/
--rw-rw-r--   0 caner     (1000) caner     (1000)     3034 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/narrative/application.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)     2747 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/narrative/controller.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)      100 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/narrative/index.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)     8713 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/narrative/model.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)     1469 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/narrative/unit.rst
--rw-rw-r--   0 caner     (1000) caner     (1000)     3238 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/readme.rst
-drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2024-02-15 17:30:34.151619 juju-3.3.1.1/docs/upstream-updates/
--rw-rw-r--   0 caner     (1000) caner     (1000)     6676 2024-02-15 16:55:42.000000 juju-3.3.1.1/docs/upstream-updates/index.rst
-drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2024-02-15 17:30:34.179619 juju-3.3.1.1/examples/
--rw-rw-r--   0 caner     (1000) caner     (1000)     1254 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/action.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1757 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/add_k8s.py
--rwxrwxr-x   0 caner     (1000) caner     (1000)     1688 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/add_machine.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1784 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/add_model.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     2073 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/add_secrets_backend.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      914 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/allwatcher.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1033 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/charmhub_deploy_k8s.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      925 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/charmhub_deploy_machine.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      956 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/charmhub_find.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      796 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/charmhub_info.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      627 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/cloud.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      651 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/clouds.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1484 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/config.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      798 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/connect_current_model.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1050 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/controller.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1541 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/credential.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     2243 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/crossmodel.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     2356 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/crossmodel_bundle.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     2561 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/crossmodel_controller.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     2974 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/crossmodel_relation.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      936 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/debug-log.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      983 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/deploy.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1557 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/deploy_bundle.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      958 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/deploy_bundle_charmhub.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1170 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/deploy_bundle_with_trust.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1045 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/deploy_constraints.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      832 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/deploy_local_big_k8s_bundle.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1155 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/deploy_local_bundle_with_resources.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1315 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/deploy_local_file_resource.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1298 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/deploy_local_resource.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      898 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/deploy_with_revision.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     2552 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/expose-application.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1331 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/formatted_status.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      517 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/fullstatus.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1165 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/future.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      737 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/get_cloud.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      678 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/leadership.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      345 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/list_secrets.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      764 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/livemodel.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      776 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/local_refresh.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      824 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/localcharm.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1169 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/machine_hostname.py
--rwxrwxr-x   0 caner     (1000) caner     (1000)      827 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/model.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1141 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/modelsummaries.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     3334 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/relate.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      947 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/run_action.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1209 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/scp.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1290 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/status.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1714 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/unitrun.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1289 2024-02-15 16:55:42.000000 juju-3.3.1.1/examples/upgrade_local_charm_k8s.py
-drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2024-02-15 17:30:34.195620 juju-3.3.1.1/juju/
--rw-rw-r--   0 caner     (1000) caner     (1000)        0 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/__init__.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1341 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/access.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      737 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/action.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      214 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/annotation.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1167 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/annotationhelper.py
--rw-rw-r--   0 caner     (1000) caner     (1000)    38148 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/application.py
--rw-rw-r--   0 caner     (1000) caner     (1000)    45606 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/bundle.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      208 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/charm.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     7284 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/charmhub.py
-drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2024-02-15 17:30:34.291622 juju-3.3.1.1/juju/client/
--rw-rw-r--   0 caner     (1000) caner     (1000)        0 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/__init__.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     8864 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   730276 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client1.py
--rw-rw-r--   0 caner     (1000) caner     (1000)    41464 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client10.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   196254 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client11.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   245218 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client12.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   244188 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client13.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   115453 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client14.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   108914 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client15.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   103511 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client16.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   103511 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client17.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   369413 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client18.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   364812 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client19.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   406826 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client2.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   192763 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client3.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   201775 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client4.py
--rw-rw-r--   0 caner     (1000) caner     (1000)    41639 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client5.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   162501 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client6.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   247072 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client7.py
--rw-rw-r--   0 caner     (1000) caner     (1000)    45251 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client8.py
--rw-rw-r--   0 caner     (1000) caner     (1000)    56944 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_client9.py
--rw-rw-r--   0 caner     (1000) caner     (1000)  1236275 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/_definitions.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1319 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/client.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1442 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/codegen.py
--rw-rw-r--   0 caner     (1000) caner     (1000)    40536 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/connection.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     9267 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/connector.py
--rw-rw-r--   0 caner     (1000) caner     (1000)    32274 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/facade.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      416 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/flags.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     3755 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/gocookies.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     7148 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/jujudata.py
--rw-rw-r--   0 caner     (1000) caner     (1000)    12560 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/overrides.py
-drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2024-02-15 17:30:34.291622 juju-3.3.1.1/juju/client/proxy/
--rw-rw-r--   0 caner     (1000) caner     (1000)      774 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/proxy/factory.py
-drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2024-02-15 17:30:34.291622 juju-3.3.1.1/juju/client/proxy/kubernetes/
--rw-rw-r--   0 caner     (1000) caner     (1000)     2210 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/proxy/kubernetes/proxy.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      563 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/proxy/proxy.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      894 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/client/runner.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     4573 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/constraints.py
--rw-rw-r--   0 caner     (1000) caner     (1000)    38295 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/controller.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     2732 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/delta.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     3726 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/errors.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      142 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/exceptions.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     3763 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/jasyncio.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1257 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/juju.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      231 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/loop.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     8863 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/machine.py
--rw-rw-r--   0 caner     (1000) caner     (1000)   125193 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/model.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     2229 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/names.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     6545 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/offerendpoints.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     5893 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/origin.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1924 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/placement.py
--rw-rw-r--   0 caner     (1000) caner     (1000)    11518 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/provisioner.py
--rw-rw-r--   0 caner     (1000) caner     (1000)        0 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/py.typed
--rw-rw-r--   0 caner     (1000) caner     (1000)     5049 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/relation.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      951 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/remoteapplication.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     3877 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/secrets.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     6616 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/status.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     1408 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/tag.py
--rw-rw-r--   0 caner     (1000) caner     (1000)    15858 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/unit.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     4863 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/url.py
--rw-rw-r--   0 caner     (1000) caner     (1000)     6486 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/user.py
--rw-rw-r--   0 caner     (1000) caner     (1000)    18997 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/utils.py
--rw-rw-r--   0 caner     (1000) caner     (1000)      230 2024-02-15 16:55:42.000000 juju-3.3.1.1/juju/version.py
-drwxrwxr-x   0 caner     (1000) caner     (1000)        0 2024-02-15 17:30:34.199620 juju-3.3.1.1/juju.egg-info/
--rw-r--r--   0 caner     (1000) caner     (1000)    41785 2024-02-15 17:30:34.000000 juju-3.3.1.1/juju.egg-info/PKG-INFO
--rw-rw-r--   0 caner     (1000) caner     (1000)     3668 2024-02-15 17:30:34.000000 juju-3.3.1.1/juju.egg-info/SOURCES.txt
--rw-rw-r--   0 caner     (1000) caner     (1000)        1 2024-02-15 17:30:34.000000 juju-3.3.1.1/juju.egg-info/dependency_links.txt
--rw-rw-r--   0 caner     (1000) caner     (1000)      178 2024-02-15 17:30:34.000000 juju-3.3.1.1/juju.egg-info/requires.txt
--rw-rw-r--   0 caner     (1000) caner     (1000)        5 2024-02-15 17:30:34.000000 juju-3.3.1.1/juju.egg-info/top_level.txt
--rw-rw-r--   0 caner     (1000) caner     (1000)       38 2024-02-15 17:30:34.295622 juju-3.3.1.1/setup.cfg
--rw-rw-r--   0 caner     (1000) caner     (1000)     1747 2024-02-15 16:55:42.000000 juju-3.3.1.1/setup.py
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.989335 juju-3.4.0.0/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      155 2024-03-28 18:05:09.000000 juju-3.4.0.0/CONTRIBUTORS
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    11344 2024-03-28 18:05:09.000000 juju-3.4.0.0/LICENSE
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      151 2024-03-28 18:05:09.000000 juju-3.4.0.0/MANIFEST.in
+-rw-r--r--   0 aflynn    (1000) aflynn    (1000)    42136 2024-03-28 18:08:28.989335 juju-3.4.0.0/PKG-INFO
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3238 2024-03-28 18:05:09.000000 juju-3.4.0.0/README.rst
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.885335 juju-3.4.0.0/docs/
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.893335 juju-3.4.0.0/docs/api/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      190 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.action.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      206 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.annotation.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      210 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.application.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2352 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.client.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      210 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.constraints.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      206 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.controller.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      186 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.delta.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      190 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.errors.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      206 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.exceptions.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      182 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.juju.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      182 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.loop.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      194 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.machine.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      186 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.model.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      202 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.placement.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      198 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.relation.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      178 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.tag.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      182 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.unit.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      186 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/juju.utils.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      575 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/api/modules.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    37933 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/changelog.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      666 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/index.rst
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.893335 juju-3.4.0.0/docs/narrative/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3034 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/narrative/application.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2747 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/narrative/controller.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      100 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/narrative/index.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     8713 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/narrative/model.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1469 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/narrative/unit.rst
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3238 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/readme.rst
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.893335 juju-3.4.0.0/docs/upstream-updates/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     6676 2024-03-28 18:05:09.000000 juju-3.4.0.0/docs/upstream-updates/index.rst
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.909335 juju-3.4.0.0/examples/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1254 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/action.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1757 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/add_k8s.py
+-rwxrwxr-x   0 aflynn    (1000) aflynn    (1000)     1688 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/add_machine.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1784 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/add_model.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2073 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/add_secrets_backend.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      914 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/allwatcher.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1033 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/charmhub_deploy_k8s.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      925 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/charmhub_deploy_machine.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      956 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/charmhub_find.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      796 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/charmhub_info.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      627 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/cloud.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      651 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/clouds.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1484 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/config.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      798 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/connect_current_model.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1050 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/controller.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1541 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/credential.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2243 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/crossmodel.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2356 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/crossmodel_bundle.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2561 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/crossmodel_controller.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2974 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/crossmodel_relation.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      936 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/debug-log.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      983 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1557 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_bundle.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      958 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_bundle_charmhub.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1170 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_bundle_with_trust.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1045 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_constraints.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      832 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_local_big_k8s_bundle.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1155 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_local_bundle_with_resources.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1315 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_local_file_resource.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1298 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_local_resource.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      898 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/deploy_with_revision.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2552 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/expose-application.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1331 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/formatted_status.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      517 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/fullstatus.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1165 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/future.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      737 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/get_cloud.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      678 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/leadership.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      345 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/list_secrets.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      764 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/livemodel.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      776 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/local_refresh.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      824 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/localcharm.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1169 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/machine_hostname.py
+-rwxrwxr-x   0 aflynn    (1000) aflynn    (1000)      827 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/model.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1141 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/modelsummaries.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3334 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/relate.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      947 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/run_action.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1209 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/scp.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1290 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/status.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1714 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/unitrun.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1289 2024-03-28 18:05:09.000000 juju-3.4.0.0/examples/upgrade_local_charm_k8s.py
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.917335 juju-3.4.0.0/juju/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/__init__.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1341 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/access.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      737 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/action.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      214 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/annotation.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1167 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/annotationhelper.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    38148 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/application.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    45606 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/bundle.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      208 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/charm.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     7284 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/charmhub.py
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.985335 juju-3.4.0.0/juju/client/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/__init__.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     8864 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   730276 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client1.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    41464 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client10.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   196254 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client11.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   245218 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client12.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   244188 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client13.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   115453 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client14.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   108914 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client15.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   103511 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client16.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   103511 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client17.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   369413 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client18.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   364812 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client19.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   406826 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client2.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   192763 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client3.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   201775 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client4.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    41639 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client5.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   162501 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client6.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   247072 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client7.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    45251 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client8.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    56944 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_client9.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)  1236275 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/_definitions.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1319 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/client.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1442 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/codegen.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    40536 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/connection.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     9267 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/connector.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    32274 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/facade.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      416 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/flags.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3755 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/gocookies.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     7148 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/jujudata.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    12560 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/overrides.py
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.989335 juju-3.4.0.0/juju/client/proxy/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      774 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/proxy/factory.py
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.989335 juju-3.4.0.0/juju/client/proxy/kubernetes/
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2210 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/proxy/kubernetes/proxy.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      563 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/proxy/proxy.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      894 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/client/runner.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     4573 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/constraints.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    38332 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/controller.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2732 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/delta.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3726 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/errors.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      142 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/exceptions.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3763 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/jasyncio.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1257 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/juju.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      231 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/loop.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    11122 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/machine.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)   125230 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/model.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     2229 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/names.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     6545 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/offerendpoints.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     5893 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/origin.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1924 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/placement.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    11518 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/provisioner.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/py.typed
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     5049 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/relation.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      951 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/remoteapplication.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3877 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/secrets.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     6616 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/status.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1408 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/tag.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    15858 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/unit.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     4863 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/url.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     6486 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/user.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)    18997 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/utils.py
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      230 2024-03-28 18:05:09.000000 juju-3.4.0.0/juju/version.py
+drwxrwxr-x   0 aflynn    (1000) aflynn    (1000)        0 2024-03-28 18:08:28.989335 juju-3.4.0.0/juju.egg-info/
+-rw-r--r--   0 aflynn    (1000) aflynn    (1000)    42136 2024-03-28 18:08:28.000000 juju-3.4.0.0/juju.egg-info/PKG-INFO
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     3668 2024-03-28 18:08:28.000000 juju-3.4.0.0/juju.egg-info/SOURCES.txt
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        1 2024-03-28 18:08:28.000000 juju-3.4.0.0/juju.egg-info/dependency_links.txt
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)      178 2024-03-28 18:08:28.000000 juju-3.4.0.0/juju.egg-info/requires.txt
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)        5 2024-03-28 18:08:28.000000 juju-3.4.0.0/juju.egg-info/top_level.txt
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)       38 2024-03-28 18:08:28.989335 juju-3.4.0.0/setup.cfg
+-rw-rw-r--   0 aflynn    (1000) aflynn    (1000)     1747 2024-03-28 18:05:09.000000 juju-3.4.0.0/setup.py
```

### Comparing `juju-3.3.1.1/LICENSE` & `juju-3.4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/PKG-INFO` & `juju-3.4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juju
-Version: 3.3.1.1
+Version: 3.4.0.0
 Summary: Python library for Juju
 Home-page: https://github.com/juju/python-libjuju
 Maintainer: Juju Ecosystem Engineering
 Maintainer-email: juju@lists.ubuntu.com
 License: Apache 2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -159,14 +159,25 @@
 a release with the same version in the following week. Newly generated schemas
 will be updated per Juju releases.
 
 
 Changelog
 ---------
 
+3.4.0.0
+^^^^^^^
+
+Monday 25th Mar 2024
+
+## What's Changed
+
+* Add build test and update issue template by @cderici in https://github.com/juju/python-libjuju/pull/1030
+* fix: machine scp & ssh by @yanksyoon in https://github.com/juju/python-libjuju/pull/1020
+* Bugfix none type on master by @Aflynn50 in https://github.com/juju/python-libjuju/pull/1036
+
 3.3.1.1
 ^^^^^^^
 
 Thursday 15th Feb 2024
 
 ## What's Changed
```

### Comparing `juju-3.3.1.1/README.rst` & `juju-3.4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/docs/api/juju.client.rst` & `juju-3.4.0.0/docs/api/juju.client.rst`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/docs/api/modules.rst` & `juju-3.4.0.0/docs/api/modules.rst`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/docs/changelog.rst` & `juju-3.4.0.0/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Changelog
 ---------
 
+3.4.0.0
+^^^^^^^
+
+Monday 25th Mar 2024
+
+## What's Changed
+
+* Add build test and update issue template by @cderici in https://github.com/juju/python-libjuju/pull/1030
+* fix: machine scp & ssh by @yanksyoon in https://github.com/juju/python-libjuju/pull/1020
+* Bugfix none type on master by @Aflynn50 in https://github.com/juju/python-libjuju/pull/1036
+
 3.3.1.1
 ^^^^^^^
 
 Thursday 15th Feb 2024
 
 ## What's Changed
```

### Comparing `juju-3.3.1.1/docs/index.rst` & `juju-3.4.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/docs/narrative/application.rst` & `juju-3.4.0.0/docs/narrative/application.rst`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/docs/narrative/controller.rst` & `juju-3.4.0.0/docs/narrative/controller.rst`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/docs/narrative/model.rst` & `juju-3.4.0.0/docs/narrative/model.rst`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/docs/narrative/unit.rst` & `juju-3.4.0.0/docs/narrative/unit.rst`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/docs/readme.rst` & `juju-3.4.0.0/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/docs/upstream-updates/index.rst` & `juju-3.4.0.0/docs/upstream-updates/index.rst`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/action.py` & `juju-3.4.0.0/examples/action.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/add_k8s.py` & `juju-3.4.0.0/examples/add_k8s.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/add_machine.py` & `juju-3.4.0.0/examples/add_machine.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/add_model.py` & `juju-3.4.0.0/examples/add_model.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/add_secrets_backend.py` & `juju-3.4.0.0/examples/add_secrets_backend.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/allwatcher.py` & `juju-3.4.0.0/examples/allwatcher.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/charmhub_deploy_k8s.py` & `juju-3.4.0.0/examples/charmhub_deploy_k8s.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/charmhub_deploy_machine.py` & `juju-3.4.0.0/examples/charmhub_deploy_machine.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/charmhub_find.py` & `juju-3.4.0.0/examples/charmhub_find.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/charmhub_info.py` & `juju-3.4.0.0/examples/charmhub_info.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/cloud.py` & `juju-3.4.0.0/examples/cloud.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/clouds.py` & `juju-3.4.0.0/examples/clouds.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/config.py` & `juju-3.4.0.0/examples/config.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/connect_current_model.py` & `juju-3.4.0.0/examples/connect_current_model.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/controller.py` & `juju-3.4.0.0/examples/controller.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/credential.py` & `juju-3.4.0.0/examples/credential.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/crossmodel.py` & `juju-3.4.0.0/examples/crossmodel.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/crossmodel_bundle.py` & `juju-3.4.0.0/examples/crossmodel_bundle.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/crossmodel_controller.py` & `juju-3.4.0.0/examples/crossmodel_controller.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/crossmodel_relation.py` & `juju-3.4.0.0/examples/crossmodel_relation.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/debug-log.py` & `juju-3.4.0.0/examples/debug-log.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/deploy.py` & `juju-3.4.0.0/examples/deploy.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/deploy_bundle.py` & `juju-3.4.0.0/examples/deploy_bundle.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/deploy_bundle_charmhub.py` & `juju-3.4.0.0/examples/deploy_bundle_charmhub.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/deploy_bundle_with_trust.py` & `juju-3.4.0.0/examples/deploy_bundle_with_trust.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/deploy_constraints.py` & `juju-3.4.0.0/examples/deploy_constraints.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/deploy_local_big_k8s_bundle.py` & `juju-3.4.0.0/examples/deploy_local_big_k8s_bundle.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/deploy_local_bundle_with_resources.py` & `juju-3.4.0.0/examples/deploy_local_bundle_with_resources.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/deploy_local_file_resource.py` & `juju-3.4.0.0/examples/deploy_local_file_resource.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/deploy_local_resource.py` & `juju-3.4.0.0/examples/deploy_local_resource.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/deploy_with_revision.py` & `juju-3.4.0.0/examples/deploy_with_revision.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/expose-application.py` & `juju-3.4.0.0/examples/expose-application.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/formatted_status.py` & `juju-3.4.0.0/examples/formatted_status.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/fullstatus.py` & `juju-3.4.0.0/examples/fullstatus.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/future.py` & `juju-3.4.0.0/examples/future.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/get_cloud.py` & `juju-3.4.0.0/examples/get_cloud.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/leadership.py` & `juju-3.4.0.0/examples/leadership.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/livemodel.py` & `juju-3.4.0.0/examples/livemodel.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/local_refresh.py` & `juju-3.4.0.0/examples/local_refresh.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/localcharm.py` & `juju-3.4.0.0/examples/localcharm.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/machine_hostname.py` & `juju-3.4.0.0/examples/machine_hostname.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/model.py` & `juju-3.4.0.0/examples/model.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/modelsummaries.py` & `juju-3.4.0.0/examples/modelsummaries.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/relate.py` & `juju-3.4.0.0/examples/relate.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/run_action.py` & `juju-3.4.0.0/examples/run_action.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/scp.py` & `juju-3.4.0.0/examples/scp.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/status.py` & `juju-3.4.0.0/examples/status.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/unitrun.py` & `juju-3.4.0.0/examples/unitrun.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/examples/upgrade_local_charm_k8s.py` & `juju-3.4.0.0/examples/upgrade_local_charm_k8s.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/access.py` & `juju-3.4.0.0/juju/access.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/action.py` & `juju-3.4.0.0/juju/action.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/annotationhelper.py` & `juju-3.4.0.0/juju/annotationhelper.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/application.py` & `juju-3.4.0.0/juju/application.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/bundle.py` & `juju-3.4.0.0/juju/bundle.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/charmhub.py` & `juju-3.4.0.0/juju/charmhub.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client.py` & `juju-3.4.0.0/juju/client/_client.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client1.py` & `juju-3.4.0.0/juju/client/_client1.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client10.py` & `juju-3.4.0.0/juju/client/_client10.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client11.py` & `juju-3.4.0.0/juju/client/_client11.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client12.py` & `juju-3.4.0.0/juju/client/_client12.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client13.py` & `juju-3.4.0.0/juju/client/_client13.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client14.py` & `juju-3.4.0.0/juju/client/_client14.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client15.py` & `juju-3.4.0.0/juju/client/_client15.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client16.py` & `juju-3.4.0.0/juju/client/_client16.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client17.py` & `juju-3.4.0.0/juju/client/_client17.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client18.py` & `juju-3.4.0.0/juju/client/_client18.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client19.py` & `juju-3.4.0.0/juju/client/_client19.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client2.py` & `juju-3.4.0.0/juju/client/_client2.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client3.py` & `juju-3.4.0.0/juju/client/_client3.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client4.py` & `juju-3.4.0.0/juju/client/_client4.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client5.py` & `juju-3.4.0.0/juju/client/_client5.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client6.py` & `juju-3.4.0.0/juju/client/_client6.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client7.py` & `juju-3.4.0.0/juju/client/_client7.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client8.py` & `juju-3.4.0.0/juju/client/_client8.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_client9.py` & `juju-3.4.0.0/juju/client/_client9.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/_definitions.py` & `juju-3.4.0.0/juju/client/_definitions.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/client.py` & `juju-3.4.0.0/juju/client/client.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/codegen.py` & `juju-3.4.0.0/juju/client/codegen.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/connection.py` & `juju-3.4.0.0/juju/client/connection.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/connector.py` & `juju-3.4.0.0/juju/client/connector.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/facade.py` & `juju-3.4.0.0/juju/client/facade.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/gocookies.py` & `juju-3.4.0.0/juju/client/gocookies.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/jujudata.py` & `juju-3.4.0.0/juju/client/jujudata.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/overrides.py` & `juju-3.4.0.0/juju/client/overrides.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/proxy/factory.py` & `juju-3.4.0.0/juju/client/proxy/factory.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/proxy/kubernetes/proxy.py` & `juju-3.4.0.0/juju/client/proxy/kubernetes/proxy.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/proxy/proxy.py` & `juju-3.4.0.0/juju/client/proxy/proxy.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/client/runner.py` & `juju-3.4.0.0/juju/client/runner.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/constraints.py` & `juju-3.4.0.0/juju/constraints.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/controller.py` & `juju-3.4.0.0/juju/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -850,15 +850,16 @@
                     log.debug("watcher id: {}".format(result.watcher_id))
                     watcher.Id = result.watcher_id
 
                 while True:
                     try:
                         results = await utils.run_with_interrupt(
                             watcher.Next(),
-                            stop_event)
+                            stop_event,
+                            log=log)
                     except JujuAPIError as e:
                         if 'watcher was stopped' not in str(e):
                             raise
                     except websockets.ConnectionClosed:
                         break
                     if stop_event.is_set():
                         try:
```

### Comparing `juju-3.3.1.1/juju/delta.py` & `juju-3.4.0.0/juju/delta.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/errors.py` & `juju-3.4.0.0/juju/errors.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/jasyncio.py` & `juju-3.4.0.0/juju/jasyncio.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/juju.py` & `juju-3.4.0.0/juju/juju.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/machine.py` & `juju-3.4.0.0/juju/machine.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright 2023 Canonical Ltd.
 # Licensed under the Apache V2, see LICENCE file for details.
 
 import ipaddress
 import logging
+import typing
 
 import pyrfc3339
 
-from . import model, tag, jasyncio
+from . import jasyncio, model, tag
 from .annotationhelper import _get_annotations, _set_annotations
 from .client import client
 from .errors import JujuError
-from juju.utils import juju_ssh_key_paths
+from juju.utils import juju_ssh_key_paths, block_until
 
 log = logging.getLogger(__name__)
 
 
 class Machine(model.ModelEntity):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -66,50 +67,56 @@
         if isinstance(ipaddr, ipaddress.IPv6Address):
             fmt = '[{}]'
         else:
             fmt = '{}'
         return fmt.format(ipaddr)
 
     async def scp_to(self, source, destination, user='ubuntu', proxy=False,
-                     scp_opts=''):
+                     scp_opts='', wait_for_active=False, timeout=None):
         """Transfer files to this machine.
 
         :param str source: Local path of file(s) to transfer
         :param str destination: Remote destination of transferred files
         :param str user: Remote username
         :param bool proxy: Proxy through the Juju API server
         :param scp_opts: Additional options to the `scp` command
         :type scp_opts: str or list
+        :param bool wait_for_active: Wait until the machine is ready to take in ssh commands.
+        :param int timeout: Time in seconds to wait until the machine becomes ready.
         """
         if proxy:
             raise NotImplementedError('proxy option is not implemented')
-
+        if wait_for_active:
+            await block_until(lambda: self.addresses, timeout=timeout)
         try:
             # if dns_name is an IP address format it appropriately
             address = self._format_addr(self.dns_name)
         except ValueError:
             # otherwise we assume it to be a DNS resolvable string
             address = self.dns_name
         destination = '{}@{}:{}'.format(user, address, destination)
         await self._scp(source, destination, scp_opts)
 
     async def scp_from(self, source, destination, user='ubuntu', proxy=False,
-                       scp_opts=''):
+                       scp_opts='', wait_for_active=False, timeout=None):
         """Transfer files from this machine.
 
         :param str source: Remote path of file(s) to transfer
         :param str destination: Local destination of transferred files
         :param str user: Remote username
         :param bool proxy: Proxy through the Juju API server
         :param scp_opts: Additional options to the `scp` command
         :type scp_opts: str or list
+        :param bool wait_for_active: Wait until the machine is ready to take in ssh commands.
+        :param int timeout: Time in seconds to wait until the machine becomes ready.
         """
         if proxy:
             raise NotImplementedError('proxy option is not implemented')
-
+        if wait_for_active:
+            await block_until(lambda: self.addresses, timeout=timeout)
         try:
             # if dns_name is an IP address format it appropriately
             address = self._format_addr(self.dns_name)
         except ValueError:
             # otherwise we assume it to be a DNS resolvable string
             address = self.dns_name
         source = '{}@{}:{}'.format(user, address, source)
@@ -125,53 +132,85 @@
             '-i', id_path,
             '-o', 'StrictHostKeyChecking=no',
             '-q',
             '-B'
         ]
         cmd.extend(scp_opts.split() if isinstance(scp_opts, str) else scp_opts)
         cmd.extend([source, destination])
-        process = await jasyncio.create_subprocess_exec(*cmd)
-        await process.wait()
+        # There's a bit of a gap between the time that the machine is assigned an IP and the ssh
+        # service is up and listening, which creates a race for the ssh command. So we retry a
+        # couple of times until either we run out of attempts, or the ssh command succeeds to
+        # mitigate that effect.
+        # TODO (cderici): refactor the ssh and scp subcommand processing into a single method.
+        retry_backoff = 2
+        retries = 10
+        for _ in range(retries):
+            process = await jasyncio.create_subprocess_exec(*cmd)
+            await process.wait()
+            if process.returncode == 0:
+                break
+            await jasyncio.sleep(retry_backoff)
         if process.returncode != 0:
-            raise JujuError("command failed: %s" % cmd)
+            raise JujuError(f"command failed after {retries} attempts: {cmd}")
 
     async def ssh(
-            self, command, user='ubuntu', proxy=False, ssh_opts=None):
+            self, command, user='ubuntu', proxy=False, ssh_opts=None, wait_for_active=False, timeout=None):
         """Execute a command over SSH on this machine.
 
         :param str command: Command to execute
         :param str user: Remote username
         :param bool proxy: Proxy through the Juju API server
         :param str ssh_opts: Additional options to the `ssh` command
-
+        :param bool wait_for_active: Wait until the machine is ready to take in ssh commands.
+        :param int timeout: Time in seconds to wait until the machine becomes ready.
         """
         if proxy:
             raise NotImplementedError('proxy option is not implemented')
+        if wait_for_active:
+            await block_until(lambda: self.addresses, timeout=timeout)
         address = self.dns_name
         destination = "{}@{}".format(user, address)
         _, id_path = juju_ssh_key_paths()
         cmd = [
             'ssh',
             '-i', id_path,
             '-o', 'StrictHostKeyChecking=no',
             '-q',
             destination
         ]
         if ssh_opts:
             cmd.extend(ssh_opts.split() if isinstance(ssh_opts, str) else ssh_opts)
         cmd.extend([command])
-        process = await jasyncio.create_subprocess_exec(
-            *cmd, stdout=jasyncio.subprocess.PIPE, stderr=jasyncio.subprocess.PIPE)
-        stdout, stderr = await process.communicate()
+
+        # There's a bit of a gap between the time that the machine is assigned an IP and the ssh
+        # service is up and listening, which creates a race for the ssh command. So we retry a
+        # couple of times until either we run out of attempts, or the ssh command succeeds to
+        # mitigate that effect.
+        retry_backoff = 2
+        retries = 10
+        for _ in range(retries):
+            process = await jasyncio.create_subprocess_exec(
+                *cmd, stdout=jasyncio.subprocess.PIPE, stderr=jasyncio.subprocess.PIPE)
+            stdout, stderr = await process.communicate()
+            if process.returncode == 0:
+                break
+            await jasyncio.sleep(retry_backoff)
         if process.returncode != 0:
-            raise JujuError("command failed: %s with %s" % (cmd, stderr.decode()))
+            raise JujuError(f"command failed: {cmd} after {retries} attempts, with {stderr.decode()}")
         # stdout is a bytes-like object, returning a string might be more useful
         return stdout.decode()
 
     @property
+    def addresses(self) -> typing.List[str]:
+        """Returns the machine addresses.
+
+        """
+        return self.safe_data['addresses'] or []
+
+    @property
     def agent_status(self):
         """Returns the current Juju agent status string.
 
         """
         return self.safe_data['agent-status']['current']
 
     @property
@@ -217,19 +256,18 @@
     @property
     def dns_name(self):
         """Get the DNS name for this machine. This is a best guess based on the
         addresses available in current data.
 
         May return None if no suitable address is found.
         """
-        addresses = self.safe_data['addresses'] or []
         ordered_addresses = []
         ordered_scopes = ['public', 'local-cloud', 'local-fan']
         for scope in ordered_scopes:
-            for address in addresses:
+            for address in self.addresses:
                 if scope == address['scope']:
                     ordered_addresses.append(address)
         for address in ordered_addresses:
             scope = address['scope']
             for check_scope in ordered_scopes:
                 if scope == check_scope:
                     return address['value']
```

### Comparing `juju-3.3.1.1/juju/model.py` & `juju-3.4.0.0/juju/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1200,15 +1200,16 @@
             try:
                 allwatcher = client.AllWatcherFacade.from_connection(
                     self.connection())
                 while not self._watch_stopping.is_set():
                     try:
                         results = await utils.run_with_interrupt(
                             allwatcher.Next(),
-                            self._watch_stopping)
+                            self._watch_stopping,
+                            log=log)
                     except JujuAPIError as e:
                         if 'watcher was stopped' not in str(e):
                             raise
                         if self._watch_stopping.is_set():
                             # this shouldn't ever actually happen, because
                             # the event should trigger before the controller
                             # has a chance to tell us the watcher is stopped
```

### Comparing `juju-3.3.1.1/juju/names.py` & `juju-3.4.0.0/juju/names.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/offerendpoints.py` & `juju-3.4.0.0/juju/offerendpoints.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/origin.py` & `juju-3.4.0.0/juju/origin.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/placement.py` & `juju-3.4.0.0/juju/placement.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/provisioner.py` & `juju-3.4.0.0/juju/provisioner.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/relation.py` & `juju-3.4.0.0/juju/relation.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/remoteapplication.py` & `juju-3.4.0.0/juju/remoteapplication.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/secrets.py` & `juju-3.4.0.0/juju/secrets.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/status.py` & `juju-3.4.0.0/juju/status.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/tag.py` & `juju-3.4.0.0/juju/tag.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/unit.py` & `juju-3.4.0.0/juju/unit.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/url.py` & `juju-3.4.0.0/juju/url.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/user.py` & `juju-3.4.0.0/juju/user.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju/utils.py` & `juju-3.4.0.0/juju/utils.py`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/juju.egg-info/PKG-INFO` & `juju-3.4.0.0/juju.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juju
-Version: 3.3.1.1
+Version: 3.4.0.0
 Summary: Python library for Juju
 Home-page: https://github.com/juju/python-libjuju
 Maintainer: Juju Ecosystem Engineering
 Maintainer-email: juju@lists.ubuntu.com
 License: Apache 2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -159,14 +159,25 @@
 a release with the same version in the following week. Newly generated schemas
 will be updated per Juju releases.
 
 
 Changelog
 ---------
 
+3.4.0.0
+^^^^^^^
+
+Monday 25th Mar 2024
+
+## What's Changed
+
+* Add build test and update issue template by @cderici in https://github.com/juju/python-libjuju/pull/1030
+* fix: machine scp & ssh by @yanksyoon in https://github.com/juju/python-libjuju/pull/1020
+* Bugfix none type on master by @Aflynn50 in https://github.com/juju/python-libjuju/pull/1036
+
 3.3.1.1
 ^^^^^^^
 
 Thursday 15th Feb 2024
 
 ## What's Changed
```

### Comparing `juju-3.3.1.1/juju.egg-info/SOURCES.txt` & `juju-3.4.0.0/juju.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `juju-3.3.1.1/setup.py` & `juju-3.4.0.0/setup.py`

 * *Files identical despite different names*

