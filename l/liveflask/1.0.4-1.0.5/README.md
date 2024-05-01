# Comparing `tmp/liveflask-1.0.4.tar.gz` & `tmp/liveflask-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveflask-1.0.4.tar", last modified: Wed May  1 20:36:56 2024, max compression
+gzip compressed data, was "liveflask-1.0.5.tar", last modified: Wed May  1 21:06:47 2024, max compression
```

## Comparing `liveflask-1.0.4.tar` & `liveflask-1.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 20:36:56.552139 liveflask-1.0.4/
--rw-rw-rw-   0        0        0     1342 2024-05-01 20:36:56.550140 liveflask-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 20:36:56.505139 liveflask-1.0.4/liveflask/
--rw-rw-rw-   0        0        0     5906 2024-05-01 20:33:29.000000 liveflask-1.0.4/liveflask/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 20:36:56.514140 liveflask-1.0.4/liveflask/attributes/
--rw-rw-rw-   0        0        0     2023 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 20:36:56.515140 liveflask-1.0.4/liveflask/attributes/__pycache__/
--rw-rw-rw-   0        0        0     3650 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/attributes/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-05-01 20:36:56.516139 liveflask-1.0.4/liveflask/static/
-drwxrwxrwx   0        0        0        0 2024-05-01 20:36:56.526140 liveflask-1.0.4/liveflask/static/liveflask/
--rw-rw-rw-   0        0        0     1566 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/static/liveflask/action.js
--rw-rw-rw-   0        0        0        0 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/static/liveflask/constants.js
--rw-rw-rw-   0        0        0      245 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/static/liveflask/events.js
--rw-rw-rw-   0        0        0      872 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/static/liveflask/liveflask.js
--rw-rw-rw-   0        0        0     2191 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/static/liveflask/model.js
--rw-rw-rw-   0        0        0     1660 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/static/liveflask/polling.js
--rw-rw-rw-   0        0        0     8447 2024-05-01 20:35:14.000000 liveflask-1.0.4/liveflask/static/liveflask/utils.js
--rw-rw-rw-   0        0        0    73154 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/static/lodash.min.js
-drwxrwxrwx   0        0        0        0 2024-05-01 20:36:56.528139 liveflask-1.0.4/liveflask/templates/
--rw-rw-rw-   0        0        0        0 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/templates/liveflask-head.html
--rw-rw-rw-   0        0        0      284 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/templates/liveflask-scripts.html
-drwxrwxrwx   0        0        0        0 2024-05-01 20:36:56.537139 liveflask-1.0.4/liveflask/traits/
--rw-rw-rw-   0        0        0      205 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/traits/Bootable.py
--rw-rw-rw-   0        0        0        0 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/traits/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 20:36:56.548139 liveflask-1.0.4/liveflask/traits/__pycache__/
--rw-rw-rw-   0        0        0      867 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/traits/__pycache__/Bootable.cpython-311.pyc
--rw-rw-rw-   0        0        0      198 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/traits/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3292 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/traits/__pycache__/has_actions.cpython-311.pyc
--rw-rw-rw-   0        0        0     4272 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/traits/__pycache__/has_props.cpython-311.pyc
--rw-rw-rw-   0        0        0     2835 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/traits/__pycache__/has_renders.cpython-311.pyc
--rw-rw-rw-   0        0        0     4776 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc
--rw-rw-rw-   0        0        0     2042 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/traits/has_actions.py
--rw-rw-rw-   0        0        0     2488 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/traits/has_props.py
--rw-rw-rw-   0        0        0     2486 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/traits/has_renders.py
--rw-rw-rw-   0        0        0     4106 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/traits/has_snapshots.py
--rw-rw-rw-   0        0        0     2032 2024-05-01 20:19:30.000000 liveflask-1.0.4/liveflask/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-01 20:36:56.512139 liveflask-1.0.4/liveflask.egg-info/
--rw-rw-rw-   0        0        0     1342 2024-05-01 20:36:56.000000 liveflask-1.0.4/liveflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1204 2024-05-01 20:36:56.000000 liveflask-1.0.4/liveflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 20:36:56.000000 liveflask-1.0.4/liveflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-01 20:36:56.000000 liveflask-1.0.4/liveflask.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-01 20:36:56.000000 liveflask-1.0.4/liveflask.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 20:36:56.552139 liveflask-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1201 2024-05-01 20:36:26.000000 liveflask-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:06:47.705043 liveflask-1.0.5/
+-rw-rw-rw-   0        0        0     1342 2024-05-01 21:06:47.703041 liveflask-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 21:06:47.650042 liveflask-1.0.5/liveflask/
+-rw-rw-rw-   0        0        0     6131 2024-05-01 20:53:47.000000 liveflask-1.0.5/liveflask/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:06:47.660042 liveflask-1.0.5/liveflask/attributes/
+-rw-rw-rw-   0        0        0     2023 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:06:47.661043 liveflask-1.0.5/liveflask/attributes/__pycache__/
+-rw-rw-rw-   0        0        0     3650 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/attributes/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-01 21:06:47.663044 liveflask-1.0.5/liveflask/static/
+drwxrwxrwx   0        0        0        0 2024-05-01 21:06:47.676045 liveflask-1.0.5/liveflask/static/liveflask/
+-rw-rw-rw-   0        0        0     1566 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/static/liveflask/action.js
+-rw-rw-rw-   0        0        0        0 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/static/liveflask/constants.js
+-rw-rw-rw-   0        0        0      245 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/static/liveflask/events.js
+-rw-rw-rw-   0        0        0      872 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/static/liveflask/liveflask.js
+-rw-rw-rw-   0        0        0     2191 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/static/liveflask/model.js
+-rw-rw-rw-   0        0        0     1660 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/static/liveflask/polling.js
+-rw-rw-rw-   0        0        0     8447 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/static/liveflask/utils.js
+-rw-rw-rw-   0        0        0    73154 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/static/lodash.min.js
+drwxrwxrwx   0        0        0        0 2024-05-01 21:06:47.679043 liveflask-1.0.5/liveflask/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/templates/liveflask-head.html
+-rw-rw-rw-   0        0        0      284 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/templates/liveflask-scripts.html
+drwxrwxrwx   0        0        0        0 2024-05-01 21:06:47.691044 liveflask-1.0.5/liveflask/traits/
+-rw-rw-rw-   0        0        0      205 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/traits/Bootable.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/traits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:06:47.701042 liveflask-1.0.5/liveflask/traits/__pycache__/
+-rw-rw-rw-   0        0        0      867 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/traits/__pycache__/Bootable.cpython-311.pyc
+-rw-rw-rw-   0        0        0      198 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/traits/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3292 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/traits/__pycache__/has_actions.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4272 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/traits/__pycache__/has_props.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2835 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/traits/__pycache__/has_renders.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4776 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2042 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/traits/has_actions.py
+-rw-rw-rw-   0        0        0     2488 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/traits/has_props.py
+-rw-rw-rw-   0        0        0     2486 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/traits/has_renders.py
+-rw-rw-rw-   0        0        0     4106 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/traits/has_snapshots.py
+-rw-rw-rw-   0        0        0     2032 2024-05-01 20:37:18.000000 liveflask-1.0.5/liveflask/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-01 21:06:47.658042 liveflask-1.0.5/liveflask.egg-info/
+-rw-rw-rw-   0        0        0     1342 2024-05-01 21:06:47.000000 liveflask-1.0.5/liveflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1204 2024-05-01 21:06:47.000000 liveflask-1.0.5/liveflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 21:06:47.000000 liveflask-1.0.5/liveflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-01 21:06:47.000000 liveflask-1.0.5/liveflask.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-01 21:06:47.000000 liveflask-1.0.5/liveflask.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 21:06:47.705043 liveflask-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2024-05-01 21:03:57.000000 liveflask-1.0.5/setup.py
```

### Comparing `liveflask-1.0.4/PKG-INFO` & `liveflask-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.4
+Version: 1.0.5
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.4/liveflask/__init__.py` & `liveflask-1.0.5/liveflask/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ast
 import functools
 import os
 import secrets
-
+import gzip
 from flask import Blueprint, render_template, Response
 from flask import request
 from markupsafe import Markup
 
 from .traits.has_actions import HasActions
 from .traits.has_props import HasProps
 from .traits.has_renders import HasRenders
@@ -144,28 +144,35 @@
             'polling.js',
             'events.js'
         ]
         combined_js = ''
         for js_file in js_files:
             with open(f'{package_dir}/static/liveflask/{js_file}', 'r') as f:
                 combined_js += f.read()
-        resp = Response(combined_js)
+        resp = Response(
+            gzip.compress(combined_js.encode('utf-8'))
+        )
+        resp.headers['Content-Encoding'] = 'gzip'
         resp.mimetype = 'application/javascript'
         resp.headers['Cache-Control'] = 'public, max-age=3600'
         return resp
 
     @liveflask_bp.route("/liveflask.js")
     def liveflask_js():
         combined_js = ''
         # serve liveflask.js from static directory with the mimetype of 'application/javascript'
         with open(f'{package_dir}/static/liveflask/liveflask.js', 'r') as f:
             combined_js += f.read()
-        resp = Response(combined_js)
+        resp = Response(
+            gzip.compress(combined_js.encode('utf-8'))
+        )
+        resp.headers['Content-Encoding'] = 'gzip'
         resp.mimetype = 'application/javascript'
         resp.headers['Cache-Control'] = 'public, max-age=3600'
+
         return resp
 
     @app.template_global()
     def liveflask_scripts():
         return Markup(render_template("liveflask-scripts.html"))
 
     app.register_blueprint(liveflask_bp, url_prefix='/liveflask')
```

### Comparing `liveflask-1.0.4/liveflask/attributes/__init__.py` & `liveflask-1.0.5/liveflask/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.4/liveflask/attributes/__pycache__/__init__.cpython-311.pyc` & `liveflask-1.0.5/liveflask/attributes/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd2a33266 (Wed May  1 20:19:30 2024 UTC)
+moddate:  0xfea73266 (Wed May  1 20:37:18 2024 UTC)
 files sz: 2023
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `liveflask-1.0.4/liveflask/static/liveflask/action.js` & `liveflask-1.0.5/liveflask/static/liveflask/action.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.4/liveflask/static/liveflask/liveflask.js` & `liveflask-1.0.5/liveflask/static/liveflask/liveflask.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.4/liveflask/static/liveflask/model.js` & `liveflask-1.0.5/liveflask/static/liveflask/model.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.4/liveflask/static/liveflask/polling.js` & `liveflask-1.0.5/liveflask/static/liveflask/polling.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.4/liveflask/static/liveflask/utils.js` & `liveflask-1.0.5/liveflask/static/liveflask/utils.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.4/liveflask/static/lodash.min.js` & `liveflask-1.0.5/liveflask/static/lodash.min.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.4/liveflask/traits/__pycache__/Bootable.cpython-311.pyc` & `liveflask-1.0.5/liveflask/traits/__pycache__/Bootable.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd2a33266 (Wed May  1 20:19:30 2024 UTC)
+moddate:  0xfea73266 (Wed May  1 20:37:18 2024 UTC)
 files sz: 205
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `liveflask-1.0.4/liveflask/traits/__pycache__/has_actions.cpython-311.pyc` & `liveflask-1.0.5/liveflask/traits/__pycache__/has_actions.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd2a33266 (Wed May  1 20:19:30 2024 UTC)
+moddate:  0xfea73266 (Wed May  1 20:37:18 2024 UTC)
 files sz: 2042
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `liveflask-1.0.4/liveflask/traits/__pycache__/has_props.cpython-311.pyc` & `liveflask-1.0.5/liveflask/traits/__pycache__/has_props.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd2a33266 (Wed May  1 20:19:30 2024 UTC)
+moddate:  0xfea73266 (Wed May  1 20:37:18 2024 UTC)
 files sz: 2488
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `liveflask-1.0.4/liveflask/traits/__pycache__/has_renders.cpython-311.pyc` & `liveflask-1.0.5/liveflask/traits/__pycache__/has_renders.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd2a33266 (Wed May  1 20:19:30 2024 UTC)
+moddate:  0xfea73266 (Wed May  1 20:37:18 2024 UTC)
 files sz: 2486
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `liveflask-1.0.4/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc` & `liveflask-1.0.5/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd2a33266 (Wed May  1 20:19:30 2024 UTC)
+moddate:  0xfea73266 (Wed May  1 20:37:18 2024 UTC)
 files sz: 4106
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `liveflask-1.0.4/liveflask/traits/has_actions.py` & `liveflask-1.0.5/liveflask/traits/has_actions.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.4/liveflask/traits/has_props.py` & `liveflask-1.0.5/liveflask/traits/has_props.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.4/liveflask/traits/has_renders.py` & `liveflask-1.0.5/liveflask/traits/has_renders.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.4/liveflask/traits/has_snapshots.py` & `liveflask-1.0.5/liveflask/traits/has_snapshots.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.4/liveflask/utils.py` & `liveflask-1.0.5/liveflask/utils.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.4/liveflask.egg-info/PKG-INFO` & `liveflask-1.0.5/liveflask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.4
+Version: 1.0.5
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.4/liveflask.egg-info/SOURCES.txt` & `liveflask-1.0.5/liveflask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.4/setup.py` & `liveflask-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme_pypi.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="liveflask",
-    version="1.0.4",
+    version="1.0.5",
     author="Jarriq Rolle",
     author_email="jrolle@baysidetechgroup.com",
     description="Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JarriqTheTechie/liveflask",
     packages=['liveflask'],
```

