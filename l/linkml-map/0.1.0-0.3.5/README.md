# Comparing `tmp/linkml_map-0.1.0.tar.gz` & `tmp/linkml_map-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_map-0.1.0.tar", max compression
+gzip compressed data, was "linkml_map-0.3.5.tar", max compression
```

## Comparing `linkml_map-0.1.0.tar` & `linkml_map-0.3.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1474 2024-04-11 04:09:00.968023 linkml_map-0.1.0/README.md
--rw-r--r--   0        0        0     1329 2024-04-11 04:09:00.968023 linkml_map-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      127 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/cli/__init__.py
--rw-r--r--   0        0        0     6182 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/cli/cli.py
--rw-r--r--   0        0        0       61 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/__init__.py
--rw-r--r--   0        0        0      447 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/awk_compiler.py
--rw-r--r--   0        0        0     2793 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/compiler.py
--rw-r--r--   0        0        0     3853 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/graphviz_compiler.py
--rw-r--r--   0        0        0     1266 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/j2_based_compiler.py
--rw-r--r--   0        0        0      268 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/markdown_compiler.py
--rw-r--r--   0        0        0     3523 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/python_compiler.py
--rw-r--r--   0        0        0      383 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/r2rml_compiler.py
--rw-r--r--   0        0        0      395 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/sparql_compiler.py
--rw-r--r--   0        0        0     4287 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/sql_compiler.py
--rw-r--r--   0        0        0      460 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/sssom_compiler.py
--rw-r--r--   0        0        0       63 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/templates/__init__.py
--rw-r--r--   0        0        0      717 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/templates/markdown.j2
--rw-r--r--   0        0        0      173 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/tr/__init__.py
--rw-r--r--   0        0        0      756 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/compiler/tr/transformer_to_mapping_tables.tr.yaml
--rw-r--r--   0        0        0      111 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/datamodel/__init__.py
--rw-r--r--   0        0        0      161 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/datamodel/sssom.map.yaml
--rw-r--r--   0        0        0    18818 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/datamodel/transformer_model.py
--rw-r--r--   0        0        0    10658 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/datamodel/transformer_model.yaml
--rw-r--r--   0        0        0        0 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/functions/__init__.py
--rw-r--r--   0        0        0     4448 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/functions/unit_conversion.py
--rw-r--r--   0        0        0        0 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/importer/__init__.py
--rw-r--r--   0        0        0      866 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/importer/importer.py
--rw-r--r--   0        0        0        0 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/inference/__init__.py
--rw-r--r--   0        0        0     1565 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/inference/inference.py
--rw-r--r--   0        0        0     7414 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/inference/inverter.py
--rw-r--r--   0        0        0    10117 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/inference/schema_mapper.py
--rw-r--r--   0        0        0     6602 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/session.py
--rw-r--r--   0        0        0        0 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/transformer/__init__.py
--rw-r--r--   0        0        0     2226 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/transformer/duckdb_transformer.py
--rw-r--r--   0        0        0    16600 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/transformer/object_transformer.py
--rw-r--r--   0        0        0     9812 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/transformer/transformer.py
--rw-r--r--   0        0        0        0 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/utils/__init__.py
--rw-r--r--   0        0        0     1306 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/utils/dynamic_object.py
--rw-r--r--   0        0        0     6824 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/utils/eval_utils.py
--rw-r--r--   0        0        0      767 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/utils/loaders.py
--rw-r--r--   0        0        0     9496 2024-04-11 04:09:00.972023 linkml_map-0.1.0/src/linkml_map/utils/multi_file_transformer.py
--rw-r--r--   0        0        0     2115 1970-01-01 00:00:00.000000 linkml_map-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1474 2024-05-02 03:03:24.839000 linkml_map-0.3.5/README.md
+-rw-r--r--   0        0        0     1516 2024-05-02 03:03:56.466852 linkml_map-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      127 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/cli/__init__.py
+-rw-r--r--   0        0        0     6182 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/cli/cli.py
+-rw-r--r--   0        0        0       61 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/__init__.py
+-rw-r--r--   0        0        0      447 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/awk_compiler.py
+-rw-r--r--   0        0        0     2793 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/compiler.py
+-rw-r--r--   0        0        0     3853 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/graphviz_compiler.py
+-rw-r--r--   0        0        0     1266 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/j2_based_compiler.py
+-rw-r--r--   0        0        0      268 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/markdown_compiler.py
+-rw-r--r--   0        0        0     3523 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/python_compiler.py
+-rw-r--r--   0        0        0      383 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/r2rml_compiler.py
+-rw-r--r--   0        0        0      395 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/sparql_compiler.py
+-rw-r--r--   0        0        0     4410 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/sql_compiler.py
+-rw-r--r--   0        0        0      460 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/sssom_compiler.py
+-rw-r--r--   0        0        0       63 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/templates/__init__.py
+-rw-r--r--   0        0        0      717 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/templates/markdown.j2
+-rw-r--r--   0        0        0      173 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/tr/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/tr/transformer_to_mapping_tables.tr.yaml
+-rw-r--r--   0        0        0      111 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/datamodel/__init__.py
+-rw-r--r--   0        0        0      161 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/datamodel/sssom.map.yaml
+-rw-r--r--   0        0        0    18689 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/datamodel/transformer_model.py
+-rw-r--r--   0        0        0    10658 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/datamodel/transformer_model.yaml
+-rw-r--r--   0        0        0        0 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/functions/__init__.py
+-rw-r--r--   0        0        0     4448 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/functions/unit_conversion.py
+-rw-r--r--   0        0        0        0 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/importer/__init__.py
+-rw-r--r--   0        0        0      866 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/importer/importer.py
+-rw-r--r--   0        0        0        0 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/inference/__init__.py
+-rw-r--r--   0        0        0     1565 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/inference/inference.py
+-rw-r--r--   0        0        0     7414 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/inference/inverter.py
+-rw-r--r--   0        0        0    10117 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/inference/schema_mapper.py
+-rw-r--r--   0        0        0     6602 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/session.py
+-rw-r--r--   0        0        0        0 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/transformer/__init__.py
+-rw-r--r--   0        0        0     2226 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/transformer/duckdb_transformer.py
+-rw-r--r--   0        0        0    16600 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/transformer/object_transformer.py
+-rw-r--r--   0        0        0     9812 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/transformer/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/utils/__init__.py
+-rw-r--r--   0        0        0     1306 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/utils/dynamic_object.py
+-rw-r--r--   0        0        0     6824 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/utils/eval_utils.py
+-rw-r--r--   0        0        0      767 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/utils/loaders.py
+-rw-r--r--   0        0        0     9496 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/utils/multi_file_transformer.py
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 linkml_map-0.3.5/PKG-INFO
```

### Comparing `linkml_map-0.1.0/README.md` & `linkml_map-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/cli/cli.py` & `linkml_map-0.3.5/src/linkml_map/cli/cli.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/compiler/compiler.py` & `linkml_map-0.3.5/src/linkml_map/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/compiler/graphviz_compiler.py` & `linkml_map-0.3.5/src/linkml_map/compiler/graphviz_compiler.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/compiler/j2_based_compiler.py` & `linkml_map-0.3.5/src/linkml_map/compiler/j2_based_compiler.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/compiler/python_compiler.py` & `linkml_map-0.3.5/src/linkml_map/compiler/python_compiler.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/compiler/sql_compiler.py` & `linkml_map-0.3.5/src/linkml_map/compiler/sql_compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,16 +62,14 @@
             stmt += f"INSERT INTO {cd.name} SELECT \n"
         col_trs = []
         for sd in cd.slot_derivations.values():
             col_trs.append(self.compile_slot_derivation(sd))
         if not col_trs:
             return
         stmt += ", \n".join(col_trs)
-        if self.new_table_when_transforming:
-            stmt += ");"
         stmt += f" FROM {cd.name}"
         compiled.serialization += f"{stmt};\n"
 
     def compile_slot_derivation(self, sd) -> str:
         expr = sd.populated_from
         if expr is None:
             expr = sd.name
@@ -110,14 +108,18 @@
             if not col_strs:
                 continue
             ddl.append(f"CREATE TABLE IF NOT EXISTS {c.name} (")
             ddl.append(",\n".join(col_strs))
             ddl.append(");")
         return "\n".join(ddl)
 
+    def create_target_ddl(self, specification: TransformationSpecification) -> str:
+        target_sv = self.derived_target_schemaview(specification)
+        return self.create_ddl(target_sv)
+
     def sql_type(self, slot: SlotDefinition, schemaview: SchemaView) -> str:
         """
         Map LinkML types to DuckDB SQL types.
 
         :param slot:
         :param schemaview:
         :return:
```

### Comparing `linkml_map-0.1.0/src/linkml_map/compiler/templates/markdown.j2` & `linkml_map-0.3.5/src/linkml_map/compiler/templates/markdown.j2`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/compiler/tr/transformer_to_mapping_tables.tr.yaml` & `linkml_map-0.3.5/src/linkml_map/compiler/tr/transformer_to_mapping_tables.tr.yaml`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/datamodel/transformer_model.py` & `linkml_map-0.3.5/src/linkml_map/datamodel/transformer_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from __future__ import annotations
 
-import re
-import sys
-from datetime import date, datetime
-from decimal import Decimal
 from enum import Enum
-from typing import Any, Dict, List, Literal, Optional, Union
+from typing import Any, Dict, List, Optional
 
 from pydantic.version import VERSION as PYDANTIC_VERSION
 
 if int(PYDANTIC_VERSION[0]) >= 2:
-    from pydantic import BaseModel, ConfigDict, Field, field_validator
+    from pydantic import BaseModel, ConfigDict, Field
 else:
-    from pydantic import BaseModel, Field, validator
+    from pydantic import BaseModel, Field
 
 metamodel_version = "None"
 version = "None"
 
 
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
```

### Comparing `linkml_map-0.1.0/src/linkml_map/datamodel/transformer_model.yaml` & `linkml_map-0.3.5/src/linkml_map/datamodel/transformer_model.yaml`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/functions/unit_conversion.py` & `linkml_map-0.3.5/src/linkml_map/functions/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/importer/importer.py` & `linkml_map-0.3.5/src/linkml_map/importer/importer.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/inference/inference.py` & `linkml_map-0.3.5/src/linkml_map/inference/inference.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/inference/inverter.py` & `linkml_map-0.3.5/src/linkml_map/inference/inverter.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/inference/schema_mapper.py` & `linkml_map-0.3.5/src/linkml_map/inference/schema_mapper.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/session.py` & `linkml_map-0.3.5/src/linkml_map/session.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/transformer/duckdb_transformer.py` & `linkml_map-0.3.5/src/linkml_map/transformer/duckdb_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/transformer/object_transformer.py` & `linkml_map-0.3.5/src/linkml_map/transformer/object_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/transformer/transformer.py` & `linkml_map-0.3.5/src/linkml_map/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/utils/dynamic_object.py` & `linkml_map-0.3.5/src/linkml_map/utils/dynamic_object.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/utils/eval_utils.py` & `linkml_map-0.3.5/src/linkml_map/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/utils/loaders.py` & `linkml_map-0.3.5/src/linkml_map/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/src/linkml_map/utils/multi_file_transformer.py` & `linkml_map-0.3.5/src/linkml_map/utils/multi_file_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.1.0/PKG-INFO` & `linkml_map-0.3.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: linkml-map
-Version: 0.1.0
-Summary: 
+Version: 0.3.5
+Summary: a framework for specifying and executing mappings between data models
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asteval (>=0.9.29,<0.10.0)
 Requires-Dist: deepdiff (>=6.7.1,<7.0.0)
 Requires-Dist: linkml-runtime (>=1.7.2)
-Requires-Dist: pydantic (>=2.5.3,<3.0.0)
+Requires-Dist: pydantic (>=2.0.0)
 Requires-Dist: ucumvert (>=0.1.1,<0.2.0)
 Description-Content-Type: text/markdown
 
 # linkml-map
 
 [![Pyversions](https://img.shields.io/pypi/pyversions/linkml-map.svg)](https://pypi.python.org/pypi/linkml-map)
 ![](https://github.com/linkml/linkml-map/workflows/Build/badge.svg)
```

