# Comparing `tmp/fz_td_recipe-0.2.2.tar.gz` & `tmp/fz_td_recipe-0.2.3.tar.gz`

## Comparing `fz_td_recipe-0.2.2.tar` & `fz_td_recipe-0.2.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/CHANGELOG.rst
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/MANIFEST.in
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tox.ini
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/doc/Makefile
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/doc/source/api.rst
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/doc/source/changelog.rst
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/doc/source/conf.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/doc/source/index.rst
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/__init__.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/cli.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/legacy.py
--rw-r--r--   0        0        0    27865 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/property.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/recipe.py
--rw-r--r--   0        0        0    11520 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/transform.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/utils.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/validate.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/data/defaults.yaml
--rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/data/schema.yaml
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/parts/__init__.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/parts/bouton_density.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/parts/common.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/parts/gap_junction_properties.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/parts/seeds.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/parts/spine_lengths.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/parts/structure.py
--rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/parts/synapse_properties.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/parts/synapse_reposition.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/parts/touch_connections.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/parts/touch_reduction.py
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/fz_td_recipe/parts/touch_rules.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/test_bouton_distance.py
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/test_convert.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/test_gap_junction_properties.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/test_property.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/test_recipe.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/test_seeds.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/test_synapse_property.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/test_touch_connections.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/test_transform.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/test_xml_recipe.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/data/.gitignore
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/data/circuit_config.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/data/faulty.xml
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/data/gap_junctions.xml
--rw-r--r--   0        0        0    12600 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/data/nodes.h5
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/data/synapse_properties.xml
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/data/synapse_properties_uhill_all.xml
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/data/synapse_properties_uhill_some.xml
--rw-r--r--   0        0        0    60302 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/data/v5.xml
--rw-r--r--   0        0        0    62158 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/data/v5builderRecipeAllPathways_no_repositioning.xml
--rw-r--r--   0        0        0    36375 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/data/v7.xml
--rw-r--r--   0        0        0   417900 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/tests/data/v7connectivity.xml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/.gitignore
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/AUTHORS.txt
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/README.rst
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    15304 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/CHANGELOG.rst
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/MANIFEST.in
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tox.ini
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/doc/Makefile
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/doc/source/api.rst
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/doc/source/changelog.rst
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/doc/source/conf.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/doc/source/index.rst
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/__init__.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/cli.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/legacy.py
+-rw-r--r--   0        0        0    27865 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/property.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/recipe.py
+-rw-r--r--   0        0        0    11520 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/transform.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/utils.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/validate.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/data/defaults.yaml
+-rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/data/schema.yaml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/parts/__init__.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/parts/bouton_density.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/parts/common.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/parts/gap_junction_properties.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/parts/seeds.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/parts/spine_lengths.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/parts/structure.py
+-rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/parts/synapse_properties.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/parts/synapse_reposition.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/parts/touch_connections.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/parts/touch_reduction.py
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/fz_td_recipe/parts/touch_rules.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/test_bouton_distance.py
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/test_convert.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/test_gap_junction_properties.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/test_property.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/test_recipe.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/test_seeds.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/test_synapse_property.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/test_touch_connections.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/test_transform.py
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/test_xml_recipe.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/data/.gitignore
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/data/circuit_config.json
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/data/faulty.xml
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/data/gap_junctions.xml
+-rw-r--r--   0        0        0    12600 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/data/nodes.h5
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/data/synapse_properties.xml
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/data/synapse_properties_uhill_all.xml
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/data/synapse_properties_uhill_some.xml
+-rw-r--r--   0        0        0    60302 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/data/v5.xml
+-rw-r--r--   0        0        0    62158 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/data/v5builderRecipeAllPathways_no_repositioning.xml
+-rw-r--r--   0        0        0    36375 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/data/v7.xml
+-rw-r--r--   0        0        0   417900 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/tests/data/v7connectivity.xml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/.gitignore
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/AUTHORS.txt
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/README.rst
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    15305 2020-02-02 00:00:00.000000 fz_td_recipe-0.2.3/PKG-INFO
```

### Comparing `fz_td_recipe-0.2.2/tox.ini` & `fz_td_recipe-0.2.3/tox.ini`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/.github/workflows/publish.yml` & `fz_td_recipe-0.2.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/.github/workflows/test.yml` & `fz_td_recipe-0.2.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/doc/Makefile` & `fz_td_recipe-0.2.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/doc/source/api.rst` & `fz_td_recipe-0.2.3/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/doc/source/conf.py` & `fz_td_recipe-0.2.3/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/fz_td_recipe/__init__.py` & `fz_td_recipe-0.2.3/fz_td_recipe/__init__.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/fz_td_recipe/cli.py` & `fz_td_recipe-0.2.3/fz_td_recipe/cli.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/fz_td_recipe/legacy.py` & `fz_td_recipe-0.2.3/fz_td_recipe/legacy.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/fz_td_recipe/property.py` & `fz_td_recipe-0.2.3/fz_td_recipe/property.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/fz_td_recipe/recipe.py` & `fz_td_recipe-0.2.3/fz_td_recipe/recipe.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/fz_td_recipe/transform.py` & `fz_td_recipe-0.2.3/fz_td_recipe/transform.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/fz_td_recipe/utils.py` & `fz_td_recipe-0.2.3/fz_td_recipe/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 logger = logging.getLogger(__name__)
 
 
 def load_xml(recipe):
     """Extract the xml root from `recipe`, which may either be a path or string."""
     try:
         # Parse the given XML file:
-        parser = etree.XMLParser(remove_comments=True)
+        parser = etree.XMLParser(remove_comments=True, resolve_entities=True)
         tree = etree.parse(recipe, parser)
     except (etree.XMLSyntaxError, etree.ParserError) as err:
         logger.warning("could not parse xml of recipe '%s'", recipe)
         raise err
     except IOError as err:
         logger.warning("error while reading xml: %s", err)
         raise err
```

### Comparing `fz_td_recipe-0.2.2/fz_td_recipe/data/schema.yaml` & `fz_td_recipe-0.2.3/fz_td_recipe/data/schema.yaml`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/fz_td_recipe/parts/structure.py` & `fz_td_recipe-0.2.3/fz_td_recipe/parts/structure.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/fz_td_recipe/parts/synapse_properties.py` & `fz_td_recipe-0.2.3/fz_td_recipe/parts/synapse_properties.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/fz_td_recipe/parts/synapse_reposition.py` & `fz_td_recipe-0.2.3/fz_td_recipe/parts/synapse_reposition.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/fz_td_recipe/parts/touch_connections.py` & `fz_td_recipe-0.2.3/fz_td_recipe/parts/touch_connections.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/fz_td_recipe/parts/touch_rules.py` & `fz_td_recipe-0.2.3/fz_td_recipe/parts/touch_rules.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/test_bouton_distance.py` & `fz_td_recipe-0.2.3/tests/test_bouton_distance.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/test_convert.py` & `fz_td_recipe-0.2.3/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/test_gap_junction_properties.py` & `fz_td_recipe-0.2.3/tests/test_gap_junction_properties.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/test_property.py` & `fz_td_recipe-0.2.3/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/test_recipe.py` & `fz_td_recipe-0.2.3/tests/test_recipe.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/test_seeds.py` & `fz_td_recipe-0.2.3/tests/test_seeds.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/test_synapse_property.py` & `fz_td_recipe-0.2.3/tests/test_synapse_property.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/test_touch_connections.py` & `fz_td_recipe-0.2.3/tests/test_touch_connections.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/test_xml_recipe.py` & `fz_td_recipe-0.2.3/tests/test_xml_recipe.py`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/data/nodes.h5` & `fz_td_recipe-0.2.3/tests/data/nodes.h5`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/data/synapse_properties.xml` & `fz_td_recipe-0.2.3/tests/data/synapse_properties.xml`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/data/synapse_properties_uhill_all.xml` & `fz_td_recipe-0.2.3/tests/data/synapse_properties_uhill_all.xml`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/data/synapse_properties_uhill_some.xml` & `fz_td_recipe-0.2.3/tests/data/synapse_properties_uhill_some.xml`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/data/v5.xml` & `fz_td_recipe-0.2.3/tests/data/v5.xml`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/data/v5builderRecipeAllPathways_no_repositioning.xml` & `fz_td_recipe-0.2.3/tests/data/v5builderRecipeAllPathways_no_repositioning.xml`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/data/v7.xml` & `fz_td_recipe-0.2.3/tests/data/v7.xml`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/tests/data/v7connectivity.xml` & `fz_td_recipe-0.2.3/tests/data/v7connectivity.xml`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/LICENSE.txt` & `fz_td_recipe-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/README.rst` & `fz_td_recipe-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `fz_td_recipe-0.2.2/pyproject.toml` & `fz_td_recipe-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Topic :: Scientific/Engineering",
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
     "click",
     "jsonschema",
     "libsonata",
-    "lxml<5",
+    "lxml>=5",
     "numpy",
     "pandas[pyarrow]",
     "pyyaml",
 ]
 
 [project.scripts]
 fz-td-recipe = "fz_td_recipe.cli:app"
```

### Comparing `fz_td_recipe-0.2.2/PKG-INFO` & `fz_td_recipe-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fz-td-recipe
-Version: 0.2.2
+Version: 0.2.3
 Summary: Read and modify parameters used in neuroscientific in silico circuit building.
 Project-URL: Homepage, https://github.com/BlueBrain/fz-td-recipe
 Project-URL: Repository, https://github.com/BlueBrain/fz-td-recipe.git
 Project-URL: Tracker, https://github.com/BlueBrain/fz-td-recipe/issues
 Author-email: Matthias Wolf <matthias.wolf@epfl.ch>
 Maintainer-email: Matthias Wolf <matthias.wolf@epfl.ch>
 License:                                  Apache License
@@ -214,15 +214,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: click
 Requires-Dist: jsonschema
 Requires-Dist: libsonata
-Requires-Dist: lxml<5
+Requires-Dist: lxml>=5
 Requires-Dist: numpy
 Requires-Dist: pandas[pyarrow]
 Requires-Dist: pyyaml
 Description-Content-Type: text/x-rst
 
 fz-td-recipe
 ============
```

