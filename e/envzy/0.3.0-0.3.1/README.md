# Comparing `tmp/envzy-0.3.0.tar.gz` & `tmp/envzy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envzy-0.3.0.tar", max compression
+gzip compressed data, was "envzy-0.3.1.tar", max compression
```

## Comparing `envzy-0.3.0.tar` & `envzy-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      227 2024-01-26 11:07:00.875796 envzy-0.3.0/AUTHORS
--rw-r--r--   0        0        0     1868 2024-01-26 11:07:00.875796 envzy-0.3.0/CONTRIBUTING
--rw-r--r--   0        0        0      578 2024-01-26 11:07:00.879796 envzy-0.3.0/LICENSE
--rw-r--r--   0        0        0     1727 2024-01-26 11:07:00.879796 envzy-0.3.0/README.md
--rw-r--r--   0        0        0      432 2024-04-23 13:52:07.289451 envzy-0.3.0/envzy/__init__.py
--rw-r--r--   0        0        0     6820 2024-04-23 13:52:07.289451 envzy-0.3.0/envzy/auto.py
--rw-r--r--   0        0        0      592 2024-04-23 13:52:07.289451 envzy-0.3.0/envzy/base.py
--rw-r--r--   0        0        0    18048 2024-04-23 13:52:07.293451 envzy-0.3.0/envzy/classify.py
--rw-r--r--   0        0        0      118 2024-01-26 11:07:00.879796 envzy-0.3.0/envzy/exceptions.py
--rw-r--r--   0        0        0      666 2024-04-23 13:52:07.293451 envzy-0.3.0/envzy/packages.py
--rw-r--r--   0        0        0        0 2024-01-26 11:07:00.879796 envzy-0.3.0/envzy/py.typed
--rw-r--r--   0        0        0     4896 2024-04-18 15:39:31.723734 envzy-0.3.0/envzy/pypi.py
--rw-r--r--   0        0        0     6706 2024-01-26 11:07:00.883796 envzy-0.3.0/envzy/search.py
--rw-r--r--   0        0        0      472 2024-04-23 13:52:07.293451 envzy-0.3.0/envzy/spec.py
--rw-r--r--   0        0        0     8969 2024-04-15 08:19:12.388985 envzy-0.3.0/envzy/utils.py
--rw-r--r--   0        0        0      234 2024-01-26 11:07:00.883796 envzy-0.3.0/envzy/version.py
--rw-r--r--   0        0        0     1369 2024-04-23 13:53:29.061848 envzy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 envzy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      227 2024-01-26 11:07:00.875796 envzy-0.3.1/AUTHORS
+-rw-r--r--   0        0        0     1868 2024-01-26 11:07:00.875796 envzy-0.3.1/CONTRIBUTING
+-rw-r--r--   0        0        0      578 2024-01-26 11:07:00.879796 envzy-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1727 2024-01-26 11:07:00.879796 envzy-0.3.1/README.md
+-rw-r--r--   0        0        0      432 2024-05-02 11:29:10.775657 envzy-0.3.1/envzy/__init__.py
+-rw-r--r--   0        0        0     6820 2024-05-02 11:29:10.775657 envzy-0.3.1/envzy/auto.py
+-rw-r--r--   0        0        0      592 2024-05-02 11:29:10.775657 envzy-0.3.1/envzy/base.py
+-rw-r--r--   0        0        0    18048 2024-05-02 11:29:10.775657 envzy-0.3.1/envzy/classify.py
+-rw-r--r--   0        0        0      118 2024-01-26 11:07:00.879796 envzy-0.3.1/envzy/exceptions.py
+-rw-r--r--   0        0        0      666 2024-05-02 11:29:10.779657 envzy-0.3.1/envzy/packages.py
+-rw-r--r--   0        0        0        0 2024-01-26 11:07:00.879796 envzy-0.3.1/envzy/py.typed
+-rw-r--r--   0        0        0     4896 2024-04-18 15:39:31.723734 envzy-0.3.1/envzy/pypi.py
+-rw-r--r--   0        0        0     6706 2024-01-26 11:07:00.883796 envzy-0.3.1/envzy/search.py
+-rw-r--r--   0        0        0      472 2024-05-02 11:29:10.779657 envzy-0.3.1/envzy/spec.py
+-rw-r--r--   0        0        0     9039 2024-05-02 12:02:57.137197 envzy-0.3.1/envzy/utils.py
+-rw-r--r--   0        0        0      234 2024-01-26 11:07:00.883796 envzy-0.3.1/envzy/version.py
+-rw-r--r--   0        0        0     1369 2024-05-02 12:03:10.485252 envzy-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 envzy-0.3.1/PKG-INFO
```

### Comparing `envzy-0.3.0/CONTRIBUTING` & `envzy-0.3.1/CONTRIBUTING`

 * *Files identical despite different names*

### Comparing `envzy-0.3.0/LICENSE` & `envzy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `envzy-0.3.0/README.md` & `envzy-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `envzy-0.3.0/envzy/auto.py` & `envzy-0.3.1/envzy/auto.py`

 * *Files identical despite different names*

### Comparing `envzy-0.3.0/envzy/base.py` & `envzy-0.3.1/envzy/base.py`

 * *Files identical despite different names*

### Comparing `envzy-0.3.0/envzy/classify.py` & `envzy-0.3.1/envzy/classify.py`

 * *Files identical despite different names*

### Comparing `envzy-0.3.0/envzy/packages.py` & `envzy-0.3.1/envzy/packages.py`

 * *Files identical despite different names*

### Comparing `envzy-0.3.0/envzy/pypi.py` & `envzy-0.3.1/envzy/pypi.py`

 * *Files identical despite different names*

### Comparing `envzy-0.3.0/envzy/search.py` & `envzy-0.3.1/envzy/search.py`

 * *Files identical despite different names*

### Comparing `envzy-0.3.0/envzy/utils.py` & `envzy-0.3.1/envzy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,16 @@
                     result[name].append(distribution)
 
     return dict(result)
 
 
 def is_wellknown_fake_module(top_level_module_name: str, module_filename: str) -> bool:
     if top_level_module_name == 'torch':
-        if module_filename in ['torch.ops', '_ops.py', '_classes.py']:
+        module_file_basename = os.path.basename(module_filename)
+        if module_file_basename in ['torch.ops', '_ops.py', '_classes.py']:
             return True
     return False
 
 
 def is_lazy_module(module: types.ModuleType) -> bool:
     module_package = getattr(module.__class__, '__module__', None)
     module_name = type(module).__name__
```

### Comparing `envzy-0.3.0/pyproject.toml` & `envzy-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "envzy"
-version = "0.3.0"
+version = "0.3.1"
 description = "A library that explores dependencies from a given module or namespace in a local Python environment, then classifies these dependencies."
 license = "Apache-2.0"
 authors = ["Vladimir Lipkin <lipkin@yandex-team.ru>"]
 readme = "README.md"
 homepage = "https://github.com/lambdazy/envzy"
 repository = "https://github.com/lambdazy/envzy"
 include = ["AUTHORS", "CONTRIBUTING"]
```

### Comparing `envzy-0.3.0/PKG-INFO` & `envzy-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envzy
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library that explores dependencies from a given module or namespace in a local Python environment, then classifies these dependencies.
 Home-page: https://github.com/lambdazy/envzy
 License: Apache-2.0
 Author: Vladimir Lipkin
 Author-email: lipkin@yandex-team.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

