# Comparing `tmp/k8s-0.8.0.tar.gz` & `tmp/k8s-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/k8s-0.8.0.tar", last modified: Thu Mar  8 14:56:35 2018, max compression
+gzip compressed data, was "dist/k8s-0.9.0.tar", last modified: Wed May  9 07:05:06 2018, max compression
```

## Comparing `k8s-0.8.0.tar` & `k8s-0.9.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-03-08 14:56:35.000000 k8s-0.8.0/
--rw-rw-r--   0 runner    (1003) runner    (1003)      296 2018-03-08 14:56:35.000000 k8s-0.8.0/setup.cfg
--rw-rw-r--   0 runner    (1003) runner    (1003)     1764 2018-03-08 14:56:15.000000 k8s-0.8.0/.gitignore
-drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-03-08 14:56:35.000000 k8s-0.8.0/bin/
--rw-rw-r--   0 runner    (1003) runner    (1003)     4012 2018-03-08 14:56:15.000000 k8s-0.8.0/bin/test_release.py
--rwxrwxr-x   0 runner    (1003) runner    (1003)     8051 2018-03-08 14:56:15.000000 k8s-0.8.0/bin/release.py
--rwxrwxr-x   0 runner    (1003) runner    (1003)     1822 2018-03-08 14:56:15.000000 k8s-0.8.0/bin/get_github_release.py
--rw-rw-r--   0 runner    (1003) runner    (1003)    11340 2018-03-08 14:56:15.000000 k8s-0.8.0/LICENSE
--rw-rw-r--   0 runner    (1003) runner    (1003)      385 2018-03-08 14:56:15.000000 k8s-0.8.0/tox.ini
--rw-rw-r--   0 runner    (1003) runner    (1003)     3447 2018-03-08 14:56:35.000000 k8s-0.8.0/PKG-INFO
--rw-rw-r--   0 runner    (1003) runner    (1003)       54 2018-03-08 14:56:15.000000 k8s-0.8.0/requirements.txt
-drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-03-08 14:56:35.000000 k8s-0.8.0/k8s.egg-info/
--rw-rw-r--   0 runner    (1003) runner    (1003)        1 2018-03-08 14:56:35.000000 k8s-0.8.0/k8s.egg-info/zip-safe
--rw-rw-r--   0 runner    (1003) runner    (1003)        1 2018-03-08 14:56:35.000000 k8s-0.8.0/k8s.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1003) runner    (1003)      256 2018-03-08 14:56:35.000000 k8s-0.8.0/k8s.egg-info/requires.txt
--rw-rw-r--   0 runner    (1003) runner    (1003)     2036 2018-03-08 14:56:35.000000 k8s-0.8.0/k8s.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1003) runner    (1003)     3447 2018-03-08 14:56:35.000000 k8s-0.8.0/k8s.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1003) runner    (1003)        4 2018-03-08 14:56:35.000000 k8s-0.8.0/k8s.egg-info/top_level.txt
-drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-03-08 14:56:35.000000 k8s-0.8.0/tests/
--rw-rw-r--   0 runner    (1003) runner    (1003)     2983 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/conftest.py
-drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-03-08 14:56:35.000000 k8s-0.8.0/tests/k8s/
--rw-rw-r--   0 runner    (1003) runner    (1003)     4161 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/k8s/test_watcher.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     2360 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/k8s/test_configmap.py
--rw-rw-r--   0 runner    (1003) runner    (1003)      311 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/k8s/util.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     7408 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/k8s/test_client.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     1204 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/k8s/conftest.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     5054 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/k8s/test_pod.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     3435 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/k8s/test_ingress.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     3028 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/k8s/test_job.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     2767 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/k8s/test_resourcequota.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     2639 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/k8s/test_model.py
--rw-rw-r--   0 runner    (1003) runner    (1003)      975 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/k8s/test_base.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     6761 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/k8s/test_service.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     4338 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/k8s/test_fields.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     6187 2018-03-08 14:56:15.000000 k8s-0.8.0/tests/k8s/test_deployer.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     1688 2018-03-08 14:56:15.000000 k8s-0.8.0/README.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      448 2018-03-08 14:56:15.000000 k8s-0.8.0/.prospector.yaml
-drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-03-08 14:56:35.000000 k8s-0.8.0/docs/
-drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-03-08 14:56:35.000000 k8s-0.8.0/docs/source/
--rw-rw-r--   0 runner    (1003) runner    (1003)     4341 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/tutorial.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)     5424 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/conf.py
--rw-rw-r--   0 runner    (1003) runner    (1003)      468 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/index.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)     6201 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/developer.rst
-drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-03-08 14:56:35.000000 k8s-0.8.0/docs/source/modules/
--rw-rw-r--   0 runner    (1003) runner    (1003)      126 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.watcher.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      149 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.models.ingress.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      123 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.fields.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      158 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.models.deployment.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      462 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.models.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      155 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.models.configmap.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      158 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.models.autoscaler.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      192 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.models.third_party_resource.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      137 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.models.pod.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      117 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.base.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      167 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.models.resourcequota.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      196 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.models.replication_controller.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      123 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.config.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      210 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.models.custom_resource_definition.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)       66 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/modules.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      123 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.client.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      149 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.models.service.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      146 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.models.common.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      265 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/source/modules/k8s.rst
--rw-rw-r--   0 runner    (1003) runner    (1003)      697 2018-03-08 14:56:15.000000 k8s-0.8.0/docs/Makefile
--rw-rw-r--   0 runner    (1003) runner    (1003)     2772 2018-03-08 14:56:15.000000 k8s-0.8.0/setup.py
-drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-03-08 14:56:35.000000 k8s-0.8.0/k8s/
-drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-03-08 14:56:35.000000 k8s-0.8.0/k8s/models/
--rw-rw-r--   0 runner    (1003) runner    (1003)      931 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/models/service.py
--rw-rw-r--   0 runner    (1003) runner    (1003)      923 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/models/pod_disruption_budget.py
--rw-rw-r--   0 runner    (1003) runner    (1003)      721 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/models/job.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     4625 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/models/pod.py
--rw-rw-r--   0 runner    (1003) runner    (1003)      485 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/models/third_party_resource.py
--rw-rw-r--   0 runner    (1003) runner    (1003)      604 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/models/replication_controller.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     1055 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/models/ingress.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     1689 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/models/custom_resource_definition.py
--rw-rw-r--   0 runner    (1003) runner    (1003)      414 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/models/common.py
--rw-rw-r--   0 runner    (1003) runner    (1003)       42 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/models/__init__.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     1352 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/models/deployment.py
--rw-rw-r--   0 runner    (1003) runner    (1003)      336 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/models/configmap.py
--rw-rw-r--   0 runner    (1003) runner    (1003)      758 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/models/resourcequota.py
--rw-rw-r--   0 runner    (1003) runner    (1003)      820 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/models/autoscaler.py
--rw-rw-r--   0 runner    (1003) runner    (1003)      208 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/config.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     1607 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/watcher.py
--rw-rw-r--   0 runner    (1003) runner    (1003)       42 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/__init__.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     8067 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/base.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     4297 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/fields.py
--rw-rw-r--   0 runner    (1003) runner    (1003)     5110 2018-03-08 14:56:15.000000 k8s-0.8.0/k8s/client.py
+drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-05-09 07:05:06.000000 k8s-0.9.0/
+-rw-rw-r--   0 runner    (1003) runner    (1003)      296 2018-05-09 07:05:06.000000 k8s-0.9.0/setup.cfg
+-rw-rw-r--   0 runner    (1003) runner    (1003)     1778 2018-05-09 07:04:38.000000 k8s-0.9.0/.gitignore
+drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-05-09 07:05:06.000000 k8s-0.9.0/bin/
+-rw-rw-r--   0 runner    (1003) runner    (1003)     4012 2018-05-09 07:04:35.000000 k8s-0.9.0/bin/test_release.py
+-rwxrwxr-x   0 runner    (1003) runner    (1003)     8051 2018-05-09 07:04:35.000000 k8s-0.9.0/bin/release.py
+-rwxrwxr-x   0 runner    (1003) runner    (1003)     1822 2018-05-09 07:04:35.000000 k8s-0.9.0/bin/get_github_release.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)    11340 2018-05-09 07:04:35.000000 k8s-0.9.0/LICENSE
+-rw-rw-r--   0 runner    (1003) runner    (1003)      385 2018-05-09 07:04:38.000000 k8s-0.9.0/tox.ini
+-rw-rw-r--   0 runner    (1003) runner    (1003)     3484 2018-05-09 07:05:06.000000 k8s-0.9.0/PKG-INFO
+-rw-rw-r--   0 runner    (1003) runner    (1003)       54 2018-05-09 07:04:35.000000 k8s-0.9.0/requirements.txt
+drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-05-09 07:05:06.000000 k8s-0.9.0/k8s.egg-info/
+-rw-rw-r--   0 runner    (1003) runner    (1003)        1 2018-05-09 07:05:06.000000 k8s-0.9.0/k8s.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1003) runner    (1003)        1 2018-05-09 07:05:06.000000 k8s-0.9.0/k8s.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1003) runner    (1003)      256 2018-05-09 07:05:06.000000 k8s-0.9.0/k8s.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1003) runner    (1003)     2036 2018-05-09 07:05:06.000000 k8s-0.9.0/k8s.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1003) runner    (1003)     3484 2018-05-09 07:05:06.000000 k8s-0.9.0/k8s.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1003) runner    (1003)        4 2018-05-09 07:05:06.000000 k8s-0.9.0/k8s.egg-info/top_level.txt
+drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-05-09 07:05:06.000000 k8s-0.9.0/tests/
+-rw-rw-r--   0 runner    (1003) runner    (1003)     2983 2018-05-09 07:04:35.000000 k8s-0.9.0/tests/conftest.py
+drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-05-09 07:05:06.000000 k8s-0.9.0/tests/k8s/
+-rw-rw-r--   0 runner    (1003) runner    (1003)     4161 2018-05-09 07:04:38.000000 k8s-0.9.0/tests/k8s/test_watcher.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     2360 2018-05-09 07:04:35.000000 k8s-0.9.0/tests/k8s/test_configmap.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)      311 2018-05-09 07:04:35.000000 k8s-0.9.0/tests/k8s/util.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     7408 2018-05-09 07:04:38.000000 k8s-0.9.0/tests/k8s/test_client.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     1204 2018-05-09 07:04:35.000000 k8s-0.9.0/tests/k8s/conftest.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     5054 2018-05-09 07:04:38.000000 k8s-0.9.0/tests/k8s/test_pod.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     3435 2018-05-09 07:04:35.000000 k8s-0.9.0/tests/k8s/test_ingress.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     3028 2018-05-09 07:04:38.000000 k8s-0.9.0/tests/k8s/test_job.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     2767 2018-05-09 07:04:35.000000 k8s-0.9.0/tests/k8s/test_resourcequota.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     4445 2018-05-09 07:04:38.000000 k8s-0.9.0/tests/k8s/test_model.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)      975 2018-05-09 07:04:35.000000 k8s-0.9.0/tests/k8s/test_base.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     6797 2018-05-09 07:04:38.000000 k8s-0.9.0/tests/k8s/test_service.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     4338 2018-05-09 07:04:38.000000 k8s-0.9.0/tests/k8s/test_fields.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     6187 2018-05-09 07:04:35.000000 k8s-0.9.0/tests/k8s/test_deployer.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     1688 2018-05-09 07:04:35.000000 k8s-0.9.0/README.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      448 2018-05-09 07:04:38.000000 k8s-0.9.0/.prospector.yaml
+drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-05-09 07:05:06.000000 k8s-0.9.0/docs/
+drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-05-09 07:05:06.000000 k8s-0.9.0/docs/source/
+-rw-rw-r--   0 runner    (1003) runner    (1003)     4341 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/tutorial.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)     5424 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/conf.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)      468 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/index.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)     6201 2018-05-09 07:04:38.000000 k8s-0.9.0/docs/source/developer.rst
+drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-05-09 07:05:06.000000 k8s-0.9.0/docs/source/modules/
+-rw-rw-r--   0 runner    (1003) runner    (1003)      126 2018-05-09 07:04:38.000000 k8s-0.9.0/docs/source/modules/k8s.watcher.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      149 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/modules/k8s.models.ingress.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      123 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/modules/k8s.fields.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      158 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/modules/k8s.models.deployment.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      462 2018-05-09 07:04:38.000000 k8s-0.9.0/docs/source/modules/k8s.models.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      155 2018-05-09 07:04:38.000000 k8s-0.9.0/docs/source/modules/k8s.models.configmap.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      158 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/modules/k8s.models.autoscaler.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      192 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/modules/k8s.models.third_party_resource.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      137 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/modules/k8s.models.pod.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      117 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/modules/k8s.base.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      167 2018-05-09 07:04:38.000000 k8s-0.9.0/docs/source/modules/k8s.models.resourcequota.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      196 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/modules/k8s.models.replication_controller.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      123 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/modules/k8s.config.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      210 2018-05-09 07:04:38.000000 k8s-0.9.0/docs/source/modules/k8s.models.custom_resource_definition.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)       66 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/modules/modules.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      123 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/modules/k8s.client.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      149 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/modules/k8s.models.service.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      146 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/source/modules/k8s.models.common.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      265 2018-05-09 07:04:38.000000 k8s-0.9.0/docs/source/modules/k8s.rst
+-rw-rw-r--   0 runner    (1003) runner    (1003)      697 2018-05-09 07:04:35.000000 k8s-0.9.0/docs/Makefile
+-rw-rw-r--   0 runner    (1003) runner    (1003)     2772 2018-05-09 07:04:38.000000 k8s-0.9.0/setup.py
+drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-05-09 07:05:06.000000 k8s-0.9.0/k8s/
+drwxrwxr-x   0 runner    (1003) runner    (1003)        0 2018-05-09 07:05:06.000000 k8s-0.9.0/k8s/models/
+-rw-rw-r--   0 runner    (1003) runner    (1003)      931 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/models/service.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)      923 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/models/pod_disruption_budget.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)      721 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/models/job.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     5364 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/models/pod.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)      485 2018-05-09 07:04:35.000000 k8s-0.9.0/k8s/models/third_party_resource.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)      604 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/models/replication_controller.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     1055 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/models/ingress.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     1689 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/models/custom_resource_definition.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)      822 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/models/common.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)       42 2018-05-09 07:04:35.000000 k8s-0.9.0/k8s/models/__init__.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     1352 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/models/deployment.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)      336 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/models/configmap.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)      758 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/models/resourcequota.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)      820 2018-05-09 07:04:35.000000 k8s-0.9.0/k8s/models/autoscaler.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)      208 2018-05-09 07:04:35.000000 k8s-0.9.0/k8s/config.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     1607 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/watcher.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)       42 2018-05-09 07:04:35.000000 k8s-0.9.0/k8s/__init__.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     8116 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/base.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     4296 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/fields.py
+-rw-rw-r--   0 runner    (1003) runner    (1003)     5110 2018-05-09 07:04:38.000000 k8s-0.9.0/k8s/client.py
```

### Comparing `k8s-0.8.0/.gitignore` & `k8s-0.9.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 
 # Unit test / coverage reports
 htmlcov/
 .tox/
 .coverage
 .coverage.*
 .cache
+.pytest_cache
 nosetests.xml
 coverage.xml
 *,cover
 
 # Created by .ignore support plugin (hsz.mobi)
 ### OSX template
 .DS_Store
```

### Comparing `k8s-0.8.0/bin/test_release.py` & `k8s-0.9.0/bin/test_release.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/bin/release.py` & `k8s-0.9.0/bin/release.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/bin/get_github_release.py` & `k8s-0.9.0/bin/get_github_release.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/LICENSE` & `k8s-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/PKG-INFO` & `k8s-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: k8s
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python client library for the Kubernetes API
 Home-page: https://github.com/fiaas/k8s
 Author: FiaaS developers
 Author-email: fiaas@googlegroups.com
 License: Apache License
 Description-Content-Type: UNKNOWN
 Description: k8s - Python client library for the Kubernetes API
@@ -31,21 +31,21 @@
         .. _tutorial: http://k8s.readthedocs.io/en/latest/tutorial.html
         .. _developer guide: http://k8s.readthedocs.io/en/latest/developer.html
         
         
         Changes since last version
         --------------------------
         
-        * `dfc64d7`_: Remove duplicated test
-        * `f6bca1b`_: Add list_url on all relevant resources
-        * `fc426d9`_: Support list and find on Models across namespaces
-        
-        .. _f6bca1b: https://github.com/fiaas/k8s/commit/f6bca1b
-        .. _fc426d9: https://github.com/fiaas/k8s/commit/fc426d9
-        .. _dfc64d7: https://github.com/fiaas/k8s/commit/dfc64d7
+        * `3bae5d5`_: Handle Field(dict) similar to other types
+        * `32b6e96`_: Add a few more volume types to Pod
+        * `de6d28b`_: Add support for more fields on ObjectMeta, in particular OwnerReference
+        
+        .. _32b6e96: https://github.com/fiaas/k8s/commit/32b6e96
+        .. _3bae5d5: https://github.com/fiaas/k8s/commit/3bae5d5
+        .. _de6d28b: https://github.com/fiaas/k8s/commit/de6d28b
 Keywords: kubernetes fiaas
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `k8s-0.8.0/k8s.egg-info/SOURCES.txt` & `k8s-0.9.0/k8s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/k8s.egg-info/PKG-INFO` & `k8s-0.9.0/k8s.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: k8s
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python client library for the Kubernetes API
 Home-page: https://github.com/fiaas/k8s
 Author: FiaaS developers
 Author-email: fiaas@googlegroups.com
 License: Apache License
 Description-Content-Type: UNKNOWN
 Description: k8s - Python client library for the Kubernetes API
@@ -31,21 +31,21 @@
         .. _tutorial: http://k8s.readthedocs.io/en/latest/tutorial.html
         .. _developer guide: http://k8s.readthedocs.io/en/latest/developer.html
         
         
         Changes since last version
         --------------------------
         
-        * `dfc64d7`_: Remove duplicated test
-        * `f6bca1b`_: Add list_url on all relevant resources
-        * `fc426d9`_: Support list and find on Models across namespaces
-        
-        .. _f6bca1b: https://github.com/fiaas/k8s/commit/f6bca1b
-        .. _fc426d9: https://github.com/fiaas/k8s/commit/fc426d9
-        .. _dfc64d7: https://github.com/fiaas/k8s/commit/dfc64d7
+        * `3bae5d5`_: Handle Field(dict) similar to other types
+        * `32b6e96`_: Add a few more volume types to Pod
+        * `de6d28b`_: Add support for more fields on ObjectMeta, in particular OwnerReference
+        
+        .. _32b6e96: https://github.com/fiaas/k8s/commit/32b6e96
+        .. _3bae5d5: https://github.com/fiaas/k8s/commit/3bae5d5
+        .. _de6d28b: https://github.com/fiaas/k8s/commit/de6d28b
 Keywords: kubernetes fiaas
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `k8s-0.8.0/tests/conftest.py` & `k8s-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/tests/k8s/test_watcher.py` & `k8s-0.9.0/tests/k8s/test_watcher.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/tests/k8s/test_configmap.py` & `k8s-0.9.0/tests/k8s/test_configmap.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/tests/k8s/test_client.py` & `k8s-0.9.0/tests/k8s/test_client.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/tests/k8s/conftest.py` & `k8s-0.9.0/tests/k8s/conftest.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/tests/k8s/test_pod.py` & `k8s-0.9.0/tests/k8s/test_pod.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/tests/k8s/test_ingress.py` & `k8s-0.9.0/tests/k8s/test_ingress.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/tests/k8s/test_job.py` & `k8s-0.9.0/tests/k8s/test_job.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/tests/k8s/test_resourcequota.py` & `k8s-0.9.0/tests/k8s/test_resourcequota.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/tests/k8s/test_base.py` & `k8s-0.9.0/tests/k8s/test_base.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/tests/k8s/test_service.py` & `k8s-0.9.0/tests/k8s/test_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,16 @@
         assert meta.namespace == SERVICE_NAMESPACE
         assert meta.labels == {"label": "value"}
         assert meta.as_dict() == {
             "name": SERVICE_NAME,
             "namespace": SERVICE_NAMESPACE,
             "labels": {
                 "label": "value"
-            }
+            },
+            "ownerReferences": []
         }
 
     def test_service_created_if_not_exists(self, post, api_get):
         api_get.side_effect = NotFound()
         service = create_default_service()
         call_params = service.as_dict()
         assert service._new
@@ -53,15 +54,15 @@
                 "namespace": SERVICE_NAMESPACE,
                 "selfLink": "/api/v1/namespaces/" + SERVICE_NAMESPACE + "/services/my-name",
                 "uid": "cc562581-cbf5-11e5-b6ef-247703d2e388",
                 "resourceVersion": "817",
                 "creationTimestamp": "2016-02-05T10:47:06Z",
                 "labels": {
                     "app": "test"
-                }
+                },
             },
             "spec": {
                 "ports": [
                     {
                         "name": "my-port", "protocol": "TCP", "port": 80, "targetPort": "name"
                     }
                 ],
```

### Comparing `k8s-0.8.0/tests/k8s/test_fields.py` & `k8s-0.9.0/tests/k8s/test_fields.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/tests/k8s/test_deployer.py` & `k8s-0.9.0/tests/k8s/test_deployer.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/README.rst` & `k8s-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/docs/source/tutorial.rst` & `k8s-0.9.0/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/docs/source/conf.py` & `k8s-0.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/docs/source/developer.rst` & `k8s-0.9.0/docs/source/developer.rst`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/docs/Makefile` & `k8s-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/setup.py` & `k8s-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/k8s/models/service.py` & `k8s-0.9.0/k8s/models/service.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/k8s/models/pod_disruption_budget.py` & `k8s-0.9.0/k8s/models/pod_disruption_budget.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/k8s/models/job.py` & `k8s-0.9.0/k8s/models/job.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/k8s/models/pod.py` & `k8s-0.9.0/k8s/models/pod.py`

 * *Files 22% similar despite different names*

```diff
@@ -150,19 +150,47 @@
     defaultMode = Field(int)
 
 
 class EmptyDirVolumeSource(Model):
     medium = Field(six.text_type)
 
 
+class NFSVolumeSource(Model):
+    path = Field(six.text_type)
+    readOnly = Field(bool)
+    server = Field(six.text_type)
+
+
+class HostPathVolumeSource(Model):
+    path = Field(six.text_type)
+
+
+class GCEPersistentDiskVolumeSource(Model):
+    fsType = Field(six.text_type)
+    partition = Field(int)
+    pdName = Field(six.text_type)
+    readOnly = Field(bool)
+
+
+class AWSElasticBlockStoreVolumeSource(Model):
+    fsType = Field(six.text_type)
+    partition = Field(int)
+    readOnly = Field(bool)
+    volumeID = Field(six.text_type)
+
+
 class Volume(Model):
     name = Field(six.text_type)
-    secret = Field(SecretVolumeSource)
+    awsElasticBlockStore = Field(AWSElasticBlockStoreVolumeSource)
     configMap = Field(ConfigMapVolumeSource)
     emptyDir = Field(EmptyDirVolumeSource)
+    gcePersistentDisk = Field(GCEPersistentDiskVolumeSource)
+    hostPath = Field(HostPathVolumeSource)
+    nfs = Field(NFSVolumeSource)
+    secret = Field(SecretVolumeSource)
 
 
 class LocalObjectReference(Model):
     name = Field(six.text_type)
 
 
 class PodSpec(Model):
```

### Comparing `k8s-0.8.0/k8s/models/replication_controller.py` & `k8s-0.9.0/k8s/models/replication_controller.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/k8s/models/ingress.py` & `k8s-0.9.0/k8s/models/ingress.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/k8s/models/custom_resource_definition.py` & `k8s-0.9.0/k8s/models/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/k8s/models/deployment.py` & `k8s-0.9.0/k8s/models/deployment.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/k8s/models/resourcequota.py` & `k8s-0.9.0/k8s/models/resourcequota.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/k8s/models/autoscaler.py` & `k8s-0.9.0/k8s/models/autoscaler.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/k8s/watcher.py` & `k8s-0.9.0/k8s/watcher.py`

 * *Files identical despite different names*

### Comparing `k8s-0.8.0/k8s/base.py` & `k8s-0.9.0/k8s/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,17 +180,18 @@
         d = {}
         for field in self._meta.fields:
             value = field.dump(self)
             if value is not None:
                 d[_api_name(field.name)] = value
         return d
 
-    def update(self, other):
+    def merge(self, other):
         for field in self._meta.fields:
             setattr(self, field.name, getattr(other, field.name))
+    update = merge  # For backwards compatibility
 
     def update_from_dict(self, d):
         for field in self._meta.fields:
             field.load(self, d.get(_api_name(field.name)))
         self._validate_fields()
 
     @classmethod
```

### Comparing `k8s-0.8.0/k8s/fields.py` & `k8s-0.9.0/k8s/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     def __set__(self, instance, new_value):
         current_value = instance._values.get(self.name)
         if new_value == current_value:
             return
         if new_value is not None:
             try:
-                current_value.update(new_value)
+                current_value.merge(new_value)
                 return
             except AttributeError:
                 pass
         instance._values[self.name] = new_value
 
     def __delete__(self, instance):
         del instance._values[self.name]
```

### Comparing `k8s-0.8.0/k8s/client.py` & `k8s-0.9.0/k8s/client.py`

 * *Files identical despite different names*

