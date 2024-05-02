# Comparing `tmp/mal_toolbox-0.0.8-py3-none-any.whl.zip` & `tmp/mal_toolbox-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 21567 bytes, number of entries: 18
--rw-rw-r--  2.0 unx     2886 b- defN 23-Sep-07 17:24 maltoolbox/__init__.py
+Zip file size: 21361 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx     2886 b- defN 23-Sep-13 10:36 maltoolbox/__init__.py
 -rw-rw-r--  2.0 unx       94 b- defN 23-Sep-07 15:05 maltoolbox/__main__.py
 -rw-rw-r--  2.0 unx     2550 b- defN 23-Sep-07 15:05 maltoolbox/cl_parser.py
 -rw-r--r--  2.0 unx      280 b- defN 23-Sep-07 15:29 maltoolbox/default.conf
 -rw-rw-r--  2.0 unx     3350 b- defN 23-Sep-07 15:05 maltoolbox/main.py
 -rw-rw-r--  2.0 unx      694 b- defN 23-Sep-07 15:05 maltoolbox/attackgraph/attacker.py
--rw-rw-r--  2.0 unx    16537 b- defN 23-Sep-07 15:29 maltoolbox/attackgraph/attackgraph.py
+-rw-rw-r--  2.0 unx    15136 b- defN 23-Sep-13 10:31 maltoolbox/attackgraph/attackgraph.py
 -rw-rw-r--  2.0 unx     1551 b- defN 23-Sep-07 15:05 maltoolbox/attackgraph/node.py
 -rw-rw-r--  2.0 unx     3582 b- defN 23-Sep-07 15:05 maltoolbox/ingestors/neo4j.py
 -rw-rw-r--  2.0 unx     7018 b- defN 23-Sep-07 15:05 maltoolbox/language/classes_factory.py
--rw-rw-r--  2.0 unx     4553 b- defN 23-Sep-07 15:05 maltoolbox/language/specification.py
--rw-rw-r--  2.0 unx     9051 b- defN 23-Sep-07 15:05 maltoolbox/model/model.py
--rw-r--r--  2.0 unx       66 b- defN 23-Sep-07 17:25 mal_toolbox-0.0.8.dist-info/AUTHORS
--rw-r--r--  2.0 unx    11357 b- defN 23-Sep-07 17:25 mal_toolbox-0.0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1288 b- defN 23-Sep-07 17:25 mal_toolbox-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Sep-07 17:25 mal_toolbox-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Sep-07 17:25 mal_toolbox-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1515 b- defN 23-Sep-07 17:25 mal_toolbox-0.0.8.dist-info/RECORD
-18 files, 66475 bytes uncompressed, 19075 bytes compressed:  71.3%
+-rw-rw-r--  2.0 unx     4727 b- defN 23-Sep-13 10:35 maltoolbox/language/specification.py
+-rw-rw-r--  2.0 unx     9071 b- defN 23-Sep-13 10:33 maltoolbox/model/model.py
+-rw-r--r--  2.0 unx       66 b- defN 23-Sep-13 10:36 mal_toolbox-0.0.9.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    11357 b- defN 23-Sep-13 10:36 mal_toolbox-0.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Sep-13 10:36 mal_toolbox-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Sep-13 10:36 mal_toolbox-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Sep-13 10:36 mal_toolbox-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1515 b- defN 23-Sep-13 10:36 mal_toolbox-0.0.9.dist-info/RECORD
+18 files, 65268 bytes uncompressed, 18869 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: maltoolbox/language/specification.py
 Comment: 
 
 Filename: maltoolbox/model/model.py
 Comment: 
 
-Filename: mal_toolbox-0.0.8.dist-info/AUTHORS
+Filename: mal_toolbox-0.0.9.dist-info/AUTHORS
 Comment: 
 
-Filename: mal_toolbox-0.0.8.dist-info/LICENSE
+Filename: mal_toolbox-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: mal_toolbox-0.0.8.dist-info/METADATA
+Filename: mal_toolbox-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: mal_toolbox-0.0.8.dist-info/WHEEL
+Filename: mal_toolbox-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: mal_toolbox-0.0.8.dist-info/top_level.txt
+Filename: mal_toolbox-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: mal_toolbox-0.0.8.dist-info/RECORD
+Filename: mal_toolbox-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## maltoolbox/__init__.py

```diff
@@ -17,15 +17,15 @@
 
 
 """
 MAL-Toolbox Framework
 """
 
 __title__ = 'maltoolbox'
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 __authors__ = ['Andrei Buhaiu']
 __license__ = 'Apache 2.0'
 __docformat__ = 'restructuredtext en'
 
 __all__ = ()
 
 import os
```

## maltoolbox/attackgraph/attackgraph.py

```diff
@@ -109,46 +109,17 @@
         """
         Return the attack node that matches the id provided.
 
         Arguments:
         node_id     - the id of the attack graph none we are looking for
         """
         logger.debug(f'Looking up node with id {node_id}')
-        return next(ag_node for ag_node in self.nodes \
-            if ag_node.id == node_id)
+        return next((ag_node for ag_node in self.nodes \
+            if ag_node.id == node_id), None)
 
-    def where(self,
-        node_id = None,
-        node_type = None,
-        cls = None,
-        objid = None,
-        is_reachable = None,
-        is_traversable = None,
-        name = None):
-        def _(ag_node):
-            query = []
-            query.append(node_id == ag_node.id)                    if node_id        is not None else query.append(True)
-            query.append(node_type == ag_node.type)                if node_type      is not None else query.append(True)
-            query.append(cls == ag_node.objclass)                  if cls            is not None else query.append(True)
-            query.append(objid == ag_node.objid)                   if objid          is not None else query.append(True)
-            query.append(name == ag_node.name)                     if name           is not None else query.append(True)
-            query.append(is_reachable == ag_node.is_reachable)     if is_reachable   is not None else query.append(True)
-            query.append(is_traversable == ag_node.is_traversable) if is_traversable is not None else query.append(True)
-            return all(query)
-        return _
-
-
-    def select(self, where_stmt_func):
-        """
-        Return the attack node that matches the id provided.
-
-        Arguments:
-        node_id     - the id of the attack graph none we are looking for
-        """
-        return [ag_node for ag_node in self.nodes if where_stmt_func(ag_node)]
 
     def attach_attackers(self, model: model.Model):
         """
         Create attackers and their entry point nodes and attach them to the
         relevant attack step nodes and to the attackers.
 
         Arguments:
@@ -224,29 +195,29 @@
                     lang, model, target_assets, step_expression['rhs'])
 
                 new_target_assets = []
                 match (step_expression['type']):
                     case 'union':
                         new_target_assets = lh_targets
                         for ag_node in rh_targets:
-                            if next(lnode for lnode in new_target_assets \
-                                if lnode.id != ag_node.id):
+                            if next((lnode for lnode in new_target_assets \
+                                if lnode.id != ag_node.id), None):
                                 new_target_assets.append(ag_node)
 
                     case 'intersection':
                         for ag_node in rh_targets:
-                            if next(lnode for lnode in new_target_assets \
-                                if lnode.id == ag_node.id):
+                            if next((lnode for lnode in new_target_assets \
+                                if lnode.id == ag_node.id), None):
                                 new_target_assets.append(ag_node)
 
                     case 'difference':
                         new_target_assets = lh_targets
                         for ag_node in lh_targets:
-                            if next(rnode for rnode in rh_target_assets \
-                                if rnode.id != ag_node.id):
+                            if next((rnode for rnode in rh_target_assets \
+                                if rnode.id != ag_node.id), None):
                                 new_target_assets.remove(ag_node)
 
                 return (new_target_assets, None)
 
             case 'variable':
                 # Fetch the step expression associated with the variable from
                 # the language specification and resolve that.
```

## maltoolbox/language/specification.py

```diff
@@ -81,16 +81,21 @@
     Return:
     A dictionary representing the set of possible attacks for the specified
     class. Each key in the dictionary is an attack name and is associated
     with a dictionary containing other characteristics of the attack such as
     type of attack, TTC distribution, child attack steps and other information
     """
     attacks = {}
-    asset = next(asset for asset in lang_spec['assets'] if asset['name'] == \
-        asset_type)
+    asset = next((asset for asset in lang_spec['assets'] if asset['name'] == \
+        asset_type), None)
+    if not asset:
+        logger.error(f'Failed to find asset type {asset_type} when '\
+            'looking for attack steps.')
+        return None
+
     if asset['superAsset']:
         attacks = get_attacks_for_class(lang_spec,
             asset['superAsset'])
 
     for attack in asset['attackSteps']:
         if attack['name'] not in attacks:
             attacks[attack['name']] = attack
@@ -116,23 +121,23 @@
                     the variable
     variable_name   - the name of the variable to search for
 
     Return:
     A dictionary representing the step expressions for the specified variable.
     """
 
-    asset = next(asset for asset in lang_spec['assets'] if asset['name'] == \
-        asset_type)
+    asset = next((asset for asset in lang_spec['assets'] if asset['name'] == \
+        asset_type), None)
     if not asset:
         logger.error(f'Failed to find asset type {asset_type} when '\
             'looking for variable.')
         return None
 
-    variable_dict = next(variable for variable in \
-        asset['variables'] if variable['name'] == variable_name)
+    variable_dict = next((variable for variable in \
+        asset['variables'] if variable['name'] == variable_name), None)
     if not variable_dict:
         logger.error(f'Failed to find variable {variable_name} in '\
             f'{asset_type}\'s language specification.')
         return None
 
     return variable_dict['stepExpression']
```

## maltoolbox/model/model.py

```diff
@@ -66,15 +66,16 @@
 
         Arguments:
         asset_id        - the id of the asset we are looking for
 
         Return:
         An asset matching the id if it exists in the model.
         """
-        return next(asset for asset in self.assets if asset.id == asset_id)
+        return next((asset for asset in self.assets if asset.id == asset_id),
+            None)
 
     def get_associated_assets_by_field_name(self, asset, field_name):
         """
         Get a list of associated assets for an asset given a fieldname.
 
         Arguments:
         asset           - the asset whose fields we are interested in
```

## Comparing `mal_toolbox-0.0.8.dist-info/LICENSE` & `mal_toolbox-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mal_toolbox-0.0.8.dist-info/METADATA` & `mal_toolbox-0.0.9.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mal-toolbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of tools used to create MAL models and attack graphs.
 Author-email: Andrei Buhaiu <buhaiu@kth.se>, Giuseppe Nebbione <nebbione@kth.se>
 License: Apache Software License
 Project-URL: Homepage, https://github.com/mal-lang/mal-toolbox
 Project-URL: Bug Tracker, https://github.com/mal-lang/mal-toolbox/issues
 Project-URL: Repository, https://github.com/mal-lang/mal-toolbox
 Keywords: mal
```

## Comparing `mal_toolbox-0.0.8.dist-info/RECORD` & `mal_toolbox-0.0.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-maltoolbox/__init__.py,sha256=5GqgCNjfwaEaYCFj-8rGxTD9He4B-_6XY1xiEqhaGd8,2886
+maltoolbox/__init__.py,sha256=Yru0Z0EqQFQnpZoSVjOFpnVce7g-QQGt6fzY51QIofI,2886
 maltoolbox/__main__.py,sha256=_kfJOkJluA3gfq3HAJM0rAK_SvGO-4Jr6wQQGrItiWs,94
 maltoolbox/cl_parser.py,sha256=zpFAhEx-ZVOQlZkXR3MfxMiYR8aPLKDeUbGhlaap2Sk,2550
 maltoolbox/default.conf,sha256=5FDwla2eQqGCqrQfB9QadGaPUc8Y8aBJ1sskodPfzaM,280
 maltoolbox/main.py,sha256=nKybJbkXP37xaEIBPwwsq0-lB8Wt3kIYddh9TT_iqJ0,3350
 maltoolbox/attackgraph/attacker.py,sha256=xRuLdXesvZmLXn6oJPCXQmE9_Iz-5VefjK89x8uyWdA,694
-maltoolbox/attackgraph/attackgraph.py,sha256=h5-1dbwzBBpfanJiAM5NM_z9v5AglLkXrwfjPasvJTU,16537
+maltoolbox/attackgraph/attackgraph.py,sha256=I2lQTVUmlmFeXuXsRVCEptXfTh8ryEaIUM_W2OWoUIo,15136
 maltoolbox/attackgraph/node.py,sha256=cW9_BEQcXcnpm1xZ3-z_l3RCo38XfZILqyOBNzZx0P8,1551
 maltoolbox/ingestors/neo4j.py,sha256=LoSdm7MIV-MZRxLdpTmos4rHvkw67vX1mAUqtW2NsnI,3582
 maltoolbox/language/classes_factory.py,sha256=US3dTlyLWncqb3SJxpzesa0eRf2RTPxUX64gb_vESsE,7018
-maltoolbox/language/specification.py,sha256=tZEjga5rsxH-zqXl9y-es8ZsI7mw6x7ut-AEvsBhxvE,4553
-maltoolbox/model/model.py,sha256=NwxTLFUFVH7FQuYdoTtzhXyCir0NK2VjbRTRx1SEArU,9051
-mal_toolbox-0.0.8.dist-info/AUTHORS,sha256=XxTP0b8fRdf1sR1DOSPlsdo5WmgENsYnE79bjKmsgi0,66
-mal_toolbox-0.0.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mal_toolbox-0.0.8.dist-info/METADATA,sha256=rWABw9OAwXUAzpSZY_kZjvrIbcgDpgbWuCZgNyP14Hc,1288
-mal_toolbox-0.0.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-mal_toolbox-0.0.8.dist-info/top_level.txt,sha256=phqRVLRKGdSUgRY03mcpi2cmbbDo5YGjkV4gkqHFFcM,11
-mal_toolbox-0.0.8.dist-info/RECORD,,
+maltoolbox/language/specification.py,sha256=XOfLyFOdwvWiM2W-JqOmn7YjsztPPEbVFNG1caV5cgw,4727
+maltoolbox/model/model.py,sha256=ukL5z0i8aHBKEKFn1vm_YbTl_VjzIim_UuINj4BK2vA,9071
+mal_toolbox-0.0.9.dist-info/AUTHORS,sha256=XxTP0b8fRdf1sR1DOSPlsdo5WmgENsYnE79bjKmsgi0,66
+mal_toolbox-0.0.9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mal_toolbox-0.0.9.dist-info/METADATA,sha256=SvlIniLijg8Na0BiYDbmV21HDXRX9daWjLmv-sgD3YQ,1288
+mal_toolbox-0.0.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+mal_toolbox-0.0.9.dist-info/top_level.txt,sha256=phqRVLRKGdSUgRY03mcpi2cmbbDo5YGjkV4gkqHFFcM,11
+mal_toolbox-0.0.9.dist-info/RECORD,,
```

