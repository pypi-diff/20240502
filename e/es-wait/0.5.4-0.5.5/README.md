# Comparing `tmp/es_wait-0.5.4.tar.gz` & `tmp/es_wait-0.5.5.tar.gz`

## Comparing `es_wait-0.5.4.tar` & `es_wait-0.5.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.4/.coveragerc
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/__init__.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/_base.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/exceptions.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/exists.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/health.py
--rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/ilm.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/restore.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 es_wait-0.5.4/src/es_wait/task.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.4/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.4/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.4/README.md
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 es_wait-0.5.5/.coveragerc
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/_base.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/exceptions.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/health.py
+-rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/ilm.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 es_wait-0.5.5/src/es_wait/task.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 es_wait-0.5.5/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.5.5/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.5.5/README.md
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 es_wait-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 es_wait-0.5.5/PKG-INFO
```

### Comparing `es_wait-0.5.4/src/es_wait/_base.py` & `es_wait-0.5.5/src/es_wait/_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         client: 'Elasticsearch',
         pause: float = 9,  # The delay between checks
         timeout: float = -1,  # How long is too long
     ) -> None:
         self.client = client
         self.pause = pause
         self.timeout = timeout
-        self.checkid = 'check for Waiter class'
+        self.waitstr = 'for Waiter class to initialize'
 
     @property
     def now(self) -> datetime:
         """Return the 'now' datetime"""
         return datetime.now(timezone.utc)
 
     @property
@@ -83,36 +83,36 @@
             if elapsed == 0:
                 loggit = False
             else:
                 loggit = elapsed % frequency == 0  # Only frequency seconds
             response = self.check
             # Successfully completed task.
             if response:
-                logger.debug('%s finished executing', self.checkid)
+                logger.debug('The wait %s is over.', self.waitstr)
                 total = f'{(self.now - start_time).total_seconds():.2f}'
                 logger.debug('Elapsed time: %s seconds', total)
                 success = True
                 break
             # Not success, and reached timeout (if defined)
             if (self.timeout != -1) and (elapsed >= self.timeout):
                 msg = (
-                    f'The {self.checkid} did not complete within {self.timeout} '
+                    f'The {self.waitstr} did not complete within {self.timeout} '
                     f'seconds.'
                 )
                 logger.error(msg)
                 break
             # Not timed out and not yet success, so we wait.
             if loggit:
                 msg = (
-                    f'The {self.checkid} is not yet complete. {elapsed} total seconds '
+                    f'The wait {self.waitstr} is ongoing. {elapsed} total seconds '
                     f'have elapsed. Pausing {self.pause} seconds between checks.'
                 )
                 logger.debug(msg)
             sleep(self.pause)  # Actual wait here
 
         if not success:
             msg = (
-                f'The {self.checkid} failed to complete in the timeout period of '
+                f'The wait {self.waitstr} failed to complete in the timeout period of '
                 f'{self.timeout} seconds'
             )
             logger.error(msg)
             raise TimeoutError(msg)
```

### Comparing `es_wait-0.5.4/src/es_wait/exists.py` & `es_wait-0.5.5/src/es_wait/exists.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ) -> None:
 
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.name = name
         self.kind = kind
         self.empty_check('name')
         self.empty_check('kind')
-        self.checkid = f'check for {self.kindmap} {name} to exist'
+        self.waitstr = f'for {self.kindmap} "{name}" to exist'
 
     @property
     def check(self) -> bool:
         """
         Check if the named entity exists, based on kind
         """
         doit = {
```

### Comparing `es_wait-0.5.4/src/es_wait/health.py` & `es_wait-0.5.5/src/es_wait/health.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         action: t.Literal[
             'allocation', 'cluster_routing', 'mount', 'replicas', 'shrink'
         ] = None,
     ) -> None:
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.action = action
         self.empty_check('action')
-        self.checkid = self.getcheckid
+        self.waitstr = self.getwaitstr
 
     def argmap(self) -> t.Union[t.Dict[str, int], t.Dict[str, str]]:
         """This is a little way to ensure many possibilities come down to one"""
         if self.action in self.RELO_ACTIONS:
             return self.RELO_ARGS
         if self.action in self.STATUS_ACTIONS:
             return self.STATUS_ARGS
@@ -75,14 +75,14 @@
                 )
                 logger.debug(msg)
         if check:
             logger.debug('Health check for action %s passed.', self.action)
         return check
 
     @property
-    def getcheckid(self) -> t.AnyStr:
+    def getwaitstr(self) -> t.AnyStr:
         retval = None
         if self.action in self.RELO_ACTIONS:
-            retval = 'check for cluster health to show zero relocating shards'
+            retval = 'for cluster health to show zero relocating shards'
         if self.action in self.STATUS_ACTIONS:
-            retval = 'check for cluster health to show green status'
+            retval = 'for cluster health to show green status'
         return retval
```

### Comparing `es_wait-0.5.4/src/es_wait/ilm.py` & `es_wait-0.5.5/src/es_wait/ilm.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,17 +71,16 @@
         name: t.Union[str, None] = None,
         phase: t.Union[str, None] = None,
     ) -> None:
         self.logger = logging.getLogger('es_wait.IlmPhase')
         super().__init__(client=client, pause=pause, timeout=timeout, name=name)
         self.phase = phase
         self.empty_check('phase')
-        self.checkid = (
-            f'check for completion of ILM transition for {self.name} to '
-            f'phase "{self.phase}"'
+        self.waitstr = (
+            f'for "{self.name}" to complete ILM transition to phase "{self.phase}"'
         )
 
     @property
     def check(self) -> bool:
         """
         Check for ILM phase change completion.  It will return ``True`` if the expected
         phase and the actually collected phase match.
@@ -110,15 +109,15 @@
         client: 'Elasticsearch',
         pause: float = 1,
         timeout: float = -1,
         name: t.Union[str, None] = None,
     ) -> None:
         self.logger = logging.getLogger('es_wait.IlmStep')
         super().__init__(client=client, pause=pause, timeout=timeout, name=name)
-        self.checkid = f'check for completion of ILM step for {self.name}'
+        self.waitstr = f'for "{self.name}" to complete the current ILM step'
 
     @property
     def check(self) -> bool:
         """
         Check for ILM step completion.  It will return ``True`` if the step and
         action values are both ``complete``
```

### Comparing `es_wait-0.5.4/src/es_wait/relocate.py` & `es_wait-0.5.5/src/es_wait/relocate.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         pause: float = 9,
         timeout: float = -1,
         name: str = None,
     ) -> None:
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.name = name
         self.empty_check('name')
-        self.checkid = f'check for the {self.name} index relocation process to complete'
+        self.waitstr = f'for index "{self.name}" to finish relocating'
 
     @property
     def check(self) -> bool:
         """
         This function calls `client.cluster.`
         :py:meth:`~.elasticsearch.client.ClusterClient.state` with a given index to
         check if all of the shards for that index are in the ``STARTED`` state. It will
```

### Comparing `es_wait-0.5.4/src/es_wait/restore.py` & `es_wait-0.5.5/src/es_wait/restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         pause: float = 9,
         timeout: float = -1,
         index_list: t.Sequence[str] = None,
     ) -> None:
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.index_list = index_list
         self.empty_check('index_list')
-        self.checkid = 'check for completion of index_list restoration from snapshot'
+        self.waitstr = 'for indices in index_list to be restored from snapshot'
 
     @property
     def check(self) -> bool:
         """
         Calls `client.indices.`
         :py:meth:`~.elasticsearch.client.IndicesClient.recovery` with a list of indices
         to check for complete recovery.  It will return ``True`` if recovery of those
```

### Comparing `es_wait-0.5.4/src/es_wait/snapshot.py` & `es_wait-0.5.5/src/es_wait/snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         repository: str = None,
     ) -> None:
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.snapshot = snapshot
         self.repository = repository
         self.empty_check('snapshot')
         self.empty_check('repository')
-        self.checkid = f'check for snapshot {self.snapshot} completion'
+        self.waitstr = f'for snapshot "{self.snapshot}" to complete'
 
     @property
     def check(self) -> bool:
         """
         This function calls `client.snapshot.`
         :py:meth:`~.elasticsearch.client.SnapshotClient.get` and tests to see whether
         the snapshot is complete, and if so, with what status. It will log errors
```

### Comparing `es_wait-0.5.4/src/es_wait/task.py` & `es_wait-0.5.5/src/es_wait/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         super().__init__(client=client, pause=pause, timeout=timeout)
         self.action = action
         self.task_id = task_id
         self.empty_check('action')
         self.empty_check('task_id')
         self.task_data = None
         self.task = None
-        self.checkid = f'check for the {self.action} task to complete'
+        self.waitstr = f'for the "{self.action}" task to complete'
 
     @property
     def check(self) -> bool:
         """
         This function calls `client.tasks.`
         :py:meth:`~.elasticsearch.client.TasksClient.get` with the provided
         ``task_id``.  If the task data contains ``'completed': True``, then it will
```

### Comparing `es_wait-0.5.4/.gitignore` & `es_wait-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.4/LICENSE` & `es_wait-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.4/pyproject.toml` & `es_wait-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `es_wait-0.5.4/PKG-INFO` & `es_wait-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.5.4
+Version: 0.5.5
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```

