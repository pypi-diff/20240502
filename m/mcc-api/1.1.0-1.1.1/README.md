# Comparing `tmp/mcc_api-1.1.0.tar.gz` & `tmp/mcc_api-1.1.1.tar.gz`

## Comparing `mcc_api-1.1.0.tar` & `mcc_api-1.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.1.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 mcc_api-1.1.0/.github/workflows/pypi_publish.yml
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 mcc_api-1.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 mcc_api-1.1.0/docs/conf.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 mcc_api-1.1.0/docs/event.rst
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 mcc_api-1.1.0/docs/index.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mcc_api-1.1.0/docs/island.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/__init__.py
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/event/__init__.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/event/enums.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/event/exceptions.py
--rw-r--r--   0        0        0    13133 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/event/responses.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/island/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/island/auth.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/island/directives.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/island/enums.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/island/scalars.py
--rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/island/types.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/run_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/__init__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/test_event.py
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/test_halloffame.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/test_participants.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/test_rundown.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/200_event.json
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/200_halloffame.json
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/200_halloffame_game.json
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/200_participants.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/200_participants_team.json
--rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/200_rundown.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/404_halloffame_game.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/404_participants_team.json
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/404_rundown.json
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/429_ratelimit.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/island/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/island/test_schema.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.1.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mcc_api-1.1.0/LICENSE
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 mcc_api-1.1.0/README.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mcc_api-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 mcc_api-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.1.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 mcc_api-1.1.1/.github/workflows/pypi_publish.yml
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 mcc_api-1.1.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 mcc_api-1.1.1/docs/conf.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 mcc_api-1.1.1/docs/event.rst
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 mcc_api-1.1.1/docs/index.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mcc_api-1.1.1/docs/island.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/__init__.py
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/event/__init__.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/event/enums.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/event/exceptions.py
+-rw-r--r--   0        0        0    13133 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/event/responses.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/island/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/island/auth.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/island/directives.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/island/enums.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/island/scalars.py
+-rw-r--r--   0        0        0    11084 2020-02-02 00:00:00.000000 mcc_api-1.1.1/mcc_api/island/types.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/run_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/__init__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/test_event.py
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/test_halloffame.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/test_participants.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/test_rundown.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/200_event.json
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/200_halloffame.json
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/200_halloffame_game.json
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/200_participants.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/200_participants_team.json
+-rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/200_rundown.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/404_halloffame_game.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/404_participants_team.json
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/404_rundown.json
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/event/mock_data/429_ratelimit.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/island/__init__.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 mcc_api-1.1.1/tests/island/test_schema.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mcc_api-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 mcc_api-1.1.1/README.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mcc_api-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 mcc_api-1.1.1/PKG-INFO
```

### Comparing `mcc_api-1.1.0/.github/workflows/docs.yml` & `mcc_api-1.1.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/.github/workflows/pypi_publish.yml` & `mcc_api-1.1.1/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/.github/workflows/tests.yml` & `mcc_api-1.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/docs/conf.py` & `mcc_api-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/docs/index.rst` & `mcc_api-1.1.1/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 .. image:: https://img.shields.io/pypi/v/mcc-api?label=🐍%20PyPI
    :alt: 🐍 PyPI
    :target: https://pypi.org/project/mcc-api/
 .. image:: https://img.shields.io/badge/👑_Targeting_Event_API-v1.3.2-red
    :alt: 👑 Targeting Event API v1.3.2
    :target: https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.2
-.. image:: https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.04.17-aqua
-   :alt: 🏝️ Targeting Island API v24.04.17
-   :target: https://github.com/Noxcrew/mccisland-api/releases/tag/v24.04.17
+.. image:: https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.05.02-aqua
+   :alt: 🏝️ Targeting Island API v24.05.02
+   :target: https://github.com/Noxcrew/mccisland-api/releases/tag/v24.05.02
 
 A helper library for the `MC Championship <https://mcchampionship.com>`_ APIs
 (`Event <https://github.com/Noxcrew/mcchampionship-api>`_, inspired by `derNiklaas's <https://github.com/derNiklaas>`_
 `node-mcc-api <https://github.com/derNiklaas/node-mcc-api>`_ project, and
 `Island <https://github.com/Noxcrew/mccisland-api>`_).
 
 - Issues: `https://github.com/JamesMCo/python_mcc_api/issues <https://github.com/JamesMCo/python_mcc_api/issues>`_
```

### Comparing `mcc_api-1.1.0/mcc_api/event/__init__.py` & `mcc_api-1.1.1/mcc_api/event/__init__.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/mcc_api/event/enums.py` & `mcc_api-1.1.1/mcc_api/event/enums.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/mcc_api/event/exceptions.py` & `mcc_api-1.1.1/mcc_api/event/exceptions.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/mcc_api/event/responses.py` & `mcc_api-1.1.1/mcc_api/event/responses.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/mcc_api/island/__init__.py` & `mcc_api-1.1.1/mcc_api/island/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,18 +13,34 @@
 
 __base_url: t.Final[str] = "https://api.mccisland.net/graphql"
 
 schema = GraphQLSchema(
     query=query_type,
     directives=[*specified_directives, one_of_directive, spectaql_directive],
     types=[
-        collections_type, currency_type, party_type, player_type, query_type,
-        server_type, social_type, statistic_type, statistic_value_result_type,
-        statistics_type, status_type, game_enum, rank_enum, server_category_enum,
-        spectaqloption_type
+        collections_type,
+        crown_level_type,
+        currency_type,
+        party_type,
+        player_type,
+        progression_data_type,
+        query_type,
+        server_type,
+        social_type,
+        statistic_type,
+        statistic_value_result_type,
+        statistics_type,
+        status_type,
+        spectaqloption_type,
+        trophy_data_type,
+
+        game_enum,
+        rank_enum,
+        server_category_enum,
+        trophy_category_enum,
     ]
 )
 
 _transport = RequestsHTTPTransport(
     url=__base_url,
     headers={"User-Agent": __user_agent}
 )
```

### Comparing `mcc_api-1.1.0/mcc_api/island/auth.py` & `mcc_api-1.1.1/mcc_api/island/auth.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/mcc_api/island/directives.py` & `mcc_api-1.1.1/mcc_api/island/directives.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/mcc_api/island/enums.py` & `mcc_api-1.1.1/mcc_api/island/enums.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/mcc_api/island/scalars.py` & `mcc_api-1.1.1/mcc_api/island/scalars.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/mcc_api/island/types.py` & `mcc_api-1.1.1/mcc_api/island/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,29 @@
 from graphql import (
     GraphQLArgument, GraphQLBoolean, GraphQLField, GraphQLInputField, GraphQLInputObjectType,
     GraphQLInt, GraphQLList, GraphQLNonNull, GraphQLObjectType, GraphQLString
 )
 
 
 __all__ = [
-    "collections_type", "crown_level_type", "currency_type", "party_type",
-    "player_type", "query_type", "server_type", "social_type", "statistic_type",
-    "statistic_value_result_type", "statistics_type", "status_type",
-    "spectaqloption_type", "trophy_data_type"
+    "collections_type",
+    "crown_level_type",
+    "currency_type",
+    "party_type",
+    "player_type",
+    "progression_data_type",
+    "query_type",
+    "server_type",
+    "social_type",
+    "statistic_type",
+    "statistic_value_result_type",
+    "statistics_type",
+    "status_type",
+    "spectaqloption_type",
+    "trophy_data_type"
 ]
 
 
 collections_type = GraphQLObjectType(
     name="Collections",
     description="Collections data.",
     fields=lambda: {
@@ -29,14 +40,22 @@
     name="CrownLevel",
     description="A Crown Level and associated trophy data.",
     fields=lambda: {
         "level": GraphQLField(
             GraphQLNonNull(GraphQLInt),
             description="The overall Crown Level."
         ),
+        "nextEvolutionLevel": GraphQLField(
+            GraphQLInt,
+            description="The next level that the crown will evolve, if any."
+        ),
+        "nextLevelProgress": GraphQLField(
+            progression_data_type,
+            description="The progress the player is making towards their next level, if any."
+        ),
         "trophies": GraphQLField(
             GraphQLNonNull(trophy_data_type),
             description="The amount of trophies the player has.",
             args={
                 "category": GraphQLArgument(
                     trophy_category_enum,
                     default_value=None
@@ -135,14 +154,29 @@
         "uuid": GraphQLField(
             GraphQLNonNull(uuid_scalar),
             description="The player's Minecraft UUID in dashed format."
         )
     }
 )
 
+progression_data_type = GraphQLObjectType(
+    name="ProgressionData",
+    description="Data for types that track some form of progression.",
+    fields={
+        "obtained": GraphQLField(
+            GraphQLNonNull(GraphQLInt),
+            description="The amount obtained."
+        ),
+        "obtainable": GraphQLField(
+            GraphQLNonNull(GraphQLInt),
+            description="The amount that can be obtained."
+        )
+    }
+)
+
 query_type = GraphQLObjectType(
     name="Query",
     description="Available queries.",
     fields=lambda: {
         "player": GraphQLField(
             player_type,
             description="Given a UUID, returns a Player if they have logged in to MCC Island.",
```

### Comparing `mcc_api-1.1.0/tests/run_tests.py` & `mcc_api-1.1.1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/tests/event/test_event.py` & `mcc_api-1.1.1/tests/event/test_event.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/tests/event/test_halloffame.py` & `mcc_api-1.1.1/tests/event/test_halloffame.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/tests/event/test_participants.py` & `mcc_api-1.1.1/tests/event/test_participants.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/tests/event/test_rundown.py` & `mcc_api-1.1.1/tests/event/test_rundown.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/tests/event/mock_data/200_halloffame.json` & `mcc_api-1.1.1/tests/event/mock_data/200_halloffame.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/tests/event/mock_data/200_participants.json` & `mcc_api-1.1.1/tests/event/mock_data/200_participants.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/tests/event/mock_data/200_participants_team.json` & `mcc_api-1.1.1/tests/event/mock_data/200_participants_team.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/tests/event/mock_data/200_rundown.json` & `mcc_api-1.1.1/tests/event/mock_data/200_rundown.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/tests/island/test_schema.py` & `mcc_api-1.1.1/tests/island/test_schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,18 +12,26 @@
             headers={"User-Agent": mcc_api_user_agent}
         )
 
         if schema_request.status_code != 200:
             self.fail(f"Unable to retrieve MCC Island API schema: {schema_request.status_code} {schema_request.reason}")
         online_schema: graphql.GraphQLSchema = graphql.build_schema(schema_request.text)
 
-        changes = graphql.find_breaking_changes(online_schema, mcc_api.island.schema) +\
-                  graphql.find_dangerous_changes(online_schema, mcc_api.island.schema)
+        changes = [("[online => mcc_api] ", change) for change in
+                       graphql.find_breaking_changes(online_schema, mcc_api.island.schema) +
+                       graphql.find_dangerous_changes(online_schema, mcc_api.island.schema)
+                  ]
+        # Check in reverse direction
+        # (adding something in a new version can be detected as if it was removed from mcc_api.island.schema)
+        changes += [("[mcc_api => online] ", change) for change in
+                        graphql.find_breaking_changes(mcc_api.island.schema, online_schema) +
+                        graphql.find_dangerous_changes(mcc_api.island.schema, online_schema)
+                   ]
 
         self.assertEqual(
             len(changes), 0,
-            "Changes in schema found:\n" + "\n".join(f"{change.type.name}: {change.description}" for change in changes)
+            "Changes in schema found:\n" + "\n".join(f"{direction}{change.type.name}: {change.description}" for direction, change in changes)
         )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mcc_api-1.1.0/.gitignore` & `mcc_api-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/LICENSE` & `mcc_api-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/README.md` & `mcc_api-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Python MCC API
 
 [![🐍 PyPI](https://img.shields.io/pypi/v/mcc-api?label=🐍%20PyPI)](https://pypi.org/project/mcc-api/)
 [![👑 Targeting Event API v1.3.2](https://img.shields.io/badge/👑_Targeting_Event_API-v1.3.2-red)](https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.2)
-[![🏝️ Targeting Island API v24.04.17](https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.04.17-aqua)](https://github.com/Noxcrew/mccisland-api/releases/tag/v24.04.17)
+[![🏝️ Targeting Island API v24.05.02](https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.05.02-aqua)](https://github.com/Noxcrew/mccisland-api/releases/tag/v24.05.02)
 
 A helper library for the [MC Championship](https://mcchampionship.com) APIs
 ([Event](https://github.com/Noxcrew/mcchampionship-api), inspired by [derNiklaas's](https://github.com/derNiklaas)
 [node-mcc-api](https://github.com/derNiklaas/node-mcc-api) project, and
 [Island](https://github.com/Noxcrew/mccisland-api)).
 
 - Issues: [https://github.com/JamesMCo/python_mcc_api/issues](https://github.com/JamesMCo/python_mcc_api/issues)
```

### Comparing `mcc_api-1.1.0/pyproject.toml` & `mcc_api-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.0/PKG-INFO` & `mcc_api-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mcc-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Wrapper for the MC Championship API
 Project-URL: Repository, https://github.com/JamesMCo/python_mcc_api
 Project-URL: Issues, https://github.com/JamesMCo/python_mcc_api/issues
 Project-URL: Documentation, https://mrjamesco.uk/python_mcc_api
 Author-email: "James C." <james@cordon.click>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # Python MCC API
 
 [![🐍 PyPI](https://img.shields.io/pypi/v/mcc-api?label=🐍%20PyPI)](https://pypi.org/project/mcc-api/)
 [![👑 Targeting Event API v1.3.2](https://img.shields.io/badge/👑_Targeting_Event_API-v1.3.2-red)](https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.2)
-[![🏝️ Targeting Island API v24.04.17](https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.04.17-aqua)](https://github.com/Noxcrew/mccisland-api/releases/tag/v24.04.17)
+[![🏝️ Targeting Island API v24.05.02](https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.05.02-aqua)](https://github.com/Noxcrew/mccisland-api/releases/tag/v24.05.02)
 
 A helper library for the [MC Championship](https://mcchampionship.com) APIs
 ([Event](https://github.com/Noxcrew/mcchampionship-api), inspired by [derNiklaas's](https://github.com/derNiklaas)
 [node-mcc-api](https://github.com/derNiklaas/node-mcc-api) project, and
 [Island](https://github.com/Noxcrew/mccisland-api)).
 
 - Issues: [https://github.com/JamesMCo/python_mcc_api/issues](https://github.com/JamesMCo/python_mcc_api/issues)
```

