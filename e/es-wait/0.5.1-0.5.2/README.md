# Comparing `tmp/es_wait-0.5.1.tar.gz` & `tmp/es_wait-0.5.2.tar.gz`

## Comparing `es_wait-0.5.1.tar` & `es_wait-0.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.1/.coveragerc
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/__init__.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/_base.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/exceptions.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/exists.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/health.py
--rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/ilm.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/restore.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/task.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.1/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.1/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.1/README.md
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.2/.coveragerc
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/_base.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/exceptions.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/health.py
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/ilm.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/task.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.2/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.2/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.2/README.md
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.2/PKG-INFO
```

### Comparing `es_wait-0.5.1/src/es_wait/_base.py` & `es_wait-0.5.2/src/es_wait/_base.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.1/src/es_wait/exists.py` & `es_wait-0.5.2/src/es_wait/exists.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.1/src/es_wait/health.py` & `es_wait-0.5.2/src/es_wait/health.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.1/src/es_wait/ilm.py` & `es_wait-0.5.2/src/es_wait/ilm.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,19 +33,16 @@
     def get_explain_data(self) -> t.Union[t.Dict, None]:
         """
         Calls `client.indices.`
         :py:meth:`~.elasticsearch.client.IlmClient.explain_lifecycle` with an index
         name and returns the resulting response.
         """
         try:
-            # The use of filter_path reduces the result set size
-            kw = {'index': self.name, 'filter_path': f'indices.{self.name}'}
-            # retval = self.client.ilm.explain_lifecycle(**kw)['indices'][self.name]
-            resp = self.client.ilm.explain_lifecycle(**kw)
-            logger.debug('response: %s', resp)
+            resp = self.client.ilm.explain_lifecycle(index=self.name)
+            logger.debug('ILM Explain response: %s', resp)
 
         except NotFoundError as exc:
             msg = (
                 f'Datastream/Index Name changed. {self.name} was not found. '
                 f'This is likely due to the index name suddenly changing, as with '
                 f'searchable snapshot mounts.'
             )
@@ -129,9 +126,19 @@
         Upstream callers need to try/catch any of KeyError (index name changed),
         :py:exc:`~.elasticsearch.exceptions.NotFoundError`, and
         :py:exc:`~.es_wait.exceptions.IlmWaitError`.
 
         We cannot not be responsible for retrying with a changed name as it's not in
         our scope as a "waiter"
         """
-        explain = DotMap(self.get_explain_data())
+        try:
+            explain = DotMap(self.get_explain_data())
+        except NotFoundError as err:
+            if self.client.indices.exists(index=self.name):
+                msg = (
+                    f'NotFoundError encountered. However, index {self.name} has been '
+                    f'confirmed to exist, so we continue to retry...'
+                )
+                self.logger.debug(msg)
+            else:
+                raise err
         return bool(explain.action == 'complete' and explain.step == 'complete')
```

### Comparing `es_wait-0.5.1/src/es_wait/relocate.py` & `es_wait-0.5.2/src/es_wait/relocate.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.1/src/es_wait/restore.py` & `es_wait-0.5.2/src/es_wait/restore.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.1/src/es_wait/snapshot.py` & `es_wait-0.5.2/src/es_wait/snapshot.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.1/src/es_wait/task.py` & `es_wait-0.5.2/src/es_wait/task.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.1/.gitignore` & `es_wait-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.1/LICENSE` & `es_wait-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.1/pyproject.toml` & `es_wait-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.1/PKG-INFO` & `es_wait-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.5.1
+Version: 0.5.2
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```

