# Comparing `tmp/hoppr-1.9.4.tar.gz` & `tmp/hoppr-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr-1.9.4.tar", max compression
+gzip compressed data, was "hoppr-1.9.5.tar", max compression
```

## Comparing `hoppr-1.9.4.tar` & `hoppr-1.9.5.tar`

### file list

```diff
@@ -1,70 +1,71 @@
--rw-r--r--   0        0        0     1084 2023-08-17 18:17:19.000000 hoppr-1.9.4/LICENSE
--rw-r--r--   0        0        0     1215 2023-08-17 18:17:19.000000 hoppr-1.9.4/README.md
--rw-r--r--   0        0        0     1064 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/__init__.py
--rw-r--r--   0        0        0      154 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/__main__.py
--rw-r--r--   0        0        0        0 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/base_plugins/__init__.py
--rw-r--r--   0        0        0    11619 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/base_plugins/collector.py
--rw-r--r--   0        0        0    10937 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/base_plugins/hoppr.py
--rw-r--r--   0        0        0        0 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/base_plugins/py.typed
--rw-r--r--   0        0        0     2953 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/cli/__init__.py
--rw-r--r--   0        0        0     7014 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/cli/bundle.py
--rw-r--r--   0        0        0     2239 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/cli/generate.py
--rw-r--r--   0        0        0     7668 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/cli/layout.py
--rw-r--r--   0        0        0     6896 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/cli/merge.py
--rw-r--r--   0        0        0        0 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/cli/py.typed
--rw-r--r--   0        0        0      563 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/constants.py
--rw-r--r--   0        0        0        0 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/__init__.py
--rw-r--r--   0        0        0     3028 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/bundle_tar.py
--rw-r--r--   0        0        0    13493 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/collect_apt_plugin.py
--rw-r--r--   0        0        0     2330 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/collect_cargo_plugin.py
--rw-r--r--   0        0        0    11138 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/collect_dnf_plugin.py
--rw-r--r--   0        0        0     5355 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/collect_docker_plugin.py
--rw-r--r--   0        0        0     4568 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/collect_git_plugin.py
--rw-r--r--   0        0        0     2330 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/collect_golang_plugin.py
--rw-r--r--   0        0        0     4156 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/collect_helm_plugin.py
--rw-r--r--   0        0        0     6364 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/collect_maven_plugin.py
--rw-r--r--   0        0        0     7839 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/collect_nexus_search.py
--rw-r--r--   0        0        0     2390 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/collect_npm_plugin.py
--rw-r--r--   0        0        0     2788 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/collect_nuget_plugin.py
--rw-r--r--   0        0        0     6905 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/collect_pypi_plugin.py
--rw-r--r--   0        0        0     3033 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/collect_raw_plugin.py
--rw-r--r--   0        0        0     3698 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/collect_yum_plugin.py
--rw-r--r--   0        0        0     4458 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/composite_collector.py
--rw-r--r--   0        0        0     5511 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/delta_sbom.py
--rw-r--r--   0        0        0     6491 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/oras_bundle.py
--rw-r--r--   0        0        0     5106 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/oras_registry.py
--rw-r--r--   0        0        0        0 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/py.typed
--rw-r--r--   0        0        0      202 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/report_generator/__init__.py
--rw-r--r--   0        0        0   126749 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
--rw-r--r--   0        0        0     4635 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/report_generator/report_generator.py
--rw-r--r--   0        0        0    60554 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
--rw-r--r--   0        0        0      518 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/report_generator/scripts/custom.js
--rw-r--r--   0        0        0   220780 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
--rw-r--r--   0        0        0     3562 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/report_generator/styles/custom.css
--rw-r--r--   0        0        0     5052 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/report_generator/templates/component_card.jinja2
--rw-r--r--   0        0        0     1230 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
--rw-r--r--   0        0        0     7246 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/core_plugins/report_generator/templates/index.jinja2
--rw-r--r--   0        0        0      458 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/exceptions.py
--rw-r--r--   0        0        0     6827 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/in_toto.py
--rw-r--r--   0        0        0     5054 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/logger.py
--rw-r--r--   0        0        0     2908 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/main.py
--rw-r--r--   0        0        0     1627 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/models/__init__.py
--rw-r--r--   0        0        0     1602 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/models/__main__.py
--rw-r--r--   0        0        0     1546 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/models/base.py
--rw-r--r--   0        0        0     4001 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/models/credentials.py
--rw-r--r--   0        0        0    13082 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/models/manifest.py
--rw-r--r--   0        0        0        0 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/models/py.typed
--rw-r--r--   0        0        0    20889 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/models/sbom.py
--rw-r--r--   0        0        0     4730 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/models/transfer.py
--rw-r--r--   0        0        0     5629 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/models/types.py
--rw-r--r--   0        0        0     2335 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/net.py
--rw-r--r--   0        0        0     4251 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/oci_artifacts.py
--rw-r--r--   0        0        0     1332 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/plugin_utils.py
--rw-r--r--   0        0        0    30568 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/processor.py
--rw-r--r--   0        0        0        0 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/py.typed
--rw-r--r--   0        0        0    22579 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/resources/hoppr-hippo.ansi
--rw-r--r--   0        0        0    19725 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/resources/hoppr-hippo.ascii
--rw-r--r--   0        0        0     4036 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/result.py
--rw-r--r--   0        0        0     7797 2023-08-17 18:17:19.000000 hoppr-1.9.4/hoppr/utils.py
--rw-r--r--   0        0        0     5300 2023-08-17 18:17:19.000000 hoppr-1.9.4/pyproject.toml
--rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 hoppr-1.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-08-23 13:07:23.000000 hoppr-1.9.5/LICENSE
+-rw-r--r--   0        0        0     1215 2023-08-23 13:07:23.000000 hoppr-1.9.5/README.md
+-rw-r--r--   0        0        0     1139 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/__init__.py
+-rw-r--r--   0        0        0      154 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/base_plugins/__init__.py
+-rw-r--r--   0        0        0    11657 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/base_plugins/collector.py
+-rw-r--r--   0        0        0    10933 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/base_plugins/hoppr.py
+-rw-r--r--   0        0        0        0 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/base_plugins/py.typed
+-rw-r--r--   0        0        0     3283 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/cli/__init__.py
+-rw-r--r--   0        0        0     7118 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/cli/bundle.py
+-rw-r--r--   0        0        0     2239 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/cli/generate.py
+-rw-r--r--   0        0        0     8130 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/cli/layout.py
+-rw-r--r--   0        0        0     6896 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/cli/merge.py
+-rw-r--r--   0        0        0     1500 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/cli/options.py
+-rw-r--r--   0        0        0        0 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/cli/py.typed
+-rw-r--r--   0        0        0      562 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/constants.py
+-rw-r--r--   0        0        0        0 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/__init__.py
+-rw-r--r--   0        0        0     2990 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/bundle_tar.py
+-rw-r--r--   0        0        0    13493 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/collect_apt_plugin.py
+-rw-r--r--   0        0        0     2330 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/collect_cargo_plugin.py
+-rw-r--r--   0        0        0    11482 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/collect_dnf_plugin.py
+-rw-r--r--   0        0        0     6411 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/collect_docker_plugin.py
+-rw-r--r--   0        0        0     4551 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/collect_git_plugin.py
+-rw-r--r--   0        0        0     2330 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/collect_golang_plugin.py
+-rw-r--r--   0        0        0     4156 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/collect_helm_plugin.py
+-rw-r--r--   0        0        0     6364 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/collect_maven_plugin.py
+-rw-r--r--   0        0        0     7787 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/collect_nexus_search.py
+-rw-r--r--   0        0        0     2390 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/collect_npm_plugin.py
+-rw-r--r--   0        0        0     2788 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/collect_nuget_plugin.py
+-rw-r--r--   0        0        0     6869 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/collect_pypi_plugin.py
+-rw-r--r--   0        0        0     3033 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/collect_raw_plugin.py
+-rw-r--r--   0        0        0     3698 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/collect_yum_plugin.py
+-rw-r--r--   0        0        0     4458 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/composite_collector.py
+-rw-r--r--   0        0        0     5437 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/delta_sbom.py
+-rw-r--r--   0        0        0     6434 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/oras_bundle.py
+-rw-r--r--   0        0        0     5106 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/oras_registry.py
+-rw-r--r--   0        0        0        0 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/py.typed
+-rw-r--r--   0        0        0      202 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/report_generator/__init__.py
+-rw-r--r--   0        0        0   126749 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
+-rw-r--r--   0        0        0     4635 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/report_generator/report_generator.py
+-rw-r--r--   0        0        0    60554 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
+-rw-r--r--   0        0        0      518 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/report_generator/scripts/custom.js
+-rw-r--r--   0        0        0   220780 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
+-rw-r--r--   0        0        0     3562 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/report_generator/styles/custom.css
+-rw-r--r--   0        0        0     5052 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/report_generator/templates/component_card.jinja2
+-rw-r--r--   0        0        0     1230 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
+-rw-r--r--   0        0        0     7246 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/core_plugins/report_generator/templates/index.jinja2
+-rw-r--r--   0        0        0      458 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/exceptions.py
+-rw-r--r--   0        0        0     6787 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/in_toto.py
+-rw-r--r--   0        0        0     4260 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/logger.py
+-rw-r--r--   0        0        0     2926 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/main.py
+-rw-r--r--   0        0        0     1627 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/models/__init__.py
+-rw-r--r--   0        0        0     1602 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/models/__main__.py
+-rw-r--r--   0        0        0     1546 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/models/base.py
+-rw-r--r--   0        0        0     4001 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/models/credentials.py
+-rw-r--r--   0        0        0    13082 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/models/manifest.py
+-rw-r--r--   0        0        0        0 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/models/py.typed
+-rw-r--r--   0        0        0    21045 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/models/sbom.py
+-rw-r--r--   0        0        0     4680 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/models/transfer.py
+-rw-r--r--   0        0        0     5629 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/models/types.py
+-rw-r--r--   0        0        0     2335 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/net.py
+-rw-r--r--   0        0        0     4251 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/oci_artifacts.py
+-rw-r--r--   0        0        0     1332 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/plugin_utils.py
+-rw-r--r--   0        0        0    31217 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/processor.py
+-rw-r--r--   0        0        0        0 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/py.typed
+-rw-r--r--   0        0        0    22579 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/resources/hoppr-hippo.ansi
+-rw-r--r--   0        0        0    19725 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/resources/hoppr-hippo.ascii
+-rw-r--r--   0        0        0     4095 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/result.py
+-rw-r--r--   0        0        0     9631 2023-08-23 13:07:23.000000 hoppr-1.9.5/hoppr/utils.py
+-rw-r--r--   0        0        0     5285 2023-08-23 13:07:23.000000 hoppr-1.9.5/pyproject.toml
+-rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 hoppr-1.9.5/PKG-INFO
```

### Comparing `hoppr-1.9.4/LICENSE` & `hoppr-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/README.md` & `hoppr-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/__init__.py` & `hoppr-1.9.5/hoppr/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 """
 Tool for manipulating bundles for airgapped transfers.
 """
 from hoppr.base_plugins.hoppr import HopprPlugin, hoppr_process, hoppr_rerunner
 from hoppr.exceptions import HopprCredentialsError, HopprError, HopprLoadDataError, HopprPluginError
+from hoppr.logger import HopprLogger
 from hoppr.models import HopprContext
 from hoppr.models.credentials import CredentialRequiredService, Credentials
 from hoppr.models.manifest import Manifest
 from hoppr.models.sbom import Component, ExternalReference, Property, Sbom
 from hoppr.models.transfer import ComponentCoverage, Transfer
 from hoppr.models.types import BomAccess, PurlType
 from hoppr.result import Result
 
+__version__ = "1.9.5"
+
 __all__ = [
+    "__version__",
     "BomAccess",
     "Component",
     "ComponentCoverage",
     "CredentialRequiredService",
     "Credentials",
     "ExternalReference",
     "hoppr_process",
     "hoppr_rerunner",
     "HopprContext",
     "HopprCredentialsError",
     "HopprError",
     "HopprLoadDataError",
+    "HopprLogger",
     "HopprPlugin",
     "HopprPluginError",
     "Manifest",
     "Property",
     "PurlType",
     "Result",
     "Sbom",
     "Transfer",
 ]
-
-__version__ = "1.9.4"
```

### Comparing `hoppr-1.9.4/hoppr/base_plugins/collector.py` & `hoppr-1.9.5/hoppr/base_plugins/collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         """
         Returns all repos listed in all BOM_PROPS_COMPONENT_SEARCH_SEQUENCE properties for this component
         """
         purl = hoppr.utils.get_package_url(comp.purl)
         purl_url = purl.qualifiers.get("repository_url")
 
         if purl_url is not None and not self.context.strict_repos:
-            return [purl_url]
+            return [purl_url] if "https://" in purl_url else [f"https://{purl_url}"]
 
         repo_list = self._get_repo_search_list(comp)
 
         if purl_url is not None:
             parsed_purl_url = self._parse_url_for_comparison(purl_url)
             for repo in repo_list:
                 parsed_repo_url = self._parse_url_for_comparison(repo)
@@ -220,25 +220,24 @@
 
         if not isinstance(result.return_obj, Component):
             return result.fail(
                 f"Collector class {type(self).__name__} process_component method returned a successful result "
                 "without updating the BOM component."
             )
 
-        missing_props = []
-        for req_prop in [
-            constants.BomProps.COLLECTION_REPOSITORY,
-            constants.BomProps.COLLECTION_DIRECTORY,
-            constants.BomProps.COLLECTION_PLUGIN,
-            constants.BomProps.COLLECTION_TIMETAG,
+        if missing_props := [
+            req_prop.value
+            for req_prop in [
+                constants.BomProps.COLLECTION_REPOSITORY,
+                constants.BomProps.COLLECTION_DIRECTORY,
+                constants.BomProps.COLLECTION_PLUGIN,
+                constants.BomProps.COLLECTION_TIMETAG,
+            ]
+            if req_prop.value not in [prop.name for prop in result.return_obj.properties or []]
         ]:
-            if req_prop.value not in [prop.name for prop in result.return_obj.properties or []]:
-                missing_props.append(req_prop.value)
-
-        if missing_props:
             return result.fail(
                 f"Collector class {type(self).__name__} process_component method returned a successful result "
                 f"without updating the following component properties: {', '.join(missing_props)}"
             )
 
         return result
```

### Comparing `hoppr-1.9.4/hoppr/base_plugins/hoppr.py` & `hoppr-1.9.5/hoppr/base_plugins/hoppr.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,16 +152,16 @@
     Decorator to ignore components which have a scope of `excluded`
     """
 
     @functools.wraps(func)
     def wrapper(self, *args, **kwargs) -> Result:
         comp = _get_component(*args, **kwargs)
         if comp is not None and str(comp.scope) in {
-            'excluded',
-            'Scope.excluded',
+            "excluded",
+            "Scope.excluded",
         }:
             return Result.excluded()
         return func(self, *args, **kwargs)
 
     return wrapper
 
 
@@ -197,17 +197,18 @@
         self,
         context: HopprContext,
         config: Optional[Dict] = None,
     ) -> None:
         self._start_time: float = 0.0
         self.config = config
         self.context = context
+
         self._logger = HopprLogger(
-            file_name=str(self.context.logfile_location),
-            log_level=self.context.log_level,
+            filename=str(self.context.logfile_location),
+            level=self.context.log_level,
             lock=self.context.logfile_lock,  # type: ignore[arg-type]
         )
 
         self.process_timeout = (self.config or {}).get("process_timeout", self.process_timeout)
 
     @abstractmethod
     def get_version(self) -> str:
@@ -302,15 +303,15 @@
                 command, check=False, shell=False, capture_output=True, cwd=cwd, timeout=self.process_timeout
             )
         except subprocess.TimeoutExpired as timeout_expired:
             self.get_logger().error(
                 'Command "%s" timed out after %d seconds', command[0], timeout_expired.timeout, indent_level=2
             )
             result = subprocess.CompletedProcess(
-                command, returncode=124, stdout=timeout_expired.stdout or b'', stderr=timeout_expired.stderr or b''
+                command, returncode=124, stdout=timeout_expired.stdout or b"", stderr=timeout_expired.stderr or b""
             )
 
         if result.returncode != 0:
             # Prefix each line of the command's stdout and stderr with 4 spaces
             stdout_indented, stderr_indented = map(
                 lambda output: "\n".join([f"    {line}" for line in output.decode("utf-8").split("\n")]),
                 [result.stdout, result.stderr],
```

### Comparing `hoppr-1.9.4/hoppr/cli/__init__.py` & `hoppr-1.9.5/hoppr/cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 Top-level CLI application
 """
 from __future__ import annotations
 
 import ctypes
-import os
 import sys
 
 from pathlib import Path
 from platform import python_version
 
 import rich
 
 from rich.ansi import AnsiDecoder
-from typer import Option, Typer
+from typer import CallbackParam, Context, Option, Typer
+
+import hoppr.main
+import hoppr.utils
 
-from hoppr import __version__, main
 from hoppr.cli import bundle, generate, merge
+from hoppr.cli.options import basic_term_option, strict_repos_option, verbose_option
 
 # Windows flags and types
 NT_ENABLE_ECHO_INPUT = 0b0100
 NT_ENABLE_LINE_INPUT = 0b0010
 NT_ENABLE_PROCESSED_INPUT = 0b0001
 NT_CONSOLE_FLAGS = NT_ENABLE_ECHO_INPUT | NT_ENABLE_LINE_INPUT | NT_ENABLE_PROCESSED_INPUT
 NT_STD_OUTPUT_HANDLE = ctypes.c_uint(-11)
@@ -31,23 +33,22 @@
 
     nt_kernel.SetConsoleMode(nt_kernel.GetStdHandle(NT_STD_OUTPUT_HANDLE), NT_CONSOLE_FLAGS)
 
 
 app = Typer(
     name="hopctl",
     context_settings={"help_option_names": ["-h", "--help"]},
-    help="Collect, process, & bundle your software supply chain",
     no_args_is_help=True,
     pretty_exceptions_show_locals=False,
     rich_markup_mode="markdown",
 )
 
-app.add_typer(typer_instance=bundle.app)
-app.add_typer(typer_instance=generate.app)
-app.add_typer(typer_instance=merge.app)
+app.add_typer(typer_instance=bundle.app, name="bundle")
+app.add_typer(typer_instance=generate.app, name="generate")
+app.add_typer(typer_instance=merge.app, name="merge")
 
 
 # Aliases for deprecated commands to preserve backward compatibility
 generate_layout = app.command(
     name="generate-layout",
     deprecated=True,
     rich_help_panel="Deprecated",
@@ -59,14 +60,25 @@
     name="generate-schemas",
     deprecated=True,
     rich_help_panel="Deprecated",
     help="See `hopctl generate schemas` subcommand",
 )(generate.schemas)
 
 
+@app.callback()
+def hopctl(  # pylint: disable=unused-argument
+    basic_term: bool = basic_term_option,
+    strict_repos: bool = strict_repos_option,
+    verbose: bool = verbose_option,
+):
+    """
+    Collect, process, & bundle your software supply chain
+    """
+
+
 @app.command()
 def validate(
     input_files: list[Path],
     credentials_file: Path = Option(
         None,
         "-c",
         "--credentials",
@@ -80,28 +92,28 @@
         help="Specify transfer config",
         envvar="HOPPR_TRANSFER_CONFIG",
     ),
 ):  # pragma: no cover
     """
     Validate multiple manifest files for schema errors
     """
-    main.validate(input_files, credentials_file, transfer_file)
+    hoppr.main.validate(input_files, credentials_file, transfer_file)
 
 
 @app.command()
 def version():
     """
     Print version information for `hoppr`
     """
-    # TTY terminals and MacOS Terminal.app do not support ANSI multibyte characters. Print low-resolution art instead
-    suffix = ".ansi" if sys.stdout.isatty() and os.getenv("TERM_PROGRAM") != "Apple_Terminal" else ".ascii"
-    hippo_file = (Path(main.__file__).parent / "resources" / "hoppr-hippo").with_suffix(suffix)
+    # Non-TTY terminals and MacOS Terminal.app don't support ANSI multibyte characters. Print low-resolution art instead
+    suffix = ".ascii" if hoppr.utils.is_basic_terminal() else ".ansi"
+    hippo_file = (Path(hoppr.main.__file__).parent / "resources" / "hoppr-hippo").with_suffix(suffix)
 
     decoder = AnsiDecoder()
     hippo = decoder.decode(hippo_file.read_text(encoding="utf-8"))
 
     rich.print(*hippo, sep="\n")
-    rich.print(f"[green]Hoppr Framework Version[/] : {__version__}")
+    rich.print(f"[green]Hoppr Framework Version[/] : {hoppr.__version__}")
     rich.print(f"[green]Python Version         [/] : {python_version()}")
 
 
 __all__ = ["app"]
```

### Comparing `hoppr-1.9.4/hoppr/cli/bundle.py` & `hoppr-1.9.5/hoppr/cli/bundle.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from rich.table import Table
 from rich.text import Text
 from rich.tree import Tree
 from typer import Argument, Context, Option, Typer
 
 from hoppr import main, processor
 from hoppr.cli.layout import HopprBasePanel, HopprJobsPanel, HopprLayout
+from hoppr.cli.options import basic_term_option, strict_repos_option, verbose_option
 
 app = Typer(
     context_settings={"allow_interspersed_args": True, "help_option_names": ["-h", "--help"]},
     help="Run the stages specified in the transfer config file on the content specified in the manifest",
     invoke_without_command=True,
     no_args_is_help=True,
     rich_markup_mode="markdown",
@@ -152,83 +153,81 @@
         callback=manifest_callback,
         dir_okay=False,
         exists=True,
         help="Path to manifest file",
         resolve_path=True,
         show_default=False,
     ),
-    credentials_file: Optional[Path] = Option(
-        None,
-        "-c",
-        "--credentials",
-        help="Specify credentials config for services",
-        envvar="HOPPR_CREDS_CONFIG",
-    ),
-    transfer_file: Path = Option(
-        "transfer.yml",
-        "-t",
-        "--transfer",
-        help="Specify transfer config",
-        envvar="HOPPR_TRANSFER_CONFIG",
-    ),
-    log_file: Optional[Path] = Option(
-        None,
-        "-l",
-        "--log",
-        help="File to which log will be written",
-        envvar="HOPPR_LOG_FILE",
-    ),
-    verbose: bool = Option(
-        False,
-        "-v",
-        "--debug",
-        "--verbose",
-        help="Enable debug output",
-    ),
-    strict_repos: bool = Option(
-        True,
-        "--strict/--no-strict",
-        help="Utilize only manifest repositories for package collection",
-        envvar="HOPPR_STRICT_REPOS",
-    ),
     create_attestations: bool = Option(
         False,
         "-a",
         "--attest",
         help="Generate in-toto attestations",
         envvar="HOPPR_ATTESTATION",
+        show_default=False,
+    ),
+    credentials_file: Optional[Path] = Option(
+        None,
+        "-c",
+        "--credentials",
+        help="Specify credentials config for services",
+        envvar="HOPPR_CREDS_CONFIG",
+        show_default=False,
     ),
     functionary_key_path: Optional[Path] = Option(
         None,
         "-fk",
         "--functionary-key",
         help="Path to key used to sign in-toto layout",
         envvar="HOPPR_FUNCTIONARY_KEY",
+        show_default=False,
+    ),
+    functionary_key_password: Optional[str] = Option(
+        None,
+        "-fk-pass",
+        "--functionary-key-password",
+        confirmation_prompt=True,
+        envvar="HOPPR_FUNCTIONARY_KEY_PASSWORD",
+        help="Password for project owner key",
+        show_default=False,
     ),
     functionary_key_prompt: bool = Option(
         False,
         "-p",
         "--prompt",
-        help="Prompt user for project owner key's password",
-        envvar="HOPPR_PROJECT_OWNER_KEY_PROMPT",
+        help="Prompt user for functionary key's password",
+        envvar="HOPPR_FUNCTIONARY_KEY_PROMPT",
     ),
-    functionary_key_password: str = Option(
+    log_file: Optional[Path] = Option(
         None,
-        "-fk-pass",
-        "--project-owner-key-password",
-        help="Password for project owner key",
-        envvar="HOPPR_PROJECT_OWNER_KEY_PASSWORD",
+        "-l",
+        "--log",
+        help="File to which log will be written",
+        envvar="HOPPR_LOG_FILE",
+        show_default=False,
     ),
     previous_delivery: Optional[Path] = Option(
         None,
         "-pd",
         "--previous-delivery",
         help="Path to manifest or tar bundle representing a previous delivery",
         envvar="HOPPR_PREVIOUS_DELIVERY",
+        show_default=False,
+    ),
+    transfer_file: Path = Option(
+        "transfer.yml",
+        "-t",
+        "--transfer",
+        help="Specify transfer config",
+        envvar="HOPPR_TRANSFER_CONFIG",
+        show_default=False,
     ),
+    basic_term: bool = basic_term_option,
+    strict_repos: bool = strict_repos_option,
+    verbose: bool = verbose_option,
 ):  # pragma: no cover
     """
     Run the stages specified in the transfer config
     file on the content specified in the manifest
     """
     processor.layout = HopprBundleLayout()
     processor.summary_panel = HopprBundleSummary()
```

### Comparing `hoppr-1.9.4/hoppr/cli/generate.py` & `hoppr-1.9.5/hoppr/cli/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from typer import Option, Typer
 
 from hoppr import main
 
 app = Typer(
     name="generate",
-    context_settings={"help_option_names": ['-h', '--help']},
+    context_settings={"help_option_names": ["-h", "--help"]},
     help="Generate `in-toto` keys/layout or schemas for Hoppr input files",
     no_args_is_help=True,
     pretty_exceptions_show_locals=False,
     rich_markup_mode="markdown",
 )
```

### Comparing `hoppr-1.9.4/hoppr/cli/layout.py` & `hoppr-1.9.5/hoppr/cli/layout.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from rich.console import Console, RenderableType
 from rich.containers import Lines
 from rich.layout import Layout
 from rich.panel import Panel
 from rich.progress import BarColumn, Progress, TaskID, TextColumn
 from rich.text import Text
 
-from hoppr import __version__
+import hoppr.utils
 
 # Renderable constants
 BORDER_LINES = 2
 HEADER_SIZE = 3
 
 # Padding constants
 PAD_BOTTOM = 0
@@ -108,19 +108,21 @@
         return self.width - BORDER_LINES - PAD_LEFT - PAD_RIGHT
 
     def print(self, msg: str, source: str | None = None, style: str = "") -> None:
         """
         Write a message to the console output panel
 
         Args:
-            line (str): Message to write
-            style (str): Style to apply to message string
+            msg (str): Message to write
+            source (str | None, optional): Source of the message. Defaults to None.
+            style (str, optional): Style to apply to message string. Defaults to "".
         """
         msg = msg if source is None else f"[bold cyan]{source}[/] {msg}"
         new_lines = Text.from_markup(text=msg, style=style)
+
         self.lines.extend(new_lines.wrap(console, self.get_width()))
 
         # Remove messages from top of output panel until most recent messages are visible
         output_height = self.get_height()
 
         while len(self.lines) > output_height:
             self.lines.pop(index=0)
@@ -146,15 +148,15 @@
 
     name: str = "root"
     job_id_map: MutableMapping[str, TaskID] = {}
     jobs_panel = HopprJobsPanel()
     output_panel = HopprOutputPanel()
     overall_progress = HopprProgressPanel()
 
-    def __init__(self, title: str = f"Hoppr v{__version__}") -> None:
+    def __init__(self, title: str = f"Hoppr v{hoppr.__version__}") -> None:
         super().__init__()
 
         self.split(Layout(name="header", size=HEADER_SIZE), Layout(name="main"))
         self["main"].split_row(Layout(name="side"), Layout(name="console", ratio=OUTPUT_PANEL_RATIO_SIZE))
         self["side"].split(Layout(name="jobs"), Layout(name="progress", size=3))
 
         # Initialize header
@@ -170,16 +172,17 @@
         self.progress_task.total = 0
 
         # Initialize main body panel
         self["console"].update(renderable=self.output_panel)
 
         # Set size attributes for output console renderable
         render_map = self.render(console, console.options)
-        self.output_panel.height = render_map[self["console"]].region.height
-        self.output_panel.width = render_map[self["console"]].region.width
+        region = render_map[self["console"]].region
+        self.output_panel.height = region.height
+        self.output_panel.width = region.width
 
     def add_job(self, description: str, total: int = 1, **fields) -> TaskID:
         """
         Add a job to the `jobs` side panel
 
         Args:
             description (str): Description of the job to add
@@ -214,17 +217,23 @@
         return self.jobs_panel.progress_bar.tasks[task_id].finished
 
     def print(self, msg: str, source: str | None = None, style: str = "") -> None:
         """
         Write a message to the console output panel
 
         Args:
-            line (str): Message to write
-        """
-        self.output_panel.print(msg, source, style=style)
+            msg (str): Message to write
+            source (str | None, optional): Message sender. Defaults to None.
+            style (str, optional): Style to apply to message. Defaults to "".
+        """
+        if hoppr.utils.is_basic_terminal():
+            msg = msg if source is None else f"[bold cyan]{source}[/] {msg}"
+            console.print(Text.from_markup(text=msg, style=style))
+        else:
+            self.output_panel.print(msg, source, style=style)
 
     def start_job(self, name: str):
         """
         Start a job in the jobs panel
 
         Args:
             name (str): Name of the job to start
```

### Comparing `hoppr-1.9.4/hoppr/cli/merge.py` & `hoppr-1.9.5/hoppr/cli/merge.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/constants.py` & `hoppr-1.9.5/hoppr/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Define constants used by Hoppr
 """
-
 from enum import Enum
 
 
 class BomProps(str, Enum):
     """
     SBOM Property Field Names
     """
```

### Comparing `hoppr-1.9.4/hoppr/core_plugins/bundle_tar.py` & `hoppr-1.9.5/hoppr/core_plugins/bundle_tar.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,18 +58,16 @@
         tarfile_name = default_filename
         if self.config is not None:
             tarfile_name = self.config.get("tarfile_name", default_filename)
             tarfile_name = os.path.expanduser(tarfile_name)
 
         if os.path.exists(tarfile_name):
             timestr = time.strftime("%Y%m%d-%H%M%S")
-            matches = re.search(r"^(.*?)(\.tar(\..*)?)?$", tarfile_name)
-
-            if matches:
-                tarfile_name = f"{matches.group(1)}-{timestr}{matches.group(2) if matches.group(2) is not None else ''}"
+            if matches := re.search(r"^(.*?)(\.tar(\..*)?)?$", tarfile_name):
+                tarfile_name = f"{matches[1]}-{timestr}{matches[2] if matches[2] is not None else ''}"
 
         msg = f"Bundling collected artifacts into {tarfile_name}"
         self.get_logger().info(msg)
         self.notify(msg, type(self).__name__)
 
         try:
             with tarfile.open(tarfile_name, f"x:{compression}") as tar:
```

### Comparing `hoppr-1.9.4/hoppr/core_plugins/collect_apt_plugin.py` & `hoppr-1.9.5/hoppr/core_plugins/collect_apt_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/collect_cargo_plugin.py` & `hoppr-1.9.5/hoppr/core_plugins/collect_cargo_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/collect_dnf_plugin.py` & `hoppr-1.9.5/hoppr/core_plugins/collect_dnf_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,20 @@
             *(self.debug_args if self.get_logger().is_verbose() else []),
         ]
 
         # Generate cache to use when downloading components
         result = self.run_command(command, self.password_list)
         self.get_logger().debug(msg=(f"Return Code: {result.returncode}"), indent_level=2)
         if result.returncode != 0:
+            if hoppr.utils.get_partition(config_dir).fstype == "vboxsf":
+                self.get_logger().warning(
+                    "NOTE: Possible attempt to run DNF from a shared vagrant directory('%s'). "
+                    "Recommend retrying outside of the shared vagrant directory",
+                    config_dir,
+                )
             return Result.fail(message="Failed to populate DNF cache.")
 
         return Result.success()
 
     @hoppr_rerunner
     def collect(self, comp: Component) -> Result:
         """
```

### Comparing `hoppr-1.9.4/hoppr/core_plugins/collect_docker_plugin.py` & `hoppr-1.9.5/hoppr/core_plugins/collect_docker_plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 Collector plugin for docker images
 """
-
-# pylint: disable=too-many-locals
-
 from __future__ import annotations
 
-import os
 import re
 import urllib.parse
 
+from pathlib import Path
+from subprocess import CalledProcessError
+
 from packageurl import PackageURL
 
 import hoppr.utils
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
@@ -38,102 +37,133 @@
     def get_version(self) -> str:  # pylint: disable=duplicate-code
         return __version__
 
     def __init__(self, context: HopprContext, config: dict | None = None) -> None:
         super().__init__(context=context, config=config)
         self.required_commands = (self.config or {}).get("skopeo_command", self.required_commands)
 
-    def get_image(self, url: str, purl: PackageURL, image_name: str) -> RepositoryUrl:
+    def _get_image(self, url: str, purl: PackageURL) -> RepositoryUrl:
         """
         Return the image details for skopeo to process
 
         Args:
             url (str): Repository URL
             purl (PackageURL): Purl of component to operate on
-            image_name (str): Name of image with tag
 
         Returns:
             RepositoryUrl: Image information
         """
+        # Determine if purl version contains SHA string, determine proper formatting for skopeo command
+        match purl.version:
+            case no_sha if re.search(r"^(sha256:)?[a-fA-F0-9]{12,64}$", no_sha) is None:
+                image_name = f"{purl.name}:{purl.version}"
+            case sha if sha.startswith("sha256:"):
+                image_name = f"{purl.name}@{purl.version}"
+            case _:
+                image_name = f"{purl.name}@sha256:{purl.version}"
+
         if purl.type == "oci" and "repository_url" in purl.qualifiers:
-            url = purl.qualifiers.get('repository_url', '')
-            url = url.replace(purl.name, '')
+            url = purl.qualifiers.get("repository_url", "")
+            url = url.replace(purl.name, "")
+
         source_image = RepositoryUrl(url=url) / (purl.namespace or "") / urllib.parse.quote_plus(image_name)
 
         if source_image.scheme != "docker":
             source_image = RepositoryUrl(url="docker://" + re.sub(r"^(.*://)", "", str(source_image)))
 
         return source_image
 
-    @hoppr_rerunner
-    def collect(self, comp: Component, repo_url: str, creds: CredentialRequiredService | None = None):
-        """
-        Copy a component to the local collection directory structure
+    def _get_target_path(self, repo_url: str, purl: PackageURL) -> Path:
         """
-        purl = hoppr.utils.get_package_url(comp.purl)
-        version_path = purl.version
+        Get target path for image download
 
-        # Determine if purl version contains SHA string, determine proper formatting for skopeo command
-        if re.search(r"^(sha256:)?[a-fA-F0-9]{12,64}$", purl.version) is None:
-            image_name = f"{purl.name}:{purl.version}"
+        Args:
+            repo_url (str): Repository URL
+            purl (PackageURL): Purl of component to operate on
 
-        elif purl.version.startswith("sha256:"):
-            image_name = f"{purl.name}@{purl.version}"
-        else:
-            image_name = f"{purl.name}@sha256:{purl.version}"
-            version_path = f"sha256:{purl.version}"
+        Returns:
+            Path: Filesystem location for downloaded image
+        """
+        version = re.sub(pattern=r"^(sha256:)?([a-f0-9]{64})$", repl=r"sha256:\2", string=purl.version)
 
-        version_path = urllib.parse.quote_plus(re.sub(r'^https?://', '', version_path))
+        version = urllib.parse.quote_plus(re.sub(r"^https?://", "", version))
         target_dir = self.directory_for(purl.type, repo_url, subdir=purl.namespace)
-        target_path = target_dir / f"{purl.name}@{version_path}"
 
-        source_image = self.get_image(url=repo_url, purl=purl, image_name=image_name)
+        return target_dir / f"{purl.name}@{version}"
 
-        if purl.type == "oci" and "tag" in purl.qualifiers:
-            command = ["skopeo", "inspect", "--format", "{{.Digest}}"]
-            command = [*command, f"{os.path.split(source_image.url)[0]}/{purl.name}:{purl.qualifiers.get('tag')}"]
-            inspect_command = self.run_command(command)
+    def _inspect_image(self, source_image: RepositoryUrl, purl: PackageURL) -> Result:
+        """
+        Verify provided image tag digest matches PURL version
 
-            if inspect_command.returncode != 0:
-                return Result.retry(message=f"Failed to get image digest for '{source_image}'")
+        Args:
+            source_image (RepositoryUrl): Full image name
+            purl (PackageURL): Purl of component to operate on
+
+        Returns:
+            Result: The result of the verification
+        """
+        image_prefix, _ = source_image.url.rsplit("/", maxsplit=1)
+        image_id = f"{purl.name}:{purl.qualifiers.get('tag')}"
+
+        command = [self.required_commands[0], "inspect", "--format", "{{.Digest}}", f"{image_prefix}/{image_id}"]
+        inspect_command = self.run_command(command)
 
+        try:
+            inspect_command.check_returncode()
             sha_tag = inspect_command.stdout.decode().strip()
-            if sha_tag != purl.version:
-                return Result.fail(
-                    message=f"Provided tag '{purl.qualifiers.get('tag')}' image digest does not match '{purl.version}'"
-                )
+        except CalledProcessError:
+            return Result.retry(message=f"Failed to get image digest for '{source_image}'")
+
+        if sha_tag != purl.version:
+            return Result.fail(
+                message=f"Provided tag '{purl.qualifiers.get('tag')}' image digest does not match '{purl.version}'"
+            )
+
+        return Result.success()
+
+    @hoppr_rerunner
+    def collect(self, comp: Component, repo_url: str, creds: CredentialRequiredService | None = None):
+        """
+        Copy a component to the local collection directory structure
+        """
+        purl = hoppr.utils.get_package_url(comp.purl)
+        source_image = self._get_image(url=repo_url, purl=purl)
+        target_path = self._get_target_path(repo_url, purl)
+
+        if purl.type == "oci" and "tag" in purl.qualifiers:
+            if not (inspect_result := self._inspect_image(source_image, purl)).is_success():
+                return inspect_result
 
         self.get_logger().info(msg=f"Copying {purl.type} image:", indent_level=2)
         self.get_logger().info(msg=f"source: {source_image}", indent_level=3)
         self.get_logger().info(msg=f"destination: {target_path}", indent_level=3)
 
         command = [self.required_commands[0], "copy"]
-
         password_list = []
 
         if creds is not None:
             password_list = [creds.password.get_secret_value()]
-            command.extend(["--src-creds", f"{creds.username}:{creds.password.get_secret_value()}"])
+            command = [*command, "--src-creds", f"{creds.username}:{creds.password.get_secret_value()}"]
 
         if re.match("^http://", repo_url):
             command = [*command, "--src-tls-verify=false"]
 
         if self.get_logger().is_verbose():
             command = [*command, "--debug"]
 
         command = [*command, urllib.parse.unquote(str(source_image)), f"{purl.type}-archive:{target_path}"]
+        copy_result = self.run_command(command, password_list)
 
-        proc = self.run_command(command, password_list)
-
-        if proc.returncode != 0:
-            msg = f"Skopeo failed to copy {purl.type} image to {target_path}, return_code={proc.returncode}"
+        try:
+            copy_result.check_returncode()
+        except CalledProcessError as ex:
+            msg = f"Skopeo failed to copy {purl.type} image to {target_path}, return_code={ex.returncode}"
             self.get_logger().debug(msg=msg, indent_level=2)
 
-            if target_path.exists():
-                self.get_logger().info(msg="Artifact collection failed, deleting file and retrying", indent_level=2)
-                target_path.unlink()
+            self.get_logger().info(msg="Artifact collection failed, deleting file and retrying", indent_level=2)
+            target_path.unlink(missing_ok=True)
 
             return Result.retry(message=msg)
 
-        self.set_collection_params(comp, repo_url, target_dir)
+        self.set_collection_params(comp, repo_url, target_path.parent)
 
         return Result.success(return_obj=comp)
```

### Comparing `hoppr-1.9.4/hoppr/core_plugins/collect_git_plugin.py` & `hoppr-1.9.5/hoppr/core_plugins/collect_git_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,17 @@
         if git_src.startswith("ssh://") and source_creds is not None:
             git_src = git_src.replace("ssh://", f"ssh://{source_creds.username}@")
 
         if not git_src.endswith(".git"):
             git_src += ".git"
 
         opts: list[str] = []
-        if str(comp.version).strip():
-            opts = [*opts, "--branch", str(comp.version)]
+
+        if comp.version:
+            opts = [*opts, "--branch", comp.version]
 
         # Allow for further depth (default: 1)
         depth = (self.config or {}).get("depth", "1")
 
         # Recognize the 'all' keyword as requesting all history
         if str(depth).lower() != "all":
             opts = [*opts, "--depth", str(depth)]
```

### Comparing `hoppr-1.9.4/hoppr/core_plugins/collect_golang_plugin.py` & `hoppr-1.9.5/hoppr/core_plugins/collect_golang_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/collect_helm_plugin.py` & `hoppr-1.9.5/hoppr/core_plugins/collect_helm_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/collect_maven_plugin.py` & `hoppr-1.9.5/hoppr/core_plugins/collect_maven_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/collect_nexus_search.py` & `hoppr-1.9.5/hoppr/core_plugins/collect_nexus_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,18 +100,17 @@
         self.set_collection_params(comp, repo_url, target_dir)
         return Result.success(return_obj=comp)
 
     @staticmethod
     def _parse_nexus_url(repo_url: str) -> tuple[str, str | None]:
         nexus_url = repo_url
         nexus_repo = None
-        repo_specified = re.search(r"(https?://.*?)/repository/(.*?)(/.*)?$", repo_url)
-        if repo_specified:
-            nexus_url = repo_specified.group(1)
-            nexus_repo = repo_specified.group(2)
+        if repo_specified := re.search(r"(https?://.*?)/repository/(.*?)(/.*)?$", nexus_url):
+            nexus_url = repo_specified[1]
+            nexus_repo = repo_specified[2]
 
         return (nexus_url, nexus_repo)
 
     def _directory_for_nexus(self, purl: PackageURL, url: str) -> Path:
         if repo_match := re.search(r"(.*?/repository/.*?)(/.*)?/(.*)", url):
             nexus_repo = repo_match[1]
             path = repo_match[2]
@@ -212,18 +211,17 @@
                         url_list.append(item["downloadUrl"])
                         break
 
         return url_list
 
     @classmethod
     def get_attestation_products(cls, config: dict | None = None) -> list[str]:
-        products = []
-        if config is not None and "purl_types" in config:
-            for purl_type in config["purl_types"]:
-                products.append(purl_type + "/*")
+        products: list[str] = []
 
+        if config is not None and "purl_types" in config:
+            products.extend(f"{purl_type}/*" for purl_type in config["purl_types"])
         else:
-            for purl_type in PurlType:
-                if str(purl_type) not in ["git", "github", "gitlab"]:
-                    products.append(str(purl_type) + "/*")
+            products.extend(
+                f"{purl_type}/*" for purl_type in PurlType if str(purl_type) not in ["git", "github", "gitlab"]
+            )
 
         return products
```

### Comparing `hoppr-1.9.4/hoppr/core_plugins/collect_npm_plugin.py` & `hoppr-1.9.5/hoppr/core_plugins/collect_npm_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/collect_nuget_plugin.py` & `hoppr-1.9.5/hoppr/core_plugins/collect_nuget_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/collect_pypi_plugin.py` & `hoppr-1.9.5/hoppr/core_plugins/collect_pypi_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,18 +88,15 @@
         base_error_msg = f"Failed to download {purl.name} version {purl.version}"
 
         collection_type = "binary-preferred"
         if self.config is not None and "type" in self.config:
             collection_type = str(self.config["type"]).lower()
 
         success_count = 0
-        successes_needed = 1
-        if collection_type == "both-required":
-            successes_needed = 2
-
+        successes_needed = 2 if collection_type == "both-required" else 1
         match collection_type:
             case "binary" | "binary-only" | "binary-preferred" | "both-preferred" | "both-required":
                 type_order = ["binary", "source"]
             case "source" | "source-only" | "source-preferred":
                 type_order = ["source", "binary"]
             case _:
                 return Result.fail(
```

### Comparing `hoppr-1.9.4/hoppr/core_plugins/collect_raw_plugin.py` & `hoppr-1.9.5/hoppr/core_plugins/collect_raw_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/collect_yum_plugin.py` & `hoppr-1.9.5/hoppr/core_plugins/collect_yum_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/composite_collector.py` & `hoppr-1.9.5/hoppr/core_plugins/composite_collector.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/delta_sbom.py` & `hoppr-1.9.5/hoppr/core_plugins/delta_sbom.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,30 +62,27 @@
         with (target_dir / "_previous_bom.json").open(mode="w", encoding="utf-8") as bom_data:
             bom_data.write(previous_sbom.json(exclude_none=True, by_alias=True, indent=2))
 
         delta_sbom = self.context.delivered_sbom.copy(deep=True)
         delta_sbom.components.clear()
 
         for new_comp in self.context.delivered_sbom.components or []:
-            include_component = True
-            for prev_comp in previous_sbom.components or []:
-                if DeltaSbom._component_match(new_comp, prev_comp):
-                    include_component = False
-                    break
-
+            include_component = not any(
+                DeltaSbom._component_match(new_comp, prev_comp) for prev_comp in previous_sbom.components or []
+            )
             if include_component:
                 self.get_logger().debug("Including purl %s", new_comp.purl, indent_level=1)
                 delta_sbom.components.append(new_comp)
 
         self.get_logger().info("Input sbom has %d components", len(self.context.delivered_sbom.components))
         self.get_logger().info("Prev  sbom has %d components", len(previous_sbom.components))
         self.get_logger().info("Delta sbom has %d components", len(delta_sbom.components))
 
         if len(delta_sbom.components) == 0:
-            return Result.fail(f"No components updated since \"{previous_source}\".")
+            return Result.fail(f'No components updated since "{previous_source}".')
 
         return Result.success(
             f"Delivering updates for {len(delta_sbom.components)} of "
             f"{len(self.context.delivered_sbom.components)} components.",
             return_obj=delta_sbom,
         )
```

### Comparing `hoppr-1.9.4/hoppr/core_plugins/oras_bundle.py` & `hoppr-1.9.5/hoppr/core_plugins/oras_bundle.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,14 @@
             media_type = "application/vnd.oci.image.layer.v1.tar"
             size = Path(filename).stat().st_size  # bytes
             annotations = {"creationTime": str(now), "size": str(size)}
             if str(root_dir / "generic" / "_metadata_" / "_delivered_bom.json") == filename:
                 media_type = "application/vnd.cyclonedx"
             elif str(root_dir / "generic" / "_metadata_" / "_consolidated_bom.json") == filename:
                 media_type = "application/vnd.cyclonedx"
-                media_type = 'application/vnd.cyclonedx'
             archives.append(
                 {
                     "path": filename,
                     "title": filename.replace(f"{root_dir}/", "", -1),
                     "media_type": media_type,
                     "annotations": annotations,
                 }
```

### Comparing `hoppr-1.9.4/hoppr/core_plugins/oras_registry.py` & `hoppr-1.9.5/hoppr/core_plugins/oras_registry.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png` & `hoppr-1.9.5/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/report_generator/report_generator.py` & `hoppr-1.9.5/hoppr/core_plugins/report_generator/report_generator.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js` & `hoppr-1.9.5/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/report_generator/scripts/custom.js` & `hoppr-1.9.5/hoppr/core_plugins/report_generator/scripts/custom.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/report_generator/styles/bootstrap.min.css` & `hoppr-1.9.5/hoppr/core_plugins/report_generator/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/report_generator/styles/custom.css` & `hoppr-1.9.5/hoppr/core_plugins/report_generator/styles/custom.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/report_generator/templates/component_card.jinja2` & `hoppr-1.9.5/hoppr/core_plugins/report_generator/templates/component_card.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/report_generator/templates/general_summary.jinja2` & `hoppr-1.9.5/hoppr/core_plugins/report_generator/templates/general_summary.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/core_plugins/report_generator/templates/index.jinja2` & `hoppr-1.9.5/hoppr/core_plugins/report_generator/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/in_toto.py` & `hoppr-1.9.5/hoppr/in_toto.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,17 @@
     """
     Function to determine what products are produced for each "hoppr stage"/"in-toto step".
 
     This is done by looking at all plugins in a stage, and create a list of "products". There
     are two additional "products" included in each step/stage which are a consolidated bom
     and a delivered bom.
     """
-    products = {}
-    stages = []
-
-    stages.append("_collect_metadata")
-    products["_collect_metadata"] = ["generic/_metadata_/*"]
+    stages = ["_collect_metadata"]
 
+    products = {"_collect_metadata": ["generic/_metadata_/*"]}
     for stage_ref in transfer.stages:
         stages.append(stage_ref.name)
 
         products[stage_ref.name] = []
         for plugin_ref in stage_ref.plugins:
             plugin_cls = plugin_class(plugin_ref.name)
             products[stage_ref.name] += plugin_cls.get_attestation_products(plugin_ref.config)
@@ -73,22 +70,22 @@
 
     layout = Layout()
     layout.set_relative_expiration(months=relative_expiration)
 
     project_owner_key = interface.import_privatekey_from_file(
         str(project_owner_key_path), password=project_owner_key_password
     )
-    functionary_pubkey = layout.add_functionary_key_from_path(str(functionary_key_path) + ".pub")
+    functionary_pubkey = layout.add_functionary_key_from_path(f"{str(functionary_key_path)}.pub")
 
     (products, stages) = _get_products(transfer)
 
     for i, stage in enumerate(stages):
         step = Step(name=stage, pubkeys=[functionary_pubkey["keyid"]])
 
-        for j in range(0, i):
+        for j in range(i):
             step.add_material_rule_from_string(f"MATCH * WITH PRODUCTS FROM {stages[j]}")
 
         for product in products[stage]:
             step.add_product_rule_from_string(f"ALLOW {product}")
 
         step.add_material_rule_from_string("DISALLOW *")
         step.add_product_rule_from_string("DISALLOW *")
```

### Comparing `hoppr-1.9.4/hoppr/logger.py` & `hoppr-1.9.5/hoppr/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 from __future__ import annotations
 
 import functools
 import inspect
 import itertools
 import logging
 
-from logging import FileHandler, Formatter, Logger
+from logging import FileHandler, Formatter, Logger, LoggerAdapter
 from logging.handlers import MemoryHandler
 from threading import _RLock as RLock
-from threading import get_ident
-from typing import Callable
+from typing import Callable, MutableMapping, cast
 
 
 def locked(func: Callable) -> Callable:
     """
     Acquire logfile lock, run the wrapped function, then release the lock
     """
 
@@ -29,135 +28,115 @@
 
         if self.lock:
             self.lock.release()
 
     return wrapper
 
 
-class HopprLogger(Logger):
+class HopprLogger(LoggerAdapter):
     """
     Logger that buffers log records in memory until flushed
     """
 
     id_iter = itertools.count()
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
-        file_name: str,
+        name: str | None = None,
+        filename: str = "hoppr.log",
+        level: int = logging.INFO,
         lock: RLock | None = None,
-        log_name: str | None = None,
-        log_level: int = logging.INFO,
         flush_immed: bool = False,
     ) -> None:
-        self.file_name = file_name
-        self.flush_immed = flush_immed
-        self.instance_id = next(self.id_iter)
-        self.lock = lock
+        """
+        Initialize the logger, formatter, and handlers
+
+        Args:
+            name (str | None, optional): Name to assign the logger. Defaults to None.
+            filename (str, optional): Log file to create. Defaults to "hoppr.log".
+            level (int, optional): Logging level. Defaults to logging.INFO.
+            lock (RLock | None, optional): Lock object to acquire/release when writing to log file. Defaults to None.
+            flush_immed (bool, optional): Flush immediately when logging. Defaults to False.
+        """
+        self.extra: MutableMapping[str, object]
+        self.logger: Logger
+
+        self.filename = filename
+        self.flush_immed: bool = flush_immed
+        self.instance_id: int = next(self.id_iter)
+        self.lock: RLock | None = lock
 
-        caller = inspect.stack()[1].function
+        _, frame_info, *_ = inspect.stack(context=2)
+        caller = frame_info.function
 
-        caller_cls = inspect.stack()[1].frame.f_locals.get("self", None)
-        if caller_cls is not None:
+        if (caller_cls := frame_info.frame.f_locals.get("self")) is not None:
             caller = type(caller_cls).__name__
 
-        log_name = log_name or f"{caller}-{get_ident()}-{self.instance_id}"
+        extra = cast(MutableMapping, {})
+        extra["caller"] = caller
 
-        super().__init__(name=log_name, level=log_level)
+        name = f"{name}-{self.instance_id}" if name else f"{caller}-{self.instance_id}"
+
+        logger = logging.getLogger(name)
+        logger.setLevel(level)
 
         formatter = Formatter(
             fmt="[$asctime] - [${caller}] - [$levelname] - $message",
             style="$",
             defaults={"caller": caller},
         )
 
-        file_handler = FileHandler(file_name)
+        file_handler = FileHandler(filename)
         file_handler.setFormatter(formatter)
 
-        self.log_handler = MemoryHandler(10000, flushLevel=logging.CRITICAL, target=file_handler)
+        log_handler = MemoryHandler(10000, flushLevel=logging.CRITICAL, target=file_handler)
+        logger.addHandler(log_handler)
 
-        self.addHandler(self.log_handler)
+        super().__init__(logger, extra)
 
-    def is_verbose(self) -> bool:
-        """
-        Check whether running with `--debug`/`--verbose` flag
+    def clear_targets(self) -> None:
         """
-        return self.level == logging.DEBUG
+        Set target for all MemoryHandlers in this logger to None
 
-    @locked
-    def flush(self) -> None:
-        """
-        Flush all handlers for this logger
+        Thus when these handlers are flushed, nothing will go to standard output
         """
-        for handler in self.handlers:
-            handler.flush()
+        for handler in self.logger.handlers:
+            if isinstance(handler, MemoryHandler):
+                handler.setTarget(None)
 
     @locked
     def close(self) -> None:
         """
         Close (and flush) all handlers for this logger
         """
-        for handler in self.handlers:
+        for handler in self.logger.handlers:
             handler.close()
 
-    def clear_targets(self) -> None:
+    @locked
+    def flush(self) -> None:
+        """
+        Flush all handlers for this logger
         """
-        Makes the target for all Memory Handlers in this logger None
+        for handler in self.logger.handlers:
+            handler.flush()
 
-        Thus when these handlers are flushed, nothing will go to standard output
+    def is_verbose(self) -> bool:
         """
-        for handler in self.handlers:
-            if isinstance(handler, MemoryHandler):
-                handler.setTarget(None)
+        Check whether running with `--debug`/`--verbose` flag
+        """
+        return self.logger.level == logging.DEBUG
 
-    def log(self, level: int, msg: str, *args, indent_level: int = 0, **kwargs) -> None:  # type: ignore[override]
+    def log(self, level: int, msg: object, *args, **kwargs) -> None:
         """
         Wrapper function for logging messages
         """
-        indent_string = " " * 4 * indent_level
-        msg = f"{indent_string}{msg}"
-
-        filename, lno, func, sinfo = self.findCaller(stack_info=False, stacklevel=1)
-        record = self.makeRecord(
-            self.name, level, filename, lno, msg, args, exc_info=None, func=func, extra=None, sinfo=sinfo
-        )
-
-        if level >= self.level:
-            self.log_handler.buffer.append(record)
+        super().log(level, msg, *args, **kwargs)
 
         if self.flush_immed:
             self.flush()
 
-    def debug(self, msg: str, *args, indent_level: int = 0, **kwargs) -> None:  # type: ignore[override]
-        """
-        Wrapper function for debug messages
-        """
-        self.log(logging.DEBUG, msg, *args, indent_level=indent_level, **kwargs)
-
-    def info(self, msg: str, *args, indent_level: int = 0, **kwargs) -> None:  # type: ignore[override]
-        """
-        Wrapper function for info messages
-        """
-        self.log(logging.INFO, msg, *args, indent_level=indent_level, **kwargs)
-
-    def warning(self, msg: str, *args, indent_level: int = 0, **kwargs) -> None:  # type: ignore[override]
-        """
-        Wrapper function for warn messages
-        """
-        self.log(logging.WARNING, msg, *args, indent_level=indent_level, **kwargs)
-
-    def error(self, msg: str, *args, indent_level: int = 0, **kwargs) -> None:  # type: ignore[override]
-        """
-        Wrapper function for error messages
-        """
-        self.log(logging.ERROR, msg, *args, indent_level=indent_level, **kwargs)
-
-    def fatal(self, msg: str, *args, indent_level: int = 0, **kwargs) -> None:  # type: ignore[override]
-        """
-        Wrapper function for fatal messages
-        """
-        self.log(logging.FATAL, msg, *args, indent_level=indent_level, **kwargs)
+    def process(self, msg: str, kwargs: MutableMapping[str, object]) -> tuple[str, MutableMapping[str, object]]:
+        indent_level = cast(int, kwargs.pop("indent_level", 0))
+        indent_string = " " * 4 * indent_level
+        msg = f"{indent_string}{msg}"
 
-    def critical(self, msg: str, *args, indent_level: int = 0, **kwargs) -> None:  # type: ignore[override]
-        """
-        Wrapper function for critical messages
-        """
-        self.log(logging.CRITICAL, msg, *args, indent_level=indent_level, **kwargs)
+        return super().process(msg, kwargs)
```

### Comparing `hoppr-1.9.4/hoppr/main.py` & `hoppr-1.9.5/hoppr/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 import sys
 
 from pathlib import Path
 from typing import List, Optional
 
 from typer import Exit, echo, prompt
 
-from hoppr import __version__
 from hoppr.in_toto import generate_in_toto_layout
 from hoppr.models.credentials import Credentials
 from hoppr.models.manifest import Manifest
 from hoppr.models.transfer import Transfer
 from hoppr.processor import HopprProcessor
 
 
-def bundle(  # pylint: disable=too-many-arguments,too-many-locals
+def bundle(  # pylint: disable=too-many-arguments, too-many-locals, unused-argument
     manifest_file: Path,
     credentials_file: Optional[Path],
     transfer_file: Path,
     log_file: Optional[Path],
     verbose: bool = False,
     strict_repos: bool = True,
     create_attestations: bool = False,
     functionary_key_path: Optional[Path] = None,
     functionary_key_prompt: bool = False,
     functionary_key_password: Optional[str] = None,
     previous_delivery: Optional[Path] = None,
+    basic_term: bool = False,
 ):
     """
     Run the stages specified in the transfer config
     file on the content specified in the manifest
     """
     log_level = logging.DEBUG if verbose else logging.INFO
```

### Comparing `hoppr-1.9.4/hoppr/models/__init__.py` & `hoppr-1.9.5/hoppr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/models/__main__.py` & `hoppr-1.9.5/hoppr/models/__main__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/models/base.py` & `hoppr-1.9.5/hoppr/models/base.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/models/credentials.py` & `hoppr-1.9.5/hoppr/models/credentials.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/models/manifest.py` & `hoppr-1.9.5/hoppr/models/manifest.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/models/sbom.py` & `hoppr-1.9.5/hoppr/models/sbom.py`

 * *Files 2% similar despite different names*

```diff
@@ -466,14 +466,17 @@
         def _unescape_unicode(value: str) -> str:
             # Decode any unicode escape sequences, e.g. "\u0026" -> "&"
             return value.encode(encoding="utf-8").decode()
 
         if values.get("purl"):
             values["purl"] = _unescape_unicode(str(values["purl"]))
 
+            if not values.get("version") and (version := hoppr.utils.get_package_url(values["purl"]).version):
+                values["version"] = version
+
         bom_ref = str(
             values.get("purl")
             or f"{'@'.join(filter(None, [values.get('name'), values.get('version')]))}"
             or values.get("bom-ref")
         )
 
         values["bom-ref"] = _unescape_unicode(bom_ref)
```

### Comparing `hoppr-1.9.4/hoppr/models/transfer.py` & `hoppr-1.9.5/hoppr/models/transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,13 +157,9 @@
             case str() | Path():
                 return cls.parse_file(source)
             case _:
                 raise TypeError("'source' argument must be one of: 'str', 'Path', 'dict[str, Any]'")
 
     def yaml(self, *args, **kwargs) -> str:
         transfer_dict = self.dict(by_alias=True)
-        transfer_dict["stages"] = {}
-
-        for stage in self.stages:
-            transfer_dict["stages"][str(stage.name)] = {"plugins": stage.plugins}
-
+        transfer_dict["stages"] = {str(stage.name): {"plugins": stage.plugins} for stage in self.stages}
         return TransferFile.parse_obj(transfer_dict).yaml(*args, **kwargs)
```

### Comparing `hoppr-1.9.4/hoppr/models/types.py` & `hoppr-1.9.5/hoppr/models/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         values["url"] = "/".join(filter(None, [values["url"], values["path"].strip("/") if values.get("path") else ""]))
         values["url"] = "?".join(filter(None, [values["url"], values.get("query")]))
         values["url"] = "#".join(filter(None, [values["url"], values.get("fragment")]))
 
         return values
 
     def __repr__(self) -> str:
-        props = ", ".join(f'{name}={repr(value)}' for name, value in dict(self).items())
+        props = ", ".join(f"{name}={repr(value)}" for name, value in dict(self).items())
         return f"RepositoryUrl({props})"
 
     def __str__(self) -> str:
         return self.url
 
     def __truediv__(self, other: str) -> RepositoryUrl:
         return self.join(other)
```

### Comparing `hoppr-1.9.4/hoppr/net.py` & `hoppr-1.9.5/hoppr/net.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/oci_artifacts.py` & `hoppr-1.9.5/hoppr/oci_artifacts.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/plugin_utils.py` & `hoppr-1.9.5/hoppr/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/processor.py` & `hoppr-1.9.5/hoppr/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Run Hoppr processing, using multiple processors
 """
 from __future__ import annotations
 
+import importlib
 import logging
 import os
 import shutil
 import socket
 import sys
 import tempfile
 import time
@@ -24,28 +25,26 @@
 
 import jmespath
 
 from rich.live import Live
 
 import hoppr.utils
 
-from hoppr.base_plugins.hoppr import HopprPlugin
 from hoppr.cli.layout import console
 from hoppr.core_plugins.report_generator import Report, ReportGenerator
 from hoppr.exceptions import HopprPluginError
 from hoppr.in_toto import HopprInTotoLinks
 from hoppr.logger import HopprLogger
 from hoppr.models import HopprContext
 from hoppr.models.credentials import Credentials
 from hoppr.models.manifest import Manifest, ManifestFile
 from hoppr.models.sbom import Component, Sbom
 from hoppr.models.transfer import ComponentCoverage, Plugin, StageRef, Transfer
 from hoppr.models.types import BomAccess
 from hoppr.result import Result
-from hoppr.utils import plugin_class, plugin_instance
 
 # Import on Unix systems only
 if os.name == "posix":
     import pwd
 
 if TYPE_CHECKING:
     from hoppr.cli.bundle import HopprBundleLayout, HopprBundleSummary
@@ -64,19 +63,19 @@
     """
     Runs a single method for a single component (if supplied) on a single plugin
     """
     plugin = hoppr.utils.plugin_instance(plugin_name, context, config)
     plugin.subscribe(observer=layout, callback=layout.print)  # pyright: ignore
 
     match method_name:
-        case HopprPlugin.pre_stage_process.__name__:
+        case "pre_stage_process":
             result = plugin.pre_stage_process()
-        case HopprPlugin.process_component.__name__:
+        case "process_component":
             result = plugin.process_component(component)
-        case HopprPlugin.post_stage_process.__name__:
+        case "post_stage_process":
             result = plugin.post_stage_process()
         case _:
             result = Result.fail(f"Invalid method: {method_name}")
 
     if result.return_obj is not None and not plugin.bom_access.has_access_to(result.return_obj):
         result = Result.fail(
             f"Plugin {type(plugin).__name__} has BOM access level {plugin.bom_access.name}, "
@@ -89,15 +88,15 @@
 
 
 class StageProcessor:  # pylint: disable=too-few-public-methods
     """
     Class to handle all processing within a single Hoppr stage
     """
 
-    component_based_methods = [HopprPlugin.process_component.__name__]
+    component_based_methods = ["process_component"]
 
     def __init__(self, stage_ref: StageRef, context: HopprContext, logger: HopprLogger):
         self.context = context
         self.logger = logger
         self.plugin_ref_list = stage_ref.plugins
         self.required_coverage = ComponentCoverage.OPTIONAL
         self.results: dict[str, list[tuple[str, str | None, Result]]] = {}
@@ -123,39 +122,39 @@
         result = self._check_bom_access()
         if not result.is_success():
             return result
 
         # Run each sub-stage (pre_stage_process, process_component, post_stage_process)
         # for all plugins (and, for process_component, for all components).
         # Each sub-stage must complete before the next can begin
-        output_width = layout.output_panel.get_width()
+        output_width = console.width if hoppr.utils.is_basic_terminal() else layout.output_panel.get_width()
 
-        plugins = [plugin_class(plugin.name) for plugin in self.plugin_ref_list]
+        plugins = [hoppr.utils.plugin_class(plugin.name) for plugin in self.plugin_ref_list]
 
         layout.overall_progress.title = f"[bold blue]Stage: {self.stage_id}"
 
         # Increment overall progress bar total by 2 to account for pre and post processing steps
         layout.progress_task.total = (layout.progress_task.total or 0) + 2
 
         def _method_label(method_name: str, label: str):
             "Print label for method if the named method is defined directly in the plugin class"
             if any(method_name in plugin.__dict__ for plugin in plugins):
                 layout.progress_task.description = label.capitalize()
                 layout.print("", source="")
                 layout.print(f" Stage: {self.stage_id} ({label}) ".center(output_width, "="))
 
         _method_label("pre_stage_process", "pre-processing")
-        result.merge(self._run_all(HopprPlugin.pre_stage_process.__name__))
+        result.merge(self._run_all("pre_stage_process"))
         layout.overall_progress.progress_bar.advance(layout.progress_task.id)
 
         _method_label("collect", "processing")
-        result.merge(self._run_all(HopprPlugin.process_component.__name__))
+        result.merge(self._run_all("process_component"))
 
         _method_label("post_stage_process", "post-processing")
-        result.merge(self._run_all(HopprPlugin.post_stage_process.__name__))
+        result.merge(self._run_all("post_stage_process"))
         layout.overall_progress.progress_bar.advance(layout.progress_task.id)
 
         return result
 
     def _populate_futures(self, method_name: str) -> tuple[int, int]:
         """
         Run the named method for all plugins.
@@ -167,27 +166,31 @@
         def _components():
             yield from self.context.delivered_sbom.components or []
 
         with ThreadPoolExecutor(max_workers=self.context.max_processes, thread_name_prefix=self.stage_id) as executor:
             failures = 0
             retries = 0
 
+            # Prevent circular import
+            base_cls = getattr(importlib.import_module(name="hoppr.base_plugins.hoppr"), "HopprPlugin")
+
             for plugin in self.plugin_ref_list:
-                plugin_cls = plugin_class(plugin.name)
+                plugin_cls = hoppr.utils.plugin_class(plugin.name)
 
-                if getattr(plugin_cls, method_name) == getattr(HopprPlugin, method_name):
+                # Skip plugin if method not defined in class directly
+                if getattr(plugin_cls, method_name) == getattr(base_cls, method_name):
                     continue
 
                 if method_name in self.component_based_methods:
                     layout.start_job(plugin_cls.__name__)
 
                     # Create one concurrent future object to run this method for each component
                     for component in _components():
                         if component.purl:
-                            instance = plugin_instance(plugin.name, self.context, plugin.config)
+                            instance = hoppr.utils.plugin_instance(plugin.name, self.context, plugin.config)
 
                             if instance.supports_purl_type(hoppr.utils.get_package_url(component.purl).type):
                                 future_proc = executor.submit(
                                     _run_plugin,
                                     plugin_name=plugin.name,
                                     context=self.context,
                                     config=plugin.config,
@@ -235,15 +238,15 @@
         """
         for future in as_completed(future_argument_map):
             # Retrieve the result
             plugin, comp = future_argument_map[future]
             future_result: Result = future.result()
 
             if not future_result.is_skip():
-                plugin_cls = plugin_class(plugin.name)
+                plugin_cls = hoppr.utils.plugin_class(plugin.name)
 
                 if not future_result.is_excluded():
                     self._save_result(method_name, plugin_cls.__name__, future_result, comp)
                     self._update_bom(future_result.return_obj, comp)
 
                 if method_name in self.component_based_methods:
                     layout.advance_job(plugin_cls.__name__)
@@ -321,16 +324,16 @@
         for _, bom_ref, _ in self.results.get(method_name, []):
             result_count[bom_ref] = result_count.get(bom_ref, 0) + 1
 
         additional_failures = 0
         for component in self.context.delivered_sbom.components or []:
             count = result_count.get(component.purl, 0)
             if not self.required_coverage.accepts_count(count) and str(component.scope) not in {
-                'excluded',
-                'Scope.excluded',
+                "excluded",
+                "Scope.excluded",
             }:
                 bad_comp_result = Result.fail(
                     f"Component processed {count} times, {self.required_coverage.name} coverage required"
                 )
                 self._save_result(method_name, f"Stage {self.stage_id}", bad_comp_result, component)
                 self._report_result(f"Stage {self.stage_id}", component, bad_comp_result)
                 additional_failures += 1
@@ -436,15 +439,15 @@
                 plugin_cls = hoppr.utils.plugin_class(plugin_ref.name)
 
                 # Determine if plugin's `supported_purl_types` are in the set of PURL types defined in SBOM components
                 plugin_needed: bool = len(used_purl_types.intersection(plugin_cls.supported_purl_types)) > 0
 
                 if len(plugin_cls.supported_purl_types) == 0 or plugin_needed:
                     plugin_list.append(plugin_ref)
-                    instance = plugin_instance(plugin_ref.name, self.context, plugin_ref.config)
+                    instance = hoppr.utils.plugin_instance(plugin_ref.name, self.context, plugin_ref.config)
 
                     msg = f"{plugin_cls.__name__} version {instance.get_version()} from {plugin_ref.name}"
                     self.logger.info(msg, indent_level=1)
                     rundata.write(f"    {msg}\n")
 
                 # Get all components in input SBOM supported by the plugin
                 for supported in plugin_cls.supported_purl_types:
@@ -469,36 +472,47 @@
         functionary_key_password: str | None = None,
         log_level: int = logging.INFO,
         log_file: str | Path | None = None,
         strict_repos: bool = True,
         previous_delivery: Path | None = None,
     ) -> None:
         self.context: HopprContext
-        self.logger: HopprLogger
         self.live_display = Live(renderable=layout, console=console, refresh_per_second=10)
         self.log_file: Path = Path(log_file or f"hoppr_{time.strftime('%Y%m%d-%H%M%S')}.log")
         self.log_level = log_level
         self.logfile_lock = RLock()
         self.metadata_files: list[Path] = [manifest_file, transfer_file]
         self.previous_delivery = previous_delivery
         self.strict_repos: bool = strict_repos
 
-        self.live_display.start(refresh=True)
+        if not hoppr.utils.is_basic_terminal():
+            self.live_display.start(refresh=True)
 
-        layout.print(f"Loading {manifest_file.name} and {transfer_file.name} files...")
+        self.logger = self.get_logger(
+            log_name=type(self).__name__,
+            log_file=self.log_file,
+            log_level=self.log_level,
+        )
+
+        self.logger.info("Loading %s and %s files...", manifest_file.name, transfer_file.name)
         self.manifest_file = ManifestFile.parse_file(manifest_file)
         self.manifest = Manifest.load(manifest_file)
         self.transfer = Transfer.load(transfer_file)
 
         self.credentials = None
         if credentials_file is not None:
-            layout.print(f"Loading {credentials_file.name} file...")
+            self.logger.info("Loading %s file...", credentials_file.name)
             self.credentials = Credentials.load(credentials_file)
             self.metadata_files.append(credentials_file)
 
+        layout.print(f"Loading {manifest_file.name} and {transfer_file.name} files...")
+        self.manifest_file = ManifestFile.parse_file(manifest_file)
+        self.manifest = Manifest.load(manifest_file)
+        self.transfer = Transfer.load(transfer_file)
+
         self.stage_processor_map: MutableMapping[StageRef, StageProcessor] = {}
 
         self.in_toto_links = HopprInTotoLinks(
             create_attestations,
             self.transfer,
             functionary_key_path,
             functionary_key_password,
@@ -620,15 +634,20 @@
             summary_panel.failure_table.add_row()
 
         summary_panel.summary_group.renderables.append(
             f"GRAND TOTAL: {summary_panel.total_success_count} jobs "
             f"succeeded, {summary_panel.total_failure_count} failed"
         )
 
-        console.print("\n", summary_panel)
+        if hoppr.utils.is_basic_terminal():
+            console.line()
+            console.rule(title="Summary", characters="=", style="[bold]rule.line")
+            console.print(summary_panel.renderable)
+        else:
+            console.print("\n", summary_panel)
 
         self.report_gen = ReportGenerator(self.context)
         self.report_gen.generate_report()
 
         return summary_panel.total_failure_count
 
     def get_logger(
@@ -646,17 +665,17 @@
             log_level (int, optional): Logging level. Defaults to logging.INFO.
 
         Returns:
             HopprLogger: A new HopprLogger instance.
         """
         if not hasattr(self, "logger"):
             self.logger = HopprLogger(
-                file_name=str(log_file),
-                log_name=log_name or f"HopprProcessor--{get_ident()}",
-                log_level=log_level,
+                filename=str(log_file),
+                name=log_name or f"HopprProcessor--{get_ident()}",
+                level=log_level,
                 flush_immed=True,
             )
 
         return self.logger
 
     def run(self) -> Result:
         """
@@ -684,20 +703,14 @@
                 repositories=self.manifest.repositories,
                 sboms=list(Sbom.loaded_sboms.values()),
                 stages=self.transfer.stages,
                 strict_repos=self.strict_repos,
                 previous_delivery=self.previous_delivery,
             )
 
-            self.logger = self.get_logger(
-                log_name="HopprProcessor",
-                log_file=self.log_file,
-                log_level=self.log_level,
-            )
-
             if self.context.consolidated_sbom is not None and len(self.context.consolidated_sbom.components or []) == 0:
                 msg = "No SBOMs defined in manifests, or SBOMs contain no components. Nothing to process."
                 layout.print(msg, style="red")
                 return Result.fail(msg)
 
             self.in_toto_links.set_collection_root(collection_root)
             self.in_toto_links.record_stage_start("_collect_metadata")
@@ -737,14 +750,15 @@
                 self._collect_delivered_bom()
                 self.in_toto_links.record_stage_stop(stage_ref.name)
 
             self.in_toto_links.record_stage_start("_finalize")
             self._collect_delivered_bom()
             self.in_toto_links.record_stage_stop("_finalize")
 
-        self.live_display.stop()
+        if not hoppr.utils.is_basic_terminal():
+            self.live_display.stop()
 
         failed_jobs = self._summarize_results()
         if failed_jobs > 0:
             result.merge(Result.fail(f"{failed_jobs} failed during this execution"))
 
         return result
```

### Comparing `hoppr-1.9.4/hoppr/resources/hoppr-hippo.ansi` & `hoppr-1.9.5/hoppr/resources/hoppr-hippo.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/resources/hoppr-hippo.ascii` & `hoppr-1.9.5/hoppr/resources/hoppr-hippo.ascii`

 * *Files identical despite different names*

### Comparing `hoppr-1.9.4/hoppr/result.py` & `hoppr-1.9.5/hoppr/result.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,15 +129,18 @@
     def from_http_response(response: requests.Response, return_obj: Any = None):
         """
         Build a Result object from an HTTP request response
         """
 
         match response.status_code:
             case response_code if 200 <= response_code <= 299:
-                return Result.success(f"HTTP Status Code: {response.status_code}", return_obj=return_obj)
-            case response_code if 500 <= response_code:
+                return Result.success(
+                    f"HTTP Status Code: {response.status_code}",
+                    return_obj=return_obj,
+                )
+            case response_code if response_code >= 500:
                 status = ResultStatus.RETRY
             case _:
                 status = ResultStatus.FAIL
 
         message = f"HTTP Status Code: {response.status_code}; {response.reason or response.text}"
         return Result(status, message, return_obj=return_obj)
```

### Comparing `hoppr-1.9.4/hoppr/utils.py` & `hoppr-1.9.5/hoppr/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """
 Hoppr utility functions
 """
 from __future__ import annotations
 
+import functools
 import importlib
 import inspect
+import os
 import pyclbr
+import sys
 
-from functools import cache
 from importlib.metadata import entry_points
 from pathlib import Path
 from types import ModuleType
 from typing import TYPE_CHECKING, Any, Iterable, Type
 from urllib.parse import unquote
 
+import psutil
+
 from packageurl import PackageURL
 from ruamel.yaml import YAML
 from ruamel.yaml.parser import ParserError as YAMLParserError
 from ruamel.yaml.scanner import ScannerError as YAMLScannerError
 
-from hoppr.exceptions import HopprLoadDataError, HopprPluginError
+from hoppr.exceptions import HopprError, HopprLoadDataError, HopprPluginError
 
 if TYPE_CHECKING:
     from hoppr.base_plugins.hoppr import HopprPlugin
     from hoppr.models import HopprContext
 
 
 def _class_in_module(plugin_module: ModuleType) -> Type[HopprPlugin]:
@@ -208,20 +212,82 @@
     if directory.is_dir() and not any(directory.iterdir()):
         directory.rmdir()
         deleted.add(directory)
 
     return deleted
 
 
-@cache
+@functools.cache
 def get_package_url(purl_string: str) -> PackageURL:
     """
     Get the PackageURL for a given purl_string and store it in a cache for improved performance.
 
     Args:
         purl_string (str): The string representation of a Package URL
 
     Returns:
         PackageURL: The object representation of a PackageURL
 
     """
     return PackageURL.from_string(unquote(purl_string))
+
+
+def get_partition(directory: os.PathLike) -> psutil._common.sdiskpart:  # pylint: disable=protected-access
+    """
+    Returns partition information for a file location
+    """
+
+    mount = Path(directory).expanduser().resolve()
+    while not mount.is_mount():
+        mount = mount.parent
+
+    try:
+        return next((part for part in psutil.disk_partitions(all=True) if part.mountpoint == str(mount)))
+    except StopIteration as ex:
+        raise HopprError(f"Unable to identify partition for path '{directory}'") from ex
+
+
+def is_cicd() -> bool:
+    """
+    Check if running in CI/CD context
+    """
+    return any(
+        os.getenv(env_var, None)
+        for env_var in [
+            "bamboo.buildKey",
+            "BUILD_ID",
+            "BUILD_NUMBER",
+            "BUILDKITE",
+            "CI",
+            "CIRCLECI",
+            "CIRRUS_CI",
+            "CODEBUILD_BUILD_ID",
+            "CONTINUOUS_INTEGRATION",
+            "GITHUB_ACTIONS",
+            "GITLAB_CI",
+            "HEROKU_TEST_RUN_ID",
+            "HUDSON_URL",
+            "JENKINS_URL",
+            "TEAMCITY_VERSION",
+            "TF_BUILD",
+            "TRAVIS",
+        ]
+    )
+
+
+@functools.cache
+def is_basic_terminal() -> bool:
+    """
+    Check if current terminal supports ANSI multi-byte characters
+
+    This function is decorated with `functools.cache` so that it always returns the same value after the initial
+    invocation. This is to prevent negating the return value once the Rich live display is started, i.e.
+    `sys.stdout.isatty()` will then return False instead of True
+    """
+    return any(
+        [
+            is_cicd(),
+            not sys.stdout.isatty(),
+            os.getenv("HOPPR_BASIC_TERM"),
+            os.getenv("TERM_PROGRAM") == "Apple_Terminal",
+        ]
+    )
```

### Comparing `hoppr-1.9.4/pyproject.toml` & `hoppr-1.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr"
-version = "1.9.4"
+version = "1.9.5"
 description = "A tool for defining, verifying, and transferring software dependencies between environments."
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev"
 repository = "https://gitlab.com/hoppr/hoppr"
 
@@ -34,14 +34,15 @@
 hoppr-cyclonedx-models = "0.*"
 in-toto = "^1.3.1"
 jc = "^1.22.2"
 Jinja2 = "^3.1.2"
 jmespath = "^1.0.1"
 oras = "0.*"
 packageurl-python = "0.*"
+psutil = "^5.9.5"
 pydantic-yaml = "0.*"
 PyYAML = "^6.0"
 rapidfuzz = "^3.1.1"
 types-PyYAML = "^6.0.5"
 
 [tool.poetry.dependencies.pydantic]
 extras = ["email"]
@@ -91,15 +92,14 @@
 delta_sbom = "hoppr.core_plugins.delta_sbom:DeltaSbom"
 oras_bundle = "hoppr.core_plugins.oras_bundle:OrasBundlePlugin"
 report_generator = "hoppr.core_plugins.report_generator:ReportGenerator"
 
 [tool.black]
 color = true
 line-length = 120
-skip-string-normalization = true
 target-version = ["py310"]
 
 [tool.coverage.report]
 exclude_also = [
   "if __name__ == .__main__.:",
   "if not TYPE_CHECKING:",
   "if self.debug:",
```

### Comparing `hoppr-1.9.4/PKG-INFO` & `hoppr-1.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr
-Version: 1.9.4
+Version: 1.9.5
 Summary: A tool for defining, verifying, and transferring software dependencies between environments.
 Home-page: https://hoppr.dev
 License: MIT
 Keywords: packaging,reports,build dependencies,software bill of materials
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
@@ -21,14 +21,15 @@
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: hoppr-cyclonedx-models (==0.*)
 Requires-Dist: in-toto (>=1.3.1,<2.0.0)
 Requires-Dist: jc (>=1.22.2,<2.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: oras (==0.*)
 Requires-Dist: packageurl-python (==0.*)
+Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pydantic-yaml (==0.*)
 Requires-Dist: pydantic[email] (>=1.9.0,<2.0.0)
 Requires-Dist: rapidfuzz (>=3.1.1,<4.0.0)
 Requires-Dist: typer[all] (==0.*)
 Requires-Dist: types-PyYAML (>=6.0.5,<7.0.0)
 Project-URL: Repository, https://gitlab.com/hoppr/hoppr
 Description-Content-Type: text/markdown
```

