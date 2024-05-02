# Comparing `tmp/galaxy-config-24.0.0.tar.gz` & `tmp/galaxy_config-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-config-24.0.0.tar", last modified: Wed Apr  3 02:44:07 2024, max compression
+gzip compressed data, was "galaxy_config-24.0.1.tar", last modified: Thu May  2 13:47:12 2024, max compression
```

## Comparing `galaxy-config-24.0.0.tar` & `galaxy_config-24.0.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:07.306464 galaxy-config-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16193 2024-04-03 02:44:07.306464 galaxy-config-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:07.294464 galaxy-config-24.0.0/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:07.298464 galaxy-config-24.0.0/galaxy/config/
--rw-r--r--   0 runner    (1001) docker     (127)    65685 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20242 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/config_manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:07.302464 galaxy-config-24.0.0/galaxy/config/sample/
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/auth_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/build_sites.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/container_resolvers.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/data_manager_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)   120374 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/datatypes_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/disposable_email_blocklist.conf.sample
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/environment_modules_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/error_report.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/file_sources_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)   133108 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/galaxy.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)    53508 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/job_conf.sample.yml
--rw-r--r--   0 runner    (1001) docker     (127)    79501 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/job_conf.xml.sample_advanced
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/job_conf.xml.sample_basic
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/job_resource_params_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/lmod_modules_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/local_conda_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)    18194 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/object_store_conf.sample.yml
--rw-r--r--   0 runner    (1001) docker     (127)    20644 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/object_store_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/oidc_backends_config.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/oidc_config.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/reports.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/themes_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/tool_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/tool_data_table_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/tool_destinations.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/tool_recommendations_overwrite.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)    17943 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/tool_shed.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/tool_sheds_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/trs_servers_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/user_preferences_extra_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/workflow_resource_mapper_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/workflow_resource_params_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/sample/workflow_schedulers_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:07.302464 galaxy-config-24.0.0/galaxy/config/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)   158390 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/schemas/config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/schemas/job_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/schemas/reports_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (127)    25120 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/schemas/tool_shed_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/config/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:44:07.306464 galaxy-config-24.0.0/galaxy_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16193 2024-04-03 02:44:07.000000 galaxy-config-24.0.0/galaxy_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-03 02:44:07.000000 galaxy-config-24.0.0/galaxy_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:44:07.000000 galaxy-config-24.0.0/galaxy_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 02:44:07.000000 galaxy-config-24.0.0/galaxy_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 02:44:07.000000 galaxy-config-24.0.0/galaxy_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:44:07.000000 galaxy-config-24.0.0/galaxy_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-03 02:44:07.306464 galaxy-config-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 02:43:42.000000 galaxy-config-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:12.629356 galaxy_config-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16004 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17449 2024-05-02 13:47:12.629356 galaxy_config-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:12.617356 galaxy_config-24.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:12.617356 galaxy_config-24.0.1/galaxy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    65685 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20242 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/config_manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:12.625356 galaxy_config-24.0.1/galaxy/config/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/auth_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/build_sites.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/container_resolvers.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/data_manager_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)   121212 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/datatypes_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/disposable_email_blocklist.conf.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/environment_modules_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/error_report.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/file_sources_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)   133915 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/galaxy.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    53508 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/job_conf.sample.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    79501 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/job_conf.xml.sample_advanced
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/job_conf.xml.sample_basic
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/job_resource_params_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/lmod_modules_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/local_conda_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/object_store_conf.sample.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    20971 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/object_store_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/oidc_backends_config.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/oidc_config.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/reports.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/themes_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/tool_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/tool_data_table_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/tool_destinations.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/tool_recommendations_overwrite.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    17943 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/tool_shed.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/tool_sheds_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/trs_servers_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/user_preferences_extra_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/workflow_resource_mapper_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/workflow_resource_params_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/sample/workflow_schedulers_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:12.625356 galaxy_config-24.0.1/galaxy/config/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   158599 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/schemas/config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/schemas/job_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/schemas/reports_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    25120 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/schemas/tool_shed_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/config/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:47:12.629356 galaxy_config-24.0.1/galaxy_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17449 2024-05-02 13:47:12.000000 galaxy_config-24.0.1/galaxy_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-02 13:47:12.000000 galaxy_config-24.0.1/galaxy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:47:12.000000 galaxy_config-24.0.1/galaxy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 13:47:12.000000 galaxy_config-24.0.1/galaxy_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 13:47:12.000000 galaxy_config-24.0.1/galaxy_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:47:12.000000 galaxy_config-24.0.1/galaxy_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-02 13:47:12.629356 galaxy_config-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 13:46:45.000000 galaxy_config-24.0.1/test-requirements.txt
```

### Comparing `galaxy-config-24.0.0/HISTORY.rst` & `galaxy_config-24.0.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,40 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Invenio plugin fixes by `@davelopez <https://github.com/davelopez>`_ in `#17997 <https://github.com/galaxyproject/galaxy/pull/17997>`_
+* clarify the object store relocate functionality by `@martenson <https://github.com/martenson>`_ in `#18033 <https://github.com/galaxyproject/galaxy/pull/18033>`_
+* Updated the datatypes name for FASTK tool by `@SaimMomin12 <https://github.com/SaimMomin12>`_ in `#18053 <https://github.com/galaxyproject/galaxy/pull/18053>`_
+
+============
+Enhancements
+============
+
+* Added 4dn_pairs and 4dn_pairsam datatypes by `@SaimMomin12 <https://github.com/SaimMomin12>`_ in `#17875 <https://github.com/galaxyproject/galaxy/pull/17875>`_
+* Add middleware for logging start and end of request by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18046 <https://github.com/galaxyproject/galaxy/pull/18046>`_
+
+=============
+Other changes
+=============
+
+* Rebuild config samples by `@davelopez <https://github.com/davelopez>`_ in `#17911 <https://github.com/galaxyproject/galaxy/pull/17911>`_
+* Backport colabfold tar file datatype by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18029 <https://github.com/galaxyproject/galaxy/pull/18029>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-config-24.0.0/LICENSE` & `galaxy_config-24.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/PKG-INFO` & `galaxy_config-24.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-config
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy configuration
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -47,14 +47,41 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Invenio plugin fixes by `@davelopez <https://github.com/davelopez>`_ in `#17997 <https://github.com/galaxyproject/galaxy/pull/17997>`_
+* clarify the object store relocate functionality by `@martenson <https://github.com/martenson>`_ in `#18033 <https://github.com/galaxyproject/galaxy/pull/18033>`_
+* Updated the datatypes name for FASTK tool by `@SaimMomin12 <https://github.com/SaimMomin12>`_ in `#18053 <https://github.com/galaxyproject/galaxy/pull/18053>`_
+
+============
+Enhancements
+============
+
+* Added 4dn_pairs and 4dn_pairsam datatypes by `@SaimMomin12 <https://github.com/SaimMomin12>`_ in `#17875 <https://github.com/galaxyproject/galaxy/pull/17875>`_
+* Add middleware for logging start and end of request by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18046 <https://github.com/galaxyproject/galaxy/pull/18046>`_
+
+=============
+Other changes
+=============
+
+* Rebuild config samples by `@davelopez <https://github.com/davelopez>`_ in `#17911 <https://github.com/galaxyproject/galaxy/pull/17911>`_
+* Backport colabfold tar file datatype by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18029 <https://github.com/galaxyproject/galaxy/pull/18029>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-config-24.0.0/galaxy/config/__init__.py` & `galaxy_config-24.0.1/galaxy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/config_manage.py` & `galaxy_config-24.0.1/galaxy/config/config_manage.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/auth_conf.xml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/auth_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/build_sites.yml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/build_sites.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/container_resolvers.yml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/container_resolvers.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/datatypes_conf.xml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/datatypes_conf.xml.sample`

 * *Files 0% similar despite different names*

#### Comparing `galaxy-config-24.0.0/galaxy/config/sample/datatypes_conf.xml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/datatypes_conf.xml.sample`

```diff
@@ -206,17 +206,17 @@
       <!-- <display file="ucsc/interval_as_bed.xml" inherit="true" /> -->
       <display file="ensembl/ensembl_interval_as_bed.xml" inherit="true"/>
       <display file="gbrowse/gbrowse_interval_as_bed.xml" inherit="true"/>
       <display file="rviewer/bed.xml" inherit="true"/>
       <display file="igv/interval_as_bed.xml" inherit="true"/>
     </datatype>
     <datatype extension="jellyfish" type="galaxy.datatypes.binary:Binary" subclass="true" display_in_upload="true" description="Jellyfish database files are k-mer counts in binary format with a readable head. They are operated on and converted to human-readable text through jellyfish commands."/>
-    <datatype extension="ktab" type="galaxy.datatypes.binary:Binary" subclass="true" description="A table of canonical k‑mers and their counts for the fastk toolkit." display_in_upload="true" description_url="https://github.com/thegenemyers/FASTK?tab=readme-ov-file#file-encodings"/>
-    <datatype extension="hist" type="galaxy.datatypes.binary:Binary" subclass="true" description="A binary histogram file of kmers and frequencies for the fastk toolkit." display_in_upload="true" description_url="https://github.com/thegenemyers/FASTK?tab=readme-ov-file#file-encodings"/>
-    <datatype extension="prof" type="galaxy.datatypes.binary:Binary" subclass="true" description="Read profile file for the fastk toolkit." display_in_upload="true" description_url="https://github.com/thegenemyers/FASTK?tab=readme-ov-file#file-encodings"/>
+    <datatype extension="fastk_ktab" type="galaxy.datatypes.binary:Binary" subclass="true" description="A table of canonical k‑mers and their counts for the fastk toolkit." display_in_upload="true" description_url="https://github.com/thegenemyers/FASTK?tab=readme-ov-file#file-encodings"/>
+    <datatype extension="fastk_hist" type="galaxy.datatypes.binary:Binary" subclass="true" description="A binary histogram file of kmers and frequencies for the fastk toolkit." display_in_upload="true" description_url="https://github.com/thegenemyers/FASTK?tab=readme-ov-file#file-encodings"/>
+    <datatype extension="fastk_prof" type="galaxy.datatypes.binary:Binary" subclass="true" description="Read profile file for the fastk toolkit." display_in_upload="true" description_url="https://github.com/thegenemyers/FASTK?tab=readme-ov-file#file-encodings"/>
     <datatype extension="npy" type="galaxy.datatypes.binary:Numpy" description="Standard format for saving numpy arrays" display_in_upload="true" description_url="https://numpy.org/devdocs/reference/generated/numpy.lib.format.html"/>
     <!-- ISA data types -->
     <datatype extension="isa-tab" type="galaxy.datatypes.isa:IsaTab" mimetype="application/isa-tools" display_in_upload="true" description="ISA-Tab data type." description_url="https://isa-tools.org"/>
     <datatype extension="isa-json" type="galaxy.datatypes.isa:IsaJson" mimetype="application/isa-tools" display_in_upload="true" description="ISA-JSON data type." description_url="https://isa-tools.org"/>
     <datatype extension="picard_interval_list" type="galaxy.datatypes.tabular:Tabular" subclass="true" display_in_upload="true">
       <converter file="picard_interval_list_to_bed6_converter.xml" target_datatype="bed6"/>
     </datatype>
@@ -363,14 +363,15 @@
     <datatype extension="gii" auto_compressed_types="gz" type="galaxy.datatypes.images:Gifti" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="tck" type="galaxy.datatypes.images:Tck" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="trk" type="galaxy.datatypes.images:Trk" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="mrc" type="galaxy.datatypes.images:Mrc2014" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="star" type="galaxy.datatypes.images:Star" display_in_upload="true"/>
     <datatype extension="peff" type="galaxy.datatypes.proteomics:PEFF" display_in_upload="true"/>
     <datatype extension="toml" type="galaxy.datatypes.data:Text" subclass="true" display_in_upload="true"/>
+    <datatype extension="colab.tar" auto_compressed_types="gz" type="galaxy.datatypes.binary:CompressedArchive" subclass="true" display_in_upload="true"/>
     <!-- End Proteomics Datatypes -->
     <!-- FlowCytometry -->
     <datatype extension="fcs" type="galaxy.datatypes.flow:FCS" mimetype="application/octet-stream" display_in_upload="true" description="A FCS binary sequence file with a '.fcs' file extension."/>
     <datatype extension="flowtext" type="galaxy.datatypes.tabular:Tabular" subclass="true" mimetype="text/tab-separated-values" display_in_upload="true" description="A Flow text file with a '.flowtext' file extension."/>
     <datatype extension="flowclr" type="galaxy.datatypes.tabular:Tabular" subclass="true" mimetype="text/tab-separated-values" display_in_upload="true" description="A Flow text file containing population information with a '.flowclr' file extension."/>
     <datatype extension="flowmfi" type="galaxy.datatypes.tabular:Tabular" subclass="true" mimetype="text/tab-separated-values" display_in_upload="true" description="A Flow MFI file with a '.flowmfi' file extension."/>
     <datatype extension="flowstat1" type="galaxy.datatypes.tabular:Tabular" subclass="true" mimetype="text/tab-separated-values" display_in_upload="true" description="A Flow Stats file with a '.flowstat1' file extension."/>
@@ -402,14 +403,16 @@
     <datatype extension="mtx" type="galaxy.datatypes.tabular:MatrixMarket" display_in_upload="true"/>
     <datatype extension="cmap" type="galaxy.datatypes.tabular:CMAP" display_in_upload="true" description="The Bionano Genomics cmap format provides location information for label sites within a genome map or an in silico digestion of a reference or sequence data. A CMAP file contains two sections, header and the map information block" description_url="https://bionanogenomics.com/wp-content/uploads/2017/03/30039-CMAP-File-Format-Specification-Sheet.pdf"/>
     <datatype extension="encodepeak" type="galaxy.datatypes.interval:ENCODEPeak" display_in_upload="true">
       <converter file="interval_to_tabix_converter.xml" target_datatype="tabix" depends_on="bgzip"/>
       <converter file="interval_to_bgzip_converter.xml" target_datatype="bgzip"/>
       <converter file="bed_gff_or_vcf_to_bigwig_converter.xml" target_datatype="bigwig"/>
     </datatype>
+    <datatype extension="4dn_pairs" type="galaxy.datatypes.tabular:Tabular" subclass="true" display_in_upload="true" description="The pairs format is a standard text format for pairs of genomic loci given as 1bp point positions" description_url="https://github.com/4dn-dcic/pairix/blob/master/pairs_format_specification.md#pairs-file"/>
+    <datatype extension="4dn_pairsam" type="galaxy.datatypes.tabular:Tabular" subclass="true" display_in_upload="true" description="A simple tabular format to store the information on ligation junctions detected in sequences from Hi-C experiments." description_url="https://pairsamtools.readthedocs.io/en/latest/pairsam.html"/>
     <datatype extension="pdf" type="galaxy.datatypes.images:Pdf" mimetype="application/pdf" display_in_upload="true"/>
     <datatype extension="pileup" type="galaxy.datatypes.tabular:Pileup" display_in_upload="true">
       <converter file="interval_to_bgzip_converter.xml" target_datatype="bgzip"/>
       <converter file="interval_to_tabix_converter.xml" target_datatype="tabix" depends_on="bgzip"/>
     </datatype>
     <datatype extension="psl" type="galaxy.datatypes.tabular:Psl" display_in_upload="true"/>
     <datatype extension="obo" type="galaxy.datatypes.text:Obo" mimetype="text/html" display_in_upload="true"/>
```

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/environment_modules_mapping.yml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/environment_modules_mapping.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/error_report.yml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/error_report.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/file_sources_conf.yml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/file_sources_conf.yml.sample`

 * *Files 6% similar despite different names*

```diff
@@ -198,18 +198,22 @@
 
 - type: drs
   label: Stock DRS filesource
   id: drsstock
   doc: Make sure to define this generic drs file source if you have defined any other drs file sources, or stock drs download capability will be disabled.
 
 - type: inveniordm
-  id: invenio
-  doc: Invenio RDM turn-key research data management repository
-  label: Invenio RDM Demo Repository
+  id: invenio_sandbox
+  doc: This is the Sandbox instance of Invenio. It is used for testing purposes only, content is NOT preserved. DOIs created in this instance are not real and will not resolve.
+  label: Invenio RDM Sandbox Repository (TESTING ONLY)
   url: https://inveniordm.web.cern.ch/
+  token: ${user.user_vault.read_secret('preferences/invenio_sandbox/token')}
+  # token: ${user.preferences['invenio_sandbox|token']} # Alternatively use this for retrieving the token from user preferences instead of the Vault
+  public_name: ${user.preferences['invenio_sandbox|public_name']}
+  writable: true
 
 - type: onedata
   id: onedata1
   label: Onedata
   doc: Your Onedata files - configure an access token via user preferences
   accessToken: ${user.preferences['onedata|access_token']}
   onezoneDomain: ${user.preferences['onedata|onezone_domain']}
```

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/galaxy.yml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/galaxy.yml.sample`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Galaxy is configured by default to be usable in a single-user development
 # environment.  To tune the application for a multi-user production
 # environment, see the documentation at:
-#
+# 
 #  https://docs.galaxyproject.org/en/master/admin/production.html
-#
+# 
 # Throughout this sample configuration file, except where stated otherwise,
 # uncommented values override the default if left unset, whereas commented
 # values are set to the default value.  Relative paths are relative to the root
 # Galaxy directory.
-#
+# 
 # Examples of many of these options are explained in more detail in the Galaxy
 # Community Hub.
-#
+# 
 #   https://galaxyproject.org/admin/config
-#
+# 
 # Config hackers are encouraged to check there before asking for help.
-#
+# 
 # Configuration for Gravity process manager.
 # ``uwsgi:`` section will be ignored if Galaxy is started via Gravity commands (e.g ``./run.sh``, ``galaxy`` or ``galaxyctl``).
 gravity:
 
   # Process manager to use.
   # ``supervisor`` is the default process manager when Gravity is invoked as a non-root user.
   # ``systemd`` is the default when Gravity is invoked as root.
@@ -177,15 +177,15 @@
   # Configuration for gx-it-proxy.
   gx_it_proxy:
 
     # Set to true to start gx-it-proxy
     # enable: false
 
     # gx-it-proxy version
-    # version: '>=0.0.5'
+    # version: '>=0.0.6'
 
     # Public-facing IP of the proxy
     # ip: localhost
 
     # Public-facing port of the proxy
     # port: 4002
 
@@ -244,14 +244,22 @@
     # Port to bind the tusd server to
     # port: 1080
 
     # Directory to store uploads in.
     # Must match ``tus_upload_store`` setting in ``galaxy:`` section.
     # upload_dir:
 
+    # Value of tusd -hooks-httpd option
+    #
+    # the default of is suitable for using tusd for Galaxy uploads and should not be changed unless you are using tusd for
+    # other purposes such as Pulsar staging.
+    #
+    # The value of galaxy_infrastructure_url is automatically prepended if the option starts with a `/`
+    # hooks_http: /api/upload/hooks
+
     # Comma-separated string of enabled tusd hooks.
     #
     # Leave at the default value to require authorization at upload creation time.
     # This means Galaxy's web process does not need to be running after creating the initial
     # upload request.
     #
     # Set to empty string to disable all authorization. This means data can be uploaded (but not processed)
@@ -329,23 +337,17 @@
     # ``supervisor``.
     # memory_limit:
 
     # Extra environment variables and their values to set when running the service. A dictionary where keys are the variable
     # names.
     # environment: {}
 
-  # Configure dynamic handlers in this section. Below is a simple example
+  # Configure dynamic handlers in this section.
   # See https://docs.galaxyproject.org/en/latest/admin/scaling.html#dynamically-defined-handlers for details.
-  #handlers:
-  #  handler:
-  #    processes: 3
-  #    pools:
-  #      - job-handlers
-  #      - workflow-schedulers
-
+  # handlers: {}
 galaxy:
 
   # The directory that will be prepended to relative paths in options
   # specifying other Galaxy config files (e.g. datatypes_config_file).
   # Defaults to the directory in which galaxy.yml is located.
   #config_dir: null
 
@@ -1026,15 +1028,15 @@
   #object_store_config_file: object_store_conf.xml
 
   # Rather than specifying an object_store_config_file, the object store
   # configuration can be embedded into Galaxy's config with this option.
   # This option has no effect if the file specified by
   # object_store_config_file exists. Otherwise, if this option is set,
   # it overrides any other objectstore settings.
-  # The syntax, available instrumenters, and documentation of their
+  # The syntax, available storage plugins, and documentation of their
   # options is explained in detail in the object store sample
   # configuration file, `object_store_conf.sample.yml`
   #object_store_config: null
 
   # Specify where cache monitoring is driven for caching object stores
   # such as S3, Azure, and iRODS. This option has no affect on disk
   # object stores. For production instances, the cache should be
@@ -1063,14 +1065,21 @@
   # <cache_dir>.
   #object_store_cache_path: object_store_cache
 
   # Default cache size for caching object stores if cache not configured
   # for that object store entry.
   #object_store_cache_size: -1
 
+  # Set this to true to indicate in the UI that a user's object store
+  # selection isn't simply a "preference" that job destinations often
+  # respect but in fact will always be respected. This should be set to
+  # true to simplify the UI as long as job destinations never override
+  # 'object_store_id's for a jobs.
+  #object_store_always_respect_user_selection: false
+
   # What Dataset attribute is used to reference files in an ObjectStore
   # implementation, this can be 'uuid' or 'id'. The default will depend
   # on how the object store is configured, starting with 20.05 Galaxy
   # will try to default to 'uuid' if it can be sure this is a new Galaxy
   # instance - but the default will be 'id' in many cases. In
   # particular, if the name of the directory set in <file_path> is
   # `objects`, the default will be set to 'uuid', otherwise it will be
@@ -1300,17 +1309,14 @@
   # subdomain. Defaults to "/".
   #interactivetools_base_path: /
 
   # Map for interactivetool proxy.
   # The value of this option will be resolved with respect to
   # <data_dir>.
   #interactivetools_map: interactivetools_map.sqlite
-  # Note: the following config should still be used due to lack of
-  # support of data_dir resolution in gx-it-proxy and gravity:
-  #interactivetools_map: database/interactivetools_map.sqlite
 
   # Prefix to use in the formation of the subdomain or path for
   # interactive tools
   #interactivetools_prefix: interactivetool
 
   # Galaxy Interactive Tools (GxITs) can be stopped from within the
   # Galaxy interface, killing the GxIT job without completing its
@@ -1543,18 +1549,23 @@
   # Galaxy can also use nginx_upload_module to receive files staged out
   # upon job completion by remote job runners (i.e. Pulsar) that
   # initiate staging operations on the remote end.  See the Galaxy nginx
   # documentation for the corresponding nginx configuration.
   #nginx_upload_job_files_path: null
 
   # The upload store is a temporary directory in which files uploaded by
-  # the tus middleware or server will be placed. Defaults to
-  # new_file_path if not set.
+  # the tus middleware or server for user uploads will be placed.
+  # Defaults to new_file_path if not set.
   #tus_upload_store: null
 
+  # The upload store is a temporary directory in which files uploaded by
+  # the tus middleware or server for remote job files (Pulsar) will be
+  # placed. Defaults to tus_upload_store if not set.
+  #tus_upload_store_job_files: null
+
   # Galaxy can upload user files in chunks without using nginx. Enable
   # the chunk uploader by specifying a chunk size larger than 0. The
   # chunk size is specified in bytes (default: 10MB).
   #chunk_upload_size: 10485760
 
   # Have Galaxy manage dynamic proxy component for routing requests to
   # other services based on Galaxy's session cookie.  It will attempt to
@@ -1728,14 +1739,18 @@
   # Debug enables access to various config options useful for
   # development and debugging: use_lint, use_profile, and
   # use_printdebug.  It also causes the files used by PBS/SGE
   # (submission script, output, and error) to remain on disk after the
   # job is complete.
   #debug: false
 
+  # Log request start as well as request end. Disables uvicorn access
+  # log handler.
+  #use_access_logging_middleware: false
+
   # Check for WSGI compliance.
   #use_lint: false
 
   # Run the Python profiler on each request.
   #use_profile: false
 
   # Intercept print statements and show them on the returned page.
@@ -2185,20 +2200,21 @@
   #oidc_config_file: oidc_config.xml
 
   # Sets the path to OIDC backends configuration file.
   # The value of this option will be resolved with respect to
   # <config_dir>.
   #oidc_backends_config_file: oidc_backends_config.xml
 
-  # Sets the prefix for OIDC scopes specific to this Galaxy instance.
-  # If an API call is made against this Galaxy instance using an OIDC bearer token,
-  # any scopes must be prefixed with this value e.g. https://galaxyproject.org/api.
-  # More concretely, to request all permissions that the user has, the scope
-  # would have to be specified as "<prefix>:*". e.g "https://galaxyproject.org/api:*".
-  # Currently, only * is recognised as a valid scope, and future iterations may
+  # Sets the prefix for OIDC scopes specific to this Galaxy instance. If
+  # an API call is made against this Galaxy instance using an OIDC
+  # bearer token, any scopes must be prefixed with this value e.g.
+  # https://galaxyproject.org/api. More concretely, to request all
+  # permissions that the user has, the scope would have to be specified
+  # as "<prefix>:*". e.g "https://galaxyproject.org/api:*". Currently,
+  # only * is recognised as a valid scope, and future iterations may
   # provide more fine-grained scopes.
   #oidc_scope_prefix: https://galaxyproject.org/api
 
   # XML config file that allows the use of different authentication
   # providers (e.g. LDAP) instead or in addition to local authentication
   # (.sample is used if default does not exist).
   # The value of this option will be resolved with respect to
@@ -2893,7 +2909,8 @@
   # The URL pointing to the Galaxy Help Forum API base URL. The API must
   # be compatible with Discourse API (https://docs.discourse.org/).
   #help_forum_api_url: https://help.galaxyproject.org/
 
   # Enable the integration of the Galaxy Help Forum in the tool panel.
   # This requires the help_forum_api_url to be set.
   #enable_help_forum_tool_panel_integration: false
+
```

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/job_conf.sample.yml` & `galaxy_config-24.0.1/galaxy/config/sample/job_conf.sample.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/job_conf.xml.sample_advanced` & `galaxy_config-24.0.1/galaxy/config/sample/job_conf.xml.sample_advanced`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/job_resource_params_conf.xml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/job_resource_params_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/lmod_modules_mapping.yml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/lmod_modules_mapping.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/object_store_conf.sample.yml` & `galaxy_config-24.0.1/galaxy/config/sample/object_store_conf.sample.yml`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     store_by: id
     files_dir: /old-fs/galaxy/files
 
 #
 # Sample Distributed Object Store with disk backends configuration
 #
 
-# In the distributed object store, existing dataests will be located by the `object_store_id` column in the `dataset`
+# In the distributed object store, existing datasets will be located by the `object_store_id` column in the `dataset`
 # table of the Galaxy database, which corresponds to the `id` option on the backend. New datasets are created based on
 # the `weight` option: a backend with weight "2" has twice the chance of being (randomly) selected for new datasets as a
 # backend with weight "1". A weight of "0" will still allow datasets in that backend to be read, but no new datasets
 # will be written to that backend.
 #
 # In distributed and hierarchical configurations, you can choose that some backends are automatically unused whenever
 # they become too full. Setting the `global_max_percent_full` option on the top level backends config enables this, or
@@ -295,28 +295,33 @@
 # with user-private storage a larger quota and warns the user the disk is routinely cleaned. Relative speed and
 # stability differences are communicated to the user using object store badges - as well as how data is backed up (in
 # the default case) and not backed up for scratch storage.
 #
 # The admin is responsible for routinely cleaning that storage using Galaxy's admin scripts - this object store
 # configuration just allows the user selection and communicates expectations to the user. Training related to Galaxy
 # cleanup scripts can be found in the Galaxy Training Network:
-# 
+#
 # Slides: https://gxy.io/GTN:S00103
 # Tutorial: https://gxy.io/GTN:T00324
 #
 # In this example, the scratch storage is marked as user-private by setting the `private` option to "true" on the
-# backend definition. This means it cannot be used in public datasets, shared between users, etc.. This is more example
+# backend definition. This means it cannot be used in public datasets, shared between users, etc.. This is for example
 # purposes - you may very well not want scratch storage to be defined as private as it prevents a lot of regular
 # functionality and Galaxy handles regularly cleaned datasets fairly gracefully when the appropriate admin scripts are
 # used.
+#
+# It is safe to just relabel the object store that a dataset belongs to if the underlying paths mapped to by the object
+# stores are the same and the dataset has not been copied. To enable users to relocate datasets this way set the
+# backends' `device` property to the same value.
 
 type: distributed
 backends:
   - id: default
     type: disk
+    device: device1
     weight: 1
     allow_selection: true
     name: Default Galaxy Storage
     description: >
       This is Galaxy's default object store - this disk space is regularly backed up and all users have a default quota
       of 200 GB.
     files_dir: database/objects/default
@@ -325,14 +330,15 @@
       - type: more_stable
       - type: backed_up
         message: >
           Backed up to Galaxy's institutional long term tape drive nightly. More information about our tape drive can be
           found on our [Archive Tier Storage](https://www.msi.umn.edu/content/archive-tier-storage) page.
   - id: scratch
     type: disk
+    device: device2
     weight: 0
     allow_selection: true
     private: true
     name: Scratch Storage
     description: >
       This object store is connected to institutional scratch storage. This disk space is not backed up and private to
       your user, and datasets belonging to this storage will be automatically deleted after one month.
```

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/object_store_conf.xml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/object_store_conf.xml.sample`

 * *Files 1% similar despite different names*

#### Comparing `galaxy-config-24.0.0/galaxy/config/sample/object_store_conf.xml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/object_store_conf.xml.sample`

```diff
@@ -54,15 +54,15 @@
         </backend>
     </backends>
 </object_store>
 -->
 <!--
     Sample Distributed Object Store with disk backends
 
-    In the distributed object store, existing dataests will be located by the
+    In the distributed object store, existing datasets will be located by the
     `object_store_id` column in the `dataset` table of the Galaxy database,
     which corresponds to the `id` attribute on the backend tag. New datasets are
     created based on the "weight" attribute: a backend with weight "2" has a
     twice the chance of being (randomly) selected for new datasets as a backend
     with weight "1". A weight of "0" will still allow datasets in that backend
     to be read, but no new datasets will be written to that backend.
 
@@ -254,29 +254,34 @@
     using the private="true" attribute on the backend definition.
     This means it cannot be used in public datasets, shared between
     users, etc.. This is more example purposes - you may very well not
     want scratch storage to be defined as private as it prevents a lot
     of regular functionality and Galaxy handles regularly cleaned
     datasets fairly gracefully when the appropriate admin scripts
     are used.
+
+    It is safe to just relabel the object store that a dataset belongs
+    to if the underlying paths mapped to by the object stores are the
+    same and the dataset has not been copied. To enable users to relocate
+    datasets this way set the backends' `device` property to the same value.
 -->
 <!--
 <object_store type="distributed">
     <backends>
-        <backend id="default" allow_selection="true" type="disk" weight="1" name="Default Galaxy Storage">
+        <backend id="default" allow_selection="true" type="disk" device="device1" weight="1" name="Default Galaxy Storage">
             <description>This is Galaxy's default object store - this disk is regularly backed up and all user's have a default quota of 200 GB.
             </description>
             <files_dir path="database/objects/deafult"/>
             <badges>
                 <slower />
                 <more_stable />
                 <backed_up>Backed up to Galaxy's institutional long term tape drive nightly. More information about our tape drive can be found on our [Archive Tier Storage](https://www.msi.umn.edu/content/archive-tier-storage) page.</backed_up>
             </badges>
         </backend>
-        <backend id="scratch" allow_selection="true" type="disk" weight="0" name="Scratch Storage" private="true">
+        <backend id="scratch" allow_selection="true" type="disk" device="device2" weight="0" name="Scratch Storage" private="true">
             <quota source="second_tier" />
             <description>This object store is connected to institutional scratch storage. This disk is not backed up and private to your user and datasets belonging to this storage will be automatically deleted after one month.
 </description>
             <files_dir path="database/objects/temp"/>
             <badges>
                 <faster />
                 <less_stable />
```

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/oidc_backends_config.xml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/oidc_backends_config.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/oidc_config.xml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/oidc_config.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/reports.yml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/reports.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/themes_conf.yml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/themes_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/tool_conf.xml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/tool_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/tool_data_table_conf.xml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/tool_data_table_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/tool_destinations.yml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/tool_destinations.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/tool_recommendations_overwrite.yml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/tool_recommendations_overwrite.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/tool_shed.yml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/tool_shed.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/trs_servers_conf.yml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/trs_servers_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/user_preferences_extra_conf.yml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/user_preferences_extra_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/workflow_resource_params_conf.xml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/workflow_resource_params_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/sample/workflow_schedulers_conf.xml.sample` & `galaxy_config-24.0.1/galaxy/config/sample/workflow_schedulers_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/schema.py` & `galaxy_config-24.0.1/galaxy/config/schema.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/schemas/config_schema.yml` & `galaxy_config-24.0.1/galaxy/config/schemas/config_schema.yml`

 * *Files 0% similar despite different names*

```diff
@@ -2189,14 +2189,21 @@
         required: false
         desc: |
           Debug enables access to various config options useful for development
           and debugging: use_lint, use_profile, and use_printdebug.  It also
           causes the files used by PBS/SGE (submission script, output, and error)
           to remain on disk after the job is complete.
 
+      use_access_logging_middleware:
+        type: bool
+        default: false
+        required: false
+        desc: |
+          Log request start as well as request end. Disables uvicorn access log handler.
+
       use_lint:
         type: bool
         default: false
         required: false
         desc: |
           Check for WSGI compliance.
```

### Comparing `galaxy-config-24.0.0/galaxy/config/schemas/job_config_schema.yml` & `galaxy_config-24.0.1/galaxy/config/schemas/job_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/schemas/reports_config_schema.yml` & `galaxy_config-24.0.1/galaxy/config/schemas/reports_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/schemas/tool_shed_config_schema.yml` & `galaxy_config-24.0.1/galaxy/config/schemas/tool_shed_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/script.py` & `galaxy_config-24.0.1/galaxy/config/script.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy/config/templates.py` & `galaxy_config-24.0.1/galaxy/config/templates.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/galaxy_config.egg-info/PKG-INFO` & `galaxy_config-24.0.1/galaxy_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-config
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy configuration
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -47,14 +47,41 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Invenio plugin fixes by `@davelopez <https://github.com/davelopez>`_ in `#17997 <https://github.com/galaxyproject/galaxy/pull/17997>`_
+* clarify the object store relocate functionality by `@martenson <https://github.com/martenson>`_ in `#18033 <https://github.com/galaxyproject/galaxy/pull/18033>`_
+* Updated the datatypes name for FASTK tool by `@SaimMomin12 <https://github.com/SaimMomin12>`_ in `#18053 <https://github.com/galaxyproject/galaxy/pull/18053>`_
+
+============
+Enhancements
+============
+
+* Added 4dn_pairs and 4dn_pairsam datatypes by `@SaimMomin12 <https://github.com/SaimMomin12>`_ in `#17875 <https://github.com/galaxyproject/galaxy/pull/17875>`_
+* Add middleware for logging start and end of request by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18046 <https://github.com/galaxyproject/galaxy/pull/18046>`_
+
+=============
+Other changes
+=============
+
+* Rebuild config samples by `@davelopez <https://github.com/davelopez>`_ in `#17911 <https://github.com/galaxyproject/galaxy/pull/17911>`_
+* Backport colabfold tar file datatype by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18029 <https://github.com/galaxyproject/galaxy/pull/18029>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-config-24.0.0/galaxy_config.egg-info/SOURCES.txt` & `galaxy_config-24.0.1/galaxy_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-config-24.0.0/setup.cfg` & `galaxy_config-24.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-config
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	boltons
 	jinja2
```

