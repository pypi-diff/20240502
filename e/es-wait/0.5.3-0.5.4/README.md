# Comparing `tmp/es_wait-0.5.3.tar.gz` & `tmp/es_wait-0.5.4.tar.gz`

## Comparing `es_wait-0.5.3.tar` & `es_wait-0.5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.3/.coveragerc
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/__init__.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/_base.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/exceptions.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/exists.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/health.py
--rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/ilm.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/restore.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/task.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.3/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.3/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.3/README.md
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.4/.coveragerc
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/_base.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/exceptions.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/health.py
+-rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/ilm.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/task.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.4/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.4/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.4/README.md
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.4/PKG-INFO
```

### Comparing `es_wait-0.5.3/src/es_wait/_base.py` & `es_wait-0.5.4/src/es_wait/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             ('underscore_numbers', False),
         ]
         kw = {}
         for tup in defaults:
             key, default = tup
             kw[key] = kwargs[key] if key in kwargs else default
 
-        return pformat(*args, **kw)
+        return f"\n{pformat(*args, **kw)}"  # newline in front so it's always clean
 
     def setup(self) -> None:
         """Setup the waiter"""
 
     def wait_for_it(self, frequency: int = 5) -> None:
         """Do the actual waiting"""
         # Now with this mapped, we can perform the wait as indicated.
```

### Comparing `es_wait-0.5.3/src/es_wait/exists.py` & `es_wait-0.5.4/src/es_wait/exists.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.3/src/es_wait/health.py` & `es_wait-0.5.4/src/es_wait/health.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.3/src/es_wait/ilm.py` & `es_wait-0.5.4/src/es_wait/ilm.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.3/src/es_wait/relocate.py` & `es_wait-0.5.4/src/es_wait/relocate.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.3/src/es_wait/restore.py` & `es_wait-0.5.4/src/es_wait/restore.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.3/src/es_wait/snapshot.py` & `es_wait-0.5.4/src/es_wait/snapshot.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.3/src/es_wait/task.py` & `es_wait-0.5.4/src/es_wait/task.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.3/.gitignore` & `es_wait-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.3/LICENSE` & `es_wait-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.3/pyproject.toml` & `es_wait-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.3/PKG-INFO` & `es_wait-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.5.3
+Version: 0.5.4
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```

