# Comparing `tmp/es_wait-0.5.2.tar.gz` & `tmp/es_wait-0.5.3.tar.gz`

## Comparing `es_wait-0.5.2.tar` & `es_wait-0.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.2/.coveragerc
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/__init__.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/_base.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/exceptions.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/exists.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/health.py
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/ilm.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/restore.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 es_wait-0.5.2/src/es_wait/task.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.2/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.2/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.2/README.md
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.3/.coveragerc
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/_base.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/exceptions.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/health.py
+-rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/ilm.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 es_wait-0.5.3/src/es_wait/task.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.3/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.3/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.3/README.md
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.3/PKG-INFO
```

### Comparing `es_wait-0.5.2/src/es_wait/_base.py` & `es_wait-0.5.3/src/es_wait/_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Base Waiter Class"""
 
 import typing as t
 import logging
+from pprint import pformat
 from time import sleep
 from datetime import datetime, timezone
 
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
 logger = logging.getLogger('es_wait.Waiter')
@@ -38,14 +39,40 @@
     def empty_check(self, name: str) -> None:
         """Ensure that no empty values sneak through"""
         if getattr(self, name) is None:
             msg = f'Keyword arg {name} cannot be None'
             logger.critical(msg)
             raise ValueError(msg)
 
+    def prettystr(self, *args, **kwargs) -> str:
+        """
+        A (nearly) straight up wrapper for pprint.pformat, except that we provide our
+        own default values for 'indent' (2) and 'sort_dicts' (False). Primarily for
+        debug logging and showing more readable dictionaries.
+
+        'Return the formatted representation of object as a string. indent, width,
+        depth, compact, sort_dicts and underscore_numbers are passed to the
+        PrettyPrinter constructor as formatting parameters' (from pprint
+        documentation).
+        """
+        defaults = [
+            ('indent', 2),
+            ('width', 80),
+            ('depth', None),
+            ('compact', False),
+            ('sort_dicts', False),
+            ('underscore_numbers', False),
+        ]
+        kw = {}
+        for tup in defaults:
+            key, default = tup
+            kw[key] = kwargs[key] if key in kwargs else default
+
+        return pformat(*args, **kw)
+
     def setup(self) -> None:
         """Setup the waiter"""
 
     def wait_for_it(self, frequency: int = 5) -> None:
         """Do the actual waiting"""
         # Now with this mapped, we can perform the wait as indicated.
         start_time = self.now
```

### Comparing `es_wait-0.5.2/src/es_wait/exists.py` & `es_wait-0.5.3/src/es_wait/exists.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.2/src/es_wait/health.py` & `es_wait-0.5.3/src/es_wait/health.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.2/src/es_wait/ilm.py` & `es_wait-0.5.3/src/es_wait/ilm.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,28 +34,27 @@
         """
         Calls `client.indices.`
         :py:meth:`~.elasticsearch.client.IlmClient.explain_lifecycle` with an index
         name and returns the resulting response.
         """
         try:
             resp = self.client.ilm.explain_lifecycle(index=self.name)
-            logger.debug('ILM Explain response: %s', resp)
-
+            logger.debug('ILM Explain response: %s', self.prettystr(resp))
         except NotFoundError as exc:
             msg = (
                 f'Datastream/Index Name changed. {self.name} was not found. '
                 f'This is likely due to the index name suddenly changing, as with '
                 f'searchable snapshot mounts.'
             )
             logger.error(msg)
             raise exc  # re-raise the original. Just wanted to log here.
         except Exception as err:
             msg = f'Unable to get ILM information for index {self.name}'
             logger.critical(msg)
-            raise IlmWaitError(f'{msg}. Exception: {err}') from err
+            raise IlmWaitError(f'{msg}. Exception: {self.prettystr(err)}') from err
         retval = resp['indices'][self.name]
         return retval
 
 
 class IlmPhase(IndexLifecycle):
     """
     ILM Phase class (child of class IndexLifecycle)
@@ -126,14 +125,15 @@
         Upstream callers need to try/catch any of KeyError (index name changed),
         :py:exc:`~.elasticsearch.exceptions.NotFoundError`, and
         :py:exc:`~.es_wait.exceptions.IlmWaitError`.
 
         We cannot not be responsible for retrying with a changed name as it's not in
         our scope as a "waiter"
         """
+        explain = DotMap(action='no', step='no')  # Set defaults so the return works
         try:
             explain = DotMap(self.get_explain_data())
         except NotFoundError as err:
             if self.client.indices.exists(index=self.name):
                 msg = (
                     f'NotFoundError encountered. However, index {self.name} has been '
                     f'confirmed to exist, so we continue to retry...'
```

### Comparing `es_wait-0.5.2/src/es_wait/relocate.py` & `es_wait-0.5.3/src/es_wait/relocate.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.2/src/es_wait/restore.py` & `es_wait-0.5.3/src/es_wait/restore.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,21 +41,21 @@
         response = {}
         for chunk in self.index_list_chunks:
             chunk_response = self.get_recovery(chunk)
             if chunk_response == {}:
                 logger.debug('_recovery API returned an empty response. Trying again.')
                 return False
             response.update(chunk_response)
-        logger.debug('Provided indices: %s', self.index_list)
-        logger.debug('Found indices: %s', list(response.keys()))
+        logger.debug('Provided indices: %s', self.prettystr(self.index_list))
+        logger.debug('Found indices: %s', self.prettystr(list(response.keys())))
         for index, data in response.items():
             for shard in data['shards']:
                 stage = shard['stage']
                 if stage != 'DONE':
-                    print(f'Index {index} is still in stage {stage}')
+                    logger.debug('Index %s is still in stage %s', index, stage)
                     return False
 
         # If we've gotten here, all of the indices have recovered
         return True
 
     @property
     def index_list_chunks(self) -> t.Sequence[t.Sequence[t.AnyStr]]:
@@ -81,11 +81,11 @@
     def get_recovery(self, chunk: t.Sequence[str]) -> t.Dict:
         """Get recovery information from Elasticsearch"""
         try:
             chunk_response = self.client.indices.recovery(index=chunk, human=True)
         except Exception as err:
             msg = (
                 f'Unable to obtain recovery information for specified indices. Error: '
-                f'{err}'
+                f'{self.prettystr(err)}'
             )
             raise ValueError(msg) from err
         return chunk_response
```

### Comparing `es_wait-0.5.2/src/es_wait/snapshot.py` & `es_wait-0.5.3/src/es_wait/snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         try:
             result = self.client.snapshot.get(
                 repository=self.repository, snapshot=self.snapshot
             )
         except Exception as err:
             raise ValueError(
                 f'Unable to obtain information for snapshot "{self.snapshot}" in '
-                f'repository "{self.repository}". Error: {err}'
+                f'repository "{self.repository}". Error: {self.prettystr(err)}'
             ) from err
         return result
 
     def log_completion(self, state: str) -> None:
         if state == 'SUCCESS':
             logger.info('Snapshot %s successfully completed.', self.snapshot)
         elif state == 'PARTIAL':
```

### Comparing `es_wait-0.5.2/src/es_wait/task.py` & `es_wait-0.5.3/src/es_wait/task.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,31 +59,34 @@
             # self.task_data = TaskArgs(
             #     settings=self.client.tasks.get(task_id=self.task_id)
             # )
             self.task_data = DotMap(self.client.tasks.get(task_id=self.task_id))
         except Exception as err:
             msg = (
                 f'Unable to obtain task information for task_id "{self.task_id}". '
-                f'Exception {err}'
+                f'Exception {self.prettystr(err)}'
             )
             raise ValueError(msg) from err
         self.task = self.task_data.task
         self.reindex_check()
         return self.task_complete
 
     def reindex_check(self) -> None:
         if self.task.action == 'indices:data/write/reindex':
             logger.debug("It's a REINDEX task")
-            logger.debug('TASK_DATA: %s', self.task_data.toDict())
-            logger.debug('TASK_DATA keys: %s', list(self.task_data.toDict().keys()))
+            logger.debug('TASK_DATA: %s', self.prettystr(self.task_data.toDict()))
+            logger.debug(
+                'TASK_DATA keys: %s',
+                self.prettystr(list(self.task_data.toDict().keys())),
+            )
             if self.task_data.response.failures:
                 if len(self.task_data.response.failures) > 0:
                     msg = (
                         f'Failures found in the {self.action} response: '
-                        f'{self.task_data.response["failures"]}'
+                        f'{self.prettystr(self.task_data.response["failures"])}'
                     )
                     raise ValueError(msg)
 
     @property
     def task_complete(self) -> bool:
         running_time = 0.000000001 * self.task.running_time_in_nanos
         logger.debug('Running time: %s seconds', running_time)
@@ -94,15 +97,15 @@
             )
             logger.debug(
                 'Task "%s" completed at %s.', self.task.description, time_string
             )
             retval = True
         else:
             # Log the task status here.
-            logger.debug('Full Task Data: %s', self.task_data.asdict)
+            logger.debug('Full Task Data: %s', self.prettystr(self.task_data.toDict()))
             msg = (
                 f'Task "{self.task.description}" with task_id "{self.task_id}" has '
                 f'been running for {running_time} seconds'
             )
             logger.debug(msg)
             retval = False
         return retval
```

### Comparing `es_wait-0.5.2/.gitignore` & `es_wait-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.2/LICENSE` & `es_wait-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.2/pyproject.toml` & `es_wait-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.2/PKG-INFO` & `es_wait-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.5.2
+Version: 0.5.3
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```

