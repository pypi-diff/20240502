# Comparing `tmp/sommify-0.8.5.tar.gz` & `tmp/sommify-0.8.6.tar.gz`

## Comparing `sommify-0.8.5.tar` & `sommify-0.8.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sommify-0.8.5/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/__init__.py
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/regex.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/test.py
--rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/utils.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/countries/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/__init__.py
--rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/categories.py
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/constants.py
--rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/cuisine.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/embeddings.py
--rw-r--r--   0        0        0   356666 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_funnel.py
--rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredients.py
--rw-r--r--   0        0        0  5768681 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/mean_ing_embedding_per_tag.csv
--rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/meat.py
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/modifiers.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/vegetables.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/vulgar_fractions.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/cheeses.py
--rw-r--r--   0        0        0     8421 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/drinks.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/fruit.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/herbs.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/legumes.py
--rw-r--r--   0        0        0     7426 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/meats.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/nuts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/pasta.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/spices.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/data/ingredient_categories/vegetables.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/prompts/__init__.py
--rw-r--r--   0        0        0    47884 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/prompts/data/__init__.py
--rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/prompts/data/default.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/pygrape/__init__.py
--rw-r--r--   0        0        0   367143 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/pygrape/data.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/pynotesandhints/__init__.py
--rw-r--r--   0        0        0    63339 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/pynotesandhints/data.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/pyregion/__init__.py
--rw-r--r--   0        0        0    53240 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/pyregion/data.py
--rw-r--r--   0        0        0    67688 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/recipes/__init__.py
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/recipes/elastic.py
--rw-r--r--   0        0        0    15890 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/recipes/reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/tests/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/tests/test_elastic.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/tests/test_prompts.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/tests/test_pygrape.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/tests/test_pyregion.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/tests/test_recipe_reader.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 sommify-0.8.5/sommify/tests/test_tag_reader.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 sommify-0.8.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sommify-0.8.5/LICENSE
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sommify-0.8.5/README.md
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 sommify-0.8.5/pyproject.toml
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 sommify-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sommify-0.8.6/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/__init__.py
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/regex.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/test.py
+-rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/utils.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/countries/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/__init__.py
+-rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/categories.py
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/constants.py
+-rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/cuisine.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/embeddings.py
+-rw-r--r--   0        0        0   356666 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/ingredient_funnel.py
+-rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/ingredients.py
+-rw-r--r--   0        0        0  5768681 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/mean_ing_embedding_per_tag.csv
+-rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/meat.py
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/modifiers.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/vegetables.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/vulgar_fractions.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/ingredient_categories/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/ingredient_categories/cheeses.py
+-rw-r--r--   0        0        0     8421 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/ingredient_categories/drinks.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/ingredient_categories/fruit.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/ingredient_categories/herbs.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/ingredient_categories/legumes.py
+-rw-r--r--   0        0        0     7426 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/ingredient_categories/meats.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/ingredient_categories/nuts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/ingredient_categories/pasta.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/ingredient_categories/spices.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/data/ingredient_categories/vegetables.py
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/prompts/__init__.py
+-rw-r--r--   0        0        0    47884 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/prompts/data/__init__.py
+-rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/prompts/data/default.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/pygrape/__init__.py
+-rw-r--r--   0        0        0   367143 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/pygrape/data.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/pynotesandhints/__init__.py
+-rw-r--r--   0        0        0    63339 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/pynotesandhints/data.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/pyregion/__init__.py
+-rw-r--r--   0        0        0    53240 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/pyregion/data.py
+-rw-r--r--   0        0        0    67688 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/recipes/__init__.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/recipes/elastic.py
+-rw-r--r--   0        0        0    15890 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/recipes/reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/tests/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/tests/test_elastic.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/tests/test_prompts.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/tests/test_pygrape.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/tests/test_pyregion.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/tests/test_recipe_reader.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 sommify-0.8.6/sommify/tests/test_tag_reader.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 sommify-0.8.6/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sommify-0.8.6/LICENSE
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sommify-0.8.6/README.md
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 sommify-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 sommify-0.8.6/PKG-INFO
```

### Comparing `sommify-0.8.5/sommify/regex.py` & `sommify-0.8.6/sommify/regex.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/test.py` & `sommify-0.8.6/sommify/test.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/utils.py` & `sommify-0.8.6/sommify/utils.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/countries/__init__.py` & `sommify-0.8.6/sommify/countries/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/categories.py` & `sommify-0.8.6/sommify/data/categories.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/constants.py` & `sommify-0.8.6/sommify/data/constants.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/cuisine.py` & `sommify-0.8.6/sommify/data/cuisine.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/embeddings.py` & `sommify-0.8.6/sommify/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/ingredient_funnel.py` & `sommify-0.8.6/sommify/data/ingredient_funnel.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/ingredients.py` & `sommify-0.8.6/sommify/data/ingredients.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/mean_ing_embedding_per_tag.csv` & `sommify-0.8.6/sommify/data/mean_ing_embedding_per_tag.csv`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/meat.py` & `sommify-0.8.6/sommify/data/meat.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/modifiers.py` & `sommify-0.8.6/sommify/data/modifiers.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/vegetables.py` & `sommify-0.8.6/sommify/data/vegetables.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/ingredient_categories/__init__.py` & `sommify-0.8.6/sommify/data/ingredient_categories/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/ingredient_categories/drinks.py` & `sommify-0.8.6/sommify/data/ingredient_categories/drinks.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/ingredient_categories/fruit.py` & `sommify-0.8.6/sommify/data/ingredient_categories/fruit.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/ingredient_categories/herbs.py` & `sommify-0.8.6/sommify/data/ingredient_categories/herbs.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/ingredient_categories/meats.py` & `sommify-0.8.6/sommify/data/ingredient_categories/meats.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/ingredient_categories/nuts.py` & `sommify-0.8.6/sommify/data/ingredient_categories/nuts.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/ingredient_categories/spices.py` & `sommify-0.8.6/sommify/data/ingredient_categories/spices.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/data/ingredient_categories/vegetables.py` & `sommify-0.8.6/sommify/data/ingredient_categories/vegetables.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/prompts/__init__.py` & `sommify-0.8.6/sommify/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/prompts/data/__init__.py` & `sommify-0.8.6/sommify/prompts/data/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/prompts/data/default.py` & `sommify-0.8.6/sommify/prompts/data/default.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/pygrape/__init__.py` & `sommify-0.8.6/sommify/pygrape/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/pygrape/data.py` & `sommify-0.8.6/sommify/pygrape/data.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/pynotesandhints/__init__.py` & `sommify-0.8.6/sommify/pynotesandhints/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/pynotesandhints/data.py` & `sommify-0.8.6/sommify/pynotesandhints/data.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/pyregion/__init__.py` & `sommify-0.8.6/sommify/pyregion/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/pyregion/data.py` & `sommify-0.8.6/sommify/pyregion/data.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/recipes/__init__.py` & `sommify-0.8.6/sommify/recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/recipes/elastic.py` & `sommify-0.8.6/sommify/recipes/elastic.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/recipes/reader.py` & `sommify-0.8.6/sommify/recipes/reader.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/tests/test_elastic.py` & `sommify-0.8.6/sommify/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/tests/test_prompts.py` & `sommify-0.8.6/sommify/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/sommify/tests/test_recipe_reader.py` & `sommify-0.8.6/sommify/tests/test_recipe_reader.py`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/.gitignore` & `sommify-0.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/LICENSE` & `sommify-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sommify-0.8.5/pyproject.toml` & `sommify-0.8.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "sommify"
-version = "0.8.5"
+version = "0.8.6"
 authors = [
   { name="William Brach", email="william@sommify.ai" },
   { name="Tomas Bedej", email="tomas@sommify.ai" },
 ]
 description = "A package for recipe parsing"
 dependencies = [
   "inflect==7.0.0",
```

### Comparing `sommify-0.8.5/PKG-INFO` & `sommify-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sommify
-Version: 0.8.5
+Version: 0.8.6
 Summary: A package for recipe parsing
 Author-email: William Brach <william@sommify.ai>, Tomas Bedej <tomas@sommify.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

