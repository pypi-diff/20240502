# Comparing `tmp/pyconfman2-0.1.8.tar.gz` & `tmp/pyconfman2-0.1.9.tar.gz`

## Comparing `pyconfman2-0.1.8.tar` & `pyconfman2-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/Devs.md
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/setup.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/.github/workflows/build-and-publish-to-pypi.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/src/pyconfman2/Exceptions.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/src/pyconfman2/Schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/src/pyconfman2/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/tests/config.yaml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/tests/config.yml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/tests/test_default_config.yml
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/tests/test_schema.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/tests/test_schema_config.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/LICENSE
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/Devs.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/setup.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/.github/workflows/build-and-publish-to-pypi.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/src/pyconfman2/Exceptions.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/src/pyconfman2/Schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/src/pyconfman2/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/tests/config.yaml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/tests/config.yml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/tests/test_default_config.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/tests/test_list_schema.yml
+-rw-r--r--   0        0        0     7580 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/tests/test_schema.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/tests/test_schema_config.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/README.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 pyconfman2-0.1.9/PKG-INFO
```

### Comparing `pyconfman2-0.1.8/.github/workflows/build-and-publish-to-pypi.yml` & `pyconfman2-0.1.9/.github/workflows/build-and-publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.8/src/pyconfman2/Schema.py` & `pyconfman2-0.1.9/src/pyconfman2/Schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 import os
 import yaml
 
-from .Exceptions import InvalidPropertyError, EmptyValueProperty, KeyExistsError
+from Exceptions import InvalidPropertyError, EmptyValueProperty, KeyExistsError
 
 class ConfigSchema():
     properties = None
+    current_idx = -1
 
     def __init__(self, default_schema={}, filepath=None, default_config=None) -> None:
         if type(default_schema) != dict:
             raise InvalidPropertyError
         
         self.properties = default_schema
+        
+        # Default Config is either: Provided or is searched for via "Config.y(a)ml" files
         if default_config:
             if os.path.isfile(default_config):
                 self.load(default_config)
-
-        # config.yaml is sorted to the top if it exists otherwise it attempts to load config.yml.
-        if not filepath:
+        elif not filepath:
             config_file = [item for item in os.listdir() if item == "config.yaml" or item == "config.yml"]
             for item in config_file:
                 if os.path.getsize(item) > 0:
                     self.load(item)
                     break
         else:
             if os.path.isfile(filepath):
                 self.load(filepath)
     
     def __str__(self) -> str:
         return str(self.properties)
+
+    def __iter__(self):
+        self.current_idx = -1
+        return self
+    
+    def __next__(self):
+        self.current_idx += 1
+        if self.current_idx < len(self.properties):
+            return self.properties[self.current_idx]
+        raise StopIteration
     
     def add(self, nkey, nvalue=None, override=True) -> None:
         if type(nkey) == dict:
             if override:
                 self.properties.update(nkey)
             else:
                 self.properties = dict(list(nkey.items()) + list(self.properties.items())) 
@@ -56,11 +67,12 @@
     def load(self, filepath):
         if not os.path.exists(filepath):
             raise FileNotFoundException
         
         with open(filepath, "r") as fh:
             config = yaml.safe_load(fh)
 
-        self.properties = config
+        if not self.properties or not len(self.properties) > 1:
+            self.properties = config
     
     def items(self):
         return self.properties.items()
```

### Comparing `pyconfman2-0.1.8/tests/test_schema.py` & `pyconfman2-0.1.9/tests/test_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,19 +15,19 @@
     
     def test_init_with_config_override(self):
         test_init_schema = ConfigSchema(filepath="config.yml")
         self.assertEqual(str(test_init_schema), "{'file_loaded': 'yml'}")
     
     def test_init_with_default_config_override(self):
         test_init_schema = ConfigSchema(default_config="test_default_config.yml")
-        self.assertEqual(str(test_init_schema), "{'file_loaded': 'yaml', 'testing': 'default'}")
+        self.assertEqual(str(test_init_schema), "{'testing': 'default'}")
     
     def test_init_with_default_schema(self):
         default_schema = { "fookey": "foo", "barkey": "bar" }
-        validated_schema = { "fookey": "foo", "barkey": "bar", 'file_loaded': 'yaml'}
+        validated_schema = { "fookey": "foo", "barkey": "bar"}
         test_default_schema = ConfigSchema(default_schema)
         self.assertEqual(str(test_default_schema), str(validated_schema))
     
     def test_init_raises_invalid_property_error(self):
         default_schema = "{ 'test' }"
         def test_func():
             ConfigSchema(default_schema)
@@ -68,45 +68,45 @@
         default_schema = { "fookey": "foo", "barkey": "bar" }
         test_schema = ConfigSchema(default_schema)
         self.assertEqual(str(test_schema), str(default_schema))
 
     # Add
     def test_add_new_key_and_value(self):
         default_schema = { "fookey": "foo", "barkey": "bar" }
-        validated_schema = { "fookey": "foo", "barkey": "bar", 'file_loaded': 'yaml', "newkey": "value"}
+        validated_schema = { "fookey": "foo", "barkey": "bar", "newkey": "value"}
         
         test_schema = ConfigSchema(default_schema)
         test_schema.add("newkey", "value")
     
         self.assertEqual(str(test_schema), str(validated_schema))
     
     def test_add_new_dict(self):
         default_schema = { "fookey": "foo", "barkey": "bar" }
         new_value = { "newkey": "value" }
-        validated_schema = { "fookey": "foo", "barkey": "bar",'file_loaded': 'yaml', "newkey": "value" }
+        validated_schema = { "fookey": "foo", "barkey": "bar", "newkey": "value" }
 
         test_schema = ConfigSchema(default_schema)
         test_schema.add(new_value)
     
         self.assertEqual(str(test_schema), str(validated_schema))
     
     def test_add_new_dict_with_override(self):
         default_schema = { "fookey": "foo", "barkey": "bar", "newkey": "value" }
         new_value = { "newkey": "new_value", "newkey_2": "new_value" }
-        validated_schema = { "fookey": "foo", "barkey": "bar", "newkey": "new_value", 'file_loaded': 'yaml', "newkey_2": "new_value" }
+        validated_schema = { "fookey": "foo", "barkey": "bar", "newkey": "new_value", "newkey_2": "new_value" }
 
         test_schema = ConfigSchema(default_schema)
         test_schema.add(new_value)
     
         self.assertEqual(str(test_schema), str(validated_schema))
     
     def test_add_new_dict_without_override(self):
         default_schema = { "fookey": "foo", "barkey": "bar", "newkey": "value" }
         new_value = { "newkey": "new_value", "newkey_2": "new_value" }
-        validated_schema = {"newkey": "value", "newkey_2": "new_value", "fookey": "foo", "barkey": "bar", 'file_loaded': 'yaml'}
+        validated_schema = {"newkey": "value", "newkey_2": "new_value", "fookey": "foo", "barkey": "bar"}
 
         test_schema = ConfigSchema(default_schema)
         test_schema.add(new_value, override=False)
     
         self.assertEqual(str(test_schema), str(validated_schema))
     
     def test_add_empty_value(self):
@@ -136,24 +136,24 @@
         def test_func():
             test_schema.get("not_a_key", strict=True)
         self.assertRaises(KeyError, test_func)
 
     # Remove
     def test_remove_valid_key(self):
         default_schema = { "fookey": "foo", "barkey": "bar" }
-        validated_schema = { "barkey": "bar", 'file_loaded': 'yaml' }
+        validated_schema = { "barkey": "bar"}
 
         test_schema = ConfigSchema(default_schema)
         test_schema.remove("fookey")
 
         self.assertEqual(str(test_schema), str(validated_schema))
 
     def test_remove_invalid_key_not_strict(self):
         default_schema = { "fookey": "foo", "barkey": "bar" }
-        validated_schema = { "fookey": "foo", "barkey": "bar", 'file_loaded': 'yaml' }
+        validated_schema = { "fookey": "foo", "barkey": "bar"}
 
         test_schema = ConfigSchema(default_schema)
         test_schema.remove("no_key")
         
         self.assertEqual(str(test_schema), str(validated_schema))
     
     def test_remove_invalid_key_strict(self):
@@ -165,15 +165,14 @@
             test_schema.remove("no_key", strict=True)
         
         self.assertRaises(KeyError, test_func)
     
     # Load
     def test_load_valid_file(self):
         validated_schema = {
-            'file_loaded': 'yaml',
             "specific": True,
             "learn": 194.3,
             "fish": {
                 "spell": {
                 "crop": False,
                 "happen": 6690.3106,
                 "taste": "three",
@@ -184,10 +183,17 @@
                 "powerful": "amount"
                 },
             "flat": -64.27,
             "hole": False,
             "lot": False
         }
 
-        test_schema = ConfigSchema(default_schema={})
+        test_schema = ConfigSchema()
         test_schema.load("test_schema_config.yml")
-        self.assertEqual(str(test_schema), str(validated_schema))
+        self.assertEqual(str(test_schema), str(validated_schema))
+
+    def test_class_is_iterable(self):
+        test_schema = ConfigSchema(filepath="test_list_schema.yml")
+        test_target_1 = [x for x in test_schema]
+        test_target_2 = [x for x in test_schema if x.get("value") == "a"]
+        self.assertEqual(test_target_1, [{'key': 1, 'value': 'a'}, {'key': 2, 'value': 'b'}, {'key': 3, 'value': 'c'}])
+        self.assertEqual(test_target_2, [{'key': 1, 'value': 'a'}])
```

### Comparing `pyconfman2-0.1.8/LICENSE` & `pyconfman2-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.8/README.md` & `pyconfman2-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.8/pyproject.toml` & `pyconfman2-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyconfman2"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Phillyp Henning", email="phillyp.henning@gmail.com" },
 ]
 description = "A python package for managing YAML configuration"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyconfman2-0.1.8/PKG-INFO` & `pyconfman2-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyconfman2
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python package for managing YAML configuration
 Project-URL: Homepage, https://github.com/PhillypHenning/python-config-parser
 Project-URL: Issues, https://github.com/PhillypHenning/python-config-parser/issues
 Author-email: Phillyp Henning <phillyp.henning@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

