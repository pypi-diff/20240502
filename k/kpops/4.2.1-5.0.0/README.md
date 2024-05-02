# Comparing `tmp/kpops-4.2.1.tar.gz` & `tmp/kpops-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpops-4.2.1.tar", max compression
+gzip compressed data, was "kpops-5.0.0.tar", max compression
```

## Comparing `kpops-4.2.1.tar` & `kpops-5.0.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1064 2024-04-25 14:53:30.739912 kpops-4.2.1/LICENSE
--rw-r--r--   0        0        0     2678 2024-04-25 14:53:30.739912 kpops-4.2.1/README.md
--rw-r--r--   0        0        0      250 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/cli/__init__.py
--rw-r--r--   0        0        0      761 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/cli/custom_formatter.py
--rw-r--r--   0        0        0      124 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/cli/exception.py
--rw-r--r--   0        0        0    16061 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/cli/main.py
--rw-r--r--   0        0        0      101 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/cli/options.py
--rw-r--r--   0        0        0     2512 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/cli/registry.py
--rw-r--r--   0        0        0      699 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/helm_wrapper/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/helm_wrapper/dry_run_handler.py
--rw-r--r--   0        0        0       92 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/helm_wrapper/exception.py
--rw-r--r--   0        0        0     8950 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/helm_wrapper/helm.py
--rw-r--r--   0        0        0     2125 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/helm_wrapper/helm_diff.py
--rw-r--r--   0        0        0     7072 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/helm_wrapper/model.py
--rw-r--r--   0        0        0      974 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/helm_wrapper/utils.py
--rw-r--r--   0        0        0        0 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/kafka_connect/__init__.py
--rw-r--r--   0        0        0     7412 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/kafka_connect/connect_wrapper.py
--rw-r--r--   0        0        0      229 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/kafka_connect/exception.py
--rw-r--r--   0        0        0     5460 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
--rw-r--r--   0        0        0     3543 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/kafka_connect/model.py
--rw-r--r--   0        0        0      797 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/kafka_connect/timeout.py
--rw-r--r--   0        0        0        0 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/kubernetes/__init__.py
--rw-r--r--   0        0        0      841 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/kubernetes/model.py
--rw-r--r--   0        0        0     1735 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/kubernetes/pvc_handler.py
--rw-r--r--   0        0        0     1116 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/kubernetes/utils.py
--rw-r--r--   0        0        0        0 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/schema_handler/__init__.py
--rw-r--r--   0        0        0     6774 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/schema_handler/schema_handler.py
--rw-r--r--   0        0        0      491 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/schema_handler/schema_provider.py
--rw-r--r--   0        0        0        0 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/topic/__init__.py
--rw-r--r--   0        0        0      225 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/topic/exception.py
--rw-r--r--   0        0        0     9534 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/topic/handler.py
--rw-r--r--   0        0        0     2420 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/topic/model.py
--rw-r--r--   0        0        0     7345 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/topic/proxy_wrapper.py
--rw-r--r--   0        0        0     2385 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/topic/utils.py
--rw-r--r--   0        0        0        0 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/utils/__init__.py
--rw-r--r--   0        0        0      625 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/component_handlers/utils/exception.py
--rw-r--r--   0        0        0      906 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/base_components/__init__.py
--rw-r--r--   0        0        0    10674 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/base_components/base_defaults_component.py
--rw-r--r--   0        0        0     1061 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/base_components/cleaner.py
--rw-r--r--   0        0        0     7237 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/base_components/helm_app.py
--rw-r--r--   0        0        0     4748 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/base_components/kafka_app.py
--rw-r--r--   0        0        0     9178 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/base_components/kafka_connector.py
--rw-r--r--   0        0        0     1828 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/base_components/kubernetes_app.py
--rw-r--r--   0        0        0      149 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/base_components/models/__init__.py
--rw-r--r--   0        0        0     1882 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/base_components/models/from_section.py
--rw-r--r--   0        0        0      217 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/base_components/models/resource.py
--rw-r--r--   0        0        0      994 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/base_components/models/to_section.py
--rw-r--r--   0        0        0     3801 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/base_components/models/topic.py
--rw-r--r--   0        0        0     8324 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/base_components/pipeline_component.py
--rw-r--r--   0        0        0     1031 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/streams_bootstrap/__init__.py
--rw-r--r--   0        0        0      217 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/streams_bootstrap/app_type.py
--rw-r--r--   0        0        0        0 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/streams_bootstrap/producer/__init__.py
--rw-r--r--   0        0        0      595 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/streams_bootstrap/producer/model.py
--rw-r--r--   0        0        0     2873 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/streams_bootstrap/producer/producer_app.py
--rw-r--r--   0        0        0        0 2024-04-25 14:53:30.747912 kpops-4.2.1/kpops/components/streams_bootstrap/streams/__init__.py
--rw-r--r--   0        0        0    10245 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/components/streams_bootstrap/streams/model.py
--rw-r--r--   0        0        0     4172 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/components/streams_bootstrap/streams/streams_app.py
--rw-r--r--   0        0        0     5147 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/config.py
--rw-r--r--   0        0        0    15340 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/pipeline.py
--rw-r--r--   0        0        0      278 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/utils/__init__.py
--rw-r--r--   0        0        0     3060 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/utils/cli_commands.py
--rw-r--r--   0        0        0      375 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/utils/colorify.py
--rw-r--r--   0        0        0     3178 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/utils/dict_differ.py
--rw-r--r--   0        0        0     4996 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/utils/dict_ops.py
--rw-r--r--   0        0        0     2431 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/utils/docstring.py
--rw-r--r--   0        0        0     1176 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/utils/environment.py
--rw-r--r--   0        0        0     5924 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/utils/gen_schema.py
--rw-r--r--   0        0        0      298 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/utils/json.py
--rw-r--r--   0        0        0     6533 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/utils/pydantic.py
--rw-r--r--   0        0        0      238 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/utils/types.py
--rw-r--r--   0        0        0     4332 2024-04-25 14:53:30.751912 kpops-4.2.1/kpops/utils/yaml.py
--rw-r--r--   0        0        0     7443 2024-04-25 14:53:30.751912 kpops-4.2.1/pyproject.toml
--rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 kpops-4.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-02 08:33:07.663153 kpops-5.0.0/LICENSE
+-rw-r--r--   0        0        0     2675 2024-05-02 08:33:07.663153 kpops-5.0.0/README.md
+-rw-r--r--   0        0        0      250 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/cli/__init__.py
+-rw-r--r--   0        0        0      761 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/cli/custom_formatter.py
+-rw-r--r--   0        0        0      124 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/cli/exception.py
+-rw-r--r--   0        0        0    16061 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/cli/main.py
+-rw-r--r--   0        0        0      101 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/cli/options.py
+-rw-r--r--   0        0        0     2512 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/cli/registry.py
+-rw-r--r--   0        0        0      699 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/helm_wrapper/__init__.py
+-rw-r--r--   0        0        0     1168 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/helm_wrapper/dry_run_handler.py
+-rw-r--r--   0        0        0       92 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/helm_wrapper/exception.py
+-rw-r--r--   0        0        0     8950 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/helm_wrapper/helm.py
+-rw-r--r--   0        0        0     2125 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/helm_wrapper/helm_diff.py
+-rw-r--r--   0        0        0     7072 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/helm_wrapper/model.py
+-rw-r--r--   0        0        0      974 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/helm_wrapper/utils.py
+-rw-r--r--   0        0        0        0 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/kafka_connect/__init__.py
+-rw-r--r--   0        0        0     7434 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/kafka_connect/connect_wrapper.py
+-rw-r--r--   0        0        0      229 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/kafka_connect/exception.py
+-rw-r--r--   0        0        0     4839 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
+-rw-r--r--   0        0        0     3543 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/kafka_connect/model.py
+-rw-r--r--   0        0        0      797 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/kafka_connect/timeout.py
+-rw-r--r--   0        0        0        0 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/kubernetes/__init__.py
+-rw-r--r--   0        0        0      841 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/kubernetes/model.py
+-rw-r--r--   0        0        0     1735 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/kubernetes/pvc_handler.py
+-rw-r--r--   0        0        0     1116 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/kubernetes/utils.py
+-rw-r--r--   0        0        0        0 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/schema_handler/__init__.py
+-rw-r--r--   0        0        0     6872 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/schema_handler/schema_handler.py
+-rw-r--r--   0        0        0      491 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/schema_handler/schema_provider.py
+-rw-r--r--   0        0        0        0 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/topic/__init__.py
+-rw-r--r--   0        0        0      225 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/topic/exception.py
+-rw-r--r--   0        0        0     9534 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/topic/handler.py
+-rw-r--r--   0        0        0     2420 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/topic/model.py
+-rw-r--r--   0        0        0     7389 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/topic/proxy_wrapper.py
+-rw-r--r--   0        0        0     2385 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/topic/utils.py
+-rw-r--r--   0        0        0        0 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/utils/__init__.py
+-rw-r--r--   0        0        0      625 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/component_handlers/utils/exception.py
+-rw-r--r--   0        0        0      906 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/base_components/__init__.py
+-rw-r--r--   0        0        0    10674 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/base_components/base_defaults_component.py
+-rw-r--r--   0        0        0     1061 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/base_components/cleaner.py
+-rw-r--r--   0        0        0     7237 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/base_components/helm_app.py
+-rw-r--r--   0        0        0     4748 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/base_components/kafka_app.py
+-rw-r--r--   0        0        0     9178 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/base_components/kafka_connector.py
+-rw-r--r--   0        0        0     1828 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/base_components/kubernetes_app.py
+-rw-r--r--   0        0        0      149 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/base_components/models/__init__.py
+-rw-r--r--   0        0        0     1882 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/base_components/models/from_section.py
+-rw-r--r--   0        0        0      217 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/base_components/models/resource.py
+-rw-r--r--   0        0        0      994 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/base_components/models/to_section.py
+-rw-r--r--   0        0        0     3801 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/base_components/models/topic.py
+-rw-r--r--   0        0        0     8324 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/base_components/pipeline_component.py
+-rw-r--r--   0        0        0     1031 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/streams_bootstrap/__init__.py
+-rw-r--r--   0        0        0      217 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/streams_bootstrap/app_type.py
+-rw-r--r--   0        0        0        0 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/streams_bootstrap/producer/__init__.py
+-rw-r--r--   0        0        0      595 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/streams_bootstrap/producer/model.py
+-rw-r--r--   0        0        0     2873 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/streams_bootstrap/producer/producer_app.py
+-rw-r--r--   0        0        0        0 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/streams_bootstrap/streams/__init__.py
+-rw-r--r--   0        0        0    10245 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/streams_bootstrap/streams/model.py
+-rw-r--r--   0        0        0     4172 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/components/streams_bootstrap/streams/streams_app.py
+-rw-r--r--   0        0        0     5299 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/config.py
+-rw-r--r--   0        0        0    15340 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/pipeline.py
+-rw-r--r--   0        0        0      278 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/utils/__init__.py
+-rw-r--r--   0        0        0     3060 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/utils/cli_commands.py
+-rw-r--r--   0        0        0      375 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/utils/colorify.py
+-rw-r--r--   0        0        0     3178 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/utils/dict_differ.py
+-rw-r--r--   0        0        0     4996 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/utils/dict_ops.py
+-rw-r--r--   0        0        0     2431 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/utils/docstring.py
+-rw-r--r--   0        0        0     1176 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/utils/environment.py
+-rw-r--r--   0        0        0     5924 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/utils/gen_schema.py
+-rw-r--r--   0        0        0      298 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/utils/json.py
+-rw-r--r--   0        0        0     6533 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/utils/pydantic.py
+-rw-r--r--   0        0        0      238 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/utils/types.py
+-rw-r--r--   0        0        0     4332 2024-05-02 08:33:07.671153 kpops-5.0.0/kpops/utils/yaml.py
+-rw-r--r--   0        0        0     7443 2024-05-02 08:33:07.675153 kpops-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 kpops-5.0.0/PKG-INFO
```

### Comparing `kpops-4.2.1/LICENSE` & `kpops-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/README.md` & `kpops-5.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 the [documentation](https://bakdata.github.io/kpops/latest).
 
 ## Install KPOps
 
 KPOps comes as a [PyPI package](https://pypi.org/project/kpops/).
 You can install it with [pip](https://github.com/pypa/pip):
 
-```shell
+```sh
 pip install kpops
 ```
 
 # GitHub action
 
 Please refer to the [GitHub Actions section](https://bakdata.github.io/kpops/latest/user/references/ci-integration/github-actions) for the documentation.
```

### Comparing `kpops-4.2.1/kpops/cli/custom_formatter.py` & `kpops-5.0.0/kpops/cli/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/cli/main.py` & `kpops-5.0.0/kpops/cli/main.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/cli/registry.py` & `kpops-5.0.0/kpops/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/__init__.py` & `kpops-5.0.0/kpops/component_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/helm_wrapper/dry_run_handler.py` & `kpops-5.0.0/kpops/component_handlers/helm_wrapper/dry_run_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/helm_wrapper/helm.py` & `kpops-5.0.0/kpops/component_handlers/helm_wrapper/helm.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/helm_wrapper/helm_diff.py` & `kpops-5.0.0/kpops/component_handlers/helm_wrapper/helm_diff.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/helm_wrapper/model.py` & `kpops-5.0.0/kpops/component_handlers/helm_wrapper/model.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/helm_wrapper/utils.py` & `kpops-5.0.0/kpops/component_handlers/helm_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/kafka_connect/connect_wrapper.py` & `kpops-5.0.0/kpops/component_handlers/kafka_connect/connect_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 class ConnectWrapper:
     """Wraps Kafka Connect APIs."""
 
     def __init__(self, config: KafkaConnectConfig) -> None:
         self._config: KafkaConnectConfig = config
-        self._client = httpx.AsyncClient()
+        self._client = httpx.AsyncClient(timeout=config.timeout)
 
     @property
     def url(self) -> AnyHttpUrl:
         return self._config.url
 
     async def create_connector(
         self, connector_config: KafkaConnectorConfig
```

### Comparing `kpops-4.2.1/kpops/component_handlers/kafka_connect/kafka_connect_handler.py` & `kpops-5.0.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import TYPE_CHECKING
 
 from kpops.component_handlers.kafka_connect.connect_wrapper import ConnectWrapper
 from kpops.component_handlers.kafka_connect.exception import (
     ConnectorNotFoundException,
     ConnectorStateException,
 )
-from kpops.component_handlers.kafka_connect.timeout import timeout
 from kpops.utils.colorify import magentaify
 from kpops.utils.dict_differ import render_diff
 
 if TYPE_CHECKING:
     try:
         from typing import Self  # pyright: ignore[reportAttributeAccessIssue]
     except ImportError:
@@ -21,21 +20,16 @@
     from kpops.component_handlers.kafka_connect.model import KafkaConnectorConfig
     from kpops.config import KpopsConfig
 
 log = logging.getLogger("KafkaConnectHandler")
 
 
 class KafkaConnectHandler:
-    def __init__(
-        self,
-        connect_wrapper: ConnectWrapper,
-        timeout: int,
-    ):
+    def __init__(self, connect_wrapper: ConnectWrapper):
         self._connect_wrapper = connect_wrapper
-        self._timeout = timeout
 
     async def create_connector(
         self, connector_config: KafkaConnectorConfig, *, dry_run: bool
     ) -> None:
         """Create a connector.
 
         If the connector exists the config of that connector gets updated.
@@ -43,49 +37,33 @@
         :param connector_config: The connector config.
         :param dry_run: Whether the connector creation should be run in dry run mode.
         """
         if dry_run:
             await self.__dry_run_connector_creation(connector_config)
         else:
             try:
-                await timeout(
-                    self._connect_wrapper.get_connector(connector_config.name),
-                    secs=self._timeout,
-                )
-
-                await timeout(
-                    self._connect_wrapper.update_connector_config(connector_config),
-                    secs=self._timeout,
-                )
+                await self._connect_wrapper.get_connector(connector_config.name)
+                await self._connect_wrapper.update_connector_config(connector_config)
 
             except ConnectorNotFoundException:
-                await timeout(
-                    self._connect_wrapper.create_connector(connector_config),
-                    secs=self._timeout,
-                )
+                await self._connect_wrapper.create_connector(connector_config)
 
     async def destroy_connector(self, connector_name: str, *, dry_run: bool) -> None:
         """Delete a connector resource from the cluster.
 
         :param connector_name: The connector name.
         :param dry_run: Whether the connector deletion should be run in dry run mode.
         """
         if dry_run:
             await self.__dry_run_connector_deletion(connector_name)
         else:
             try:
-                await timeout(
-                    self._connect_wrapper.get_connector(connector_name),
-                    secs=self._timeout,
-                )
+                await self._connect_wrapper.get_connector(connector_name)
+                await self._connect_wrapper.delete_connector(connector_name)
 
-                await timeout(
-                    self._connect_wrapper.delete_connector(connector_name),
-                    secs=self._timeout,
-                )
             except ConnectorNotFoundException:
                 log.warning(
                     f"Connector Destruction: the connector {connector_name} does not exist. Skipping."
                 )
 
     async def __dry_run_connector_creation(
         self, connector_config: KafkaConnectorConfig
@@ -134,9 +112,8 @@
                 f"Connector Destruction: connector {connector_name} does not exist and cannot be deleted. Skipping."
             )
 
     @classmethod
     def from_kpops_config(cls, config: KpopsConfig) -> Self:
         return cls(
             connect_wrapper=ConnectWrapper(config.kafka_connect),
-            timeout=config.timeout,
         )
```

### Comparing `kpops-4.2.1/kpops/component_handlers/kafka_connect/model.py` & `kpops-5.0.0/kpops/component_handlers/kafka_connect/model.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/kafka_connect/timeout.py` & `kpops-5.0.0/kpops/component_handlers/kafka_connect/timeout.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/kubernetes/model.py` & `kpops-5.0.0/kpops/component_handlers/kubernetes/model.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/kubernetes/pvc_handler.py` & `kpops-5.0.0/kpops/component_handlers/kubernetes/pvc_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/kubernetes/utils.py` & `kpops-5.0.0/kpops/component_handlers/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/schema_handler/schema_handler.py` & `kpops-5.0.0/kpops/component_handlers/schema_handler/schema_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 
 log = logging.getLogger("SchemaHandler")
 
 
 class SchemaHandler:
     def __init__(self, kpops_config: KpopsConfig) -> None:
         self.schema_registry_client = AsyncSchemaRegistryClient(
-            str(kpops_config.schema_registry.url)
+            str(kpops_config.schema_registry.url),
+            timeout=kpops_config.schema_registry.timeout,  # pyright: ignore[reportArgumentType]
         )
         self.components_module = kpops_config.components_module
 
     @cached_property
     def schema_provider(self) -> SchemaProvider:
         try:
             if not self.components_module:
```

### Comparing `kpops-4.2.1/kpops/component_handlers/topic/handler.py` & `kpops-5.0.0/kpops/component_handlers/topic/handler.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/topic/model.py` & `kpops-5.0.0/kpops/component_handlers/topic/model.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/topic/proxy_wrapper.py` & `kpops-5.0.0/kpops/component_handlers/topic/proxy_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 
 class ProxyWrapper:
     """Wraps Kafka REST Proxy APIs."""
 
     def __init__(self, config: KafkaRestConfig) -> None:
         self._config: KafkaRestConfig = config
-        self._client = httpx.AsyncClient()
-        self._sync_client = httpx.Client()
+        self._client = httpx.AsyncClient(timeout=config.timeout)
+        self._sync_client = httpx.Client(timeout=config.timeout)
 
     @cached_property
     def cluster_id(self) -> str:
         """Get the Kafka cluster ID by sending a request to Kafka REST proxy.
 
         More information about the cluster ID can be found here:
         https://docs.confluent.io/platform/current/kafka-rest/api.html#cluster-v3.
```

### Comparing `kpops-4.2.1/kpops/component_handlers/topic/utils.py` & `kpops-5.0.0/kpops/component_handlers/topic/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/component_handlers/utils/exception.py` & `kpops-5.0.0/kpops/component_handlers/utils/exception.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/__init__.py` & `kpops-5.0.0/kpops/components/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/base_components/base_defaults_component.py` & `kpops-5.0.0/kpops/components/base_components/base_defaults_component.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/base_components/cleaner.py` & `kpops-5.0.0/kpops/components/base_components/cleaner.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/base_components/helm_app.py` & `kpops-5.0.0/kpops/components/base_components/helm_app.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/base_components/kafka_app.py` & `kpops-5.0.0/kpops/components/base_components/kafka_app.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/base_components/kafka_connector.py` & `kpops-5.0.0/kpops/components/base_components/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/base_components/kubernetes_app.py` & `kpops-5.0.0/kpops/components/base_components/kubernetes_app.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/base_components/models/from_section.py` & `kpops-5.0.0/kpops/components/base_components/models/from_section.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/base_components/models/to_section.py` & `kpops-5.0.0/kpops/components/base_components/models/to_section.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/base_components/models/topic.py` & `kpops-5.0.0/kpops/components/base_components/models/topic.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/base_components/pipeline_component.py` & `kpops-5.0.0/kpops/components/base_components/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/streams_bootstrap/__init__.py` & `kpops-5.0.0/kpops/components/streams_bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/streams_bootstrap/producer/model.py` & `kpops-5.0.0/kpops/components/streams_bootstrap/producer/model.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/streams_bootstrap/producer/producer_app.py` & `kpops-5.0.0/kpops/components/streams_bootstrap/producer/producer_app.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/streams_bootstrap/streams/model.py` & `kpops-5.0.0/kpops/components/streams_bootstrap/streams/model.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/components/streams_bootstrap/streams/streams_app.py` & `kpops-5.0.0/kpops/components/streams_bootstrap/streams/streams_app.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/config.py` & `kpops-5.0.0/kpops/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,32 +37,41 @@
         default=False,
         description="Whether the Schema Registry handler should be initialized.",
     )
     url: AnyHttpUrl = Field(
         default=TypeAdapter(AnyHttpUrl).validate_python("http://localhost:8081"),  # pyright: ignore[reportCallIssue]
         description="Address of the Schema Registry.",
     )
+    timeout: int | float = Field(
+        default=30, description="Operation timeout in seconds."
+    )
 
 
 class KafkaRestConfig(BaseSettings):
     """Configuration for Kafka REST Proxy."""
 
     url: AnyHttpUrl = Field(
         default=TypeAdapter(AnyHttpUrl).validate_python("http://localhost:8082"),  # pyright: ignore[reportCallIssue]
         description="Address of the Kafka REST Proxy.",
     )
+    timeout: int | float = Field(
+        default=30, description="Operation timeout in seconds."
+    )
 
 
 class KafkaConnectConfig(BaseSettings):
     """Configuration for Kafka Connect."""
 
     url: AnyHttpUrl = Field(
         default=TypeAdapter(AnyHttpUrl).validate_python("http://localhost:8083"),  # pyright: ignore[reportCallIssue]
         description="Address of Kafka Connect.",
     )
+    timeout: int | float = Field(
+        default=30, description="Operation timeout in seconds."
+    )
 
 
 class KpopsConfig(BaseSettings):
     """Global configuration for KPOps project."""
 
     components_module: str | None = Field(
         default=None,
@@ -95,18 +104,14 @@
         default=KafkaRestConfig(),
         description=describe_object(KafkaRestConfig.__doc__),
     )
     kafka_connect: KafkaConnectConfig = Field(
         default=KafkaConnectConfig(),
         description=describe_object(KafkaConnectConfig.__doc__),
     )
-    timeout: int = Field(
-        default=300,
-        description="The timeout in seconds that specifies when actions like deletion or deploy timeout.",
-    )
     create_namespace: bool = Field(
         default=False,
         description="Flag for `helm upgrade --install`. Create the release namespace if not present.",
     )
     helm_config: HelmConfig = Field(
         default=HelmConfig(),
         description="Global flags for Helm.",
```

### Comparing `kpops-4.2.1/kpops/pipeline.py` & `kpops-5.0.0/kpops/pipeline.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/utils/cli_commands.py` & `kpops-5.0.0/kpops/utils/cli_commands.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/utils/dict_differ.py` & `kpops-5.0.0/kpops/utils/dict_differ.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/utils/dict_ops.py` & `kpops-5.0.0/kpops/utils/dict_ops.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/utils/docstring.py` & `kpops-5.0.0/kpops/utils/docstring.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/utils/environment.py` & `kpops-5.0.0/kpops/utils/environment.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/utils/gen_schema.py` & `kpops-5.0.0/kpops/utils/gen_schema.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/utils/pydantic.py` & `kpops-5.0.0/kpops/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/kpops/utils/yaml.py` & `kpops-5.0.0/kpops/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `kpops-4.2.1/pyproject.toml` & `kpops-5.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kpops"
-version = "4.2.1"
+version = "5.0.0"
 description = "KPOps is a tool to deploy Kafka pipelines to Kubernetes"
 authors = ["bakdata <opensource@bakdata.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bakdata/kpops"
 documentation = "https://bakdata.github.io/kpops/latest"
 keywords = ["kafka", "kubernetes", "stream-processing", "pipelines"]
```

### Comparing `kpops-4.2.1/PKG-INFO` & `kpops-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kpops
-Version: 4.2.1
+Version: 5.0.0
 Summary: KPOps is a tool to deploy Kafka pipelines to Kubernetes
 Home-page: https://github.com/bakdata/kpops
 License: MIT
 Keywords: kafka,kubernetes,stream-processing,pipelines
 Author: bakdata
 Author-email: opensource@bakdata.com
 Requires-Python: >=3.10,<3.13
@@ -61,15 +61,15 @@
 the [documentation](https://bakdata.github.io/kpops/latest).
 
 ## Install KPOps
 
 KPOps comes as a [PyPI package](https://pypi.org/project/kpops/).
 You can install it with [pip](https://github.com/pypa/pip):
 
-```shell
+```sh
 pip install kpops
 ```
 
 # GitHub action
 
 Please refer to the [GitHub Actions section](https://bakdata.github.io/kpops/latest/user/references/ci-integration/github-actions) for the documentation.
```

