# Comparing `tmp/parliamentarch-0.1.tar.gz` & `tmp/parliamentarch-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parliamentarch-0.1.tar", last modified: Thu May  2 17:47:48 2024, max compression
+gzip compressed data, was "parliamentarch-0.2.tar", last modified: Thu May  2 20:38:22 2024, max compression
```

## Comparing `parliamentarch-0.1.tar` & `parliamentarch-0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:47:48.157703 parliamentarch-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:47:48.153703 parliamentarch-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:47:48.153703 parliamentarch-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-02 17:47:43.000000 parliamentarch-0.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-02 17:47:43.000000 parliamentarch-0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 17:47:43.000000 parliamentarch-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-02 17:47:43.000000 parliamentarch-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-02 17:47:43.000000 parliamentarch-0.1/LISEZMOI.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14134 2024-05-02 17:47:48.157703 parliamentarch-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-05-02 17:47:43.000000 parliamentarch-0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-02 17:47:43.000000 parliamentarch-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:47:48.157703 parliamentarch-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:47:48.153703 parliamentarch-0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:47:48.153703 parliamentarch-0.1/src/ParliamentArch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14134 2024-05-02 17:47:48.000000 parliamentarch-0.1/src/ParliamentArch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-02 17:47:48.000000 parliamentarch-0.1/src/ParliamentArch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:47:48.000000 parliamentarch-0.1/src/ParliamentArch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 17:47:48.000000 parliamentarch-0.1/src/ParliamentArch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:47:48.153703 parliamentarch-0.1/src/parliamentarch/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-02 17:47:43.000000 parliamentarch-0.1/src/parliamentarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-02 17:47:43.000000 parliamentarch-0.1/src/parliamentarch/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-05-02 17:47:43.000000 parliamentarch-0.1/src/parliamentarch/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-02 17:47:43.000000 parliamentarch-0.1/src/parliamentarch/svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:38:22.186259 parliamentarch-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:38:22.182259 parliamentarch-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:38:22.182259 parliamentarch-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-02 20:38:17.000000 parliamentarch-0.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-02 20:38:17.000000 parliamentarch-0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 20:38:17.000000 parliamentarch-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-02 20:38:17.000000 parliamentarch-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-02 20:38:17.000000 parliamentarch-0.2/LISEZMOI.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13883 2024-05-02 20:38:22.186259 parliamentarch-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-05-02 20:38:17.000000 parliamentarch-0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-02 20:38:17.000000 parliamentarch-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:38:22.186259 parliamentarch-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:38:22.182259 parliamentarch-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:38:22.186259 parliamentarch-0.2/src/ParliamentArch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13883 2024-05-02 20:38:22.000000 parliamentarch-0.2/src/ParliamentArch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-02 20:38:22.000000 parliamentarch-0.2/src/ParliamentArch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:38:22.000000 parliamentarch-0.2/src/ParliamentArch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 20:38:22.000000 parliamentarch-0.2/src/ParliamentArch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:38:22.186259 parliamentarch-0.2/src/parliamentarch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-02 20:38:17.000000 parliamentarch-0.2/src/parliamentarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-02 20:38:17.000000 parliamentarch-0.2/src/parliamentarch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-02 20:38:17.000000 parliamentarch-0.2/src/parliamentarch/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-05-02 20:38:17.000000 parliamentarch-0.2/src/parliamentarch/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-02 20:38:17.000000 parliamentarch-0.2/src/parliamentarch/svg.py
```

### Comparing `parliamentarch-0.1/.github/workflows/python-package.yml` & `parliamentarch-0.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `parliamentarch-0.1/.github/workflows/python-publish.yml` & `parliamentarch-0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `parliamentarch-0.1/LICENSE` & `parliamentarch-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parliamentarch-0.1/LISEZMOI.rst` & `parliamentarch-0.2/LISEZMOI.rst`

 * *Files identical despite different names*

### Comparing `parliamentarch-0.1/PKG-INFO` & `parliamentarch-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParliamentArch
-Version: 0.1
+Version: 0.2
 Summary: Generation of arch-styled parliamentary arches
 Author: Gouvernathor
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Gouvernathor
         
         Redistribution and use in source and binary forms, with or without
@@ -276,20 +276,15 @@
 from left to right. ``sorted(di, key=di.get, reverse=True)`` helps with that.
 
 SeatData and dispatch_seats may be moved to another module in the future.
 
 Todos and future features
 -------------------------
 
-- Document the new SVG direct content
 - Have the main functions support a sequence of SeatData objects using ``dict.fromkeys(seq, 1)``
 - Allow SeatData to take some <a> element properties (like href), and if so use <a> instead of <g>
 - Allow SeatData to contain more creative SVG content like gradients
   - Maybe give it a .wrap method that wraps the circles in a g or a, and make it subclassable ?
   - Maybe just give a style method ?
-- Move the SVG direct content to the module root, move svg_base to svg, and stop importing geometry into root
-- Add LICENSE
 - Add tests
 - Add the option to force all rows to contain an even number of seats
-- Enquire about the unsure_param in svg
-- Maybe add support for named colors, if acceptable in SVG
-- Add a CLI for SVG files generation
+- Add a simpler way to input parameters in CLI
```

### Comparing `parliamentarch-0.1/README.rst` & `parliamentarch-0.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -237,20 +237,15 @@
 from left to right. ``sorted(di, key=di.get, reverse=True)`` helps with that.
 
 SeatData and dispatch_seats may be moved to another module in the future.
 
 Todos and future features
 -------------------------
 
-- Document the new SVG direct content
 - Have the main functions support a sequence of SeatData objects using ``dict.fromkeys(seq, 1)``
 - Allow SeatData to take some <a> element properties (like href), and if so use <a> instead of <g>
 - Allow SeatData to contain more creative SVG content like gradients
   - Maybe give it a .wrap method that wraps the circles in a g or a, and make it subclassable ?
   - Maybe just give a style method ?
-- Move the SVG direct content to the module root, move svg_base to svg, and stop importing geometry into root
-- Add LICENSE
 - Add tests
 - Add the option to force all rows to contain an even number of seats
-- Enquire about the unsure_param in svg
-- Maybe add support for named colors, if acceptable in SVG
-- Add a CLI for SVG files generation
+- Add a simpler way to input parameters in CLI
```

### Comparing `parliamentarch-0.1/src/ParliamentArch.egg-info/PKG-INFO` & `parliamentarch-0.2/src/ParliamentArch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParliamentArch
-Version: 0.1
+Version: 0.2
 Summary: Generation of arch-styled parliamentary arches
 Author: Gouvernathor
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Gouvernathor
         
         Redistribution and use in source and binary forms, with or without
@@ -276,20 +276,15 @@
 from left to right. ``sorted(di, key=di.get, reverse=True)`` helps with that.
 
 SeatData and dispatch_seats may be moved to another module in the future.
 
 Todos and future features
 -------------------------
 
-- Document the new SVG direct content
 - Have the main functions support a sequence of SeatData objects using ``dict.fromkeys(seq, 1)``
 - Allow SeatData to take some <a> element properties (like href), and if so use <a> instead of <g>
 - Allow SeatData to contain more creative SVG content like gradients
   - Maybe give it a .wrap method that wraps the circles in a g or a, and make it subclassable ?
   - Maybe just give a style method ?
-- Move the SVG direct content to the module root, move svg_base to svg, and stop importing geometry into root
-- Add LICENSE
 - Add tests
 - Add the option to force all rows to contain an even number of seats
-- Enquire about the unsure_param in svg
-- Maybe add support for named colors, if acceptable in SVG
-- Add a CLI for SVG files generation
+- Add a simpler way to input parameters in CLI
```

### Comparing `parliamentarch-0.1/src/parliamentarch/__init__.py` & `parliamentarch-0.2/src/parliamentarch/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 from .geometry import get_seats_centers
 from .svg import SeatData, dispatch_seats, write_grouped_svg
 from ._util import filter_kwargs, get_from_write
 
 __all__ = ("get_svg_from_attribution", "write_svg_from_attribution", "SeatData")
 
-_GET_SEATS_CENTERS_PARAMS = {k for k, p in signature(get_seats_centers).parameters.items() if p.kind==p.KEYWORD_ONLY}
-_WRITE_GROUPED_SVG_PARAMS = {k for k, p in signature(write_grouped_svg).parameters.items() if p.kind==p.KEYWORD_ONLY}
+_GET_SEATS_CENTERS_PARAM_NAMES = {k for k, p in signature(get_seats_centers).parameters.items() if p.kind==p.KEYWORD_ONLY}
+_WRITE_GROUPED_SVG_PARAM_NAMES = {k for k, p in signature(write_grouped_svg).parameters.items() if p.kind==p.KEYWORD_ONLY}
 
 def write_svg_from_attribution(file: TextIOBase, attrib: dict[SeatData, int], **kwargs) -> None:
     nseats = sum(attrib.values())
-    get_seats_centers_kwargs, write_grouped_svg_kwargs, kwargs = filter_kwargs(_GET_SEATS_CENTERS_PARAMS, _WRITE_GROUPED_SVG_PARAMS, **kwargs)
+    get_seats_centers_kwargs, write_grouped_svg_kwargs, kwargs = filter_kwargs(_GET_SEATS_CENTERS_PARAM_NAMES, _WRITE_GROUPED_SVG_PARAM_NAMES, **kwargs)
 
     if kwargs:
         raise TypeError("Unknown parameters : " + ", ".join(kwargs))
 
     results = get_seats_centers(nseats, **get_seats_centers_kwargs)
-    seat_centers_by_group = dispatch_seats(attrib, sorted(results, key=results.get, reverse=True))
+    seat_centers_by_group = dispatch_seats(attrib, sorted(results, key=results.__getitem__, reverse=True))
     write_grouped_svg(file, seat_centers_by_group, results.seat_actual_radius, **write_grouped_svg_kwargs)
 
 get_svg_from_attribution = get_from_write(write_svg_from_attribution)
```

### Comparing `parliamentarch-0.1/src/parliamentarch/_util.py` & `parliamentarch-0.2/src/parliamentarch/_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections.abc import Container, Sequence
 from io import StringIO
-from typing import Any, NamedTuple
+from typing import NamedTuple
 
 class FactoryDict(dict):
     def __init__(self, default_factory, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.default_factory = default_factory
 
     def __missing__(self, key):
@@ -43,28 +43,27 @@
 def get_from_write(write_func):
     def get(*args, **kwargs) -> str:
         sio = StringIO()
         write_func(sio, *args, **kwargs)
         return sio.getvalue()
     return get
 
-def filter_kwargs(
+def filter_kwargs[V](
         *sets: Container[str],
-        **kwargs: Any,
-        ) -> list[dict[str, Any]]:
+        **kwargs: V,
+        ) -> list[dict[str, V]]:
     """
     The length of the list is one more than the number of sets passed.
     The sets may actually be any container.
     """
 
     rvdicts = []
     for s in sets:
         rvdict = {}
         # no set operations in order to keep the ordering
         for k in tuple(kwargs):
             if k in s:
                 rvdict[k] = kwargs.pop(k)
-        if not kwargs:
-            break
+        rvdicts.append(rvdict)
 
     rvdicts.append(kwargs)
     return rvdicts
```

### Comparing `parliamentarch-0.1/src/parliamentarch/geometry.py` & `parliamentarch-0.2/src/parliamentarch/geometry.py`

 * *Files identical despite different names*

### Comparing `parliamentarch-0.1/src/parliamentarch/svg.py` & `parliamentarch-0.2/src/parliamentarch/svg.py`

 * *Files identical despite different names*

