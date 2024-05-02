# Comparing `tmp/cognite_pygen-0.99.8.tar.gz` & `tmp/cognite_pygen-0.99.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_pygen-0.99.8.tar", max compression
+gzip compressed data, was "cognite_pygen-0.99.9.tar", max compression
```

## Comparing `cognite_pygen-0.99.8.tar` & `cognite_pygen-0.99.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    11342 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/LICENSE
--rw-r--r--   0        0        0     5342 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/README.md
--rw-r--r--   0        0        0      395 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/__init__.py
--rw-r--r--   0        0        0        0 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/__init__.py
--rw-r--r--   0        0        0    22476 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/generators.py
--rw-r--r--   0        0        0      871 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/models/__init__.py
--rw-r--r--   0        0        0     8408 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/models/api_casses.py
--rw-r--r--   0        0        0    14012 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/models/data_classes.py
--rw-r--r--   0        0        0    22320 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/models/fields.py
--rw-r--r--   0        0        0    13662 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/models/filter_method.py
--rw-r--r--   0        0        0     7716 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/templates/_api_client_multi_model.py.jinja
--rw-r--r--   0        0        0     7793 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/templates/_api_client_single_model.py.jinja
--rw-r--r--   0        0        0       99 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/templates/_client_init.py.jinja
--rw-r--r--   0        0        0     2500 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/templates/api_class_edge.py.jinja
--rw-r--r--   0        0        0    22075 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/templates/api_class_node.py.jinja
--rw-r--r--   0        0        0     6495 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/templates/api_class_query.py.jinja
--rw-r--r--   0        0        0    25667 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/templates/api_class_timeseries.py.jinja
--rw-r--r--   0        0        0    30184 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/templates/api_core.py.jinja
--rw-r--r--   0        0        0    12060 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/templates/data_class_edge.py.jinja
--rw-r--r--   0        0        0    13321 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/templates/data_class_node.py.jinja
--rw-r--r--   0        0        0    17445 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/templates/data_classes_core.py.jinja
--rw-r--r--   0        0        0     1964 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/templates/data_classes_init.py.jinja
--rw-r--r--   0        0        0     1850 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_core/validation.py
--rw-r--r--   0        0        0    17044 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_generator.py
--rw-r--r--   0        0        0     4292 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_settings.py
--rw-r--r--   0        0        0       24 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/_version.py
--rw-r--r--   0        0        0     9111 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/cli.py
--rw-r--r--   0        0        0      799 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/config/__init__.py
--rw-r--r--   0        0        0     3367 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/config/filtering_methods.py
--rw-r--r--   0        0        0     6774 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/config/naming.py
--rw-r--r--   0        0        0     1936 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/config/reserved_words.py
--rw-r--r--   0        0        0       65 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/__init__.py
--rw-r--r--   0        0        0       55 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/_constants.py
--rw-r--r--   0        0        0     9460 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/_solar_apm.py
--rw-r--r--   0        0        0     1596 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/Asset.csv
--rw-r--r--   0        0        0      229 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/Asset.documents.csv
--rw-r--r--   0        0        0      343 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/Asset.linkedAssets.csv
--rw-r--r--   0        0        0      171 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/Asset.metrics.csv
--rw-r--r--   0        0        0      235 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/FileMetadata.csv
--rw-r--r--   0        0        0      421 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/TimeSeries.csv
--rw-r--r--   0        0        0      519 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/WorkItem.csv
--rw-r--r--   0        0        0      177 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/WorkItem.linkedAssets.csv
--rw-r--r--   0        0        0      919 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/WorkOrder.csv
--rw-r--r--   0        0        0      187 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/WorkOrder.linkedAssets.csv
--rw-r--r--   0        0        0      129 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/WorkOrder.workItems.csv
--rw-r--r--   0        0        0     1089 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/model.graphql
--rw-r--r--   0        0        0     1617 2024-02-11 09:59:06.987730 cognite_pygen-0.99.8/cognite/pygen/exceptions.py
--rw-r--r--   0        0        0      259 2024-02-11 09:59:06.991730 cognite_pygen-0.99.8/cognite/pygen/utils/__init__.py
--rw-r--r--   0        0        0    29901 2024-02-11 09:59:06.991730 cognite_pygen-0.99.8/cognite/pygen/utils/cdf.py
--rw-r--r--   0        0        0     4669 2024-02-11 09:59:06.991730 cognite_pygen-0.99.8/cognite/pygen/utils/external_id_factories.py
--rw-r--r--   0        0        0      881 2024-02-11 09:59:06.991730 cognite_pygen-0.99.8/cognite/pygen/utils/helper.py
--rw-r--r--   0        0        0    43321 2024-02-11 09:59:06.991730 cognite_pygen-0.99.8/cognite/pygen/utils/mock_generator.py
--rw-r--r--   0        0        0     9387 2024-02-11 09:59:06.991730 cognite_pygen-0.99.8/cognite/pygen/utils/text.py
--rw-r--r--   0        0        0     1941 2024-02-11 09:59:06.991730 cognite_pygen-0.99.8/cognite/pygen/warnings.py
--rw-r--r--   0        0        0     4011 2024-02-11 09:59:07.023730 cognite_pygen-0.99.8/pyproject.toml
--rw-r--r--   0        0        0     7074 1970-01-01 00:00:00.000000 cognite_pygen-0.99.8/PKG-INFO
+-rw-r--r--   0        0        0    11342 2024-02-11 12:19:25.901243 cognite_pygen-0.99.9/LICENSE
+-rw-r--r--   0        0        0     5342 2024-02-11 12:19:25.901243 cognite_pygen-0.99.9/README.md
+-rw-r--r--   0        0        0      395 2024-02-11 12:19:25.901243 cognite_pygen-0.99.9/cognite/pygen/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-11 12:19:25.901243 cognite_pygen-0.99.9/cognite/pygen/_core/__init__.py
+-rw-r--r--   0        0        0    22674 2024-02-11 12:19:25.901243 cognite_pygen-0.99.9/cognite/pygen/_core/generators.py
+-rw-r--r--   0        0        0      871 2024-02-11 12:19:25.901243 cognite_pygen-0.99.9/cognite/pygen/_core/models/__init__.py
+-rw-r--r--   0        0        0     8408 2024-02-11 12:19:25.901243 cognite_pygen-0.99.9/cognite/pygen/_core/models/api_casses.py
+-rw-r--r--   0        0        0    14012 2024-02-11 12:19:25.901243 cognite_pygen-0.99.9/cognite/pygen/_core/models/data_classes.py
+-rw-r--r--   0        0        0    22320 2024-02-11 12:19:25.901243 cognite_pygen-0.99.9/cognite/pygen/_core/models/fields.py
+-rw-r--r--   0        0        0    13662 2024-02-11 12:19:25.901243 cognite_pygen-0.99.9/cognite/pygen/_core/models/filter_method.py
+-rw-r--r--   0        0        0     7716 2024-02-11 12:19:25.901243 cognite_pygen-0.99.9/cognite/pygen/_core/templates/_api_client_multi_model.py.jinja
+-rw-r--r--   0        0        0     7793 2024-02-11 12:19:25.901243 cognite_pygen-0.99.9/cognite/pygen/_core/templates/_api_client_single_model.py.jinja
+-rw-r--r--   0        0        0       99 2024-02-11 12:19:25.901243 cognite_pygen-0.99.9/cognite/pygen/_core/templates/_client_init.py.jinja
+-rw-r--r--   0        0        0     2500 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/_core/templates/api_class_edge.py.jinja
+-rw-r--r--   0        0        0    22075 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/_core/templates/api_class_node.py.jinja
+-rw-r--r--   0        0        0     6495 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/_core/templates/api_class_query.py.jinja
+-rw-r--r--   0        0        0    25667 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/_core/templates/api_class_timeseries.py.jinja
+-rw-r--r--   0        0        0    30184 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/_core/templates/api_core.py.jinja
+-rw-r--r--   0        0        0    12060 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/_core/templates/data_class_edge.py.jinja
+-rw-r--r--   0        0        0    13321 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/_core/templates/data_class_node.py.jinja
+-rw-r--r--   0        0        0    17445 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/_core/templates/data_classes_core.py.jinja
+-rw-r--r--   0        0        0     2068 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/_core/templates/data_classes_init.py.jinja
+-rw-r--r--   0        0        0     1850 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/_core/validation.py
+-rw-r--r--   0        0        0    17044 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/_generator.py
+-rw-r--r--   0        0        0     4292 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/_settings.py
+-rw-r--r--   0        0        0       24 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/_version.py
+-rw-r--r--   0        0        0     9111 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/cli.py
+-rw-r--r--   0        0        0      799 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/config/__init__.py
+-rw-r--r--   0        0        0     3367 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/config/filtering_methods.py
+-rw-r--r--   0        0        0     6774 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/config/naming.py
+-rw-r--r--   0        0        0     1936 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/config/reserved_words.py
+-rw-r--r--   0        0        0       65 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/__init__.py
+-rw-r--r--   0        0        0       55 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/_constants.py
+-rw-r--r--   0        0        0     9460 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/_solar_apm.py
+-rw-r--r--   0        0        0     1596 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/Asset.csv
+-rw-r--r--   0        0        0      229 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/Asset.documents.csv
+-rw-r--r--   0        0        0      343 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/Asset.linkedAssets.csv
+-rw-r--r--   0        0        0      171 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/Asset.metrics.csv
+-rw-r--r--   0        0        0      235 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/FileMetadata.csv
+-rw-r--r--   0        0        0      421 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/TimeSeries.csv
+-rw-r--r--   0        0        0      519 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/WorkItem.csv
+-rw-r--r--   0        0        0      177 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/WorkItem.linkedAssets.csv
+-rw-r--r--   0        0        0      919 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/WorkOrder.csv
+-rw-r--r--   0        0        0      187 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/WorkOrder.linkedAssets.csv
+-rw-r--r--   0        0        0      129 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/WorkOrder.workItems.csv
+-rw-r--r--   0        0        0     1089 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/model.graphql
+-rw-r--r--   0        0        0     1617 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/exceptions.py
+-rw-r--r--   0        0        0      259 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/utils/__init__.py
+-rw-r--r--   0        0        0    29901 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/utils/cdf.py
+-rw-r--r--   0        0        0     4669 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/utils/external_id_factories.py
+-rw-r--r--   0        0        0      881 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/utils/helper.py
+-rw-r--r--   0        0        0    43321 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/utils/mock_generator.py
+-rw-r--r--   0        0        0     9387 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/utils/text.py
+-rw-r--r--   0        0        0     1941 2024-02-11 12:19:25.905243 cognite_pygen-0.99.9/cognite/pygen/warnings.py
+-rw-r--r--   0        0        0     4011 2024-02-11 12:19:25.937242 cognite_pygen-0.99.9/pyproject.toml
+-rw-r--r--   0        0        0     7074 1970-01-01 00:00:00.000000 cognite_pygen-0.99.9/PKG-INFO
```

### Comparing `cognite_pygen-0.99.8/LICENSE` & `cognite_pygen-0.99.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/README.md` & `cognite_pygen-0.99.9/README.md`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/generators.py` & `cognite_pygen-0.99.9/cognite/pygen/_core/generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,18 +298,24 @@
     def generate_client_init_file(self) -> str:
         client_init = self.env.get_template("_client_init.py.jinja")
         return client_init.render(client_name=self.client_name, top_level_package=self.top_level_package) + "\n"
 
     def generate_data_classes_init_file(self) -> str:
         data_class_init = self.env.get_template("data_classes_init.py.jinja")
 
-        dependencies_by_names: dict[tuple[str, str], list[DataClass]] = defaultdict(list)
+        dependencies_by_names: dict[tuple[str, str, bool], list[DataClass]] = defaultdict(list)
         for api in self.unique_apis:
             for dep in api.data_class.dependencies:
-                dependencies_by_names[(api.data_class.read_name, api.data_class.write_name)].append(dep)
+                dependencies_by_names[
+                    (
+                        api.data_class.read_name,
+                        api.data_class.write_name,
+                        api.data_class.is_writable or api.data_class.is_interface,
+                    )
+                ].append(dep)
 
         return (
             data_class_init.render(
                 classes=sorted([api.data_class for api in self.unique_apis]),
                 is_pydantic_v2=self.pydantic_version == "v2",
                 dependencies_by_names=dependencies_by_names,
                 ft=fields,
```

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/models/__init__.py` & `cognite_pygen-0.99.9/cognite/pygen/_core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/models/api_casses.py` & `cognite_pygen-0.99.9/cognite/pygen/_core/models/api_casses.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/models/data_classes.py` & `cognite_pygen-0.99.9/cognite/pygen/_core/models/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/models/fields.py` & `cognite_pygen-0.99.9/cognite/pygen/_core/models/fields.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/models/filter_method.py` & `cognite_pygen-0.99.9/cognite/pygen/_core/models/filter_method.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/templates/_api_client_multi_model.py.jinja` & `cognite_pygen-0.99.9/cognite/pygen/_core/templates/_api_client_multi_model.py.jinja`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/templates/_api_client_single_model.py.jinja` & `cognite_pygen-0.99.9/cognite/pygen/_core/templates/_api_client_single_model.py.jinja`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/templates/api_class_edge.py.jinja` & `cognite_pygen-0.99.9/cognite/pygen/_core/templates/api_class_edge.py.jinja`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/templates/api_class_node.py.jinja` & `cognite_pygen-0.99.9/cognite/pygen/_core/templates/api_class_node.py.jinja`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/templates/api_class_query.py.jinja` & `cognite_pygen-0.99.9/cognite/pygen/_core/templates/api_class_query.py.jinja`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/templates/api_class_timeseries.py.jinja` & `cognite_pygen-0.99.9/cognite/pygen/_core/templates/api_class_timeseries.py.jinja`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/templates/api_core.py.jinja` & `cognite_pygen-0.99.9/cognite/pygen/_core/templates/api_core.py.jinja`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/templates/data_class_edge.py.jinja` & `cognite_pygen-0.99.9/cognite/pygen/_core/templates/data_class_edge.py.jinja`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/templates/data_class_node.py.jinja` & `cognite_pygen-0.99.9/cognite/pygen/_core/templates/data_class_node.py.jinja`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/templates/data_classes_core.py.jinja` & `cognite_pygen-0.99.9/cognite/pygen/_core/templates/data_classes_core.py.jinja`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/templates/data_classes_init.py.jinja` & `cognite_pygen-0.99.9/cognite/pygen/_core/templates/data_classes_init.py.jinja`

 * *Files 11% similar despite different names*

```diff
@@ -7,27 +7,27 @@
     DomainModelList,
     DomainRelationWrite,
     ResourcesWrite,
     ResourcesWriteResult,
 )
 {% for class_ in classes %}{{ class_.init_import }}
 {% endfor %}
-{% if is_pydantic_v2 %}{% for (read_name, write_name) in dependencies_by_names %}{{ read_name }}.model_rebuild()
+{% if is_pydantic_v2 %}{% for (read_name, write_name, has_write_class) in dependencies_by_names %}{{ read_name }}.model_rebuild(){% if has_write_class %}
 {{ write_name }}.model_rebuild()
-{{ read_name }}Apply.model_rebuild()
-{% endfor %}{% else %}{% for (read_name, write_name), dependencies in dependencies_by_names.items() %}
+{{ read_name }}Apply.model_rebuild(){% endif %}
+{% endfor %}{% else %}{% for (read_name, write_name, has_write_class), dependencies in dependencies_by_names.items() %}
 {{ read_name }}.update_forward_refs({% for dependency in dependencies %}
     {{ dependency.read_name }}={{ dependency.read_name }},{%  endfor %}
-)
+){% if has_write_class %}
 {{ write_name }}.update_forward_refs({% for dependency in dependencies %}{% if dependency.is_writable or dependency.is_interface %}
     {{ dependency.write_name }}={{ dependency.write_name }},{% endif %}{%  endfor %}
 )
 {{ read_name }}Apply.update_forward_refs({% for dependency in dependencies %}{% if dependency.is_writable or dependency.is_interface %}
     {{ dependency.write_name }}={{ dependency.write_name }},{% endif %}{%  endfor %}
-)
+){% endif %}
 {% endfor %}{% endif %}
 __all__ = [
     "DataRecord",
     "DataRecordWrite",
     "ResourcesWrite",
     "DomainModel",
     "DomainModelCore",
```

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_core/validation.py` & `cognite_pygen-0.99.9/cognite/pygen/_core/validation.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_generator.py` & `cognite_pygen-0.99.9/cognite/pygen/_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/_settings.py` & `cognite_pygen-0.99.9/cognite/pygen/_settings.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/cli.py` & `cognite_pygen-0.99.9/cognite/pygen/cli.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/config/__init__.py` & `cognite_pygen-0.99.9/cognite/pygen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/config/filtering_methods.py` & `cognite_pygen-0.99.9/cognite/pygen/config/filtering_methods.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/config/naming.py` & `cognite_pygen-0.99.9/cognite/pygen/config/naming.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/config/reserved_words.py` & `cognite_pygen-0.99.9/cognite/pygen/config/reserved_words.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/demo/_solar_apm.py` & `cognite_pygen-0.99.9/cognite/pygen/demo/_solar_apm.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/Asset.csv` & `cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/Asset.csv`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/WorkItem.csv` & `cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/WorkItem.csv`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/WorkOrder.csv` & `cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/WorkOrder.csv`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/demo/solar_apm_data/model.graphql` & `cognite_pygen-0.99.9/cognite/pygen/demo/solar_apm_data/model.graphql`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/exceptions.py` & `cognite_pygen-0.99.9/cognite/pygen/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/utils/cdf.py` & `cognite_pygen-0.99.9/cognite/pygen/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/utils/external_id_factories.py` & `cognite_pygen-0.99.9/cognite/pygen/utils/external_id_factories.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/utils/helper.py` & `cognite_pygen-0.99.9/cognite/pygen/utils/helper.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/utils/mock_generator.py` & `cognite_pygen-0.99.9/cognite/pygen/utils/mock_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/utils/text.py` & `cognite_pygen-0.99.9/cognite/pygen/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/cognite/pygen/warnings.py` & `cognite_pygen-0.99.9/cognite/pygen/warnings.py`

 * *Files identical despite different names*

### Comparing `cognite_pygen-0.99.8/pyproject.toml` & `cognite_pygen-0.99.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-pygen"
-version = "0.99.8"
+version = "0.99.9"
 description = "Cognite Python SDK Generator"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache-2.0"
 documentation = "https://cognite-pygen.readthedocs-hosted.com/en/latest/"
 homepage = "https://cognite-pygen.readthedocs-hosted.com/en/latest/"
 repository = "https://github.com/cognitedata/pygen"
```

### Comparing `cognite_pygen-0.99.8/PKG-INFO` & `cognite_pygen-0.99.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-pygen
-Version: 0.99.8
+Version: 0.99.9
 Summary: Cognite Python SDK Generator
 Home-page: https://cognite-pygen.readthedocs-hosted.com/en/latest/
 License: Apache-2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

