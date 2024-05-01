# Comparing `tmp/hsmodels-1.0.0.tar.gz` & `tmp/hsmodels-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsmodels-1.0.0.tar", last modified: Mon Feb 19 13:46:16 2024, max compression
+gzip compressed data, was "hsmodels-1.0.3.tar", last modified: Wed May  1 22:43:18 2024, max compression
```

## Comparing `hsmodels-1.0.0.tar` & `hsmodels-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 13:46:16.759987 hsmodels-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-02-19 13:46:09.000000 hsmodels-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-19 13:46:16.759987 hsmodels-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 13:46:16.755987 hsmodels-1.0.0/hsmodels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/namespaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 13:46:16.755987 hsmodels-1.0.0/hsmodels/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20170 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/base_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    35893 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/fields.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14232 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/languages_iso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 13:46:16.759987 hsmodels-1.0.0/hsmodels/schemas/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12460 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/rdf/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (127)    15706 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/rdf/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/rdf/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/rdf/root_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/rdf/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/root_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/schemas/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-19 13:46:09.000000 hsmodels-1.0.0/hsmodels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 13:46:16.759987 hsmodels-1.0.0/hsmodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-19 13:46:16.000000 hsmodels-1.0.0/hsmodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-19 13:46:16.000000 hsmodels-1.0.0/hsmodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 13:46:16.000000 hsmodels-1.0.0/hsmodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-19 13:46:16.000000 hsmodels-1.0.0/hsmodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-19 13:46:16.000000 hsmodels-1.0.0/hsmodels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-19 13:46:16.759987 hsmodels-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-19 13:46:09.000000 hsmodels-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 13:46:16.759987 hsmodels-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-19 13:46:09.000000 hsmodels-1.0.0/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-02-19 13:46:09.000000 hsmodels-1.0.0/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-02-19 13:46:09.000000 hsmodels-1.0.0/tests/test_metadata_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-02-19 13:46:09.000000 hsmodels-1.0.0/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    13934 2024-02-19 13:46:09.000000 hsmodels-1.0.0/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:43:18.263707 hsmodels-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-01 22:43:14.000000 hsmodels-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-01 22:43:18.263707 hsmodels-1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:43:18.255707 hsmodels-1.0.3/hsmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/namespaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:43:18.259707 hsmodels-1.0.3/hsmodels/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21851 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/base_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36312 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/fields.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14232 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/languages_iso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:43:18.259707 hsmodels-1.0.3/hsmodels/schemas/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12460 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/rdf/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15706 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/rdf/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/rdf/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/rdf/root_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/rdf/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/root_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/schemas/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-01 22:43:14.000000 hsmodels-1.0.3/hsmodels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:43:18.259707 hsmodels-1.0.3/hsmodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-01 22:43:18.000000 hsmodels-1.0.3/hsmodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-01 22:43:18.000000 hsmodels-1.0.3/hsmodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:43:18.000000 hsmodels-1.0.3/hsmodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 22:43:18.000000 hsmodels-1.0.3/hsmodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 22:43:18.000000 hsmodels-1.0.3/hsmodels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-01 22:43:18.263707 hsmodels-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-01 22:43:14.000000 hsmodels-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:43:18.259707 hsmodels-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-01 22:43:14.000000 hsmodels-1.0.3/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6616 2024-05-01 22:43:14.000000 hsmodels-1.0.3/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-05-01 22:43:14.000000 hsmodels-1.0.3/tests/test_metadata_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-01 22:43:14.000000 hsmodels-1.0.3/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13611 2024-05-01 22:43:14.000000 hsmodels-1.0.3/tests/test_validation.py
```

### Comparing `hsmodels-1.0.0/LICENSE.txt` & `hsmodels-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/PKG-INFO` & `hsmodels-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: hsmodels
-Version: 1.0.0
+Version: 1.0.3
 Summary: Pydantic models for HydroShare metadata
 Home-page: https://github.com/hydroshare/hsmodels
 Author: Scott Black
 Author-email: sblack@cuahsi.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: rdflib<6.0.0
-Requires-Dist: pydantic==2.*
+Requires-Dist: pydantic==2.7.*
 Requires-Dist: email-validator
 
 Refer to the models section of https://hydroshare.github.io/hsclient/
```

### Comparing `hsmodels-1.0.0/hsmodels/namespaces.py` & `hsmodels-1.0.3/hsmodels/namespaces.py`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/hsmodels/schemas/__init__.py` & `hsmodels-1.0.3/hsmodels/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/hsmodels/schemas/aggregations.py` & `hsmodels-1.0.3/hsmodels/schemas/aggregations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import date
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 
 from pydantic import AnyUrl, ConfigDict, Field, GetJsonSchemaHandler, model_validator, field_validator
 from pydantic.json_schema import JsonSchemaValue
 from pydantic_core import CoreSchema
 
 from hsmodels.schemas.base_models import BaseMetadata
 from hsmodels.schemas.enums import AggregationType
@@ -57,20 +57,20 @@
         description="The 3-character string for the language in which the metadata and content are expressed",
     )
     additional_metadata: Dict[str, str] = Field(
         default={},
         title="Additional metadata",
         description="A dictionary of additional metadata elements expressed as key-value pairs",
     )
-    spatial_coverage: Union[PointCoverage, BoxCoverage] = Field(
+    spatial_coverage: Optional[Union[PointCoverage, BoxCoverage]] = Field(
         default=None,
         title="Spatial coverage",
         description="An object containing the geospatial coverage for the aggregation expressed as either a bounding box or point",
     )
-    period_coverage: PeriodCoverage = Field(
+    period_coverage: Optional[PeriodCoverage] = Field(
         default=None,
         title="Temporal coverage",
         description="An object containing the temporal coverage for a aggregation expressed as a date range",
     )
 
     _parse_additional_metadata = model_validator(mode='before')(parse_additional_metadata)
     _parse_coverages = model_validator(mode='before')(split_coverages)
@@ -112,14 +112,19 @@
 
     model_config = ConfigDict(title="Geographic Raster Aggregation Metadata")
 
     band_information: BandInformation = Field(
         title="Band information",
         description="An object containing information about the bands contained in the raster dataset",
     )
+    spatial_coverage: Union[PointCoverage, BoxCoverage] = Field(
+        default=None,
+        title="Spatial coverage",
+        description="An object containing the geospatial coverage for the aggregation expressed as either a bounding box or point",
+    )
     spatial_reference: Union[BoxSpatialReference, PointSpatialReference] = Field(
         default=None,
         title="Spatial reference",
         description="An object containing spatial reference information for the dataset",
     )
     cell_information: CellInformation = Field(
         title="Cell information", description="An object containing information about the raster grid cells"
@@ -138,15 +143,15 @@
     )
 
     url: AnyUrl = Field(
         title="Aggregation URL", description="An object containing the URL of the aggregation", frozen=True,
         json_schema_extra={"readOnly": True},
     )
 
-    rights: Rights = Field(
+    rights: Optional[Rights] = Field(
         default=None,
         title="Rights statement",
         description="An object containing information about the rights held in and over the aggregation and the license under which a aggregation is shared",
     )
 
     _parse_url = model_validator(mode='before')(parse_url)
 
@@ -167,14 +172,19 @@
         title="Field information",
         description="A list of objects containing information about the fields in the dataset attribute table",
     )
     geometry_information: GeometryInformation = Field(
         title="Geometry information",
         description="An object containing information about the geometry of the features in the dataset",
     )
+    spatial_coverage: Union[PointCoverage, BoxCoverage] = Field(
+        default=None,
+        title="Spatial coverage",
+        description="An object containing the geospatial coverage for the aggregation expressed as either a bounding box or point",
+    )
     spatial_reference: Union[BoxSpatialReference, PointSpatialReference] = Field(
         default=None,
         title="Spatial reference",
         description="An object containing spatial reference information for the dataset",
     )
 
     _parse_spatial_reference = field_validator("spatial_reference", mode='before')(parse_spatial_reference)
@@ -190,15 +200,15 @@
     )
 
     url: AnyUrl = Field(
         title="Aggregation URL", description="An object containing the URL of the aggregation", frozen=True,
         json_schema_extra={"readOnly": True},
     )
 
-    rights: Rights = Field(
+    rights: Optional[Rights] = Field(
         default=None,
         title="Rights statement",
         description="An object containing information about the rights held in and over the aggregation and the license under which a aggregation is shared",
     )
 
     _parse_url = model_validator(mode='before')(parse_url)
 
@@ -214,20 +224,29 @@
     model_config = ConfigDict(title="Multidimensional Aggregation Metadata")
 
     variables: List[Variable] = Field(
         default=[],
         title="Variables",
         description="A list containing information about the variables for which data are stored in the dataset",
     )
+    spatial_coverage: Union[PointCoverage, BoxCoverage] = Field(
+        default=None,
+        title="Spatial coverage",
+        description="An object containing the geospatial coverage for the aggregation expressed as either a bounding box or point",
+    )
     spatial_reference: Union[MultidimensionalBoxSpatialReference, MultidimensionalPointSpatialReference] = Field(
         default=None,
         title="Spatial reference",
         description="An object containing spatial reference information for the dataset",
     )
-
+    period_coverage: PeriodCoverage = Field(
+        default=None,
+        title="Temporal coverage",
+        description="An object containing the temporal coverage for a aggregation expressed as a date range",
+    )
     _parse_spatial_reference = field_validator("spatial_reference", mode='before')(
         parse_multidimensional_spatial_reference
     )
 
 
 class MultidimensionalMetadata(MultidimensionalMetadataIn):
     type: AggregationType = Field(
@@ -239,15 +258,15 @@
     )
 
     url: AnyUrl = Field(
         title="Aggregation URL", description="An object containing the URL of the aggregation", frozen=True,
         json_schema_extra={"readOnly": True},
     )
 
-    rights: Rights = Field(
+    rights: Optional[Rights] = Field(
         default=None,
         title="Rights statement",
         description="An object containing information about the rights held in and over the aggregation and the license under which a aggregation is shared",
     )
 
     _parse_url = model_validator(mode='before')(parse_url)
 
@@ -274,15 +293,15 @@
     )
 
     url: AnyUrl = Field(
         title="Aggregation URL", description="An object containing the URL of the aggregation", frozen=True,
         json_schema_extra={"readOnly": True},
     )
 
-    rights: Rights = Field(
+    rights: Optional[Rights] = Field(
         default=None,
         title="Rights statement",
         description="An object containing information about the rights held in and over the aggregation and the license under which a aggregation is shared",
     )
 
     _parse_url = model_validator(mode='before')(parse_url)
 
@@ -309,15 +328,15 @@
     )
 
     url: AnyUrl = Field(
         title="Aggregation URL", description="An object containing the URL of the aggregation", frozen=True,
         json_schema_extra={"readOnly": True},
     )
 
-    rights: Rights = Field(
+    rights: Optional[Rights] = Field(
         default=None,
         title="Rights statement",
         description="An object containing information about the rights held in and over the aggregation and the license under which a aggregation is shared",
     )
 
     _parse_url = model_validator(mode='before')(parse_url)
 
@@ -343,15 +362,15 @@
     )
 
     url: AnyUrl = Field(
         title="Aggregation URL", description="An object containing the URL of the aggregation", frozen=True,
         json_schema_extra={"readOnly": True},
     )
 
-    rights: Rights = Field(
+    rights: Optional[Rights] = Field(
         default=None,
         title="Rights statement",
         description="An object containing information about the rights held in and over the aggregation and the license under which a aggregation is shared",
     )
 
     _parse_url = model_validator(mode='before')(parse_url)
 
@@ -371,15 +390,25 @@
 
     time_series_results: List[TimeSeriesResult] = Field(
         default=[],
         title="Time series results",
         description="A list of time series results contained within the time series aggregation",
     )
 
-    abstract: str = Field(default=None, title="Abstract", description="A string containing a summary of a aggregation")
+    abstract: Optional[str] = Field(default=None, title="Abstract", description="A string containing a summary of a aggregation")
+    spatial_coverage: Union[PointCoverage, BoxCoverage] = Field(
+        default=None,
+        title="Spatial coverage",
+        description="An object containing the geospatial coverage for the aggregation expressed as either a bounding box or point",
+    )
+    period_coverage: PeriodCoverage = Field(
+        default=None,
+        title="Temporal coverage",
+        description="An object containing the temporal coverage for a aggregation expressed as a date range",
+    )
 
     _parse_abstract = model_validator(mode='before')(parse_abstract)
 
 
 class TimeSeriesMetadata(TimeSeriesMetadataIn):
     type: AggregationType = Field(
         frozen=True,
@@ -390,15 +419,15 @@
     )
 
     url: AnyUrl = Field(
         title="Aggregation URL", description="An object containing the URL of the aggregation", frozen=True,
         json_schema_extra={"readOnly": True},
     )
 
-    rights: Rights = Field(
+    rights: Optional[Rights] = Field(
         default=None,
         title="Rights statement",
         description="An object containing information about the rights held in and over the aggregation and the license under which a aggregation is shared",
     )
 
     _parse_url = model_validator(mode='before')(parse_url)
 
@@ -406,15 +435,15 @@
 class ModelProgramMetadataIn(BaseAggregationMetadataIn):
     """
     A class used to represent the metadata associated with a model program aggregation
     """
 
     model_config = ConfigDict(title="Model Program Aggregation Metadata")
 
-    version: str = Field(
+    version: Optional[str] = Field(
         default=None, title="Version", description="The software version or build number of the model", max_length=255
     )
 
     programming_languages: List[str] = Field(
         default=[],
         max_length=100,
         title="Programming Languages",
@@ -424,35 +453,35 @@
     operating_systems: List[str] = Field(
         default=[],
         max_length=100,
         title="Operating Systems",
         description="Compatible operating systems to setup and run the model",
     )
 
-    release_date: date = Field(
+    release_date: Optional[date] = Field(
         default=None, title="Release Date", description="The date that this version of the model was released"
     )
 
-    website: AnyUrl = Field(
+    website: Optional[AnyUrl] = Field(
         default=None,
         title='Website',
         description='A URL to a website describing the model that is maintained by the model developers',
     )
 
-    code_repository: AnyUrl = Field(
+    code_repository: Optional[AnyUrl] = Field(
         default=None,
         title='Software Repository',
         description='A URL to the source code repository for the model code (e.g., git, mercurial, svn, etc.)',
     )
 
     file_types: List[ModelProgramFile] = Field(
         default=[], title='File Types', description='File types used by the model program'
     )
 
-    program_schema_json: AnyUrl = Field(
+    program_schema_json: Optional[AnyUrl] = Field(
         default=None,
         title='Model program schema',
         description='A url to the JSON metadata schema for the model program',
     )
 
     _parse_file_types = model_validator(mode='before')(parse_file_types)
 
@@ -467,15 +496,15 @@
     )
 
     url: AnyUrl = Field(
         title="Aggregation URL", description="An object containing the URL of the aggregation", frozen=True,
         json_schema_extra={"readOnly": True},
     )
 
-    rights: Rights = Field(
+    rights: Optional[Rights] = Field(
         default=None,
         title="Rights statement",
         description="An object containing information about the rights held in and over the aggregation and the license under which a aggregation is shared",
     )
 
     _parse_url = model_validator(mode='before')(parse_url)
 
@@ -488,27 +517,27 @@
     model_config = ConfigDict(title="Model Instance Aggregation Metadata")
 
     includes_model_output: bool = Field(
         title="Includes Model Output",
         description="Indicates whether model output files are included in the aggregation",
     )
 
-    executed_by: AnyUrl = Field(
+    executed_by: Optional[AnyUrl] = Field(
         default=None,
         title="Executed By",
         description="A URL to the Model Program that can be used to execute this model instance",
     )
 
-    program_schema_json: AnyUrl = Field(
+    program_schema_json: Optional[AnyUrl] = Field(
         default=None,
         title="JSON Metadata schema URL",
         description="A URL to the JSON metadata schema for the related model program",
     )
 
-    program_schema_json_values: AnyUrl = Field(
+    program_schema_json_values: Optional[AnyUrl] = Field(
         default=None,
         title="JSON metadata schema values URL",
         description="A URL to a JSON file containing the metadata values conforming to the JSON metadata schema for the related model program",
     )
 
 
 class ModelInstanceMetadata(ModelInstanceMetadataIn):
@@ -521,14 +550,14 @@
     )
 
     url: AnyUrl = Field(
         title="Aggregation URL", description="An object containing the URL of the aggregation", frozen=True,
         json_schema_extra={"readOnly": True},
     )
 
-    rights: Rights = Field(
+    rights: Optional[Rights] = Field(
         default=None,
         title="Rights statement",
         description="An object containing information about the rights held in and over the aggregation and the license under which a aggregation is shared",
     )
 
     _parse_url = model_validator(mode='before')(parse_url)
```

### Comparing `hsmodels-1.0.0/hsmodels/schemas/base_models.py` & `hsmodels-1.0.3/hsmodels/schemas/base_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,93 @@
 from datetime import datetime
-from typing import Any, Dict, Union
+from typing import Any, Literal, Union
 
+import typing_extensions
 from pydantic import BaseModel, ConfigDict
 
 
 class BaseMetadata(BaseModel):
     def model_dump(
         self,
         *,
-        include: Union['AbstractSetIntStr', 'MappingIntStrAny'] = None,
-        exclude: Union['AbstractSetIntStr', 'MappingIntStrAny'] = None,
+        mode: Union[typing_extensions.Literal['json', 'python'], str] = 'python',
+        include: 'IncEx' = None,
+        exclude: 'IncEx' = None,
+        context: Union[dict[str, Any], None] = None,
         by_alias: bool = False,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = True,
         round_trip: bool = False,
-        warnings: bool = False,
+        warnings: Union[bool, Literal['none', 'warn', 'error']] = False,
+        serialize_as_any: bool = False,
         to_rdf: bool = False,
     ) -> dict[str, Any]:
         """
         Generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
 
         Checks the config for a schema_config dictionary_field and converts a dictionary to a list of key/value pairs.
         This converts the dictionary to a format that can be described in a json schema (which can be found below in the
         schema_extra staticmethod.
 
         Override the default of exclude_none to True
         """
         d = super().model_dump(
+            mode=mode,
             include=include,
             exclude=exclude,
+            context=context,
             by_alias=by_alias,
             exclude_unset=exclude_unset,
             exclude_defaults=exclude_defaults,
             exclude_none=exclude_none,
             round_trip=round_trip,
             warnings=warnings,
+            serialize_as_any=serialize_as_any,
         )
         if to_rdf and "additional_metadata" in d:
             additional_metadata = d["additional_metadata"]
             d["additional_metadata"] = [{"key": key, "value": value} for key, value in additional_metadata.items()]
 
         return d
 
     def model_dump_json(
         self,
         *,
         indent: Union[int, None] = None,
-        include: Union['AbstractSetIntStr', 'MappingIntStrAny'] = None,
-        exclude: Union['AbstractSetIntStr', 'MappingIntStrAny'] = None,
+        include: 'IncEx' = None,
+        exclude: 'IncEx' = None,
+        context: Union[dict[str, Any], None] = None,
         by_alias: bool = False,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = True,
         round_trip: bool = False,
-        warnings: bool = False,
+        warnings: Union[bool, Literal['none', 'warn', 'error']] = False,
+        serialize_as_any: bool = False,
     ) -> str:
         """
         Generate a JSON representation of the model, `include` and `exclude` arguments as per `dict()`.
 
         `encoder` is an optional function to supply as `default` to json.dumps(), other arguments as per `json.dumps()`.
 
         Override the default of exclude_none to True
         """
         return super().model_dump_json(
             indent=indent,
             include=include,
             exclude=exclude,
+            context=context,
             by_alias=by_alias,
             exclude_unset=exclude_unset,
             exclude_defaults=exclude_defaults,
             exclude_none=exclude_none,
             round_trip=round_trip,
             warnings=warnings,
+            serialize_as_any=serialize_as_any,
         )
 
     model_config = ConfigDict(validate_assignment=True)
 
 
 class BaseCoverage(BaseMetadata):
     def __str__(self):
```

### Comparing `hsmodels-1.0.0/hsmodels/schemas/enums.py` & `hsmodels-1.0.3/hsmodels/schemas/enums.py`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/hsmodels/schemas/fields.py` & `hsmodels-1.0.3/hsmodels/schemas/fields.py`

 * *Files 15% similar despite different names*

```diff
@@ -126,41 +126,41 @@
     """
 
     model_config = ConfigDict(title='Creator Metadata')
 
     name: str = Field(
         default=None, max_length=100, title="Name", description="A string containing the name of the creator"
     )
-    phone: str = Field(
+    phone: Optional[str] = Field(
         default=None, max_length=25, title="Phone", description="A string containing a phone number for the creator"
     )
-    address: str = Field(
+    address: Optional[str] = Field(
         default=None, max_length=250, title="Address", description="A string containing an address for the creator"
     )
-    organization: str = Field(
+    organization: Optional[str] = Field(
         default=None,
         max_length=200,
         title="Organization",
         description="A string containing the name of the organization with which the creator is affiliated",
     )
-    email: EmailStr = Field(
+    email: Optional[EmailStr] = Field(
         default=None, title="Email", description="A string containing an email address for the creator"
     )
-    homepage: HttpUrl = Field(
+    homepage: Optional[HttpUrl] = Field(
         default=None,
         title="Homepage",
         description="An object containing the URL for website associated with the creator",
     )
     creator_order: Optional[int] = Field(
         default=None,
         title="Creator order",
         description="An integer to order creators",
         frozen=True,
     )
-    hydroshare_user_id: int = Field(
+    hydroshare_user_id: Optional[int] = Field(
         default=None,
         title="Hydroshare user id",
         description="An integer containing the Hydroshare user ID",
         frozen=True,
         json_schema_extra={"readOnly": True},
     )
     identifiers: Dict[UserIdentifierType, AnyUrl] = Field(
@@ -187,34 +187,34 @@
     """
     A class used to represent the metadata associated with a contributor to a resource
     """
 
     model_config = ConfigDict(title='Contributor Metadata')
 
     name: str = Field(default=None, title="Name", description="A string containing the name of the contributor")
-    phone: str = Field(
+    phone: Optional[str] = Field(
         default=None, title="Phone", description="A string containing a phone number for the contributor"
     )
-    address: str = Field(
+    address: Optional[str] = Field(
         default=None, title="Address", description="A string containing an address for the contributor"
     )
-    organization: str = Field(
+    organization: Optional[str] = Field(
         default=None,
         title="Organization",
         description="A string containing the name of the organization with which the contributor is affiliated",
     )
-    email: EmailStr = Field(
+    email: Optional[EmailStr] = Field(
         default=None, title="Email", description="A string containing an email address for the contributor"
     )
-    homepage: HttpUrl = Field(
+    homepage: Optional[HttpUrl] = Field(
         default=None,
         title="Homepage",
         description="An object containing the URL for website associated with the contributor",
     )
-    hydroshare_user_id: int = Field(
+    hydroshare_user_id: Optional[int] = Field(
         default=None,
         title="Hyroshare user id",
         description="An integer containing the Hydroshare user ID",
         frozen=True,
         json_schema_extra={"readOnly": True},
     )
     identifiers: Dict[UserIdentifierType, AnyUrl] = Field(
@@ -247,21 +247,21 @@
     """
 
     model_config = ConfigDict(title='Funding Agency Metadata')
 
     funding_agency_name: str = Field(
         title="Agency name", description="A string containing the name of the funding agency or organization",
     )
-    title: str = Field(
+    title: Optional[str] = Field(
         default=None, title="Award title", description="A string containing the title of the project or award",
     )
-    number: str = Field(
+    number: Optional[str] = Field(
         default=None, title="Award number", description="A string containing the award number or other identifier",
     )
-    funding_agency_url: AnyUrl = Field(
+    funding_agency_url: Optional[AnyUrl] = Field(
         default=None,
         title="Agency URL",
         description="An object containing a URL pointing to a website describing the funding award",
     )
 
 
 class BandInformation(BaseMetadata):
@@ -269,45 +269,45 @@
     A class used to represent the metadata associated with the raster bands of a geographic raster aggregation
     """
 
     model_config = ConfigDict(title='Raster Band Metadata')
 
     name: str = Field(max_length=500, title="Name", description="A string containing the name of the raster band",
                       )
-    variable_name: str = Field(
+    variable_name: Optional[str] = Field(
         default=None,
         max_length=100,
         title="Variable name",
         description="A string containing the name of the variable represented by the raster band",
     )
-    variable_unit: str = Field(
+    variable_unit: Optional[str] = Field(
         default=None,
         max_length=50,
         title="Variable unit",
         description="A string containing the units for the raster band variable",
     )
-    no_data_value: str = Field(
+    no_data_value: Optional[str] = Field(
         default=None,
         title="Nodata value",
         description="A string containing the numeric nodata value for the raster band",
     )
-    maximum_value: str = Field(
+    maximum_value: Optional[str] = Field(
         default=None,
         title="Maximum value",
         description="A string containing the maximum numeric value for the raster band",
     )
-    comment: str = Field(
+    comment: Optional[str] = Field(
         default=None, title="Comment", description="A string containing a comment about the raster band",
     )
-    method: str = Field(
+    method: Optional[str] = Field(
         default=None,
         title="Method",
         description="A string containing a description of the method used to create the raster band data",
     )
-    minimum_value: str = Field(
+    minimum_value: Optional[str] = Field(
         default=None,
         title="Minimum value",
         description="A string containing the minimum numerica value for the raster dataset",
     )
 
 
 class FieldInformation(BaseMetadata):
@@ -322,24 +322,24 @@
         max_length=128, title="Field name", description="A string containing the name of the attribute table field",
     )
     field_type: str = Field(
         max_length=128, title="Field type", description="A string containing the data type of the values in the field",
     )
     # TODO: What is the "field_type_code"? It's not displayed on the resource landing page, but it's encoded in the
     #  aggregation metadata as an integer value.
-    field_type_code: str = Field(
+    field_type_code: Optional[str] = Field(
         default=None,
         max_length=50,
         title="Field type code",
         description="A string value containing a code that indicates the field type",
     )
-    field_width: int = Field(
+    field_width: Optional[int] = Field(
         default=None, title="Field width", description="An integer value containing the width of the attribute field",
     )
-    field_precision: int = Field(
+    field_precision: Optional[int] = Field(
         default=None,
         title="Field precision",
         description="An integer value containing the precision of the attribute field",
     )
 
 
 class GeometryInformation(BaseMetadata):
@@ -379,26 +379,26 @@
     type: VariableType = Field(title="Type", description="The data type of the values for the variable",
                                )
     shape: str = Field(
         max_length=1000,
         title="Shape",
         description="A string containing the shape of the variable expressed as a list of dimensions",
     )
-    descriptive_name: str = Field(
+    descriptive_name: Optional[str] = Field(
         default=None,
         max_length=1000,
         title="Descriptive name",
         description="A string containing a descriptive name for the variable",
     )
-    method: str = Field(
+    method: Optional[str] = Field(
         default=None,
         title="Method",
         description="A string containing a description of the method used to create the values for the variable",
     )
-    missing_value: str = Field(
+    missing_value: Optional[str] = Field(
         default=None,
         max_length=1000,
         title="Missing value",
         description="A string containing the value used to indicate missing values for the variable",
     )
 
 
@@ -438,21 +438,21 @@
         description="A string containing the type of variable from the ODM2 VariableType controlled vocabulary",
     )
     # TODO: The NoData value for a variable in an ODM2 database is not always an integer.
     #  It could be a floating point value. We might want to change this to a string or a floating point value
     #  It is an integer in the HydroShare database, so will have to be updated there as well if changed
     no_data_value: int = Field(title="NoData value", description="The NoData value for the variable",
                                )
-    variable_definition: str = Field(
+    variable_definition: Optional[str] = Field(
         default=None,
         max_length=255,
         title="Variable definition",
         description="A string containing a detailed description of the variable",
     )
-    speciation: str = Field(
+    speciation: Optional[str] = Field(
         default=None,
         max_length=255,
         title="Speciation",
         description="A string containing the speciation for the variable from the ODM2 Speciation control vocabulary",
     )
 
 
@@ -464,40 +464,40 @@
     model_config = ConfigDict(title='Time Series Site Metadata')
 
     site_code: str = Field(
         max_length=200,
         title="Site code",
         description="A string containing a short but meaningful code identifying the site",
     )
-    site_name: str = Field(
+    site_name: Optional[str] = Field(
         default=None, max_length=255, title="Site name", description="A string containing the name of the site",
     )
-    elevation_m: float = Field(
+    elevation_m: Optional[float] = Field(
         default=None,
         title="Elevation",
         description="A floating point number expressing the elevation of the site in meters",
     )
-    elevation_datum: str = Field(
+    elevation_datum: Optional[str] = Field(
         default=None,
         max_length=50,
         title="Elevation datum",
         description="A string expressing the elevation datum used from the ODM2 Elevation Datum controlled vocabulary",
     )
-    site_type: str = Field(
+    site_type: Optional[str] = Field(
         default=None,
         max_length=100,
         title="Site type",
         description="A string containing the type of site from the ODM2 Sampling Feature Type controlled vocabulary ",
     )
-    latitude: float = Field(
+    latitude: Optional[float] = Field(
         default=None,
         title="Latitude",
         description="A floating point value expressing the latitude coordinate of the site",
     )
-    longitude: float = Field(
+    longitude: Optional[float] = Field(
         default=None,
         title="Longitude",
         description="A floating point value expressing the longitude coordinate of the site",
     )
 
 
 class TimeSeriesMethod(BaseMetadata):
@@ -516,19 +516,19 @@
         max_length=200, title="Method name", description="A string containing the name of the method",
     )
     method_type: str = Field(
         max_length=200,
         title="Method type",
         description="A string containing the method type from the ODM2 Method Type controlled vocabulary",
     )
-    method_description: str = Field(
+    method_description: Optional[str] = Field(
         default=None, title="Method description",
         description="A string containing a detailed description of the method",
     )
-    method_link: AnyUrl = Field(
+    method_link: Optional[AnyUrl] = Field(
         default=None,
         title="Method link",
         description="An object containing a URL that points to a website having a detailed description of the method",
     )
 
 
 class ProcessingLevel(BaseMetadata):
@@ -540,21 +540,21 @@
     model_config = ConfigDict(title='Time Series Processing Level Metadata')
 
     processing_level_code: str = Field(
         max_length=50,
         title="Processing level code",
         description="A string containing a short but meaningful code identifying the processing level",
     )
-    definition: str = Field(
+    definition: Optional[str] = Field(
         default=None,
         max_length=200,
         title="Definition",
         description="A string containing a description of the processing level",
     )
-    explanation: str = Field(
+    explanation: Optional[str] = Field(
         default=None,
         title="Explanation",
         description="A string containing a more extensive explanation of the meaning of the processing level",
     )
 
 
 class Unit(BaseMetadata):
@@ -608,15 +608,15 @@
         description="A string containing a unique identifier for the time series result",
     )
     unit: Unit = Field(
         default=None,
         title="Units",
         description="An object containing the units in which the values of the time series are expressed",
     )
-    status: str = Field(
+    status: Optional[str] = Field(
         default=None,
         max_length=255,
         title="Status",
         description="A string containing the status of the time series result chosen from the ODM2 Status controlled vocabulary",
     )
     sample_medium: str = Field(
         max_length=255,
@@ -642,26 +642,26 @@
         description="A string containing a label for the time series result",
     )
     site: TimeSeriesSite = Field(
         title="Site",
         description="An object containing metadata about the site at which the time series result was created",
     )
     variable: TimeSeriesVariable = Field(
-        title="Variablef",
+        title="Variable",
         description="An object containing metadata about the observed variable associated with the time series result values",
     )
     method: TimeSeriesMethod = Field(
         title="Method",
         description="An object containing metadata about the method used to produce the time series result values",
     )
     processing_level: ProcessingLevel = Field(
         title="Processing level",
         description="An object containing metadata about the processing level or level of quality control to which the time series result values have been subjected",
     )
-    utc_offset: float = Field(
+    utc_offset: Optional[float] = Field(
         default=None,
         title="UTC Offset",
         description="A floating point value that represents the time offset from UTC time in hours associated with the time series result value timestamps",
     )
     _parse_utc_offset = model_validator(mode='before')(parse_utc_offset_value)
```

### Comparing `hsmodels-1.0.0/hsmodels/schemas/languages_iso.py` & `hsmodels-1.0.3/hsmodels/schemas/languages_iso.py`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/hsmodels/schemas/rdf/aggregations.py` & `hsmodels-1.0.3/hsmodels/schemas/rdf/aggregations.py`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/hsmodels/schemas/rdf/fields.py` & `hsmodels-1.0.3/hsmodels/schemas/rdf/fields.py`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/hsmodels/schemas/rdf/resource.py` & `hsmodels-1.0.3/hsmodels/schemas/rdf/resource.py`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/hsmodels/schemas/rdf/root_validators.py` & `hsmodels-1.0.3/hsmodels/schemas/rdf/root_validators.py`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/hsmodels/schemas/rdf/validators.py` & `hsmodels-1.0.3/hsmodels/schemas/rdf/validators.py`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/hsmodels/schemas/resource.py` & `hsmodels-1.0.3/hsmodels/schemas/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Dict, List, Union, Literal
+from typing import Dict, List, Union, Literal, Optional
 
 from pydantic import AnyUrl, ConfigDict, Field, GetJsonSchemaHandler, field_validator, model_validator
 from pydantic.json_schema import JsonSchemaValue
 from pydantic_core import CoreSchema
 
 from hsmodels.schemas.base_models import BaseMetadata
 from hsmodels.schemas.fields import (
@@ -74,20 +74,20 @@
         description="An object containing information about rights held in an over a resource",
     )
     awards: List[AwardInfo] = Field(
         default=[],
         title="Funding agency information",
         description="A list of objects containing information about the funding agencies and awards associated with a resource",
     )
-    spatial_coverage: Union[PointCoverage, BoxCoverage] = Field(
+    spatial_coverage: Optional[Union[PointCoverage, BoxCoverage]] = Field(
         default=None,
         title="Spatial coverage",
         description="An object containing information about the spatial topic of a resource, the spatial applicability of a resource, or jurisdiction under with a resource is relevant",
     )
-    period_coverage: PeriodCoverage = Field(
+    period_coverage: Optional[PeriodCoverage] = Field(
         default=None,
         title="Temporal coverage",
         description="An object containing information about the temporal topic or applicability of a resource",
     )
     publisher: Publisher = Field(
         default=None,
         title="Publisher",
```

### Comparing `hsmodels-1.0.0/hsmodels/schemas/root_validators.py` & `hsmodels-1.0.3/hsmodels/schemas/root_validators.py`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/hsmodels/schemas/validators.py` & `hsmodels-1.0.3/hsmodels/schemas/validators.py`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/hsmodels.egg-info/PKG-INFO` & `hsmodels-1.0.3/hsmodels.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: hsmodels
-Version: 1.0.0
+Version: 1.0.3
 Summary: Pydantic models for HydroShare metadata
 Home-page: https://github.com/hydroshare/hsmodels
 Author: Scott Black
 Author-email: sblack@cuahsi.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: rdflib<6.0.0
-Requires-Dist: pydantic==2.*
+Requires-Dist: pydantic==2.7.*
 Requires-Dist: email-validator
 
 Refer to the models section of https://hydroshare.github.io/hsclient/
```

### Comparing `hsmodels-1.0.0/hsmodels.egg-info/SOURCES.txt` & `hsmodels-1.0.3/hsmodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/setup.py` & `hsmodels-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 README = 'Refer to the models section of https://hydroshare.github.io/hsclient/'# (pathlib.Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='hsmodels',
-    version='1.0.0',
+    version='1.0.3',
     packages=find_packages(include=['hsmodels', 'hsmodels.*', 'hsmodels.schemas.*', 'hsmodels.schemas.rdf.*'],
                            exclude=("tests",)),
     install_requires=[
         'rdflib<6.0.0',
-        'pydantic==2.*',
+        'pydantic==2.7.*',
         'email-validator'
     ],
     url='https://github.com/hydroshare/hsmodels',
     license='MIT',
     author='Scott Black',
     author_email='sblack@cuahsi.org',
     description='Pydantic models for HydroShare metadata',
```

### Comparing `hsmodels-1.0.0/tests/test_defaults.py` & `hsmodels-1.0.3/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/tests/test_metadata.py` & `hsmodels-1.0.3/tests/test_metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,14 +82,17 @@
 
     assert str(res_md.identifier) == "http://www.hydroshare.org/resource/84805fd615a04d63b4eada65644a1e20"
 
     assert len(res_md.additional_metadata) == 3
     assert "key2" in res_md.additional_metadata
     assert res_md.additional_metadata["key2"] == "value2"
 
+    # test additional_metadata can be optional
+    res_md.additional_metadata = {}
+
     assert len(res_md.creators) == 3
     for cr in res_md.creators:
         assert cr.creator_order in (1, 2, 3)
     creator_orders = [cr.creator_order for cr in res_md.creators]
     assert len(creator_orders) == len(set(creator_orders))
 
     creator = res_md.creators[0]
@@ -115,38 +118,48 @@
     assert contributor.phone == "tel:4357973172"
     assert contributor.address == "Utah, US"
     assert str(contributor.homepage) == "http://hydrology.usu.edu/dtarb"
     assert contributor.organization == "Utah State University"
     assert str(contributor.identifiers[UserIdentifierType.ORCID]) == "https://orcid.org/0000-0002-1998-3479"
     assert contributor.name == "David Tarboton"
 
+    # test contributor can be optional
+    res_md.contributors = []
+
     assert len(res_md.relations) == 3
     assert any(x for x in res_md.relations if x.value == "https://sadf.com" and x.type == RelationType.isPartOf)
     assert any(
         x for x in res_md.relations if x.value == "https://www.google.com/" and x.type == RelationType.isCreatedBy
     )
 
+    # test relation can be optional
+    res_md.relations = []
+
     assert res_md.rights.statement == "my statement"
     assert str(res_md.rights.url) == "http://studio.bakajo.com/"
 
     assert res_md.modified == datetime.fromisoformat("2020-11-13T19:40:57.276064+00:00")
     assert res_md.created == datetime.fromisoformat("2020-07-09T19:12:21.354703+00:00")
     assert res_md.review_started == datetime.fromisoformat("2020-11-12T18:53:19.778819+00:00")
     assert res_md.published == datetime.fromisoformat("2020-11-13T18:53:19.778819+00:00")
 
     assert len(res_md.awards) == 2
     award = next(x for x in res_md.awards if x.title == "t")
     assert award
     assert award.number == "n"
     assert award.funding_agency_name == "agency1"
     assert str(award.funding_agency_url) == "https://google.com/"
+    # test awards can be optional
+    res_md.awards = []
 
     assert res_md.period_coverage == PeriodCoverage(
         start=datetime.fromisoformat("2020-07-10T00:00:00"), end=datetime.fromisoformat("2020-07-29T00:00:00")
     )
+    # test period_coverage can be optional
+    res_md.period_coverage = None
 
     assert res_md.spatial_coverage == BoxCoverage(
         name="asdfsadf",
         northlimit=42.1505,
         eastlimit=-84.5739,
         projection='WGS 84 EPSG:4326',
         southlimit=30.282,
@@ -161,13 +174,15 @@
         east=-111.8351,
         projection='WGS 84 EPSG:4326',
         type='point',
         units='Decimal degrees',
     )
 
     res_md.spatial_coverage = pc
+    # test spatial_coverage can be optional
+    res_md.spatial_coverage = None
 
     assert res_md.publisher
     assert (
         res_md.publisher.name == "Consortium of Universities for the Advancement of Hydrologic Science, Inc. (CUAHSI)"
     )
     assert str(res_md.publisher.url) == "https://www.cuahsi.org/"
```

### Comparing `hsmodels-1.0.0/tests/test_schemas.py` & `hsmodels-1.0.3/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `hsmodels-1.0.0/tests/test_validation.py` & `hsmodels-1.0.3/tests/test_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,28 +323,28 @@
             "northlimit": 30.214583003567654,
             "eastlimit": -97.92170777387547,
             "southlimit": 30.127513332692264,
             "westlimit": -98.01556648306897,
             "units": "Decimal degrees",
             "projection": "WGS 84 EPSG:4326",
         },
-        # "period_coverage": None,
+        "period_coverage": None,
         "rights": {
             "statement": "This resource is shared under the Creative Commons Attribution CC BY.",
             "url": "http://creativecommons.org/licenses/by/4.0/",
         },
         "type": "GeoRaster",
         "band_information": {
             "name": "Band_1",
-            # "variable_name": None,
-            # "variable_unit": None,
+            "variable_name": None,
+            "variable_unit": None,
             "no_data_value": "-3.40282346639e+38",
             "maximum_value": "2880.00708008",
-            # "comment": None,
-            # "method": None,
+            "comment": None,
+            "method": None,
             "minimum_value": "2274.95898438",
         },
         "spatial_reference": {
             "northlimit": 30.214583003567654,
             "eastlimit": -97.92170777387547,
             "southlimit": 30.127513332692264,
             "westlimit": -98.01556648306897,
@@ -380,17 +380,10 @@
 
 def test_subjects_aggregation(agg_md):
     agg_md.subjects = ["", "a ", "a ", "a"]
     assert agg_md.subjects == ["a"]
 
 
 def test_default_exclude_none(res_md):
-    # TODO: we can't do the following assignment unless we change the schema for spatial_coverage
-    #  to Optional[Union[PointCoverage, BoxCoverage]]
-    # res_md.spatial_coverage = None
-    assert "spatial_coverage" in res_md.model_dump()
-    model_data = res_md.model_dump()
-
-    # remove spatial_coverage from input data
-    model_data.pop("spatial_coverage")
-    res_md = type(res_md)(**model_data)
+    res_md.spatial_coverage = None
+    assert "spatial_coverage" not in res_md.model_dump()
     assert "spatial_coverage" in res_md.model_dump(exclude_none=False)
```

