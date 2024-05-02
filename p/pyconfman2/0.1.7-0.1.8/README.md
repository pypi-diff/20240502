# Comparing `tmp/pyconfman2-0.1.7.tar.gz` & `tmp/pyconfman2-0.1.8.tar.gz`

## Comparing `pyconfman2-0.1.7.tar` & `pyconfman2-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/Devs.md
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/setup.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/.github/workflows/build-and-publish-to-pypi.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/src/pyconfman2/Exceptions.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/src/pyconfman2/Schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/src/pyconfman2/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/tests/config.yaml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/tests/config.yml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/tests/test_default_config.yml
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/tests/test_schema.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/tests/test_schema_config.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/LICENSE
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 pyconfman2-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/Devs.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/setup.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/.github/workflows/build-and-publish-to-pypi.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/src/pyconfman2/Exceptions.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/src/pyconfman2/Schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/src/pyconfman2/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/tests/config.yaml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/tests/config.yml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/tests/test_default_config.yml
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/tests/test_schema.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/tests/test_schema_config.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/README.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 pyconfman2-0.1.8/PKG-INFO
```

### Comparing `pyconfman2-0.1.7/.github/workflows/build-and-publish-to-pypi.yml` & `pyconfman2-0.1.8/.github/workflows/build-and-publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.7/src/pyconfman2/Schema.py` & `pyconfman2-0.1.8/src/pyconfman2/Schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,13 +54,13 @@
 
     
     def load(self, filepath):
         if not os.path.exists(filepath):
             raise FileNotFoundException
         
         with open(filepath, "r") as fh:
-            config_file = yaml.safe_load(fh)
-        
-        self.add(config_file)
+            config = yaml.safe_load(fh)
+
+        self.properties = config
     
     def items(self):
         return self.properties.items()
```

### Comparing `pyconfman2-0.1.7/tests/test_schema.py` & `pyconfman2-0.1.8/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.7/LICENSE` & `pyconfman2-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.7/README.md` & `pyconfman2-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pyconfman2-0.1.7/pyproject.toml` & `pyconfman2-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyconfman2"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Phillyp Henning", email="phillyp.henning@gmail.com" },
 ]
 description = "A python package for managing YAML configuration"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyconfman2-0.1.7/PKG-INFO` & `pyconfman2-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyconfman2
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python package for managing YAML configuration
 Project-URL: Homepage, https://github.com/PhillypHenning/python-config-parser
 Project-URL: Issues, https://github.com/PhillypHenning/python-config-parser/issues
 Author-email: Phillyp Henning <phillyp.henning@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

