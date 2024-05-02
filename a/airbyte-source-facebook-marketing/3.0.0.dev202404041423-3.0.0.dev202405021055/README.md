# Comparing `tmp/airbyte_source_facebook_marketing-3.0.0.dev202404041423.tar.gz` & `tmp/airbyte_source_facebook_marketing-3.0.0.dev202405021055.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_facebook_marketing-3.0.0.dev202404041423.tar", max compression
+gzip compressed data, was "airbyte_source_facebook_marketing-3.0.0.dev202405021055.tar", max compression
```

## Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423.tar` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     4712 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/README.md
--rw-r--r--   0        0        0      904 2024-04-04 14:23:19.230402 airbyte_source_facebook_marketing-3.0.0.dev202404041423/pyproject.toml
--rw-r--r--   0        0        0     4784 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/README.md
--rw-r--r--   0        0        0      455 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/__init__.py
--rw-r--r--   0        0        0     8030 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/api.py
--rw-r--r--   0        0        0     5157 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/config_migrations.py
--rw-r--r--   0        0        0      469 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/run.py
--rw-r--r--   0        0        0      885 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/activities.json
--rw-r--r--   0        0        0     5948 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ad_account.json
--rw-r--r--   0        0        0    42732 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ad_creatives.json
--rw-r--r--   0        0        0     2660 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ad_sets.json
--rw-r--r--   0        0        0    11058 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ads.json
--rw-r--r--   0        0        0     7681 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ads_insights.json
--rw-r--r--   0        0        0      609 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ads_insights_action_breakdowns.json
--rw-r--r--   0        0        0     2981 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ads_insights_breakdowns.json
--rw-r--r--   0        0        0     2606 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/campaigns.json
--rw-r--r--   0        0        0     3587 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/custom_audiences.json
--rw-r--r--   0        0        0     1458 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/custom_conversions.json
--rw-r--r--   0        0        0     1195 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/images.json
--rw-r--r--   0        0        0      764 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/ads_action_stats.json
--rw-r--r--   0        0        0      302 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/ads_histogram_stats.json
--rw-r--r--   0        0        0     1341 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/ads_image_crops.json
--rw-r--r--   0        0        0     3152 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/geo_locations.json
--rw-r--r--   0        0        0     7241 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/targeting.json
--rw-r--r--   0        0        0     2403 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/videos.json
--rw-r--r--   0        0        0    13493 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/source.py
--rw-r--r--   0        0        0    10791 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/spec.py
--rw-r--r--   0        0        0     1728 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/__init__.py
--rw-r--r--   0        0        0    13938 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/async_job.py
--rw-r--r--   0        0        0     6544 2024-04-04 14:20:01.540351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/async_job_manager.py
--rw-r--r--   0        0        0    17218 2024-04-04 14:20:01.544351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/base_insight_streams.py
--rw-r--r--   0        0        0    15508 2024-04-04 14:20:01.544351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/base_streams.py
--rw-r--r--   0        0        0     6949 2024-04-04 14:20:01.544351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/common.py
--rw-r--r--   0        0        0     2484 2024-04-04 14:20:01.544351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/patches.py
--rw-r--r--   0        0        0    13957 2024-04-04 14:20:01.544351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/streams.py
--rw-r--r--   0        0        0     2551 2024-04-04 14:20:01.544351 airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/utils.py
--rw-r--r--   0        0        0     5550 1970-01-01 00:00:00.000000 airbyte_source_facebook_marketing-3.0.0.dev202404041423/PKG-INFO
+-rw-r--r--   0        0        0     4717 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/README.md
+-rw-r--r--   0        0        0      908 2024-05-02 10:55:22.611555 airbyte_source_facebook_marketing-3.0.0.dev202405021055/pyproject.toml
+-rw-r--r--   0        0        0     4784 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/README.md
+-rw-r--r--   0        0        0      455 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/__init__.py
+-rw-r--r--   0        0        0     8030 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/api.py
+-rw-r--r--   0        0        0     5175 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/config_migrations.py
+-rw-r--r--   0        0        0      469 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/run.py
+-rw-r--r--   0        0        0     1978 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/activities.json
+-rw-r--r--   0        0        0    11759 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/ad_account.json
+-rw-r--r--   0        0        0    47204 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/ad_creatives.json
+-rw-r--r--   0        0        0     5227 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/ad_sets.json
+-rw-r--r--   0        0        0    17173 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/ads.json
+-rw-r--r--   0        0        0    13643 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/ads_insights.json
+-rw-r--r--   0        0        0     1443 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/ads_insights_action_breakdowns.json
+-rw-r--r--   0        0        0     5569 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/ads_insights_breakdowns.json
+-rw-r--r--   0        0        0     4899 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/campaigns.json
+-rw-r--r--   0        0        0     7458 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/custom_audiences.json
+-rw-r--r--   0        0        0     2954 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/custom_conversions.json
+-rw-r--r--   0        0        0     2517 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/images.json
+-rw-r--r--   0        0        0      764 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/shared/ads_action_stats.json
+-rw-r--r--   0        0        0      302 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/shared/ads_histogram_stats.json
+-rw-r--r--   0        0        0     1341 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/shared/ads_image_crops.json
+-rw-r--r--   0        0        0     3152 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/shared/geo_locations.json
+-rw-r--r--   0        0        0     7241 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/shared/targeting.json
+-rw-r--r--   0        0        0     4838 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/videos.json
+-rw-r--r--   0        0        0    13493 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/source.py
+-rw-r--r--   0        0        0    10791 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/spec.py
+-rw-r--r--   0        0        0     1728 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/__init__.py
+-rw-r--r--   0        0        0    13938 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/async_job.py
+-rw-r--r--   0        0        0     6544 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/async_job_manager.py
+-rw-r--r--   0        0        0    17771 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/base_insight_streams.py
+-rw-r--r--   0        0        0    15508 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/base_streams.py
+-rw-r--r--   0        0        0     8279 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/common.py
+-rw-r--r--   0        0        0     2484 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/patches.py
+-rw-r--r--   0        0        0    13957 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/streams.py
+-rw-r--r--   0        0        0     2569 2024-05-02 07:59:51.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/utils.py
+-rw-r--r--   0        0        0     5557 1970-01-01 00:00:00.000000 airbyte_source_facebook_marketing-3.0.0.dev202405021055/PKG-INFO
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/README.md` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 ### Locally running the connector
 ```
 poetry run source-facebook-marketing spec
 poetry run source-facebook-marketing check --config secrets/config.json
 poetry run source-facebook-marketing discover --config secrets/config.json
-poetry run source-facebook-marketing read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-facebook-marketing read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 ```
 poetry run pytest unit_tests
 ```
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/pyproject.toml` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "3.0.0.dev202404041423"
+version = "3.0.0.dev202405021055"
 name = "airbyte-source-facebook-marketing"
 description = "Source implementation for Facebook Marketing."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_facebook_marketing" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.81.6"
 facebook-business = "19.0.0"
 cached-property = "==1.5.2"
 
 [tool.poetry.scripts]
 source-facebook-marketing = "source_facebook_marketing.run:run"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/README.md` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/api.py` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/api.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/config_migrations.py` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/config_migrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         This method determines whether the config should be migrated to have the new structure for the `custom_reports`,
         based on the source spec.
         Returns:
             > True, if the transformation is necessary
             > False, otherwise.
             > Raises the Exception if the structure could not be migrated.
         """
-        return False if config.get(cls.migrate_to_key) else True
+        return cls.migrate_from_key in config and cls.migrate_to_key not in config
 
     @classmethod
     def transform(cls, config: Mapping[str, Any]) -> Mapping[str, Any]:
         # transform the config
         config[cls.migrate_to_key] = [config[cls.migrate_from_key]]
         # return transformed config
         return config
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ad_account.json` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/shared/targeting.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.25%*

 * *Differences: {"'definitions'": "OrderedDict([('id_name_pairs', OrderedDict([('items', OrderedDict([('type', "*

 * *                  "['null', 'object']), ('properties', OrderedDict([('name', OrderedDict([('type', "*

 * *                  "['null', 'string'])])), ('id', OrderedDict([('type', ['null', "*

 * *                  "'string'])]))]))])), ('type', ['null', 'array'])])), ('targeting_fields', "*

 * *                  "OrderedDict([('type', ['null', 'object']), ('properties', "*

 * *                  "OrderedDict([('household_composition', […]*

```diff
@@ -1,505 +1,416 @@
 {
-    "additionalProperties": true,
-    "properties": {
-        "account_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "account_status": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "age": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "amount_spent": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "balance": {
+    "definitions": {
+        "id_name_pairs": {
+            "items": {
+                "properties": {
+                    "id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "business": {
+        "targeting_fields": {
             "properties": {
-                "id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
+                "behaviors": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "connections": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "custom_audiences": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "education_majors": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "excluded_connections": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
                 },
-                "name": {
+                "excluded_custom_audiences": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "family_statuses": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "friends_of_connections": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "generation": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "home_ownership": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "home_type": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "household_composition": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "income": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "industries": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "interests": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "life_events": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "moms": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "net_worth": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "politics": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "relationship_statuses": {
+                    "items": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
                     "type": [
                         "null",
-                        "string"
+                        "array"
                     ]
+                },
+                "user_adclusters": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "work_employers": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
+                },
+                "work_positions": {
+                    "$ref": "targeting.json#/definitions/id_name_pairs"
                 }
             },
             "type": [
                 "null",
                 "object"
             ]
-        },
-        "business_city": {
+        }
+    },
+    "properties": {
+        "age_max": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "business_country_code": {
+        "age_min": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "business_name": {
+        "app_install_state": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "business_state": {
+        "audience_network_positions": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "business_street": {
-            "type": [
-                "null",
-                "string"
-            ]
+        "behaviors": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "business_street2": {
+        "brand_safety_content_filter_levels": {
+            "items": {
+                "type": "string"
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "business_zip": {
-            "type": [
-                "null",
-                "string"
-            ]
+        "connections": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "can_create_brand_lift_study": {
-            "type": [
-                "null",
-                "boolean"
-            ]
+        "custom_audiences": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "capabilities": {
+        "device_platforms": {
             "items": {
-                "type": "string"
+                "type": [
+                    "null",
+                    "string"
+                ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "created_time": {
-            "format": "date-time",
-            "type": "string"
-        },
-        "currency": {
+        "education_statuses": {
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "disable_reason": {
-            "type": [
-                "null",
-                "number"
-            ]
+        "excluded_connections": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "end_advertiser": {
-            "type": [
-                "null",
-                "number"
-            ]
+        "excluded_custom_audiences": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "end_advertiser_name": {
-            "type": [
-                "null",
-                "string"
-            ]
+        "excluded_geo_locations": {
+            "$ref": "geo_locations.json"
         },
-        "extended_credit_invoice_group": {
-            "properties": {
-                "auto_enroll": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                },
-                "customer_po_number": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "email": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "emails": {
-                    "items": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "type": [
-                        "null",
-                        "array"
-                    ]
-                },
-                "id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
+        "excluded_publisher_categories": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
             },
             "type": [
                 "null",
-                "object"
+                "array"
             ]
         },
-        "failed_delivery_checks": {
+        "excluded_user_device": {
             "items": {
-                "properties": {
-                    "check_name": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "description": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "summary": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
-                },
                 "type": [
                     "null",
-                    "object"
+                    "string"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "fb_entity": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "funding_source": {
-            "type": [
-                "null",
-                "number"
-            ]
+        "exclusions": {
+            "$ref": "targeting.json#/definitions/targeting_fields"
         },
-        "funding_source_details": {
-            "properties": {
-                "display_string": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "type": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                }
+        "facebook_positions": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
             },
             "type": [
                 "null",
-                "object"
+                "array"
             ]
         },
-        "has_migrated_permissions": {
-            "type": [
-                "null",
-                "boolean"
-            ]
+        "family_statuses": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "id": {
+        "flexible_spec": {
+            "items": {
+                "$ref": "targeting.json#/definitions/targeting_fields"
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "io_number": {
-            "type": [
-                "null",
-                "number"
-            ]
+        "friends_of_connections": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "is_attribution_spec_system_default": {
+        "genders": {
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "boolean"
+                "array"
             ]
         },
-        "is_direct_deals_enabled": {
-            "type": [
-                "null",
-                "boolean"
-            ]
+        "generation": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "is_in_3ds_authorization_enabled_market": {
-            "type": [
-                "null",
-                "boolean"
-            ]
+        "geo_locations": {
+            "$ref": "geo_locations.json"
         },
-        "is_notifications_enabled": {
-            "type": [
-                "null",
-                "boolean"
-            ]
+        "home_ownership": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "is_personal": {
-            "type": [
-                "null",
-                "number"
-            ]
+        "home_type": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "is_prepay_account": {
-            "type": [
-                "null",
-                "boolean"
-            ]
+        "income": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "is_tax_id_required": {
-            "type": [
-                "null",
-                "boolean"
-            ]
+        "industries": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "line_numbers": {
+        "instagram_positions": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
             "type": [
                 "null",
-                "number"
+                "array"
             ]
         },
-        "media_agency": {
+        "interested_in": {
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "number"
+                "array"
             ]
         },
-        "min_campaign_group_spend_cap": {
-            "type": [
-                "null",
-                "number"
-            ]
+        "interests": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "min_daily_budget": {
+        "locales": {
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "number"
+                "array"
             ]
         },
-        "name": {
+        "messenger_positions": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "offsite_pixels_tos_accepted": {
-            "type": [
-                "null",
-                "boolean"
-            ]
+        "moms": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "owner": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "partner": {
-            "type": [
-                "null",
-                "number"
-            ]
+        "net_worth": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "rf_spec": {
-            "properties": {
-                "countries": {
-                    "items": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "type": [
-                        "null",
-                        "array"
-                    ]
-                },
-                "global_io_max_campaign_duration": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "max_campaign_duration": {
-                    "additionalProperties": true,
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "max_days_to_finish": {
-                    "additionalProperties": true,
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "min_campaign_duration": {
-                    "additionalProperties": true,
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                },
-                "min_reach_limits": {
-                    "additionalProperties": true,
-                    "type": [
-                        "null",
-                        "object"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
+        "office_type": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "spend_cap": {
-            "type": [
-                "null",
-                "string"
-            ]
+        "politics": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "tax_id": {
+        "publisher_platforms": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "tax_id_status": {
+        "relationship_statuses": {
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "number"
+                "array"
             ]
         },
-        "tax_id_type": {
+        "targeting_optimization": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "timezone_id": {
+        "targeting_relaxation_types": {
             "type": [
                 "null",
-                "number"
-            ]
-        },
-        "timezone_name": {
-            "type": [
-                "null",
-                "string"
+                "object"
             ]
         },
-        "timezone_offset_hours_utc": {
-            "type": [
-                "null",
-                "number"
-            ]
+        "user_adclusters": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         },
-        "tos_accepted": {
-            "properties": {
-                "web_custom_audience_tos": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                }
+        "user_device": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
             },
             "type": [
                 "null",
-                "object"
+                "array"
             ]
         },
-        "user_tasks": {
+        "user_os": {
             "items": {
                 "type": [
                     "null",
                     "string"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "user_tos_accepted": {
-            "properties": {
-                "web_custom_audience_tos": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                }
-            },
-            "type": [
-                "null",
-                "object"
-            ]
+        "work_positions": {
+            "$ref": "targeting.json#/definitions/id_name_pairs"
         }
     },
-    "type": "object"
+    "type": [
+        "null",
+        "object"
+    ]
 }
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/ad_sets.json` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/shared/geo_locations.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('regions', OrderedDict([('items', OrderedDict([('type', "*

 * *                 "['null', 'object']), ('properties', OrderedDict([('name', OrderedDict([('type', "*

 * *                 "['null', 'string'])])), ('country', OrderedDict([('type', ['null', "*

 * *                 "'string'])])), ('key', OrderedDict([('type', ['null', 'string'])]))]))])), "*

 * *                 "('type', ['null', 'array'])])), ('countries', OrderedDict([('items', "*

 * *                 "OrderedDict([('type', [ […]*

```diff
@@ -1,225 +1,269 @@
 {
     "properties": {
-        "account_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "adlabels": {
+        "cities": {
             "items": {
                 "properties": {
-                    "created_time": {
-                        "format": "date-time",
-                        "type": "string"
+                    "country": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
                     },
-                    "id": {
-                        "type": "string"
+                    "distance_unit": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "key": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
                     },
                     "name": {
-                        "type": "string"
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "radius": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "region": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
                     },
-                    "updated_time": {
-                        "format": "date-time",
-                        "type": "string"
+                    "region_id": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
                     }
                 },
-                "type": "object"
+                "type": [
+                    "null",
+                    "object"
+                ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "bid_amount": {
+        "countries": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
             "type": [
                 "null",
-                "number"
+                "array"
             ]
         },
-        "bid_constraints": {
-            "properties": {
-                "roas_average_floor": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                }
+        "country_groups": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
             },
             "type": [
                 "null",
-                "object"
+                "array"
             ]
         },
-        "bid_info": {
-            "properties": {
-                "ACTIONS": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "CLICKS": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "IMPRESSIONS": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
+        "custom_locations": {
+            "items": {
+                "properties": {
+                    "address_string": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "country": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "distance_unit": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "latitude": {
+                        "type": [
+                            "null",
+                            "number"
+                        ]
+                    },
+                    "longitude": {
+                        "type": [
+                            "null",
+                            "number"
+                        ]
+                    },
+                    "name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "primary_city_id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "radius": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "region_id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    }
                 },
-                "REACH": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                }
+                "type": [
+                    "null",
+                    "object"
+                ]
             },
             "type": [
                 "null",
-                "object"
-            ]
-        },
-        "bid_strategy": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "budget_remaining": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "campaign_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "created_time": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "daily_budget": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "effective_status": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "end_time": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "id": {
-            "type": [
-                "null",
-                "string"
+                "array"
             ]
         },
-        "lifetime_budget": {
+        "geo-markets": {
+            "items": {
+                "properties": {
+                    "key": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
             "type": [
                 "null",
-                "number"
+                "array"
             ]
         },
-        "name": {
+        "location_types": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "promoted_object": {
-            "properties": {
-                "application_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "custom_event_type": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "object_store_url": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "offer_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "page_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "pixel_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "pixel_rule": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
+        "regions": {
+            "items": {
+                "properties": {
+                    "country": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "key": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
                 },
-                "product_set_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
+                "type": [
+                    "null",
+                    "object"
+                ]
             },
             "type": [
                 "null",
-                "object"
-            ]
-        },
-        "start_time": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
+                "array"
             ]
         },
-        "targeting": {
-            "$ref": "targeting.json"
-        },
-        "updated_time": {
-            "format": "date-time",
+        "zips": {
+            "items": {
+                "properties": {
+                    "country": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "key": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "name": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "primary_city_id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    },
+                    "region_id": {
+                        "type": [
+                            "null",
+                            "integer"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         }
     },
     "type": [
         "null",
         "object"
     ]
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/campaigns.json` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/custom_conversions.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7644230769230769%*

 * *Differences: {"'properties'": "{'account_id': {'description': 'Unique identifier for the Facebook ad "*

 * *                 "account.'}, 'id': {'description': 'Unique identifier for the custom "*

 * *                 "conversion.'}, 'name': {'description': 'Name of the custom conversion.'}, "*

 * *                 "'business': OrderedDict([('description', 'Information about the business "*

 * *                 "associated with the custom conversion.'), ('type', ['null', 'string'])]), "*

 * *                 "'creation_time': OrderedDict([('des […]*

```diff
@@ -1,195 +1,138 @@
 {
     "properties": {
         "account_id": {
+            "description": "Unique identifier for the Facebook ad account.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "adlabels": {
-            "items": {
-                "properties": {
-                    "created_time": {
-                        "format": "date-time",
-                        "type": "string"
-                    },
-                    "id": {
-                        "type": "string"
-                    },
-                    "name": {
-                        "type": "string"
-                    },
-                    "updated_time": {
-                        "format": "date-time",
-                        "type": "string"
-                    }
-                },
-                "type": "object"
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "bid_strategy": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "boosted_object_id": {
+        "business": {
+            "description": "Information about the business associated with the custom conversion.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "budget_rebalance_flag": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "budget_remaining": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "buying_type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "configured_status": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "created_time": {
+        "creation_time": {
+            "description": "Date and time when the custom conversion was created.",
             "format": "date-time",
             "type": "string"
         },
-        "daily_budget": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "effective_status": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "id": {
+        "custom_event_type": {
+            "description": "Type of custom event triggering the conversion.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "issues_info": {
+        "data_sources": {
+            "description": "Data sources related to the custom conversion.",
             "items": {
                 "properties": {
-                    "error_code": {
-                        "type": "string"
-                    },
-                    "error_message": {
-                        "type": "string"
-                    },
-                    "error_summary": {
+                    "id": {
+                        "description": "Identifier of the data source.",
                         "type": "string"
                     },
-                    "error_type": {
+                    "name": {
+                        "description": "Name of the data source.",
                         "type": "string"
                     },
-                    "level": {
+                    "source_type": {
+                        "description": "Type of data source.",
                         "type": "string"
                     }
                 },
                 "type": "object"
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "lifetime_budget": {
+        "default_conversion_value": {
+            "description": "Default value assigned to the conversion event if no specific value is provided.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "name": {
+        "description": {
+            "description": "Brief description of the custom conversion.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "objective": {
+        "event_source_type": {
+            "description": "Type of event source triggering the custom conversion.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "smart_promotion_type": {
+        "first_fired_time": {
+            "description": "Date and time when the custom conversion was first triggered.",
+            "format": "date-time",
+            "type": "string"
+        },
+        "id": {
+            "description": "Unique identifier for the custom conversion.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "source_campaign_id": {
+        "is_archived": {
+            "description": "Flag indicating if the custom conversion is archived.",
             "type": [
                 "null",
-                "number"
+                "boolean"
             ]
         },
-        "special_ad_category": {
+        "is_unavailable": {
+            "description": "Flag indicating if the custom conversion is unavailable.",
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "last_fired_time": {
+            "description": "Date and time when the custom conversion was last triggered.",
+            "format": "date-time",
+            "type": "string"
+        },
+        "name": {
+            "description": "Name of the custom conversion.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "special_ad_category_country": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
+        "offline_conversion_data_set": {
+            "description": "If applicable, the data set for offline conversions.",
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
-        "spend_cap": {
+        "retention_days": {
+            "description": "Number of days for which the conversion data is retained.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "start_time": {
-            "format": "date-time",
-            "type": "string"
-        },
-        "status": {
+        "rule": {
+            "description": "Rules or conditions triggering the custom conversion.",
             "type": [
                 "null",
                 "string"
             ]
-        },
-        "stop_time": {
-            "format": "date-time",
-            "type": "string"
-        },
-        "updated_time": {
-            "format": "date-time",
-            "type": "string"
         }
     },
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/custom_conversions.json` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/activities.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7564655172413793%*

 * *Differences: {"'properties'": "{'account_id': {'description': 'The unique identifier for the account associated "*

 * *                 "with the activity.'}, 'actor_id': OrderedDict([('description', 'The unique "*

 * *                 "identifier for the actor (user/page) who performed the activity.'), ('type', "*

 * *                 "['null', 'string'])]), 'actor_name': OrderedDict([('description', 'The name of "*

 * *                 "the actor (user/page) who performed the activity.'), ('type', ['null', "*

 * *                 "'string'])] […]*

```diff
@@ -1,114 +1,93 @@
 {
     "properties": {
         "account_id": {
+            "description": "The unique identifier for the account associated with the activity.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "business": {
+        "actor_id": {
+            "description": "The unique identifier for the actor (user/page) who performed the activity.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "creation_time": {
-            "format": "date-time",
-            "type": "string"
-        },
-        "custom_event_type": {
+        "actor_name": {
+            "description": "The name of the actor (user/page) who performed the activity.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "data_sources": {
-            "items": {
-                "properties": {
-                    "id": {
-                        "type": "string"
-                    },
-                    "name": {
-                        "type": "string"
-                    },
-                    "source_type": {
-                        "type": "string"
-                    }
-                },
-                "type": "object"
-            },
+        "application_id": {
+            "description": "The unique identifier for the application involved in the activity.",
             "type": [
                 "null",
-                "array"
-            ]
-        },
-        "default_conversion_value": {
-            "type": [
-                "null",
-                "number"
+                "string"
             ]
         },
-        "description": {
+        "application_name": {
+            "description": "The name of the application involved in the activity.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "event_source_type": {
+        "date_time_in_timezone": {
+            "description": "The date and time of the activity adjusted to the timezone.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "first_fired_time": {
+        "event_time": {
+            "description": "The exact date and time when the activity occurred.",
             "format": "date-time",
             "type": "string"
         },
-        "id": {
+        "event_type": {
+            "description": "The type of event/action performed in the activity.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "is_archived": {
+        "extra_data": {
+            "description": "Additional data associated with the activity.",
             "type": [
                 "null",
-                "boolean"
-            ]
-        },
-        "is_unavailable": {
-            "type": [
-                "null",
-                "boolean"
+                "string"
             ]
         },
-        "last_fired_time": {
-            "format": "date-time",
-            "type": "string"
-        },
-        "name": {
+        "object_id": {
+            "description": "The unique identifier for the object (post/ad/etc.) related to the activity.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "offline_conversion_data_set": {
+        "object_name": {
+            "description": "The name/label of the object related to the activity.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "retention_days": {
+        "object_type": {
+            "description": "The type/category of the object related to the activity.",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "rule": {
+        "translated_event_type": {
+            "description": "The translated or localized version of the event type.",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": [
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/images.json` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/shared/ads_image_crops.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('100x100', OrderedDict([('items', OrderedDict([('items', "*

 * *                 "OrderedDict([('type', ['null', 'integer'])])), ('type', ['null', 'array'])])), "*

 * *                 "('type', ['null', 'array'])])), ('100x72', OrderedDict([('items', "*

 * *                 "OrderedDict([('items', OrderedDict([('type', ['null', 'integer'])])), ('type', "*

 * *                 "['null', 'array'])])), ('type', ['null', 'array'])])), ('191x100', "*

 * *                 "OrderedDict([('items', […]*

```diff
@@ -1,110 +1,134 @@
 {
-    "additionalProperties": true,
     "properties": {
-        "account_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "created_time": {
-            "format": "date-time",
-            "type": "string"
-        },
-        "creatives": {
+        "100x100": {
             "items": {
+                "items": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
                 "type": [
                     "null",
-                    "string"
+                    "array"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "filename": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "hash": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "height": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "is_associated_creatives_in_adgroups": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "original_height": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "original_width": {
+        "100x72": {
+            "items": {
+                "items": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "type": [
+                    "null",
+                    "array"
+                ]
+            },
             "type": [
                 "null",
-                "integer"
+                "array"
             ]
         },
-        "permalink_url": {
+        "191x100": {
+            "items": {
+                "items": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "type": [
+                    "null",
+                    "array"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "status": {
+        "400x150": {
+            "items": {
+                "items": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "type": [
+                    "null",
+                    "array"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "updated_time": {
-            "format": "date-time",
-            "type": "string"
-        },
-        "url": {
+        "400x500": {
+            "items": {
+                "items": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "type": [
+                    "null",
+                    "array"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "url_128": {
+        "600x360": {
+            "items": {
+                "items": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "type": [
+                    "null",
+                    "array"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "width": {
+        "90x160": {
+            "items": {
+                "items": {
+                    "type": [
+                        "null",
+                        "integer"
+                    ]
+                },
+                "type": [
+                    "null",
+                    "array"
+                ]
+            },
             "type": [
                 "null",
-                "integer"
+                "array"
             ]
         }
     },
-    "type": "object"
+    "type": [
+        "null",
+        "object"
+    ]
 }
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/ads_action_stats.json` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/shared/ads_action_stats.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/schemas/shared/geo_locations.json` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/schemas/images.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'additionalProperties'": 'True',*

 * * "'properties'": "{replace: OrderedDict([('account_id', OrderedDict([('description', 'The unique "*

 * *                 'identifier of the Facebook advertising account associated with the image '*

 * *                 "data.'), ('type', ['null', 'string'])])), ('id', OrderedDict([('description', "*

 * *                 "'The unique identifier of the image data.'), ('type', ['null', 'string'])])), "*

 * *                 "('name', OrderedDict([('description', 'The name or label assigned to th […]*

```diff
@@ -1,270 +1,127 @@
 {
+    "additionalProperties": true,
     "properties": {
-        "cities": {
-            "items": {
-                "properties": {
-                    "country": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "distance_unit": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "key": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "name": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "radius": {
-                        "type": [
-                            "null",
-                            "integer"
-                        ]
-                    },
-                    "region": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "region_id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
-                },
-                "type": [
-                    "null",
-                    "object"
-                ]
-            },
+        "account_id": {
+            "description": "The unique identifier of the Facebook advertising account associated with the image data.",
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
-        "countries": {
+        "created_time": {
+            "description": "The date and time when the image was initially created.",
+            "format": "date-time",
+            "type": "string"
+        },
+        "creatives": {
+            "description": "Additional information or metadata related to the image.",
             "items": {
                 "type": [
                     "null",
                     "string"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "country_groups": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
+        "filename": {
+            "description": "The name of the file containing the image data.",
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
-        "custom_locations": {
-            "items": {
-                "properties": {
-                    "address_string": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "country": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "distance_unit": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "latitude": {
-                        "type": [
-                            "null",
-                            "number"
-                        ]
-                    },
-                    "longitude": {
-                        "type": [
-                            "null",
-                            "number"
-                        ]
-                    },
-                    "name": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "primary_city_id": {
-                        "type": [
-                            "null",
-                            "integer"
-                        ]
-                    },
-                    "radius": {
-                        "type": [
-                            "null",
-                            "integer"
-                        ]
-                    },
-                    "region_id": {
-                        "type": [
-                            "null",
-                            "integer"
-                        ]
-                    }
-                },
-                "type": [
-                    "null",
-                    "object"
-                ]
-            },
+        "hash": {
+            "description": "A unique hash value generated for the image.",
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
-        "geo-markets": {
-            "items": {
-                "properties": {
-                    "key": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "name": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
-                },
-                "type": [
-                    "null",
-                    "object"
-                ]
-            },
+        "height": {
+            "description": "The height dimension of the image in pixels.",
             "type": [
                 "null",
-                "array"
+                "integer"
             ]
         },
-        "location_types": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
+        "id": {
+            "description": "The unique identifier of the image data.",
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
-        "regions": {
-            "items": {
-                "properties": {
-                    "country": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "key": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "name": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
-                },
-                "type": [
-                    "null",
-                    "object"
-                ]
-            },
+        "is_associated_creatives_in_adgroups": {
+            "description": "Indicates if the image is associated with creatives in ad groups.",
             "type": [
                 "null",
-                "array"
+                "boolean"
             ]
         },
-        "zips": {
-            "items": {
-                "properties": {
-                    "country": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "key": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "name": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "primary_city_id": {
-                        "type": [
-                            "null",
-                            "integer"
-                        ]
-                    },
-                    "region_id": {
-                        "type": [
-                            "null",
-                            "integer"
-                        ]
-                    }
-                },
-                "type": [
-                    "null",
-                    "object"
-                ]
-            },
+        "name": {
+            "description": "The name or label assigned to the image.",
             "type": [
                 "null",
-                "array"
+                "string"
+            ]
+        },
+        "original_height": {
+            "description": "The original height dimension of the image in pixels.",
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "original_width": {
+            "description": "The original width dimension of the image in pixels.",
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "permalink_url": {
+            "description": "The permanent URL where the image can be accessed or viewed.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "status": {
+            "description": "The current status or state of the image data.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "updated_time": {
+            "description": "The date and time when the image data was last updated.",
+            "format": "date-time",
+            "type": "string"
+        },
+        "url": {
+            "description": "The URL pointing to the image file.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "url_128": {
+            "description": "The URL pointing to a lower resolution (128px) version of the image file.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "width": {
+            "description": "The width dimension of the image in pixels.",
+            "type": [
+                "null",
+                "integer"
             ]
         }
     },
-    "type": [
-        "null",
-        "object"
-    ]
+    "type": "object"
 }
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/source.py` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/spec.py` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/spec.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/__init__.py` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/async_job.py` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/async_job.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/async_job_manager.py` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/async_job_manager.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/base_insight_streams.py` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/base_insight_streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,18 @@
             if breakdown in record:
                 record[self.object_breakdowns[breakdown]] = record[breakdown]["id"]
         return record
 
     def list_objects(self, params: Mapping[str, Any]) -> Iterable:
         """Because insights has very different read_records we don't need this method anymore"""
 
+    def _add_account_id(self, record: dict[str, Any], account_id: str):
+        if "account_id" not in record:
+            record["account_id"] = account_id
+
     def read_records(
         self,
         sync_mode: SyncMode,
         cursor_field: List[str] = None,
         stream_slice: Mapping[str, Any] = None,
         stream_state: Mapping[str, Any] = None,
     ) -> Iterable[Mapping[str, Any]]:
@@ -152,14 +156,15 @@
         job = stream_slice["insight_job"]
         account_id = stream_slice["account_id"]
 
         try:
             for obj in job.get_result():
                 data = obj.export_all_data()
                 if self._response_data_is_valid(data):
+                    self._add_account_id(data, account_id)
                     yield self._transform_breakdown(data)
         except FacebookBadObjectError as e:
             raise AirbyteTracedException(
                 message=f"API error occurs on Facebook side during job: {job}, wrong (empty) response received with errors: {e} "
                 f"Please try again later",
                 failure_type=FailureType.system_error,
             ) from e
@@ -319,15 +324,15 @@
             - don't read data older than retention date
         Also there are difference between start_date and cursor_value in how the value must be interpreted:
             - cursor - last value that we synced
             - start_date - the first value that should be synced
 
         :return: the first date to sync
         """
-        today = pendulum.today().date()
+        today = pendulum.today(tz=pendulum.tz.UTC).date()
         oldest_date = today - self.INSIGHTS_RETENTION_PERIOD
 
         start_dates_for_account = {}
         for account_id in self._account_ids:
             cursor_value = self._cursor_values.get(account_id) if self._cursor_values else None
             if cursor_value:
                 start_date = cursor_value
@@ -375,14 +380,19 @@
         if self._custom_fields:
             # 'date_stop' and 'account_id' are also returned by default, even if they are not requested
             custom_fields = set(self._custom_fields + [self.cursor_field, "date_stop", "account_id", "ad_id"])
             schema["properties"] = {k: v for k, v in schema["properties"].items() if k in custom_fields}
         if self.breakdowns:
             breakdowns_properties = loader.get_schema("ads_insights_breakdowns")["properties"]
             schema["properties"].update({prop: breakdowns_properties[prop] for prop in self.breakdowns})
+            # adding object breakdown id to schema
+            for prop in self.breakdowns:
+                object_breakdown_id = self.object_breakdowns.get(prop)
+                if object_breakdown_id:
+                    schema["properties"].update({object_breakdown_id: breakdowns_properties[object_breakdown_id]})
         return schema
 
     def fields(self, **kwargs) -> List[str]:
         """List of fields that we want to query, for now just all properties from stream's schema"""
         if self._custom_fields:
             return self._custom_fields
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/base_streams.py` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/base_streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/common.py` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import http.client
 import logging
+import re
 import sys
 from typing import Any
 
 import backoff
 import pendulum
 from airbyte_cdk.models import FailureType
 from airbyte_cdk.utils import AirbyteTracedException
 from facebook_business.exceptions import FacebookRequestError
 
 # The Facebook API error codes indicating rate-limiting are listed at
 # https://developers.facebook.com/docs/graph-api/overview/rate-limiting/
-FACEBOOK_RATE_LIMIT_ERROR_CODES = (
+FACEBOOK_RATE_LIMIT_ERROR_CODES = {
     4,
     17,
     32,
     613,
     80000,
     80001,
     80002,
     80003,
     80004,
     80005,
     80006,
     80008,
-)
+}
 FACEBOOK_TEMPORARY_OAUTH_ERROR_CODE = 2
 FACEBOOK_BATCH_ERROR_CODE = 960
 FACEBOOK_UNKNOWN_ERROR_CODE = 99
 FACEBOOK_CONNECTION_RESET_ERROR_CODE = 104
 DEFAULT_SLEEP_INTERVAL = pendulum.duration(minutes=1)
 
 logger = logging.getLogger("airbyte")
@@ -80,41 +81,53 @@
         """
         # reference issue: https://github.com/airbytehq/airbyte/issues/25383
         # set the flag to the api class that the last api call was successful
         details.get("args")[0].last_api_call_is_successfull = True
         # set the flag to the api class that the `limit` param is restored
         details.get("args")[0].request_record_limit_is_reduced = False
 
+    def give_up(details):
+        if isinstance(details["exception"], FacebookRequestError):
+            raise traced_exception(details["exception"])
+
+    def is_transient_cannot_include_error(exc: FacebookRequestError) -> bool:
+        """After migration to API v19.0, some customers randomly face a BAD_REQUEST error (OAuthException) with the pattern:"Cannot include ..."
+        According to the last comment in https://developers.facebook.com/community/threads/286697364476462/, this might be a transient issue that can be solved with a retry."""
+        pattern = r"Cannot include .* in summary param because they weren't there while creating the report run."
+        return bool(exc.http_status() == http.client.BAD_REQUEST and re.search(pattern, exc.api_error_message()))
+
     def should_retry_api_error(exc):
         if isinstance(exc, FacebookRequestError):
             call_rate_limit_error = exc.api_error_code() in FACEBOOK_RATE_LIMIT_ERROR_CODES
             temporary_oauth_error = exc.api_error_code() == FACEBOOK_TEMPORARY_OAUTH_ERROR_CODE
             batch_timeout_error = exc.http_status() == http.client.BAD_REQUEST and exc.api_error_code() == FACEBOOK_BATCH_ERROR_CODE
             unknown_error = exc.api_error_subcode() == FACEBOOK_UNKNOWN_ERROR_CODE
             connection_reset_error = exc.api_error_code() == FACEBOOK_CONNECTION_RESET_ERROR_CODE
             server_error = exc.http_status() == http.client.INTERNAL_SERVER_ERROR
             return any(
                 (
                     exc.api_transient_error(),
                     unknown_error,
                     call_rate_limit_error,
                     batch_timeout_error,
+                    is_transient_cannot_include_error(exc),
                     connection_reset_error,
                     temporary_oauth_error,
                     server_error,
                 )
             )
         return True
 
     return backoff.on_exception(
         backoff_type,
         exception,
         jitter=None,
         on_backoff=[log_retry_attempt, reduce_request_record_limit],
         on_success=[revert_request_record_limit],
+        on_giveup=[give_up],
         giveup=lambda exc: not should_retry_api_error(exc),
         **wait_gen_kwargs,
     )
 
 
 def deep_merge(a: Any, b: Any) -> Any:
     """Merge two values, with `b` taking precedence over `a`."""
@@ -163,14 +176,22 @@
             failure_type = FailureType.config_error
             friendly_msg = (
                 "Current profile is not linked to delegate page. Check if correct business (not personal) "
                 "Ad Account Id is used (as in Ads Manager), re-authenticate if FB oauth is used or refresh "
                 "access token with all required permissions."
             )
 
+    elif fb_exception.api_error_code() in FACEBOOK_RATE_LIMIT_ERROR_CODES:
+        return AirbyteTracedException(
+            message="The maximum number of requests on the Facebook API has been reached. See https://developers.facebook.com/docs/graph-api/overview/rate-limiting/ for more information",
+            internal_message=str(fb_exception),
+            failure_type=FailureType.transient_error,
+            exception=fb_exception,
+        )
+
     else:
         failure_type = FailureType.system_error
         friendly_msg = f"Error: {fb_exception.api_error_code()}, {fb_exception.api_error_message()}."
 
     return AirbyteTracedException(
         message=friendly_msg or msg,
         internal_message=msg,
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/patches.py` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/patches.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/streams/streams.py` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/streams/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/source_facebook_marketing/utils.py` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/source_facebook_marketing/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         return target_date
     if isinstance(target_date, DateTime):
         return target_date.date()
     return pendulum.datetime(target_date.year, target_date.month, target_date.day)
 
 
 def validate_start_date(start_date: DateOrDateTime) -> DateOrDateTime:
-    today = cast_to_type(start_date, pendulum.today())
+    today = cast_to_type(start_date, pendulum.today(tz=pendulum.tz.UTC))
     retention_date = today.subtract(months=DATA_RETENTION_PERIOD)
     if retention_date.day != today.day:
         # `.subtract(months=37)` can be erroneous, for instance:
         # 2023-03-31 - 37 month = 2020-02-29 which is incorrect, should be 2020-03-01
         # that's why we're adjusting the date to the 1st day of the next month
         retention_date = retention_date.replace(month=retention_date.month + 1, day=1)
```

### Comparing `airbyte_source_facebook_marketing-3.0.0.dev202404041423/PKG-INFO` & `airbyte_source_facebook_marketing-3.0.0.dev202405021055/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-facebook-marketing
-Version: 3.0.0.dev202404041423
+Version: 3.0.0.dev202405021055
 Summary: Source implementation for Facebook Marketing.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (==0.81.6)
 Requires-Dist: cached-property (==1.5.2)
 Requires-Dist: facebook-business (==19.0.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/facebook-marketing
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Facebook-Marketing source connector
@@ -47,15 +47,15 @@
 
 
 ### Locally running the connector
 ```
 poetry run source-facebook-marketing spec
 poetry run source-facebook-marketing check --config secrets/config.json
 poetry run source-facebook-marketing discover --config secrets/config.json
-poetry run source-facebook-marketing read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-facebook-marketing read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 ```
 poetry run pytest unit_tests
 ```
```

