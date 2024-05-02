# Comparing `tmp/es_wait-0.3.5.tar.gz` & `tmp/es_wait-0.5.0.tar.gz`

## Comparing `es_wait-0.3.5.tar` & `es_wait-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.3.5/pytest.ini
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/__init__.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/args.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/base.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/exists.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/health.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/restore.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 es_wait-0.3.5/src/es_wait/task.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.3.5/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.3.5/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.3.5/README.md
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 es_wait-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.0/.coveragerc
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/_base.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/exceptions.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/health.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/ilm.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 es_wait-0.5.0/src/es_wait/task.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.0/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.0/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.0/README.md
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.0/PKG-INFO
```

### Comparing `es_wait-0.3.5/src/es_wait/base.py` & `es_wait-0.5.0/src/es_wait/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 """Base Waiter Class"""
 
 import typing as t
 import logging
 from time import sleep
 from datetime import datetime, timezone
-from elasticsearch8 import Elasticsearch
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
 
 
 class Waiter:
     """Class Definition"""
 
-    ACTIONS = ['any', 'listed', 'actions']
-
     def __init__(
         self,
-        client: Elasticsearch,
-        action: str = '',
+        client: 'Elasticsearch',
         pause: float = 9,  # The delay between checks
         timeout: float = -1,  # How long is too long
     ) -> None:
         self.logger = logging.getLogger('es_wait.Base')
         self.client = client
-        self.action = action
         self.pause = pause
         self.timeout = timeout
         self.checkid = 'check for Waiter class'
 
     @property
-    def acceptable(self) -> t.Union[str, t.Sequence[str]]:
-        """Return acceptable actions for this class"""
-        return self.ACTIONS
-
-    @property
     def now(self) -> datetime:
         """Return the 'now' datetime"""
         return datetime.now(timezone.utc)
 
     @property
     def check(self) -> bool:
         """This will need to be redefined by each child class"""
```

### Comparing `es_wait-0.3.5/src/es_wait/exists.py` & `es_wait-0.5.0/src/es_wait/exists.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 """Entity Exists"""
 
 import typing as t
 import logging
-from elasticsearch8 import Elasticsearch
-from .base import Waiter
+from ._base import Waiter
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class Exists(Waiter):
     """Class Definition"""
 
-    IDX_OR_DS = ['index', 'datastream', 'idx', 'ds']
+    IDX_OR_DS = ['index', 'data_stream', 'datastream', 'idx', 'ds']
     TEMPLATE = ['index_template', 'template', 'tmpl']
     COMPONENT = ['component_template', 'component', 'comp']
 
     def __init__(
         self,
-        client: Elasticsearch,
-        action: str = '',
+        client: 'Elasticsearch',
         pause: float = 1.5,
         timeout: float = 15,
         name: str = '',
         kind: str = '',
     ) -> None:
-        super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Exists')
+        super().__init__(client=client, pause=pause, timeout=timeout)
         self.name = name
         self.kind = kind
         self.empty_check('name')
         self.empty_check('kind')
         self.checkid = f'check for {self.kindmap} {name} to exist'
 
     @property
     def check(self) -> bool:
         """
         Check if the named entity exists, based on kind
         """
         doit = {
-            'index or datastream': {
+            'index or data_stream': {
                 'func': self.client.indices.exists,
                 'kwargs': {'index': self.name},
             },
             'index template': {
                 'func': self.client.indices.exists_index_template,
                 'kwargs': {'name': self.name},
             },
@@ -58,14 +59,14 @@
     def kindmap(
         self,
     ) -> t.Literal[
         'index or datastream', 'index template', 'component template', 'FAIL'
     ]:
         """This is a little way to ensure many possibilities come down to one"""
         if self.kind in self.IDX_OR_DS:
-            return 'index or datastream'
+            return 'index or data_stream'
         if self.kind in self.TEMPLATE:
             return 'index template'
         if self.kind in self.COMPONENT:
             return 'component template'
         self.logger.error('%s is not an acceptable value for kind', self.kind)
         return 'FAIL'  # We should not see this, like, ever
```

### Comparing `es_wait-0.3.5/src/es_wait/health.py` & `es_wait-0.5.0/src/es_wait/health.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 """Health Check"""
 
 import typing as t
 import logging
-from elasticsearch8 import Elasticsearch
-from .base import Waiter
+from ._base import Waiter
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class Health(Waiter):
     ACTIONS = ['allocation', 'cluster_routing', 'mount', 'replicas', 'shrink']
     RELO_ACTIONS = ['allocation', 'cluster_routing']
     STATUS_ACTIONS = ['mount', 'replicas', 'shrink']
     RELO_ARGS = {'relocating_shards': 0}
     STATUS_ARGS = {'status': 'green'}
 
     def __init__(
         self,
-        client: Elasticsearch,
+        client: 'Elasticsearch',
+        pause: float = 1.5,
+        timeout: float = 15,
         action: t.Literal[
             'allocation', 'cluster_routing', 'mount', 'replicas', 'shrink'
         ] = None,
-        pause: float = 1.5,
-        timeout: float = 15,
     ) -> None:
-        super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Health')
+        super().__init__(client=client, pause=pause, timeout=timeout)
+        self.action = action
         self.empty_check('action')
         self.checkid = self.getcheckid
 
-    @property
     def argmap(self) -> t.Union[t.Dict[str, int], t.Dict[str, str]]:
         """This is a little way to ensure many possibilities come down to one"""
         if self.action in self.RELO_ACTIONS:
             return self.RELO_ARGS
         if self.action in self.STATUS_ACTIONS:
             return self.STATUS_ARGS
         msg = f'{self.action} is not an acceptable value for action'
@@ -48,15 +50,15 @@
         contents of self.argmap, will return ``True`` or ``False`` depending on whether
         that particular keyword appears in the output, and has the expected value.
 
         If multiple keys are provided, all must match for a ``True`` response.
         """
         output = self.client.cluster.health()
         check = True
-        args = self.argmap
+        args = self.argmap()
         for key, value in args.items():
             # First, verify that the key is in output
             if key not in output:
                 raise KeyError(f'Key "{key}" not in cluster health output')
             # Verify that the output matches the expected value
             if output[key] != value:
                 msg = (
@@ -73,12 +75,13 @@
                 self.logger.debug(msg)
         if check:
             self.logger.debug('Health check for action %s passed.', self.action)
         return check
 
     @property
     def getcheckid(self) -> t.AnyStr:
+        retval = None
         if self.action in self.RELO_ACTIONS:
             retval = 'check for cluster health to show zero relocating shards'
         if self.action in self.STATUS_ACTIONS:
             retval = 'check for cluster health to show green status'
         return retval
```

### Comparing `es_wait-0.3.5/src/es_wait/relocate.py` & `es_wait-0.5.0/src/es_wait/relocate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Relocate Check"""
 
 import typing as t
 import logging
-from elasticsearch8 import Elasticsearch
-from .base import Waiter
+from ._base import Waiter
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class Relocate(Waiter):
-    ACTIONS: t.Optional[str] = None
 
     def __init__(
         self,
-        client: Elasticsearch,
-        action: t.Optional[str] = None,
+        client: 'Elasticsearch',
         pause: float = 9,
         timeout: float = -1,
         name: str = None,
     ) -> None:
-        super().__init__(client=client, action=action, pause=pause, timeout=timeout)
-        self.logger = logging.getLogger('es_wait.Health')
+        self.logger = logging.getLogger('es_wait.Relocate')
+        super().__init__(client=client, pause=pause, timeout=timeout)
         self.name = name
         self.empty_check('name')
         self.checkid = f'check for the {self.name} index relocation process to complete'
 
     @property
     def check(self) -> bool:
         """
@@ -37,24 +37,40 @@
         finished = self.finished_state
         if finished:
             self.logger.debug('Relocate Check for index: "%s" has passed.', self.name)
         return finished
 
     @property
     def finished_state(self) -> bool:
+        """
+        Return the boolean state of whether all shards in the index are 'STARTED'
+
+        The all() function returns True if all items in an iterable are true,
+        otherwise it returns False. We use it twice here, nested.
+        """
         return all(
             all(shard['state'] == "STARTED" for shard in shards)
             for shards in self.routing_table.values()
         )
 
     @property
     def routing_table(self) -> t.Dict:
         msg = f'Unable to get routing table data from cluster state for {self.name}'
+        # Using filter_path drastically reduces the result size
+        fpath = f'routing_table.indices.{self.name}'
         try:
-            result = self.client.cluster.state(index=self.name)
+            result = self.client.cluster.state(index=self.name, filter_path=fpath)
+            # {
+            #     "routing_table": {
+            #         "indices": {
+            #         "SELF.NAME": {
+            #             "shards": {
+            #             "0": [
+            #                   {
+            #                    "state": "SHARD_STATE",
         except Exception as exc:
             self.logger.critical(msg)
             raise ValueError(msg) from exc
         try:
             return result['routing_table']['indices'][self.name]['shards']
         except KeyError as err:
             self.logger.critical(msg)
```

### Comparing `es_wait-0.3.5/src/es_wait/restore.py` & `es_wait-0.5.0/src/es_wait/restore.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """Snapshot Restore Check"""
 
 import typing as t
 import logging
-from elasticsearch8 import Elasticsearch
-from .base import Waiter
+from ._base import Waiter
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class Restore(Waiter):
-    ACTIONS: t.Optional[str] = None
+    """Restore Waiter class"""
 
     def __init__(
         self,
-        client: Elasticsearch,
-        action: t.Optional[str] = None,
+        client: 'Elasticsearch',
         pause: float = 9,
         timeout: float = -1,
         index_list: t.Sequence[str] = None,
     ) -> None:
-        super().__init__(client=client, action=action, pause=pause, timeout=timeout)
-        self.logger = logging.getLogger('es_wait.Snapshot')
+        self.logger = logging.getLogger('es_wait.Restore')
+        super().__init__(client=client, pause=pause, timeout=timeout)
         self.index_list = index_list
         self.empty_check('index_list')
         self.checkid = 'check for completion of index_list restoration from snapshot'
 
     @property
     def check(self) -> bool:
         """
@@ -48,14 +49,15 @@
         self.logger.debug('Provided indices: %s', self.index_list)
         self.logger.debug('Found indices: %s', list(response.keys()))
         for index, data in response.items():
             for shard in data['shards']:
                 stage = shard['stage']
                 if stage != 'DONE':
                     print(f'Index {index} is still in stage {stage}')
+                    return False
 
         # If we've gotten here, all of the indices have recovered
         return True
 
     @property
     def index_list_chunks(self) -> t.Sequence[t.Sequence[t.AnyStr]]:
         """
@@ -74,14 +76,15 @@
             else:
                 chunks.append(chunk.split(','))
                 chunk = index
         chunks.append(chunk.split(','))
         return chunks
 
     def get_recovery(self, chunk: t.Sequence[str]) -> t.Dict:
+        """Get recovery information from Elasticsearch"""
         try:
             chunk_response = self.client.indices.recovery(index=chunk, human=True)
         except Exception as err:
             msg = (
                 f'Unable to obtain recovery information for specified indices. Error: '
                 f'{err}'
             )
```

### Comparing `es_wait-0.3.5/src/es_wait/snapshot.py` & `es_wait-0.5.0/src/es_wait/snapshot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """Snapshot Check"""
 
 import typing as t
 import logging
-from elasticsearch8 import Elasticsearch
-from .base import Waiter
+from ._base import Waiter
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class Snapshot(Waiter):
     ACTIONS: t.Optional[str] = None
 
     def __init__(
         self,
-        client: Elasticsearch,
-        action: t.Optional[str] = None,
+        client: 'Elasticsearch',
         pause: float = 9,
         timeout: float = -1,
         snapshot: str = None,
         repository: str = None,
     ) -> None:
-        super().__init__(client=client, action=action, pause=pause, timeout=timeout)
         self.logger = logging.getLogger('es_wait.Snapshot')
+        super().__init__(client=client, pause=pause, timeout=timeout)
         self.snapshot = snapshot
         self.repository = repository
         self.empty_check('snapshot')
         self.empty_check('repository')
         self.checkid = f'check for snapshot {self.snapshot} completion'
 
     @property
```

### Comparing `es_wait-0.3.5/src/es_wait/task.py` & `es_wait-0.5.0/src/es_wait/task.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,89 @@
 """Task Check"""
 
 import typing as t
 import logging
 from time import localtime, strftime
-from elasticsearch8 import Elasticsearch
-from .base import Waiter
-from .args import TaskArgs
+from dotmap import DotMap
+from ._base import Waiter
+
+# from .args import TaskArgs
+
+if t.TYPE_CHECKING:
+    from elasticsearch8 import Elasticsearch
 
 # pylint: disable=missing-docstring,too-many-arguments
 
 
 class Task(Waiter):
     ACTIONS = ['forcemerge', 'reindex', 'update_by_query']
 
     def __init__(
         self,
-        client: Elasticsearch,
-        action: t.Literal['forcemerge', 'reindex', 'update_by_query'] = None,
+        client: 'Elasticsearch',
         pause: float = 9,
         timeout: float = -1,
+        action: t.Literal['forcemerge', 'reindex', 'update_by_query'] = None,
         task_id: str = None,
     ) -> None:
-        super().__init__(client=client, action=action, pause=pause, timeout=timeout)
-        self.logger = logging.getLogger('es_wait.Health')
+        self.logger = logging.getLogger('es_wait.Task')
+        super().__init__(client=client, pause=pause, timeout=timeout)
+        self.action = action
         self.task_id = task_id
-        self.empty_check(task_id)
+        self.empty_check('action')
+        self.empty_check('task_id')
         self.task_data = None
         self.task = None
         self.checkid = f'check for the {self.action} task to complete'
 
     @property
     def check(self) -> bool:
         """
         This function calls `client.tasks.`
         :py:meth:`~.elasticsearch.client.TasksClient.get` with the provided
         ``task_id``.  If the task data contains ``'completed': True``, then it will
         return ``True``. If the task is not completed, it will log some information
         about the task and return ``False``
         """
+        # The properties for TaskArgs
+        # TASK_DATA
+        # self.task_data.response = {}
+        # self.task_data.completed = False
+        # self.task_data.task = {} -> Becomes TASK
+        # TASK
+        # self.task.action = str
+        # self.task.description = str
+        # self.task.running_time_in_nanos = 0
+
         try:
-            self.task_data = TaskArgs(
-                settings=self.client.tasks.get(task_id=self.task_id)
-            )
+            # self.task_data = TaskArgs(
+            #     settings=self.client.tasks.get(task_id=self.task_id)
+            # )
+            self.task_data = DotMap(self.client.tasks.get(task_id=self.task_id))
         except Exception as err:
             msg = (
                 f'Unable to obtain task information for task_id "{self.task_id}". '
                 f'Exception {err}'
             )
             raise ValueError(msg) from err
-        self.task = TaskArgs(settings=self.task_data.task)
+        self.task = self.task_data.task
         self.reindex_check()
         return self.task_complete
 
     def reindex_check(self) -> None:
         if self.task.action == 'indices:data/write/reindex':
             self.logger.debug("It's a REINDEX task")
-            self.logger.debug('TASK_DATA: %s', self.task_data.asdict)
-            self.logger.debug('TASK_DATA keys: %s', list(self.task_data.asdict.keys()))
-            if self.task_data.response:
-                if 'failures' in self.task_data.response:
+            self.logger.debug('TASK_DATA: %s', self.task_data.toDict())
+            self.logger.debug(
+                'TASK_DATA keys: %s', list(self.task_data.toDict().keys())
+            )
+            if self.task_data.response.failures:
+                if len(self.task_data.response.failures) > 0:
                     msg = (
-                        f'Failures found in reindex response: '
+                        f'Failures found in the {self.action} response: '
                         f'{self.task_data.response["failures"]}'
                     )
                     raise ValueError(msg)
 
     @property
     def task_complete(self) -> bool:
         running_time = 0.000000001 * self.task.running_time_in_nanos
```

### Comparing `es_wait-0.3.5/.gitignore` & `es_wait-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.3.5/LICENSE` & `es_wait-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.3.5/PKG-INFO` & `es_wait-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.3.5
+Version: 0.5.0
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
@@ -16,19 +16,21 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: elasticsearch>=8.12.0
+Requires-Dist: dotmap==1.3.30
+Requires-Dist: elasticsearch8>=8.13.0
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == 'doc'
 Requires-Dist: sphinx-rtd-theme; extra == 'doc'
 Provides-Extra: test
+Requires-Dist: es-client==8.13.4; extra == 'test'
 Requires-Dist: mock; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=7.2.1; extra == 'test'
 Requires-Dist: requests; extra == 'test'
 Description-Content-Type: text/markdown
 
 # es-wait
```

