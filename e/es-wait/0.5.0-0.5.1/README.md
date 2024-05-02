# Comparing `tmp/es_wait-0.5.0.tar.gz` & `tmp/es_wait-0.5.1.tar.gz`

## Comparing `es_wait-0.5.0.tar` & `es_wait-0.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.0/.coveragerc
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/__init__.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/_base.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/exceptions.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/exists.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/health.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/ilm.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/restore.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/task.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.0/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.0/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.0/README.md
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.1/.coveragerc
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/_base.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/exceptions.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/health.py
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/ilm.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 es_wait-0.5.1/src/es_wait/task.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.1/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.1/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.1/README.md
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.1/PKG-INFO
```

### Comparing `es_wait-0.5.0/src/es_wait/_base.py` & `es_wait-0.5.1/src/es_wait/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 import logging
 from time import sleep
 from datetime import datetime, timezone
 
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
+logger = logging.getLogger('es_wait.Waiter')
+
 
 class Waiter:
     """Class Definition"""
 
     def __init__(
         self,
         client: 'Elasticsearch',
         pause: float = 9,  # The delay between checks
         timeout: float = -1,  # How long is too long
     ) -> None:
-        self.logger = logging.getLogger('es_wait.Base')
         self.client = client
         self.pause = pause
         self.timeout = timeout
         self.checkid = 'check for Waiter class'
 
     @property
     def now(self) -> datetime:
@@ -34,57 +35,57 @@
         """This will need to be redefined by each child class"""
         return False
 
     def empty_check(self, name: str) -> None:
         """Ensure that no empty values sneak through"""
         if getattr(self, name) is None:
             msg = f'Keyword arg {name} cannot be None'
-            self.logger.critical(msg)
+            logger.critical(msg)
             raise ValueError(msg)
 
     def setup(self) -> None:
         """Setup the waiter"""
 
     def wait_for_it(self, frequency: int = 5) -> None:
         """Do the actual waiting"""
         # Now with this mapped, we can perform the wait as indicated.
         start_time = self.now
         success = False
-        self.logger.debug('Only logging every %s seconds', frequency)
+        logger.debug('Only logging every %s seconds', frequency)
         while True:
             elapsed = int((self.now - start_time).total_seconds())
             if elapsed == 0:
                 loggit = False
             else:
                 loggit = elapsed % frequency == 0  # Only frequency seconds
             response = self.check
             # Successfully completed task.
             if response:
-                self.logger.debug('%s finished executing', self.checkid)
+                logger.debug('%s finished executing', self.checkid)
                 total = f'{(self.now - start_time).total_seconds():.2f}'
-                self.logger.debug('Elapsed time: %s seconds', total)
+                logger.debug('Elapsed time: %s seconds', total)
                 success = True
                 break
             # Not success, and reached timeout (if defined)
             if (self.timeout != -1) and (elapsed >= self.timeout):
                 msg = (
                     f'The {self.checkid} did not complete within {self.timeout} '
                     f'seconds.'
                 )
-                self.logger.error(msg)
+                logger.error(msg)
                 break
             # Not timed out and not yet success, so we wait.
             if loggit:
                 msg = (
                     f'The {self.checkid} is not yet complete. {elapsed} total seconds '
                     f'have elapsed. Pausing {self.pause} seconds between checks.'
                 )
-                self.logger.debug(msg)
+                logger.debug(msg)
             sleep(self.pause)  # Actual wait here
 
         if not success:
             msg = (
                 f'The {self.checkid} failed to complete in the timeout period of '
                 f'{self.timeout} seconds'
             )
-            self.logger.error(msg)
+            logger.error(msg)
             raise TimeoutError(msg)
```

### Comparing `es_wait-0.5.0/src/es_wait/exists.py` & `es_wait-0.5.1/src/es_wait/exists.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import typing as t
 import logging
 from ._base import Waiter
 
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
+logger = logging.getLogger('es_wait.Exists')
+
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class Exists(Waiter):
     """Class Definition"""
 
     IDX_OR_DS = ['index', 'data_stream', 'datastream', 'idx', 'ds']
@@ -21,15 +23,15 @@
         self,
         client: 'Elasticsearch',
         pause: float = 1.5,
         timeout: float = 15,
         name: str = '',
         kind: str = '',
     ) -> None:
-        self.logger = logging.getLogger('es_wait.Exists')
+
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.name = name
         self.kind = kind
         self.empty_check('name')
         self.empty_check('kind')
         self.checkid = f'check for {self.kindmap} {name} to exist'
 
@@ -64,9 +66,9 @@
         """This is a little way to ensure many possibilities come down to one"""
         if self.kind in self.IDX_OR_DS:
             return 'index or data_stream'
         if self.kind in self.TEMPLATE:
             return 'index template'
         if self.kind in self.COMPONENT:
             return 'component template'
-        self.logger.error('%s is not an acceptable value for kind', self.kind)
+        logger.error('%s is not an acceptable value for kind', self.kind)
         return 'FAIL'  # We should not see this, like, ever
```

### Comparing `es_wait-0.5.0/src/es_wait/health.py` & `es_wait-0.5.1/src/es_wait/health.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import typing as t
 import logging
 from ._base import Waiter
 
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
+logger = logging.getLogger('es_wait.Health')
+
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class Health(Waiter):
     ACTIONS = ['allocation', 'cluster_routing', 'mount', 'replicas', 'shrink']
     RELO_ACTIONS = ['allocation', 'cluster_routing']
     STATUS_ACTIONS = ['mount', 'replicas', 'shrink']
@@ -22,28 +24,27 @@
         client: 'Elasticsearch',
         pause: float = 1.5,
         timeout: float = 15,
         action: t.Literal[
             'allocation', 'cluster_routing', 'mount', 'replicas', 'shrink'
         ] = None,
     ) -> None:
-        self.logger = logging.getLogger('es_wait.Health')
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.action = action
         self.empty_check('action')
         self.checkid = self.getcheckid
 
     def argmap(self) -> t.Union[t.Dict[str, int], t.Dict[str, str]]:
         """This is a little way to ensure many possibilities come down to one"""
         if self.action in self.RELO_ACTIONS:
             return self.RELO_ARGS
         if self.action in self.STATUS_ACTIONS:
             return self.STATUS_ARGS
         msg = f'{self.action} is not an acceptable value for action'
-        self.logger.error(msg)
+        logger.error(msg)
         raise ValueError(msg)
 
     @property
     def check(self) -> bool:
         """
         This function calls `client.cluster.`
         :py:meth:`~.elasticsearch.client.ClusterClient.health` and, based on the
@@ -61,24 +62,24 @@
                 raise KeyError(f'Key "{key}" not in cluster health output')
             # Verify that the output matches the expected value
             if output[key] != value:
                 msg = (
                     f'NO MATCH: Value for key "{value}", health check output: '
                     f'{output[key]}'
                 )
-                self.logger.debug(msg)
+                logger.debug(msg)
                 check = False  # We do not match
             else:
                 msg = (
                     f'MATCH: Value for key "{value}", health check output: '
                     f'{output[key]}'
                 )
-                self.logger.debug(msg)
+                logger.debug(msg)
         if check:
-            self.logger.debug('Health check for action %s passed.', self.action)
+            logger.debug('Health check for action %s passed.', self.action)
         return check
 
     @property
     def getcheckid(self) -> t.AnyStr:
         retval = None
         if self.action in self.RELO_ACTIONS:
             retval = 'check for cluster health to show zero relocating shards'
```

### Comparing `es_wait-0.5.0/src/es_wait/ilm.py` & `es_wait-0.5.1/src/es_wait/ilm.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 from elasticsearch8.exceptions import NotFoundError
 from ._base import Waiter
 from .exceptions import IlmWaitError
 
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
+logger = logging.getLogger('es_wait.IndexLifecycle')
+
 # pylint: disable=R0913
 
 
 class IndexLifecycle(Waiter):
     """ILM Step and Phase Parent Class"""
 
     def __init__(
         self,
         client: 'Elasticsearch',
         pause: float = 1,
         timeout: float = -1,
         name: t.Union[str, None] = None,
     ) -> None:
-        self.logger = logging.getLogger('es_wait.IndexLifecycle')
+
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.name = name
         self.empty_check('name')
 
     def get_explain_data(self) -> t.Union[t.Dict, None]:
         """
         Calls `client.indices.`
@@ -35,27 +37,27 @@
         name and returns the resulting response.
         """
         try:
             # The use of filter_path reduces the result set size
             kw = {'index': self.name, 'filter_path': f'indices.{self.name}'}
             # retval = self.client.ilm.explain_lifecycle(**kw)['indices'][self.name]
             resp = self.client.ilm.explain_lifecycle(**kw)
-            self.logger.debug('response: %s', resp)
+            logger.debug('response: %s', resp)
 
         except NotFoundError as exc:
             msg = (
                 f'Datastream/Index Name changed. {self.name} was not found. '
                 f'This is likely due to the index name suddenly changing, as with '
                 f'searchable snapshot mounts.'
             )
-            self.logger.error(msg)
+            logger.error(msg)
             raise exc  # re-raise the original. Just wanted to log here.
         except Exception as err:
             msg = f'Unable to get ILM information for index {self.name}'
-            self.logger.critical(msg)
+            logger.critical(msg)
             raise IlmWaitError(f'{msg}. Exception: {err}') from err
         retval = resp['indices'][self.name]
         return retval
 
 
 class IlmPhase(IndexLifecycle):
     """
```

### Comparing `es_wait-0.5.0/src/es_wait/relocate.py` & `es_wait-0.5.1/src/es_wait/relocate.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 import typing as t
 import logging
 from ._base import Waiter
 
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
+logger = logging.getLogger('es_wait.Relocate')
+
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class Relocate(Waiter):
 
     def __init__(
         self,
         client: 'Elasticsearch',
         pause: float = 9,
         timeout: float = -1,
         name: str = None,
     ) -> None:
-        self.logger = logging.getLogger('es_wait.Relocate')
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.name = name
         self.empty_check('name')
         self.checkid = f'check for the {self.name} index relocation process to complete'
 
     @property
     def check(self) -> bool:
@@ -32,15 +33,15 @@
         :py:meth:`~.elasticsearch.client.ClusterClient.state` with a given index to
         check if all of the shards for that index are in the ``STARTED`` state. It will
         return ``True`` if all primary and replica shards are in the ``STARTED`` state,
         and it will return ``False`` if any shard is in a different state.
         """
         finished = self.finished_state
         if finished:
-            self.logger.debug('Relocate Check for index: "%s" has passed.', self.name)
+            logger.debug('Relocate Check for index: "%s" has passed.', self.name)
         return finished
 
     @property
     def finished_state(self) -> bool:
         """
         Return the boolean state of whether all shards in the index are 'STARTED'
 
@@ -64,14 +65,14 @@
             #         "indices": {
             #         "SELF.NAME": {
             #             "shards": {
             #             "0": [
             #                   {
             #                    "state": "SHARD_STATE",
         except Exception as exc:
-            self.logger.critical(msg)
+            logger.critical(msg)
             raise ValueError(msg) from exc
         try:
             return result['routing_table']['indices'][self.name]['shards']
         except KeyError as err:
-            self.logger.critical(msg)
+            logger.critical(msg)
             raise KeyError(msg) from err
```

### Comparing `es_wait-0.5.0/src/es_wait/restore.py` & `es_wait-0.5.1/src/es_wait/restore.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 import typing as t
 import logging
 from ._base import Waiter
 
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
+logger = logging.getLogger('es_wait.Restore')
+
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class Restore(Waiter):
     """Restore Waiter class"""
 
     def __init__(
         self,
         client: 'Elasticsearch',
         pause: float = 9,
         timeout: float = -1,
         index_list: t.Sequence[str] = None,
     ) -> None:
-        self.logger = logging.getLogger('es_wait.Restore')
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.index_list = index_list
         self.empty_check('index_list')
         self.checkid = 'check for completion of index_list restoration from snapshot'
 
     @property
     def check(self) -> bool:
@@ -37,21 +38,19 @@
         it will immediately return ``False``, rather than complete iterating over the
         rest of the response.
         """
         response = {}
         for chunk in self.index_list_chunks:
             chunk_response = self.get_recovery(chunk)
             if chunk_response == {}:
-                self.logger.debug(
-                    '_recovery API returned an empty response. Trying again.'
-                )
+                logger.debug('_recovery API returned an empty response. Trying again.')
                 return False
             response.update(chunk_response)
-        self.logger.debug('Provided indices: %s', self.index_list)
-        self.logger.debug('Found indices: %s', list(response.keys()))
+        logger.debug('Provided indices: %s', self.index_list)
+        logger.debug('Found indices: %s', list(response.keys()))
         for index, data in response.items():
             for shard in data['shards']:
                 stage = shard['stage']
                 if stage != 'DONE':
                     print(f'Index {index} is still in stage {stage}')
                     return False
```

### Comparing `es_wait-0.5.0/src/es_wait/snapshot.py` & `es_wait-0.5.1/src/es_wait/snapshot.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 import typing as t
 import logging
 from ._base import Waiter
 
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
+logger = logging.getLogger('es_wait.Snapshot')
+
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class Snapshot(Waiter):
     ACTIONS: t.Optional[str] = None
 
     def __init__(
         self,
         client: 'Elasticsearch',
         pause: float = 9,
         timeout: float = -1,
         snapshot: str = None,
         repository: str = None,
     ) -> None:
-        self.logger = logging.getLogger('es_wait.Snapshot')
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.snapshot = snapshot
         self.repository = repository
         self.empty_check('snapshot')
         self.empty_check('repository')
         self.checkid = f'check for snapshot {self.snapshot} completion'
 
@@ -60,18 +61,14 @@
                 f'Unable to obtain information for snapshot "{self.snapshot}" in '
                 f'repository "{self.repository}". Error: {err}'
             ) from err
         return result
 
     def log_completion(self, state: str) -> None:
         if state == 'SUCCESS':
-            self.logger.info('Snapshot %s successfully completed.', self.snapshot)
+            logger.info('Snapshot %s successfully completed.', self.snapshot)
         elif state == 'PARTIAL':
-            self.logger.warning(
-                'Snapshot %s completed with state PARTIAL.', self.snapshot
-            )
+            logger.warning('Snapshot %s completed with state PARTIAL.', self.snapshot)
         elif state == 'FAILED':
-            self.logger.error('Snapshot %s completed with state FAILED.', self.snapshot)
+            logger.error('Snapshot %s completed with state FAILED.', self.snapshot)
         else:
-            self.logger.warning(
-                'Snapshot %s completed with state: %s', self.snapshot, state
-            )
+            logger.warning('Snapshot %s completed with state: %s', self.snapshot, state)
```

### Comparing `es_wait-0.5.0/src/es_wait/task.py` & `es_wait-0.5.1/src/es_wait/task.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 from ._base import Waiter
 
 # from .args import TaskArgs
 
 if t.TYPE_CHECKING:
     from elasticsearch8 import Elasticsearch
 
+logger = logging.getLogger('es_wait.Task')
+
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class Task(Waiter):
     ACTIONS = ['forcemerge', 'reindex', 'update_by_query']
 
     def __init__(
         self,
         client: 'Elasticsearch',
         pause: float = 9,
         timeout: float = -1,
         action: t.Literal['forcemerge', 'reindex', 'update_by_query'] = None,
         task_id: str = None,
     ) -> None:
-        self.logger = logging.getLogger('es_wait.Task')
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.action = action
         self.task_id = task_id
         self.empty_check('action')
         self.empty_check('task_id')
         self.task_data = None
         self.task = None
@@ -67,43 +68,41 @@
             raise ValueError(msg) from err
         self.task = self.task_data.task
         self.reindex_check()
         return self.task_complete
 
     def reindex_check(self) -> None:
         if self.task.action == 'indices:data/write/reindex':
-            self.logger.debug("It's a REINDEX task")
-            self.logger.debug('TASK_DATA: %s', self.task_data.toDict())
-            self.logger.debug(
-                'TASK_DATA keys: %s', list(self.task_data.toDict().keys())
-            )
+            logger.debug("It's a REINDEX task")
+            logger.debug('TASK_DATA: %s', self.task_data.toDict())
+            logger.debug('TASK_DATA keys: %s', list(self.task_data.toDict().keys()))
             if self.task_data.response.failures:
                 if len(self.task_data.response.failures) > 0:
                     msg = (
                         f'Failures found in the {self.action} response: '
                         f'{self.task_data.response["failures"]}'
                     )
                     raise ValueError(msg)
 
     @property
     def task_complete(self) -> bool:
         running_time = 0.000000001 * self.task.running_time_in_nanos
-        self.logger.debug('Running time: %s seconds', running_time)
+        logger.debug('Running time: %s seconds', running_time)
         if self.task_data.completed:
             completion_time = (running_time * 1000) + self.task['start_time_in_millis']
             time_string = strftime(
                 '%Y-%m-%dT%H:%M:%S', localtime(completion_time / 1000)
             )
-            self.logger.debug(
+            logger.debug(
                 'Task "%s" completed at %s.', self.task.description, time_string
             )
             retval = True
         else:
             # Log the task status here.
-            self.logger.debug('Full Task Data: %s', self.task_data.asdict)
+            logger.debug('Full Task Data: %s', self.task_data.asdict)
             msg = (
                 f'Task "{self.task.description}" with task_id "{self.task_id}" has '
                 f'been running for {running_time} seconds'
             )
-            self.logger.debug(msg)
+            logger.debug(msg)
             retval = False
         return retval
```

### Comparing `es_wait-0.5.0/.gitignore` & `es_wait-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.0/LICENSE` & `es_wait-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.0/pyproject.toml` & `es_wait-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.0/PKG-INFO` & `es_wait-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.5.0
+Version: 0.5.1
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```

