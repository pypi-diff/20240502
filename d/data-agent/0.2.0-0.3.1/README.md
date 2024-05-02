# Comparing `tmp/data-agent-0.2.0.tar.gz` & `tmp/data_agent-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-agent-0.2.0.tar", last modified: Tue Nov 28 17:57:40 2023, max compression
+gzip compressed data, was "data_agent-0.3.1.tar", last modified: Thu May  2 20:58:47 2024, max compression
```

## Comparing `data-agent-0.2.0.tar` & `data_agent-0.3.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.923679 data-agent-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-11-28 17:57:10.000000 data-agent-0.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.907679 data-agent-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.911679 data-agent-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2023-11-28 17:57:10.000000 data-agent-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-11-28 17:57:10.000000 data-agent-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-28 17:57:10.000000 data-agent-0.2.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2023-11-28 17:57:10.000000 data-agent-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-11-28 17:57:10.000000 data-agent-0.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-28 17:57:10.000000 data-agent-0.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-28 17:57:10.000000 data-agent-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13516 2023-11-28 17:57:10.000000 data-agent-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-11-28 17:57:10.000000 data-agent-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2023-11-28 17:57:40.923679 data-agent-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2023-11-28 17:57:10.000000 data-agent-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.915679 data-agent-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-11-28 17:57:10.000000 data-agent-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.915679 data-agent-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-28 17:57:10.000000 data-agent-0.2.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-28 17:57:10.000000 data-agent-0.2.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-28 17:57:10.000000 data-agent-0.2.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10041 2023-11-28 17:57:10.000000 data-agent-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-28 17:57:10.000000 data-agent-0.2.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-11-28 17:57:10.000000 data-agent-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-11-28 17:57:10.000000 data-agent-0.2.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-28 17:57:10.000000 data-agent-0.2.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-11-28 17:57:10.000000 data-agent-0.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-11-28 17:57:10.000000 data-agent-0.2.0/docs/windows-service.md
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-11-28 17:57:10.000000 data-agent-0.2.0/make-runtime.bat
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-11-28 17:57:10.000000 data-agent-0.2.0/make-service.bat
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-11-28 17:57:10.000000 data-agent-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-11-28 17:57:40.923679 data-agent-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-11-28 17:57:10.000000 data-agent-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.907679 data-agent-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.915679 data-agent-0.2.0/src/data_agent/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/abstract_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/broker_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/broker_agent_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/cli_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/config_persist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6500 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/config_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/connection_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.919679 data-agent-0.2.0/src/data_agent/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/connectors/fake_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7710 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/daq_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/exchanger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/groups_aware_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.919679 data-agent-0.2.0/src/data_agent/linux/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/linux/config_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/local_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/safe_manipulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.919679 data-agent-0.2.0/src/data_agent/win32/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/win32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/win32/config_default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.919679 data-agent-0.2.0/src/data_agent/win32/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/win32/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/win32/hooks/hook-data_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/win32/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/win32/win_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2023-11-28 17:57:10.000000 data-agent-0.2.0/src/data_agent/win32/win_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.923679 data-agent-0.2.0/src/data_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2023-11-28 17:57:40.000000 data-agent-0.2.0/src/data_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2023-11-28 17:57:40.000000 data-agent-0.2.0/src/data_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 17:57:40.000000 data-agent-0.2.0/src/data_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-11-28 17:57:40.000000 data-agent-0.2.0/src/data_agent.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 17:57:40.000000 data-agent-0.2.0/src/data_agent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-11-28 17:57:40.000000 data-agent-0.2.0/src/data_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-28 17:57:40.000000 data-agent-0.2.0/src/data_agent.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.919679 data-agent-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2023-11-28 17:57:10.000000 data-agent-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.907679 data-agent-0.2.0/tests/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.907679 data-agent-0.2.0/tests/docker/rabbitmq/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:57:40.923679 data-agent-0.2.0/tests/docker/rabbitmq/etc/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-11-28 17:57:10.000000 data-agent-0.2.0/tests/docker/rabbitmq/etc/definitions.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-28 17:57:10.000000 data-agent-0.2.0/tests/docker/rabbitmq/etc/enabled_plugins
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-11-28 17:57:10.000000 data-agent-0.2.0/tests/docker/rabbitmq/etc/rabbitmq.conf
--rw-r--r--   0 runner    (1001) docker     (127)      467 2023-11-28 17:57:10.000000 data-agent-0.2.0/tests/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2023-11-28 17:57:10.000000 data-agent-0.2.0/tests/test_api_config_provision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2023-11-28 17:57:10.000000 data-agent-0.2.0/tests/test_api_daq_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2023-11-28 17:57:10.000000 data-agent-0.2.0/tests/test_api_safe_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6910 2023-11-28 17:57:10.000000 data-agent-0.2.0/tests/test_api_target_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8494 2023-11-28 17:57:10.000000 data-agent-0.2.0/tests/test_connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10342 2023-11-28 17:57:10.000000 data-agent-0.2.0/tests/test_daq_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2023-11-28 17:57:10.000000 data-agent-0.2.0/tests/test_fake_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2023-11-28 17:57:10.000000 data-agent-0.2.0/tests/test_safe_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2023-11-28 17:57:10.000000 data-agent-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.882989 data_agent-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-02 20:58:15.000000 data_agent-0.3.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.866989 data_agent-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.870989 data_agent-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-02 20:58:15.000000 data_agent-0.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-02 20:58:15.000000 data_agent-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 20:58:15.000000 data_agent-0.3.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-02 20:58:15.000000 data_agent-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 20:58:15.000000 data_agent-0.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 20:58:15.000000 data_agent-0.3.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 20:58:15.000000 data_agent-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-05-02 20:58:15.000000 data_agent-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-02 20:58:15.000000 data_agent-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-02 20:58:47.882989 data_agent-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-02 20:58:15.000000 data_agent-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.870989 data_agent-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-02 20:58:15.000000 data_agent-0.3.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.870989 data_agent-0.3.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 20:58:15.000000 data_agent-0.3.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-02 20:58:15.000000 data_agent-0.3.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-02 20:58:15.000000 data_agent-0.3.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-05-02 20:58:15.000000 data_agent-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 20:58:15.000000 data_agent-0.3.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-02 20:58:15.000000 data_agent-0.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 20:58:15.000000 data_agent-0.3.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 20:58:15.000000 data_agent-0.3.1/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-02 20:58:15.000000 data_agent-0.3.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-02 20:58:15.000000 data_agent-0.3.1/docs/windows-service.md
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 20:58:15.000000 data_agent-0.3.1/make-runtime.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 20:58:15.000000 data_agent-0.3.1/make-service.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-02 20:58:15.000000 data_agent-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-02 20:58:47.882989 data_agent-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-02 20:58:15.000000 data_agent-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.866989 data_agent-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.874989 data_agent-0.3.1/src/data_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/abstract_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12044 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/broker_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/broker_agent_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/config_persist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/config_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/connection_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.874989 data_agent-0.3.1/src/data_agent/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/connectors/fake_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/daq_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/exchanger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/groups_aware_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.874989 data_agent-0.3.1/src/data_agent/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/linux/config_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/local_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/safe_manipulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.878989 data_agent-0.3.1/src/data_agent/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/win32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/win32/config_default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.878989 data_agent-0.3.1/src/data_agent/win32/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/win32/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/win32/hooks/hook-data_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/win32/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/win32/win_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-05-02 20:58:15.000000 data_agent-0.3.1/src/data_agent/win32/win_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.878989 data_agent-0.3.1/src/data_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-02 20:58:47.000000 data_agent-0.3.1/src/data_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-02 20:58:47.000000 data_agent-0.3.1/src/data_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:58:47.000000 data_agent-0.3.1/src/data_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 20:58:47.000000 data_agent-0.3.1/src/data_agent.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:58:47.000000 data_agent-0.3.1/src/data_agent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 20:58:47.000000 data_agent-0.3.1/src/data_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 20:58:47.000000 data_agent-0.3.1/src/data_agent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.878989 data_agent-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-02 20:58:15.000000 data_agent-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.866989 data_agent-0.3.1/tests/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.866989 data_agent-0.3.1/tests/docker/rabbitmq/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:58:47.878989 data_agent-0.3.1/tests/docker/rabbitmq/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-02 20:58:15.000000 data_agent-0.3.1/tests/docker/rabbitmq/etc/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 20:58:15.000000 data_agent-0.3.1/tests/docker/rabbitmq/etc/enabled_plugins
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 20:58:15.000000 data_agent-0.3.1/tests/docker/rabbitmq/etc/rabbitmq.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-02 20:58:15.000000 data_agent-0.3.1/tests/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-02 20:58:15.000000 data_agent-0.3.1/tests/test_api_config_provision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-02 20:58:15.000000 data_agent-0.3.1/tests/test_api_daq_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-02 20:58:15.000000 data_agent-0.3.1/tests/test_api_safe_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-05-02 20:58:15.000000 data_agent-0.3.1/tests/test_api_target_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-05-02 20:58:15.000000 data_agent-0.3.1/tests/test_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10342 2024-05-02 20:58:15.000000 data_agent-0.3.1/tests/test_daq_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-02 20:58:15.000000 data_agent-0.3.1/tests/test_fake_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-02 20:58:15.000000 data_agent-0.3.1/tests/test_safe_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-02 20:58:15.000000 data_agent-0.3.1/tox.ini
```

### Comparing `data-agent-0.2.0/.coveragerc` & `data_agent-0.3.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/.github/workflows/ci.yml` & `data_agent-0.3.1/.github/workflows/ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-# GitHub Actions configuration **EXAMPLE**,
-# MODIFY IT ACCORDING TO YOUR NEEDS!
-# Reference: https://docs.github.com/en/actions
-
-name: tests
+name: build
 
 on:
   push:
     # Avoid using all the resources/limits available by checking only
     # relevant branches and tags. Other branches can be checked via PRs.
     branches: [main]
     tags: ['v[0-9]*', '[0-9]+.[0-9]+*']  # Match tags that resemble a version
@@ -28,32 +24,32 @@
 
 jobs:
   prepare:
     runs-on: ubuntu-latest
     outputs:
       wheel-distribution: ${{ steps.wheel-distribution.outputs.path }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with: {fetch-depth: 0}  # deep clone for setuptools-scm
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         id: setup-python
         with: {python-version: "3.11"}
       - name: Run static analysis and format checkers
         run: pipx run pre-commit run --all-files --show-diff-on-failure
       - name: Build package distribution files
         run: >-
           pipx run --python '${{ steps.setup-python.outputs.python-path }}'
           tox -e clean,build
       - name: Record the path of wheel distribution
         id: wheel-distribution
         run: echo "path=$(ls dist/*.whl)" >> $GITHUB_OUTPUT
       - name: Store the distribution files for use in other stages
         # `tests` and `publish` will use the same pre-built distributions,
         # so we make sure to release the exact same package that was tested
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: python-distribution-files
           path: dist/
           retention-days: 1
 
   test:
     needs: prepare
@@ -69,21 +65,21 @@
         - "3.8"  # oldest Python supported by PSF
         - "3.11"  # newest Python that is stable
         platform:
         - ubuntu-latest
 #        - windows-latest
     runs-on: ${{ matrix.platform }}
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         id: setup-python
         with:
           python-version: ${{ matrix.python }}
       - name: Retrieve pre-built distribution files
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with: {name: python-distribution-files, path: dist/}
       - name: Run tests
         run: >-
           pipx run --python '${{ steps.setup-python.outputs.python-path }}'
           tox --installpkg '${{ needs.prepare.outputs.wheel-distribution }}'
           -- -rFEx --durations 10 --color yes  # pytest args
       - name: Generate coverage report
@@ -109,19 +105,19 @@
   publish:
     needs: finalize
     if: ${{ github.event_name == 'push' && contains(github.ref, 'refs/tags/') }}
     runs-on: ubuntu-latest
     permissions:
       contents: write
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with: {python-version: "3.11"}
       - name: Retrieve pre-built distribution files
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with: {name: python-distribution-files, path: dist/}
       - name: Publish Package
         env:
           # TODO: Set your PYPI_TOKEN as a secret using GitHub UI
           # - https://pypi.org/help/#apitoken
           # - https://docs.github.com/en/actions/security-guides/encrypted-secrets
           TWINE_REPOSITORY: pypi
```

### Comparing `data-agent-0.2.0/.gitignore` & `data_agent-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/.pre-commit-config.yaml` & `data_agent-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/.readthedocs.yml` & `data_agent-0.3.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/CONTRIBUTING.md` & `data_agent-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/LICENSE.txt` & `data_agent-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/PKG-INFO` & `data_agent-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-agent
-Version: 0.2.0
+Version: 0.3.1
 Summary: Data Agent is a python library for pipelining real-time and historical data to and from industrial historians and control systems
 Home-page: https://github.com/imubit/data-agent/
 Author: Meir Tseitlin
 License: LGPLv3
 Project-URL: Documentation, https://github.com/imubit/data-agent/
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `data-agent-0.2.0/README.md` & `data_agent-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/docs/Makefile` & `data_agent-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/docs/conf.py` & `data_agent-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/docs/index.md` & `data_agent-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/docs/windows-service.md` & `data_agent-0.3.1/docs/windows-service.md`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/setup.cfg` & `data_agent-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/setup.py` & `data_agent-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/__init__.py` & `data_agent-0.3.1/src/data_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/abstract_connector.py` & `data_agent-0.3.1/src/data_agent/abstract_connector.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,24 @@
     OVERRIDE_TAG_PERIOD = 6
     READ_TAG_META = 7
     WRITE_TAG_META = 8
     CREATE_TAG = 9
     DELETE_TAG = 10
 
 
+STANDARD_ATTRIBUTES = {
+    "Name": {"Type": "str", "Name": "Tag Name"},
+    "Type": {"Type": "str", "Name": "Data Type"},
+    "EngUnits": {"Type": "str", "Name": "Eng. Units"},
+    "Path": {"Type": "str", "Name": "Tag Path"},
+    "Description": {"Type": "str", "Name": "Description"},
+    "HasChildren": {"Type": "str", "Name": "HasChildren"},
+}
+
+
 def active_connection(func):
     @wraps(func)
     def inner(self, *args, **kwargs):
         if not self.connected:
             raise ConnectionNotActive("Not connected")
 
         return func(self, *args, **kwargs)
@@ -42,29 +52,38 @@
     return inner
 
 
 class AbstractConnector(ABC):
     TYPE = "abstract_connector"
     _name = ""
 
+    @staticmethod
+    def plugin_supported():
+        return False
+
+    @staticmethod
+    def list_connection_fields():
+        return {}
+
+    @staticmethod
+    @abstractmethod
+    def target_info(target_ref):
+        return {}
+
     def __init__(self, conn_name):
         self._name = conn_name
 
     def __del__(self):
         if self.connected:
             self.disconnect()
 
     @property
     def name(self):
         return self._name
 
-    @staticmethod
-    def target_info(target_host):
-        return {}
-
     @property
     @abstractmethod
     def connected(self):
         pass
 
     @abstractmethod
     def connect(self):
```

### Comparing `data-agent-0.2.0/src/data_agent/api.py` & `data_agent-0.3.1/src/data_agent/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,22 +45,22 @@
 
     @traceapi
     def list_supported_connectors(self):
         """Return a list of supported connector types by this agent"""
         return self._connection_manager.list_supported_connectors()
 
     @traceapi
-    def target_info(self, target_host: str, conn_type: str):
+    def target_info(self, target_ref: str, conn_type: str):
         """Retrieve information about target host (including endpoint enumeration if availailble)
 
-        :param target_host:
+        :param target_ref:
         :param conn_type:
         :return:
         """
-        return self._connection_manager.target_info(target_host, conn_type)
+        return self._connection_manager.target_info(target_ref, conn_type)
 
     @traceapi
     def list_connections(self):
         """List configured connections with connection status and type
 
         :return:
         """
```

### Comparing `data-agent-0.2.0/src/data_agent/broker_agent.py` & `data_agent-0.3.1/src/data_agent/broker_agent.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/broker_agent_main.py` & `data_agent-0.3.1/src/data_agent/broker_agent_main.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/cli_main.py` & `data_agent-0.3.1/src/data_agent/cli_main.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/config_manager.py` & `data_agent-0.3.1/src/data_agent/config_manager.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/config_template.py` & `data_agent-0.3.1/src/data_agent/config_template.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/connection_manager.py` & `data_agent-0.3.1/src/data_agent/connection_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,18 +78,23 @@
             f"configured connections: {list(self._connections_map.keys()) if self._connections_map else ''}"
         )
 
     def __del__(self):
         self.close()
 
     def close(self):
+        if not self._connector_classes:
+            return
+
         # Remove connections, but not from persistance
         existing_connections = list(self._connections_map.keys())
         for conn in existing_connections:
             self._delete_connection(conn)
+
+        self._connector_classes = None
         log.info("ConnectionManager terminated successfully.")
 
     def reset(self):
         existing_connections = list(self._connections_map.keys())
         for conn in existing_connections:
             self.delete_connection(conn)
 
@@ -98,24 +103,29 @@
         if sys.version_info[:3] < (3, 10):
             return entry_points().get("data_agent.connectors", [])
 
         return entry_points(group="data_agent.connectors")
 
     @staticmethod
     def list_supported_connectors():
+        entries = {
+            entry.name: entry.load() for entry in ConnectionManager.list_plugins()
+        }
+
         return {
-            entry.name: {
-                "category": entry.load().CATEGORY,
-                "connection_fields": entry.load().list_connection_fields(),
+            entry: {
+                "category": entries[entry].CATEGORY,
+                "connection_fields": entries[entry].list_connection_fields(),
             }
-            for entry in ConnectionManager.list_plugins()
+            for entry in entries
+            if entries[entry].plugin_supported()
         }
 
-    def target_info(self, target_host, conn_type):
-        return self._connector_classes[conn_type].target_info(target_host)
+    def target_info(self, target_ref, conn_type):
+        return self._connector_classes[conn_type].target_info(target_ref)
 
     def list_connections(self, include_details=True):
         if not include_details:
             return list(self._connections_map.keys())
 
         return [self._conn_descriptor(v) for k, v in self._connections_map.items()]
```

### Comparing `data-agent-0.2.0/src/data_agent/connectors/fake_connector.py` & `data_agent-0.3.1/src/data_agent/connectors/fake_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,26 @@
         SupportedOperation.READ_TAG_PERIOD,
         SupportedOperation.READ_TAG_META,
     ]
     DEFAULT_ATTRIBUTES = [
         ("tag", {"Type": "str", "Name": "Tag Name"}),
     ]
 
+    @staticmethod
+    def supported():
+        return True
+
+    @staticmethod
+    def list_connection_fields():
+        return {}
+
+    @staticmethod
+    def target_info(_):
+        return {"Name": "absolute-fake", "Endpoints": []}
+
     def __init__(self, conn_name="fake_client", **kwargs):
         super(FakeConnector, self).__init__(conn_name)
         self._connected = False
         self._tags = {
             "Static": {
                 "Float": {
                     "Value": 83289.48243,
@@ -63,30 +75,22 @@
                     "Quality": "Good",
                     "Timestamp": "09/02/2021T07:40:22.040",
                     "DataType": "Int4",
                 },
             },
         }
 
-    @staticmethod
-    def list_connection_fields():
-        return {}
-
     def _update_random(self):
         self._tags["Random"]["Real8"]["Value"] = random.random() * 1000
         self._tags["Random"]["Real8"]["Timestamp"] = str(datetime.utcnow())
         self._tags["Random"]["String"]["Value"] = random.choice(
             "We are going to win this race.".split(" ")
         )
         self._tags["Random"]["String"]["Timestamp"] = str(datetime.utcnow())
 
-    @staticmethod
-    def target_info(_):
-        return {"Name": "absolute-fake", "Endpoints": []}
-
     @property
     def connected(self):
         return self._connected
 
     def connect(self):
         self._connected = True
```

### Comparing `data-agent-0.2.0/src/data_agent/daq_scheduler.py` & `data_agent-0.3.1/src/data_agent/daq_scheduler.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/exceptions.py` & `data_agent-0.3.1/src/data_agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/exchanger.py` & `data_agent-0.3.1/src/data_agent/exchanger.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/groups_aware_connector.py` & `data_agent-0.3.1/src/data_agent/groups_aware_connector.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/linux/config_default.yaml` & `data_agent-0.3.1/src/data_agent/linux/config_default.yaml`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/local_agent.py` & `data_agent-0.3.1/src/data_agent/local_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         )
 
         log.info("")
         log.info(
             "************ Data Agent Service Initialized *************************"
         )
         log.info(
-            f" Supported connectors: {self._connection_manager.list_supported_connectors().keys()}"
+            f" Supported connectors: {list(self._connection_manager.list_supported_connectors().keys())}"
         )
         log.info(
             "***********************************************************************"
         )
 
     @property
     def api(self):
```

### Comparing `data-agent-0.2.0/src/data_agent/safe_manipulator.py` & `data_agent-0.3.1/src/data_agent/safe_manipulator.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/win32/config_default.yaml` & `data_agent-0.3.1/src/data_agent/win32/config_default.yaml`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/win32/hooks/hook-data_agent.py` & `data_agent-0.3.1/src/data_agent/win32/hooks/hook-data_agent.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/win32/service.py` & `data_agent-0.3.1/src/data_agent/win32/service.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent/win32/win_service.py` & `data_agent-0.3.1/src/data_agent/win32/win_service.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/src/data_agent.egg-info/PKG-INFO` & `data_agent-0.3.1/src/data_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-agent
-Version: 0.2.0
+Version: 0.3.1
 Summary: Data Agent is a python library for pipelining real-time and historical data to and from industrial historians and control systems
 Home-page: https://github.com/imubit/data-agent/
 Author: Meir Tseitlin
 License: LGPLv3
 Project-URL: Documentation, https://github.com/imubit/data-agent/
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `data-agent-0.2.0/src/data_agent.egg-info/SOURCES.txt` & `data_agent-0.3.1/src/data_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/tests/conftest.py` & `data_agent-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/tests/docker/rabbitmq/etc/definitions.json` & `data_agent-0.3.1/tests/docker/rabbitmq/etc/definitions.json`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/tests/test_api_config_provision.py` & `data_agent-0.3.1/tests/test_api_config_provision.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/tests/test_api_daq_job.py` & `data_agent-0.3.1/tests/test_api_daq_job.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/tests/test_api_safe_manipulator.py` & `data_agent-0.3.1/tests/test_api_safe_manipulator.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/tests/test_api_target_connection.py` & `data_agent-0.3.1/tests/test_api_target_connection.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/tests/test_connection_manager.py` & `data_agent-0.3.1/tests/test_connection_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def test_list_supported_connectors(connection_manager):
     assert connection_manager.list_supported_connectors() == {}
 
 
 def test_target_info(connection_manager):
-    info = connection_manager.target_info(target_host="localhost", conn_type="fake")
+    info = connection_manager.target_info(target_ref="localhost", conn_type="fake")
     assert info == {"Name": "absolute-fake", "Endpoints": []}
 
 
 def test_connection_lifecycle(connection_manager):
     conn_name = "test1"
 
     # Create
```

### Comparing `data-agent-0.2.0/tests/test_daq_scheduler.py` & `data_agent-0.3.1/tests/test_daq_scheduler.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/tests/test_fake_connector.py` & `data_agent-0.3.1/tests/test_fake_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from data_agent.exceptions import ErrorAddingTagsToGroup
 
 
 def test_sanity():
     conn = FakeConnector()
     conn.connect()
 
+    assert conn.supported()
     assert conn.TYPE == "fake"
     assert conn.name == "fake_client"
 
     info = conn.connection_info()
     print(info)
     # assert info['Version'].startswith('1')
```

### Comparing `data-agent-0.2.0/tests/test_safe_manipulator.py` & `data_agent-0.3.1/tests/test_safe_manipulator.py`

 * *Files identical despite different names*

### Comparing `data-agent-0.2.0/tox.ini` & `data_agent-0.3.1/tox.ini`

 * *Files identical despite different names*

