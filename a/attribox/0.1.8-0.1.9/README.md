# Comparing `tmp/attribox-0.1.8.tar.gz` & `tmp/attribox-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attribox-0.1.8.tar", last modified: Fri Apr 12 17:06:49 2024, max compression
+gzip compressed data, was "attribox-0.1.9.tar", last modified: Wed May  1 08:53:34 2024, max compression
```

## Comparing `attribox-0.1.8.tar` & `attribox-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:06:49.902114 attribox-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 17:06:39.000000 attribox-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-12 17:06:49.902114 attribox-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-12 17:06:39.000000 attribox-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-12 17:06:46.000000 attribox-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-12 17:06:49.902114 attribox-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:06:49.898115 attribox-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:06:49.902114 attribox-0.1.8/src/attribox/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-12 17:06:39.000000 attribox-0.1.8/src/attribox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-12 17:06:39.000000 attribox-0.1.8/src/attribox/_abstract_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-12 17:06:39.000000 attribox-0.1.8/src/attribox/_attri_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-12 17:06:39.000000 attribox-0.1.8/src/attribox/_delayed_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-12 17:06:39.000000 attribox-0.1.8/src/attribox/_this_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-12 17:06:39.000000 attribox-0.1.8/src/attribox/_typed_descriptor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:06:49.902114 attribox-0.1.8/src/attribox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-12 17:06:49.000000 attribox-0.1.8/src/attribox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-12 17:06:49.000000 attribox-0.1.8/src/attribox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:06:49.000000 attribox-0.1.8/src/attribox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 17:06:49.000000 attribox-0.1.8/src/attribox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:53:34.544466 attribox-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 08:53:22.000000 attribox-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-01 08:53:34.544466 attribox-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-01 08:53:22.000000 attribox-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-01 08:53:30.000000 attribox-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-01 08:53:34.544466 attribox-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:53:34.540466 attribox-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:53:34.544466 attribox-0.1.9/src/attribox/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-01 08:53:22.000000 attribox-0.1.9/src/attribox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-01 08:53:22.000000 attribox-0.1.9/src/attribox/_abstract_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-01 08:53:22.000000 attribox-0.1.9/src/attribox/_attri_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-01 08:53:22.000000 attribox-0.1.9/src/attribox/_delayed_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-01 08:53:22.000000 attribox-0.1.9/src/attribox/_this_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-01 08:53:22.000000 attribox-0.1.9/src/attribox/_typed_descriptor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:53:34.544466 attribox-0.1.9/src/attribox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-01 08:53:34.000000 attribox-0.1.9/src/attribox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-01 08:53:34.000000 attribox-0.1.9/src/attribox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:53:34.000000 attribox-0.1.9/src/attribox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 08:53:34.000000 attribox-0.1.9/src/attribox.egg-info/top_level.txt
```

### Comparing `attribox-0.1.8/LICENSE` & `attribox-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `attribox-0.1.8/PKG-INFO` & `attribox-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attribox
-Version: 0.1.8
+Version: 0.1.9
 Summary: Allows for deferred instantiation of class attributes.
 Home-page: https://github.com/AsgerJon/attribox
 Author: Asger Jon Vistisen
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/attribox
 Project-URL: Bug Tracker, https://github.com/AsgerJon/attribox
 Classifier: Programming Language :: Python :: 3
```

### Comparing `attribox-0.1.8/README.md` & `attribox-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `attribox-0.1.8/pyproject.toml` & `attribox-0.1.9/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools>=68.2']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = "attribox"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name = "Asger Jon Vistisen", email = "asgerjon2@gmail.com" },
 ]
 description = "Allows for deferred instantiation of class attributes."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `attribox-0.1.8/setup.cfg` & `attribox-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = attribox
-version = 0.1.8
+version = 0.1.9
 author = Asger Jon Vistisen
 author_email = asgerjon2@gmail.com
 description = Class attributes as descriptors.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AsgerJon/attribox
 classifiers =
```

### Comparing `attribox-0.1.8/src/attribox/__init__.py` & `attribox-0.1.9/src/attribox/__init__.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.8/src/attribox/_abstract_descriptor.py` & `attribox-0.1.9/src/attribox/_abstract_descriptor.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.8/src/attribox/_attri_box.py` & `attribox-0.1.9/src/attribox/_attri_box.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,39 +2,53 @@
 syntactic sugar for setting the inner class, and for the inner object
 creation. """
 #  GPL-3.0 license
 #  Copyright (c) 2024 Asger Jon Vistisen
 from __future__ import annotations
 
 import sys
-from typing import Any
+from typing import Any, Callable
 
 from icecream import ic
 from vistutils.text import monoSpace
 from vistutils.waitaminute import typeMsg
 
 from attribox import TypedDescriptor, scope, this
 
 if sys.version_info.minor < 11:
   from typing_extensions import Self
 else:
   from typing import Self
 
-
 ic.configureOutput(includeContext=True, )
 
 
 class AttriBox(TypedDescriptor):
   """AttriBox subclasses the TypedDescriptor class and incorporates
   syntactic sugar for setting the inner class, and for the inner object
   creation. """
 
   __positional_args__ = None
   __keyword_args__ = None
 
+  @staticmethod
+  def _getterFactory(attributeName: str, attributeType: type) -> Callable:
+    """Returns a function that returns the attribute. """
+
+    def func(self, ) -> Any:
+      attribute = getattr(self, attributeName, None)
+      if attribute is None:
+        raise AttributeError('The attribute is not set!')
+      if isinstance(attribute, attributeType):
+        return attribute
+      e = typeMsg('attribute', attribute, attributeType)
+      raise TypeError(e)
+
+    return func
+
   def __init__(self, *args, **kwargs) -> None:
     """Initializes the AttriBox instance. """
     if not kwargs.get('_root', False):
       e = """The AttriBox class should not be instantiated directly!"""
       raise TypeError(e)
     if not args:
       e = """The inner class must be provided. """
@@ -69,15 +83,32 @@
     for arg in self.__positional_args__:
       if arg is this:
         args.append(instance)
       elif arg is scope:
         args.append(self._getFieldOwner())
       else:
         args.append(arg)
-    return innerClass(*args, **kwargs)
+    innerObject = innerClass(*args, **kwargs)
+    setattr(innerObject, '__outer_box__', self)
+    setattr(innerObject, '__owning_instance__', instance)
+    setattr(innerObject, '__field_owner__', self._getFieldOwner())
+    setattr(innerObject, '__field_name__', self._getFieldName())
+    setattr(innerObject,
+            'getFieldOwner',
+            self._getterFactory('__field_owner__', type))
+    setattr(innerObject,
+            'getFieldName',
+            self._getterFactory('__field_name__', str))
+    setattr(innerObject,
+            'getOuterBox',
+            self._getterFactory('__outer_box__', AttriBox))
+    setattr(innerObject,
+            'getOwningInstance',
+            self._getterFactory('__owning_instance__', object))
+    return innerObject
 
   def _typeGuard(self, item: object) -> Any:
     """Raises a TypeError if the item is not an instance of the inner
     class. """
     innerClass = self._getInnerClass()
     if not isinstance(item, innerClass):
       e = typeMsg('item', item, innerClass)
```

### Comparing `attribox-0.1.8/src/attribox/_delayed_descriptor.py` & `attribox-0.1.9/src/attribox/_delayed_descriptor.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.8/src/attribox/_this_scope.py` & `attribox-0.1.9/src/attribox/_this_scope.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.8/src/attribox/_typed_descriptor.py` & `attribox-0.1.9/src/attribox/_typed_descriptor.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.8/src/attribox.egg-info/PKG-INFO` & `attribox-0.1.9/src/attribox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attribox
-Version: 0.1.8
+Version: 0.1.9
 Summary: Allows for deferred instantiation of class attributes.
 Home-page: https://github.com/AsgerJon/attribox
 Author: Asger Jon Vistisen
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/attribox
 Project-URL: Bug Tracker, https://github.com/AsgerJon/attribox
 Classifier: Programming Language :: Python :: 3
```

