# Comparing `tmp/clisync-1.2.0.tar.gz` & `tmp/clisync-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clisync-1.2.0.tar", last modified: Thu Mar 14 17:46:42 2024, max compression
+gzip compressed data, was "clisync-1.3.0.tar", last modified: Thu May  2 20:06:30 2024, max compression
```

## Comparing `clisync-1.2.0.tar` & `clisync-1.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 17:46:42.545797 clisync-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 17:46:42.541797 clisync-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 17:46:42.541797 clisync-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-14 17:46:31.000000 clisync-1.2.0/.github/workflows/pypi_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-03-14 17:46:31.000000 clisync-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-14 17:46:31.000000 clisync-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-14 17:46:31.000000 clisync-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-14 17:46:42.545797 clisync-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-03-14 17:46:31.000000 clisync-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 17:46:42.541797 clisync-1.2.0/clisync/
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-03-14 17:46:31.000000 clisync-1.2.0/clisync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-03-14 17:46:31.000000 clisync-1.2.0/clisync/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-03-14 17:46:31.000000 clisync-1.2.0/clisync/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 17:46:42.545797 clisync-1.2.0/clisync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-14 17:46:42.000000 clisync-1.2.0/clisync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-14 17:46:42.000000 clisync-1.2.0/clisync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 17:46:42.000000 clisync-1.2.0/clisync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 17:46:37.000000 clisync-1.2.0/clisync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-14 17:46:42.000000 clisync-1.2.0/clisync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-14 17:46:42.000000 clisync-1.2.0/clisync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 17:46:42.545797 clisync-1.2.0/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-14 17:46:31.000000 clisync-1.2.0/demo/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 17:46:42.545797 clisync-1.2.0/demo/clisyncdemo/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-14 17:46:31.000000 clisync-1.2.0/demo/clisyncdemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 17:46:31.000000 clisync-1.2.0/demo/clisyncdemo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-14 17:46:31.000000 clisync-1.2.0/demo/clisyncdemo/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-14 17:46:31.000000 clisync-1.2.0/demo/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-14 17:46:31.000000 clisync-1.2.0/demo/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-14 17:46:31.000000 clisync-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-14 17:46:31.000000 clisync-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 17:46:42.545797 clisync-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-14 17:46:31.000000 clisync-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:30.877676 clisync-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:30.869675 clisync-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:30.873675 clisync-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-02 20:06:21.000000 clisync-1.3.0/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-02 20:06:21.000000 clisync-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-02 20:06:21.000000 clisync-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 20:06:21.000000 clisync-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-02 20:06:30.873675 clisync-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-02 20:06:21.000000 clisync-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:30.873675 clisync-1.3.0/clisync/
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-02 20:06:21.000000 clisync-1.3.0/clisync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-02 20:06:21.000000 clisync-1.3.0/clisync/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-02 20:06:21.000000 clisync-1.3.0/clisync/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:30.873675 clisync-1.3.0/clisync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-02 20:06:30.000000 clisync-1.3.0/clisync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-02 20:06:30.000000 clisync-1.3.0/clisync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:06:30.000000 clisync-1.3.0/clisync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:06:26.000000 clisync-1.3.0/clisync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 20:06:30.000000 clisync-1.3.0/clisync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 20:06:30.000000 clisync-1.3.0/clisync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:30.873675 clisync-1.3.0/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-02 20:06:21.000000 clisync-1.3.0/demo/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:30.873675 clisync-1.3.0/demo/clisyncdemo/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 20:06:21.000000 clisync-1.3.0/demo/clisyncdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:06:21.000000 clisync-1.3.0/demo/clisyncdemo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-02 20:06:21.000000 clisync-1.3.0/demo/clisyncdemo/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 20:06:21.000000 clisync-1.3.0/demo/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-02 20:06:21.000000 clisync-1.3.0/demo/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-02 20:06:21.000000 clisync-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 20:06:21.000000 clisync-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:06:30.877676 clisync-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-02 20:06:21.000000 clisync-1.3.0/setup.py
```

### Comparing `clisync-1.2.0/.github/workflows/pypi_release.yml` & `clisync-1.3.0/.github/workflows/pypi_release.yml`

 * *Files identical despite different names*

### Comparing `clisync-1.2.0/.gitignore` & `clisync-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `clisync-1.2.0/LICENSE` & `clisync-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clisync-1.2.0/PKG-INFO` & `clisync-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clisync
-Version: 1.2.0
+Version: 1.3.0
 Summary: Generate click commands from your project
 Home-page: https://clisync.surge.sh
 Author: Edward Laurence
 Author-email: edwardl@hectiq.ai
 Keywords: pip requirements imports
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `clisync-1.2.0/README.md` & `clisync-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `clisync-1.2.0/clisync/__init__.py` & `clisync-1.3.0/clisync/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 import click
-from typing import List, Union, Optional
+from typing import List, Union
 import importlib
 
 from clisync.utils import list_static_method, cli_callback, cli_doc
-from clisync.shell import setup_autocomplete
 
 from functools import wraps
 
 
-def include():
+def include(**override_kwargs):
     def _exposed_method(f):
         @wraps(f)
         def wrapper(*args, **kwargs):
+            kwargs.update(override_kwargs)
             return f(*args, **kwargs)
 
         wrapper._clisync = True
+        wrapper._overriden_kwargs = override_kwargs
         return wrapper
 
     return _exposed_method
 
 
 def exclude():
     def _exposed_method(f):
@@ -41,32 +42,33 @@
 
     ```python
     from clisync import CliSync
     group = CliSync(module="hectiq_lab", classes=["Run", "Project"])
     ```
     """
 
-    def __init__(self, module: Union[str, type], classes: List[str], requires_decorator: bool = True, **kwargs):
+    def __init__(
+        self, module: Union[str, type], classes: List[Union[str, type]], requires_decorator: bool = True, **kwargs
+    ):
         super().__init__(**kwargs)
         self.requires_decorator = requires_decorator
         self.module = importlib.import_module(module) if isinstance(module, str) else module
-        self.classes = classes
+        self.classes = [getattr(self.module, c) if isinstance(c, str) else c for c in classes]
 
     def list_commands(self, ctx):
         """Required method for click.MultiCommand."""
         rv = []
         for cls in self.classes:
-            cls = getattr(self.module, cls)
             rv += list_static_method(cls, requires_decorator=self.requires_decorator)
         return rv
 
     def get_command(self, ctx, name):
         """Required method for click.MultiCommand."""
         cls, name = name.split(".")
-        cls = getattr(self.module, cls)
+        cls = list(filter(lambda c: c.__name__ == cls, self.classes))[0]
         method = getattr(cls, name)
         helps, params = cli_doc(method)
         # In later versions of click, this is necessary as `params` cannot be used in `click.command`.
         callback = cli_callback(cls, method)
         callback.__click_params__ = params
         command = click.command(name=f"{cls.__name__}.{name}", help=helps)(callback)
         return command
```

### Comparing `clisync-1.2.0/clisync/shell.py` & `clisync-1.3.0/clisync/shell.py`

 * *Files identical despite different names*

### Comparing `clisync-1.2.0/clisync/utils.py` & `clisync-1.3.0/clisync/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from typing import List, get_type_hints, Union
+import importlib
 import click
-from typing import List
 import re
 
+
 def get_method_description(method: callable):
     """Get the first line of the method docstring as the description.
     If the method has no docstring, return an empty string.
 
     Args:
         method (callable): The method to get the description for.
     """
@@ -13,14 +15,15 @@
         return ""
     rows = method.__doc__.split("\n")
     for r in rows:
         if len(r) > 0:
             return r.strip()
     return ""
 
+
 def get_params_from_docstring(docstring: str) -> dict:
     """Get the parameters and their descriptions from the method docstring.
     It parses the docstring and extracts the parameters and their descriptions.
     Any line in the format `param: description` or `param (type): description` will be extracted.
 
     Args:
         method (callable): The method to get the parameters for.
@@ -30,22 +33,22 @@
     """
     params = {}
     if docstring is None:
         return params
     for a in docstring.split("\n"):
         if len(a.split(":")) <= 1:
             continue
-        # If the line has a format of "param: description", or "param (type): description", extract the 
+        # If the line has a format of "param: description", or "param (type): description", extract the
         # param and description using a regex
-        match = re.match(r"(\w+)\s*\((\w+)\):\s*(.*)", a.strip())
+        match = re.match(r"(\w+)\s*\((.*?)\):\s*(.*)", a.strip())
         if match:
             param, param_type, description = match.groups()
             param = param.strip()
             if param_type:
-                params[param] = f"{description.strip()} (type: {param_type})"
+                params[param] = f"({param_type if param_type != 'bool' else 'flag'}) {description.strip()}"
             else:
                 params[param] = description.strip()
     return params
 
 
 def cli_doc(method: callable):
     """
@@ -56,58 +59,62 @@
 
     Returns:
         tuple: A tuple of the help string and a list of click.Option objects.
     """
     params = []
     helps = get_method_description(method)
     param_docs = get_params_from_docstring(method.__doc__)
-    return_in_annots = "return" in method.__annotations__
-    for idx, (key, value) in enumerate(method.__annotations__.items()):
-        if key == "return":
+    annotations = get_type_hints(method)
+    return_in_annots = "return" in annotations
+    for idx, (key, value) in enumerate(annotations.items()):
+        if key == "return" or key in method._overriden_kwargs:
             continue
         default_value = None
-        di = len(method.__annotations__) - len(method.__defaults__ or []) - int(return_in_annots)
+        di = len(annotations) - len(method.__defaults__ or []) - int(return_in_annots)
         if method.__defaults__ and len(method.__defaults__) > 0 and idx >= di:
             default_value = method.__defaults__[idx - di]
         multiple = False
         if str(value).startswith("typing.Optional"):
             value = value.__args__[0]
         if str(value).startswith("typing.Literal"):
             value = str
         if str(value).startswith("typing.Union"):
             value = value.__args__[0]
         if str(value).startswith("typing.Dict"):
             value = str
         if str(value).startswith("typing.List"):
             value = list
             multiple = True
-
+        if value == bool:
+            default_value = False
         param = click.Option(
             [f"--{key}"],
             default=default_value,
             prompt_required=default_value is None,
             type=value,
             multiple=multiple,
             help=param_docs.get(key, f""),
             show_default=True,
+            is_flag=value == bool,
         )
         params.append(param)
-    return helps, params
+    return helps, list(reversed(params))
 
 
 def cli_callback(cls: type, method: str) -> callable:
     """Create a callback function for a click command.
 
     Args:
         cls (type): The class of the method.
         method (str): The name of the method.
-    
+
     Returns:
         callable: A callback function for the click command.
     """
+
     def callback(**kwargs):
         for key, value in kwargs.items():
             # Convert the tuples of tuple to dict.
             if isinstance(value, tuple) and len(value) > 0 and isinstance(value[0], tuple):
                 kwargs[key] = dict(value)
         result = method(**kwargs)
         click.echo(result)
@@ -130,13 +137,12 @@
         if v.__class__ != staticmethod:
             continue
         method = getattr(cls, k)
         if hasattr(method, "_clisync"):
             if method._clisync is False:
                 continue
         if requires_decorator:
-            if (not hasattr(method, "_clisync") or
-                    getattr(method, "_clisync") is False):
+            if not hasattr(method, "_clisync") or getattr(method, "_clisync") is False:
                 continue
         rv.append(cls.__name__ + "." + k)
     rv.sort()
     return rv
```

### Comparing `clisync-1.2.0/clisync.egg-info/PKG-INFO` & `clisync-1.3.0/clisync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clisync
-Version: 1.2.0
+Version: 1.3.0
 Summary: Generate click commands from your project
 Home-page: https://clisync.surge.sh
 Author: Edward Laurence
 Author-email: edwardl@hectiq.ai
 Keywords: pip requirements imports
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `clisync-1.2.0/demo/clisyncdemo/__init__.py` & `clisync-1.3.0/demo/clisyncdemo/__init__.py`

 * *Files identical despite different names*

### Comparing `clisync-1.2.0/demo/clisyncdemo/objects.py` & `clisync-1.3.0/demo/clisyncdemo/objects.py`

 * *Files identical despite different names*

### Comparing `clisync-1.2.0/setup.py` & `clisync-1.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
```

