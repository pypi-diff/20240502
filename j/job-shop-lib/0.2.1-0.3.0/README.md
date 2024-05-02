# Comparing `tmp/job_shop_lib-0.2.1.tar.gz` & `tmp/job_shop_lib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "job_shop_lib-0.2.1.tar", max compression
+gzip compressed data, was "job_shop_lib-0.3.0.tar", max compression
```

## Comparing `job_shop_lib-0.2.1.tar` & `job_shop_lib-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1069 2024-02-06 16:50:21.344036 job_shop_lib-0.2.1/LICENSE
--rw-r--r--   0        0        0    11817 2024-04-24 20:06:27.816437 job_shop_lib-0.2.1/README.md
--rw-r--r--   0        0        0      581 2024-04-17 18:49:25.563004 job_shop_lib-0.2.1/job_shop_lib/__init__.py
--rw-r--r--   0        0        0     1368 2024-04-17 18:49:22.658989 job_shop_lib-0.2.1/job_shop_lib/base_solver.py
--rw-r--r--   0        0        0     3354 2024-04-17 18:29:10.381234 job_shop_lib-0.2.1/job_shop_lib/benchmarking/__init__.py
--rw-r--r--   0        0        0   464841 2024-03-01 17:52:19.596032 job_shop_lib-0.2.1/job_shop_lib/benchmarking/benchmark_instances.json
--rw-r--r--   0        0        0     5625 2024-04-13 15:45:21.680914 job_shop_lib-0.2.1/job_shop_lib/benchmarking/load_benchmark.py
--rw-r--r--   0        0        0       97 2024-04-13 17:42:22.701917 job_shop_lib-0.2.1/job_shop_lib/cp_sat/__init__.py
--rw-r--r--   0        0        0     8130 2024-04-17 18:26:23.704578 job_shop_lib-0.2.1/job_shop_lib/cp_sat/ortools_solver.py
--rw-r--r--   0        0        0     1432 2024-04-17 18:51:16.107562 job_shop_lib-0.2.1/job_shop_lib/dispatching/__init__.py
--rw-r--r--   0        0        0    10135 2024-04-17 18:40:15.600273 job_shop_lib-0.2.1/job_shop_lib/dispatching/dispatcher.py
--rw-r--r--   0        0        0     4392 2024-04-17 18:50:15.491255 job_shop_lib-0.2.1/job_shop_lib/dispatching/dispatching_rule_solver.py
--rw-r--r--   0        0        0     5557 2024-04-17 14:11:05.549956 job_shop_lib-0.2.1/job_shop_lib/dispatching/dispatching_rules.py
--rw-r--r--   0        0        0     7267 2024-04-17 18:36:42.623252 job_shop_lib-0.2.1/job_shop_lib/dispatching/factories.py
--rw-r--r--   0        0        0     4378 2024-04-17 14:09:16.084490 job_shop_lib-0.2.1/job_shop_lib/dispatching/pruning_functions.py
--rw-r--r--   0        0        0      899 2024-04-16 16:26:15.416010 job_shop_lib-0.2.1/job_shop_lib/exceptions.py
--rw-r--r--   0        0        0      154 2024-04-17 18:37:08.259373 job_shop_lib-0.2.1/job_shop_lib/generators/__init__.py
--rw-r--r--   0        0        0     7533 2024-04-17 18:37:26.163458 job_shop_lib-0.2.1/job_shop_lib/generators/basic_generator.py
--rw-r--r--   0        0        0     5290 2024-04-24 20:22:00.457532 job_shop_lib-0.2.1/job_shop_lib/generators/transformations.py
--rw-r--r--   0        0        0     1454 2024-04-17 18:38:06.339650 job_shop_lib-0.2.1/job_shop_lib/graphs/__init__.py
--rw-r--r--   0        0        0     7128 2024-04-02 19:34:54.999808 job_shop_lib-0.2.1/job_shop_lib/graphs/build_agent_task_graph.py
--rw-r--r--   0        0        0     2877 2024-04-17 18:51:04.799505 job_shop_lib-0.2.1/job_shop_lib/graphs/build_disjunctive_graph.py
--rw-r--r--   0        0        0      374 2024-03-27 15:56:38.467324 job_shop_lib-0.2.1/job_shop_lib/graphs/constants.py
--rw-r--r--   0        0        0     6229 2024-04-25 12:04:33.212307 job_shop_lib-0.2.1/job_shop_lib/graphs/job_shop_graph.py
--rw-r--r--   0        0        0     4880 2024-03-28 10:18:53.973376 job_shop_lib-0.2.1/job_shop_lib/graphs/node.py
--rw-r--r--   0        0        0    12801 2024-04-03 10:47:39.697352 job_shop_lib-0.2.1/job_shop_lib/job_shop_instance.py
--rw-r--r--   0        0        0     3862 2024-04-06 19:26:36.742129 job_shop_lib-0.2.1/job_shop_lib/operation.py
--rw-r--r--   0        0        0     6509 2024-04-11 17:06:21.882095 job_shop_lib-0.2.1/job_shop_lib/schedule.py
--rw-r--r--   0        0        0     3127 2024-04-11 17:12:11.243224 job_shop_lib-0.2.1/job_shop_lib/scheduled_operation.py
--rw-r--r--   0        0        0      693 2024-04-17 18:46:13.614040 job_shop_lib-0.2.1/job_shop_lib/visualization/__init__.py
--rw-r--r--   0        0        0     8284 2024-04-03 10:47:25.781302 job_shop_lib-0.2.1/job_shop_lib/visualization/agent_task_graph.py
--rw-r--r--   0        0        0     6382 2024-04-17 18:51:20.995586 job_shop_lib-0.2.1/job_shop_lib/visualization/create_gif.py
--rw-r--r--   0        0        0     5803 2024-04-17 18:49:29.543024 job_shop_lib-0.2.1/job_shop_lib/visualization/disjunctive_graph.py
--rw-r--r--   0        0        0     4415 2024-04-17 18:52:22.519817 job_shop_lib-0.2.1/job_shop_lib/visualization/gantt_chart.py
--rw-r--r--   0        0        0     1352 2024-04-25 12:08:01.950791 job_shop_lib-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    12624 1970-01-01 00:00:00.000000 job_shop_lib-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-02-06 16:50:21.344036 job_shop_lib-0.3.0/LICENSE
+-rw-r--r--   0        0        0    11817 2024-04-24 20:06:27.816437 job_shop_lib-0.3.0/README.md
+-rw-r--r--   0        0        0      582 2024-05-02 11:40:12.230468 job_shop_lib-0.3.0/job_shop_lib/__init__.py
+-rw-r--r--   0        0        0     1368 2024-04-17 18:49:22.658989 job_shop_lib-0.3.0/job_shop_lib/base_solver.py
+-rw-r--r--   0        0        0     3354 2024-04-17 18:29:10.381234 job_shop_lib-0.3.0/job_shop_lib/benchmarking/__init__.py
+-rw-r--r--   0        0        0   464841 2024-03-01 17:52:19.596032 job_shop_lib-0.3.0/job_shop_lib/benchmarking/benchmark_instances.json
+-rw-r--r--   0        0        0     5625 2024-04-13 15:45:21.680914 job_shop_lib-0.3.0/job_shop_lib/benchmarking/load_benchmark.py
+-rw-r--r--   0        0        0       97 2024-04-13 17:42:22.701917 job_shop_lib-0.3.0/job_shop_lib/cp_sat/__init__.py
+-rw-r--r--   0        0        0     8130 2024-04-17 18:26:23.704578 job_shop_lib-0.3.0/job_shop_lib/cp_sat/ortools_solver.py
+-rw-r--r--   0        0        0     1568 2024-05-02 11:40:12.230468 job_shop_lib-0.3.0/job_shop_lib/dispatching/__init__.py
+-rw-r--r--   0        0        0    12582 2024-05-02 11:40:12.230468 job_shop_lib-0.3.0/job_shop_lib/dispatching/dispatcher.py
+-rw-r--r--   0        0        0     4669 2024-05-02 11:40:12.230468 job_shop_lib-0.3.0/job_shop_lib/dispatching/dispatching_rule_solver.py
+-rw-r--r--   0        0        0     5557 2024-04-17 14:11:05.549956 job_shop_lib-0.3.0/job_shop_lib/dispatching/dispatching_rules.py
+-rw-r--r--   0        0        0     7267 2024-04-17 18:36:42.623252 job_shop_lib-0.3.0/job_shop_lib/dispatching/factories.py
+-rw-r--r--   0        0        0      649 2024-05-02 11:40:12.230468 job_shop_lib-0.3.0/job_shop_lib/dispatching/history_tracker.py
+-rw-r--r--   0        0        0     4378 2024-04-27 08:34:21.170127 job_shop_lib-0.3.0/job_shop_lib/dispatching/pruning_functions.py
+-rw-r--r--   0        0        0      899 2024-04-16 16:26:15.416010 job_shop_lib-0.3.0/job_shop_lib/exceptions.py
+-rw-r--r--   0        0        0      154 2024-04-17 18:37:08.259373 job_shop_lib-0.3.0/job_shop_lib/generators/__init__.py
+-rw-r--r--   0        0        0     7533 2024-04-17 18:37:26.163458 job_shop_lib-0.3.0/job_shop_lib/generators/basic_generator.py
+-rw-r--r--   0        0        0     5290 2024-04-25 17:39:57.821984 job_shop_lib-0.3.0/job_shop_lib/generators/transformations.py
+-rw-r--r--   0        0        0     1454 2024-04-17 18:38:06.339650 job_shop_lib-0.3.0/job_shop_lib/graphs/__init__.py
+-rw-r--r--   0        0        0     7128 2024-04-02 19:34:54.999808 job_shop_lib-0.3.0/job_shop_lib/graphs/build_agent_task_graph.py
+-rw-r--r--   0        0        0     2877 2024-04-17 18:51:04.799505 job_shop_lib-0.3.0/job_shop_lib/graphs/build_disjunctive_graph.py
+-rw-r--r--   0        0        0      374 2024-03-27 15:56:38.467324 job_shop_lib-0.3.0/job_shop_lib/graphs/constants.py
+-rw-r--r--   0        0        0     7404 2024-05-02 11:40:12.230468 job_shop_lib-0.3.0/job_shop_lib/graphs/job_shop_graph.py
+-rw-r--r--   0        0        0     5613 2024-05-02 11:40:12.230468 job_shop_lib-0.3.0/job_shop_lib/graphs/node.py
+-rw-r--r--   0        0        0    12801 2024-04-03 10:47:39.697352 job_shop_lib-0.3.0/job_shop_lib/job_shop_instance.py
+-rw-r--r--   0        0        0     3924 2024-05-02 11:40:12.230468 job_shop_lib-0.3.0/job_shop_lib/operation.py
+-rw-r--r--   0        0        0     6509 2024-04-11 17:06:21.882095 job_shop_lib-0.3.0/job_shop_lib/schedule.py
+-rw-r--r--   0        0        0     3127 2024-04-11 17:12:11.243224 job_shop_lib-0.3.0/job_shop_lib/scheduled_operation.py
+-rw-r--r--   0        0        0      693 2024-04-17 18:46:13.614040 job_shop_lib-0.3.0/job_shop_lib/visualization/__init__.py
+-rw-r--r--   0        0        0     8284 2024-04-26 16:30:40.546774 job_shop_lib-0.3.0/job_shop_lib/visualization/agent_task_graph.py
+-rw-r--r--   0        0        0     6674 2024-05-02 11:40:12.230468 job_shop_lib-0.3.0/job_shop_lib/visualization/create_gif.py
+-rw-r--r--   0        0        0     5905 2024-05-02 11:40:12.230468 job_shop_lib-0.3.0/job_shop_lib/visualization/disjunctive_graph.py
+-rw-r--r--   0        0        0     4415 2024-04-17 18:52:22.519817 job_shop_lib-0.3.0/job_shop_lib/visualization/gantt_chart.py
+-rw-r--r--   0        0        0     1352 2024-05-02 11:40:12.230468 job_shop_lib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12624 1970-01-01 00:00:00.000000 job_shop_lib-0.3.0/PKG-INFO
```

### Comparing `job_shop_lib-0.2.1/LICENSE` & `job_shop_lib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/README.md` & `job_shop_lib-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/__init__.py` & `job_shop_lib-0.3.0/job_shop_lib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Contains the main data structures and base classes.
 """
 
+from job_shop_lib.exceptions import JobShopLibError, NoSolutionFoundError
 from job_shop_lib.operation import Operation
 from job_shop_lib.job_shop_instance import JobShopInstance
 from job_shop_lib.scheduled_operation import ScheduledOperation
 from job_shop_lib.schedule import Schedule
 from job_shop_lib.base_solver import BaseSolver, Solver
-from job_shop_lib.exceptions import JobShopLibError, NoSolutionFoundError
+
 
 __all__ = [
     "Operation",
     "JobShopInstance",
     "ScheduledOperation",
     "Schedule",
     "Solver",
```

### Comparing `job_shop_lib-0.2.1/job_shop_lib/base_solver.py` & `job_shop_lib-0.3.0/job_shop_lib/base_solver.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/benchmarking/__init__.py` & `job_shop_lib-0.3.0/job_shop_lib/benchmarking/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/benchmarking/benchmark_instances.json` & `job_shop_lib-0.3.0/job_shop_lib/benchmarking/benchmark_instances.json`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/benchmarking/load_benchmark.py` & `job_shop_lib-0.3.0/job_shop_lib/benchmarking/load_benchmark.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/cp_sat/ortools_solver.py` & `job_shop_lib-0.3.0/job_shop_lib/cp_sat/ortools_solver.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/dispatching/__init__.py` & `job_shop_lib-0.3.0/job_shop_lib/dispatching/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Package containing all the functionality to solve the Job Shop Scheduling
 Problem step-by-step."""
 
-from job_shop_lib.dispatching.dispatcher import Dispatcher
+from job_shop_lib.dispatching.dispatcher import Dispatcher, DispatcherObserver
+from job_shop_lib.dispatching.history_tracker import HistoryTracker
 from job_shop_lib.dispatching.dispatching_rules import (
     shortest_processing_time_rule,
     first_come_first_served_rule,
     most_work_remaining_rule,
     most_operations_remaining_rule,
     random_operation_rule,
 )
@@ -42,8 +43,10 @@
     "DispatchingRuleSolver",
     "prune_dominated_operations",
     "prune_non_immediate_machines",
     "create_composite_pruning_function",
     "PruningFunction",
     "pruning_function_factory",
     "composite_pruning_function_factory",
+    "DispatcherObserver",
+    "HistoryTracker",
 ]
```

### Comparing `job_shop_lib-0.2.1/job_shop_lib/dispatching/dispatcher.py` & `job_shop_lib-0.3.0/job_shop_lib/dispatching/dispatcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,143 @@
 """Home of the `Dispatcher` class."""
 
 from __future__ import annotations
 
+import abc
+from typing import Any
 from collections.abc import Callable
 from collections import deque
+from functools import wraps
 
 from job_shop_lib import (
     JobShopInstance,
     Schedule,
     ScheduledOperation,
     Operation,
 )
 
 
+# Added here to avoid circular imports
+class DispatcherObserver(abc.ABC):
+    """Interface for classes that observe the dispatcher."""
+
+    def __init__(self, dispatcher: Dispatcher):
+        """Initializes the observer with the dispatcher and subscribes to
+        it."""
+        self.dispatcher = dispatcher
+        self.dispatcher.subscribe(self)
+
+    @abc.abstractmethod
+    def update(self, scheduled_operation: ScheduledOperation):
+        """Called when an operation is scheduled on a machine."""
+
+    @abc.abstractmethod
+    def reset(self):
+        """Called when the dispatcher is reset."""
+
+    def __str__(self) -> str:
+        return self.__class__.__name__
+
+    def __repr__(self) -> str:
+        return str(self)
+
+
+def _dispatcher_cache(method):
+    """Decorator to cache results of a method based on its name.
+
+    This decorator assumes that the class has an attribute called `_cache`
+    that is a dictionary. It caches the result of the method based on its
+    name. If the result is already cached, it returns the cached result
+    instead of recomputing it.
+
+    The decorator is useful since the dispatcher class can clear the cache
+    when the state of the dispatcher changes.
+    """
+
+    @wraps(method)
+    def wrapper(self: Dispatcher, *args, **kwargs):
+        # pylint: disable=protected-access
+        cache_key = method.__name__
+        cached_result = self._cache.get(cache_key)
+        if cached_result is not None:
+            return cached_result
+
+        result = method(self, *args, **kwargs)
+        self._cache[cache_key] = result
+        return result
+
+    return wrapper
+
+
+# pylint: disable=too-many-instance-attributes
 class Dispatcher:
     """Handles the logic of scheduling operations on machines.
 
     This class allow us to just define the order in which operations are
     sequenced and the machines in which they are processed. It is then
     responsible for scheduling the operations on the machines and keeping
     track of the next available time for each machine and job.
 
     Attributes:
         instance:
             The instance of the job shop problem to be scheduled.
         schedule:
             The schedule of operations on machines.
         pruning_function:
-            The pipeline of pruning methods to be used to filter out
-            operations from the list of available operations.
+            A function that filters out operations that are not ready to be
+            scheduled.
+        subscribers:
+            A list of observers that are subscribed to the dispatcher.
     """
 
     __slots__ = (
         "instance",
         "schedule",
         "_machine_next_available_time",
         "_job_next_operation_index",
         "_job_next_available_time",
         "pruning_function",
+        "subscribers",
+        "_cache",
     )
 
     def __init__(
         self,
         instance: JobShopInstance,
         pruning_function: (
             Callable[[Dispatcher, list[Operation]], list[Operation]] | None
         ) = None,
     ) -> None:
         """Initializes the object with the given instance.
 
         Args:
             instance:
                 The instance of the job shop problem to be solved.
-            pruning_strategies:
-                A list of pruning strategies to be used to filter out
-                operations from the list of available operations. Supported
-                values are 'dominated_operations' and 'non_immediate_machines'.
-                Defaults to [PruningStrategy.DOMINATED_OPERATIONS]. To disable
-                pruning, pass an empty list.
+            pruning_function:
+                A function that filters out operations that are not ready to
+                be scheduled. The function should take the dispatcher and a
+                list of operations as input and return a list of operations
+                that are ready to be scheduled. If `None`, no pruning is done.
         """
 
         self.instance = instance
         self.schedule = Schedule(self.instance)
+        self.pruning_function = pruning_function
+
         self._machine_next_available_time = [0] * self.instance.num_machines
         self._job_next_operation_index = [0] * self.instance.num_jobs
         self._job_next_available_time = [0] * self.instance.num_jobs
-        self.pruning_function = pruning_function
+        self.subscribers: list[DispatcherObserver] = []
+        self._cache: dict[str, Any] = {}
+
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}({self.instance})"
+
+    def __repr__(self) -> str:
+        return str(self)
 
     @property
     def machine_next_available_time(self) -> list[int]:
         """Returns the next available time for each machine."""
         return self._machine_next_available_time
 
     @property
@@ -113,20 +181,31 @@
                     continue
                 operation = operations[0]
                 if dispatcher.is_operation_ready(operation):
                     dispatcher.dispatch(operation, machine_id)
                     operations.popleft()
         return dispatcher.schedule
 
+    def subscribe(self, observer: DispatcherObserver):
+        """Subscribes an observer to the dispatcher."""
+        self.subscribers.append(observer)
+
+    def unsubscribe(self, observer: DispatcherObserver):
+        """Unsubscribes an observer from the dispatcher."""
+        self.subscribers.remove(observer)
+
     def reset(self) -> None:
         """Resets the dispatcher to its initial state."""
         self.schedule.reset()
         self._machine_next_available_time = [0] * self.instance.num_machines
         self._job_next_operation_index = [0] * self.instance.num_jobs
         self._job_next_available_time = [0] * self.instance.num_jobs
+        self._cache = {}
+        for subscriber in self.subscribers:
+            subscriber.reset()
 
     def dispatch(self, operation: Operation, machine_id: int) -> None:
         """Schedules the given operation on the given machine.
 
         The start time of the operation is computed based on the next
         available time for the machine and the next available time for the
         job to which the operation belongs. The operation is then scheduled
@@ -149,121 +228,128 @@
 
         scheduled_operation = ScheduledOperation(
             operation, start_time, machine_id
         )
         self.schedule.add(scheduled_operation)
         self._update_tracking_attributes(scheduled_operation)
 
+        # Notify subscribers
+        for subscriber in self.subscribers:
+            subscriber.update(scheduled_operation)
+
     def is_operation_ready(self, operation: Operation) -> bool:
         """Returns True if the given operation is ready to be scheduled.
 
         An operation is ready to be scheduled if it is the next operation
         to be scheduled for its job.
 
         Args:
             operation:
                 The operation to be checked.
         """
         return (
-            self.job_next_operation_index[operation.job_id]
+            self._job_next_operation_index[operation.job_id]
             == operation.position_in_job
         )
 
-    def start_time(self, operation: Operation, machine_id: int) -> int:
+    def start_time(
+        self,
+        operation: Operation,
+        machine_id: int,
+    ) -> int:
         """Computes the start time for the given operation on the given
         machine.
 
         The start time is the maximum of the next available time for the
         machine and the next available time for the job to which the
         operation belongs.
 
         Args:
             operation:
                 The operation to be scheduled.
             machine_id:
                 The id of the machine on which the operation is to be
-                scheduled.
+                scheduled. If None, the start time is computed based on the
+                next available time for the operation on any machine.
         """
         return max(
-            self.machine_next_available_time[machine_id],
-            self.job_next_available_time[operation.job_id],
+            self._machine_next_available_time[machine_id],
+            self._job_next_available_time[operation.job_id],
         )
 
     def _update_tracking_attributes(
         self, scheduled_operation: ScheduledOperation
     ) -> None:
         # Variables defined here to make the lines shorter
         job_id = scheduled_operation.job_id
         machine_id = scheduled_operation.machine_id
         end_time = scheduled_operation.end_time
 
-        self.machine_next_available_time[machine_id] = end_time
-        self.job_next_operation_index[job_id] += 1
-        self.job_next_available_time[job_id] = end_time
+        self._machine_next_available_time[machine_id] = end_time
+        self._job_next_operation_index[job_id] += 1
+        self._job_next_available_time[job_id] = end_time
+        self._cache = {}
 
+    @_dispatcher_cache
     def current_time(self) -> int:
         """Returns the current time of the schedule.
 
         The current time is the minimum start time of the available
         operations.
         """
         available_operations = self.available_operations()
-        return self.min_start_time(available_operations)
+        current_time = self.min_start_time(available_operations)
+        return current_time
 
     def min_start_time(self, operations: list[Operation]) -> int:
         """Returns the minimum start time of the available operations."""
         if not operations:
             return self.schedule.makespan()
         min_start_time = float("inf")
         for op in operations:
             for machine_id in op.machines:
                 start_time = self.start_time(op, machine_id)
                 min_start_time = min(min_start_time, start_time)
         return int(min_start_time)
 
+    @_dispatcher_cache
     def uncompleted_operations(self) -> list[Operation]:
         """Returns the list of operations that have not been scheduled.
 
         An operation is uncompleted if it has not been scheduled yet.
 
         It is more efficient than checking all operations in the instance.
         """
         uncompleted_operations = []
-        for job_id, next_position in enumerate(self.job_next_operation_index):
+        for job_id, next_position in enumerate(self._job_next_operation_index):
             operations = self.instance.jobs[job_id][next_position:]
             uncompleted_operations.extend(operations)
         return uncompleted_operations
 
+    @_dispatcher_cache
     def available_operations(self) -> list[Operation]:
         """Returns a list of available operations for processing, optionally
-        filtering out operations known to be bad choices.
+        filtering out operations using the pruning function.
 
         This method first gathers all possible next operations from the jobs
-        being processed. It then optionally filters these operations to exclude
-        ones that are deemed inefficient or suboptimal choices.
-
-        An operation is sub-optimal if there is another operation that could
-        be scheduled in the same machine that would finish before the start
-        time of the sub-optimal operation.
+        being processed. It then optionally filters these operations using the
+        pruning function.
 
         Returns:
             A list of Operation objects that are available for scheduling.
-
-        Raises:
-            ValueError: If using the filter_bad_choices option and one of the
-                available operations can be scheduled in more than one machine.
         """
+
         available_operations = self._available_operations()
         if self.pruning_function is not None:
             available_operations = self.pruning_function(
                 self, available_operations
             )
         return available_operations
 
     def _available_operations(self) -> list[Operation]:
         available_operations = []
-        for job_id, next_position in enumerate(self.job_next_operation_index):
+        for job_id, next_position in enumerate(self._job_next_operation_index):
             if next_position == len(self.instance.jobs[job_id]):
                 continue
             operation = self.instance.jobs[job_id][next_position]
             available_operations.append(operation)
         return available_operations
```

### Comparing `job_shop_lib-0.2.1/job_shop_lib/dispatching/dispatching_rule_solver.py` & `job_shop_lib-0.3.0/job_shop_lib/dispatching/dispatching_rule_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,20 +72,23 @@
         if isinstance(pruning_function, str):
             pruning_function = pruning_function_factory(pruning_function)
 
         self.dispatching_rule = dispatching_rule
         self.machine_chooser = machine_chooser
         self.pruning_function = pruning_function
 
-    def solve(self, instance: JobShopInstance) -> Schedule:
+    def solve(
+        self, instance: JobShopInstance, dispatcher: Dispatcher | None = None
+    ) -> Schedule:
         """Returns a schedule for the given job shop instance using the
         dispatching rule algorithm."""
-        dispatcher = Dispatcher(
-            instance, pruning_function=self.pruning_function
-        )
+        if dispatcher is None:
+            dispatcher = Dispatcher(
+                instance, pruning_function=self.pruning_function
+            )
         while not dispatcher.schedule.is_complete():
             self.step(dispatcher)
 
         return dispatcher.schedule
 
     def step(self, dispatcher: Dispatcher) -> None:
         """Executes one step of the dispatching rule algorithm.
@@ -97,15 +100,20 @@
         """
         selected_operation = self.dispatching_rule(dispatcher)
         machine_id = self.machine_chooser(dispatcher, selected_operation)
         dispatcher.dispatch(selected_operation, machine_id)
 
 
 if __name__ == "__main__":
-    import cProfile
+    import time
     from job_shop_lib.benchmarking import load_benchmark_instance
 
     ta_instances = []
     for i in range(1, 81):
         ta_instances.append(load_benchmark_instance(f"ta{i:02d}"))
     solver = DispatchingRuleSolver(dispatching_rule="most_work_remaining")
-    cProfile.run("for instance in ta_instances: solver.solve(instance)")
+    # cProfile.run("for instance in ta_instances: solver.solve(instance)")
+    start = time.perf_counter()
+    for instance_ in ta_instances:
+        solver.solve(instance_)
+    end = time.perf_counter()
+    print(f"Elapsed time: {end - start:.2f} seconds.")
```

### Comparing `job_shop_lib-0.2.1/job_shop_lib/dispatching/dispatching_rules.py` & `job_shop_lib-0.3.0/job_shop_lib/dispatching/dispatching_rules.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/dispatching/factories.py` & `job_shop_lib-0.3.0/job_shop_lib/dispatching/factories.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/dispatching/pruning_functions.py` & `job_shop_lib-0.3.0/job_shop_lib/dispatching/pruning_functions.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/exceptions.py` & `job_shop_lib-0.3.0/job_shop_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/generators/basic_generator.py` & `job_shop_lib-0.3.0/job_shop_lib/generators/basic_generator.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/generators/transformations.py` & `job_shop_lib-0.3.0/job_shop_lib/generators/transformations.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/graphs/__init__.py` & `job_shop_lib-0.3.0/job_shop_lib/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/graphs/build_agent_task_graph.py` & `job_shop_lib-0.3.0/job_shop_lib/graphs/build_agent_task_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/graphs/build_disjunctive_graph.py` & `job_shop_lib-0.3.0/job_shop_lib/graphs/build_disjunctive_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/graphs/job_shop_graph.py` & `job_shop_lib-0.3.0/job_shop_lib/graphs/job_shop_graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Home of the `JobShopGraph` class."""
 
 import collections
 import networkx as nx
 
-from job_shop_lib import JobShopInstance, Operation
+from job_shop_lib import JobShopInstance, JobShopLibError
 from job_shop_lib.graphs import Node, NodeType
 
 
 NODE_ATTR = "node"
 
 
+# pylint: disable=too-many-instance-attributes
 class JobShopGraph:
     """Data structure to represent a `JobShopInstance` as a graph.
 
     Provides a comprehensive graph-based representation of a job shop
     scheduling problem, utilizing the `networkx` library to model the complex
     relationships between jobs, operations, and machines. This class transforms
     the abstract scheduling problem into a directed graph, where various
@@ -26,90 +27,92 @@
     Attributes:
         instance:
             The job shop instance encapsulated by this graph.
         graph:
             The directed graph representing the job shop, where nodes are
                 operations, machines, jobs, or abstract concepts like global,
                 source, and sink, with edges indicating dependencies.
-        nodes:
-            A list of all nodes, encapsulated by the `Node` class, in the
-                graph.
-        nodes_by_type:
-            A dictionary categorizing nodes by their `NodeType`,
-                facilitating access to nodes of a particular type.
-        nodes_by_machine:
-            A nested list mapping each machine to its associated
-                operation nodes, aiding in machine-specific analysis.
-        nodes_by_job:
-            Similar to `nodes_by_machine`, but maps jobs to their
-                operation nodes, useful for job-specific traversal.
     """
 
-    __slots__ = (
-        "instance",
-        "graph",
-        "nodes",
-        "nodes_by_type",
-        "nodes_by_machine",
-        "nodes_by_job",
-        "_next_node_id",
-    )
-
     def __init__(self, instance: JobShopInstance):
         """Initializes the graph with the given instance.
 
         Nodes of type `OPERATION` are added to the graph based on the
         operations of the instance.
 
         Args:
             instance:
                 The job shop instance that the graph represents.
         """
         self.graph = nx.DiGraph()
         self.instance = instance
 
-        self.nodes: list[Node] = []
-
-        self.nodes_by_type: dict[NodeType, list[Node]] = (
+        self._nodes: list[Node] = []
+        self._nodes_by_type: dict[NodeType, list[Node]] = (
             collections.defaultdict(list)
         )
-
-        self.nodes_by_machine: list[list[Node]] = [
+        self._nodes_by_machine: list[list[Node]] = [
             [] for _ in range(instance.num_machines)
         ]
-
-        self.nodes_by_job: list[list[Node]] = [
+        self._nodes_by_job: list[list[Node]] = [
             [] for _ in range(instance.num_jobs)
         ]
-
         self._next_node_id = 0
-
+        self.removed_nodes: list[bool] = []
         self._add_operation_nodes()
 
     @property
-    def num_nodes(self) -> int:
-        """Number of nodes in the graph."""
-        return len(self.nodes)
+    def nodes(self) -> list[Node]:
+        """List of all nodes added to the graph.
+
+        It may contain nodes that have been removed from the graph.
+        """
+        return self._nodes
+
+    @property
+    def nodes_by_type(self) -> dict[NodeType, list[Node]]:
+        """Dictionary mapping node types to lists of nodes.
+
+        It may contain nodes that have been removed from the graph.
+        """
+        return self._nodes_by_type
+
+    @property
+    def nodes_by_machine(self) -> list[list[Node]]:
+        """List of lists mapping machine ids to operation nodes.
+
+        It may contain nodes that have been removed from the graph.
+        """
+        return self._nodes_by_machine
+
+    @property
+    def nodes_by_job(self) -> list[list[Node]]:
+        """List of lists mapping job ids to operation nodes.
+
+        It may contain nodes that have been removed from the graph.
+        """
+        return self._nodes_by_job
 
     @property
     def num_edges(self) -> int:
         """Number of edges in the graph."""
         return self.graph.number_of_edges()
 
+    @property
+    def num_job_nodes(self) -> int:
+        """Number of job nodes in the graph."""
+        return len(self._nodes_by_type[NodeType.JOB])
+
     def _add_operation_nodes(self) -> None:
         """Adds operation nodes to the graph."""
         for job in self.instance.jobs:
             for operation in job:
                 node = Node(node_type=NodeType.OPERATION, operation=operation)
                 self.add_node(node)
 
-    def get_operation_from_id(self, operation_id: int) -> Operation:
-        """Returns the operation with the given id."""
-        return self.nodes[operation_id].operation
-
     def add_node(self, node_for_adding: Node) -> None:
         """Adds a node to the graph and updates relevant class attributes.
 
         This method assigns a unique identifier to the node, adds it to the
         graph, and updates the nodes list and the nodes_by_type dictionary. If
         the node is of type `OPERATION`, it also updates `nodes_by_job` and
         `nodes_by_machine` based on the operation's job_id and machine_ids.
@@ -127,23 +130,24 @@
             should be done exclusively through this method to avoid
             inconsistencies.
         """
         node_for_adding.node_id = self._next_node_id
         self.graph.add_node(
             node_for_adding.node_id, **{NODE_ATTR: node_for_adding}
         )
-        self.nodes_by_type[node_for_adding.node_type].append(node_for_adding)
-        self.nodes.append(node_for_adding)
+        self._nodes_by_type[node_for_adding.node_type].append(node_for_adding)
+        self._nodes.append(node_for_adding)
         self._next_node_id += 1
+        self.removed_nodes.append(False)
 
         if node_for_adding.node_type == NodeType.OPERATION:
             operation = node_for_adding.operation
-            self.nodes_by_job[operation.job_id].append(node_for_adding)
+            self._nodes_by_job[operation.job_id].append(node_for_adding)
             for machine_id in operation.machines:
-                self.nodes_by_machine[machine_id].append(node_for_adding)
+                self._nodes_by_machine[machine_id].append(node_for_adding)
 
     def add_edge(
         self, u_of_edge: Node | int, v_of_edge: Node | int, **attr
     ) -> None:
         """Adds an edge to the graph.
 
         Args:
@@ -152,18 +156,47 @@
                 the node_id of the source.
             v_of_edge: The destination node of the edge. If it is a `Node`, its
                 `node_id` is used as the destination. Otherwise, it is assumed
                 to be the node_id of the destination.
             **attr: Additional attributes to be added to the edge.
 
         Raises:
-            ValueError: If `u_of_edge` or `v_of_edge` are not in the graph.
+            JobShopLibError: If `u_of_edge` or `v_of_edge` are not in the
+                graph.
         """
         if isinstance(u_of_edge, Node):
             u_of_edge = u_of_edge.node_id
         if isinstance(v_of_edge, Node):
             v_of_edge = v_of_edge.node_id
         if u_of_edge not in self.graph or v_of_edge not in self.graph:
-            raise ValueError(
+            raise JobShopLibError(
                 "`u_of_edge` and `v_of_edge` must be in the graph."
             )
         self.graph.add_edge(u_of_edge, v_of_edge, **attr)
+
+    def remove_node(self, node_id: int) -> None:
+        """Removes a node from the graph and the isolated nodes that result
+        from the removal.
+
+        Args:
+            node_id: The id of the node to remove.
+        """
+        self.graph.remove_node(node_id)
+        self.removed_nodes[node_id] = True
+
+        isolated_nodes = list(nx.isolates(self.graph))
+        for isolated_node in isolated_nodes:
+            self.removed_nodes[isolated_node] = True
+
+        self.graph.remove_nodes_from(isolated_nodes)
+
+    def is_removed(self, node: int | Node) -> bool:
+        """Returns whether the node is removed from the graph.
+
+        Args:
+            node: The node to check. If it is a `Node`, its `node_id` is used
+                as the node to check. Otherwise, it is assumed to be the
+                `node_id` of the node to check.
+        """
+        if isinstance(node, Node):
+            node = node.node_id
+        return self.removed_nodes[node]
```

### Comparing `job_shop_lib-0.2.1/job_shop_lib/graphs/node.py` & `job_shop_lib-0.3.0/job_shop_lib/graphs/node.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Home of the `Node` class."""
 
-from job_shop_lib import Operation
+from job_shop_lib import Operation, JobShopLibError
 from job_shop_lib.graphs.constants import NodeType
 
 
 class Node:
     """Data structure to represent a node in the `JobShopGraph`.
 
     A node is hashable by its id. The id is assigned when the node is added to
@@ -31,97 +31,116 @@
     node = Node(NodeType.SOURCE)
     node.node_id = 1
     graph = {node: "some value"}
     print(graph[node])  # "some value"
     print(graph[1])  # "some value"
     ```
 
-    Args:
+    Attributes:
         node_type:
             The type of the node. It can be one of the following:
             - NodeType.OPERATION
             - NodeType.MACHINE
             - NodeType.JOB
             - NodeType.GLOBAL
             ...
-        operation:
-            The operation of the node. It should be provided if the node_type
-            is NodeType.OPERATION.
-        machine_id:
-            The id of the machine of the node. It should be provided if the
-            node_type is NodeType.MACHINE.
-        job_id:
-            The id of the job of the node. It should be provided if the
-            node_type is NodeType.JOB.
     """
 
     __slots__ = "node_type", "_node_id", "_operation", "_machine_id", "_job_id"
 
     def __init__(
         self,
         node_type: NodeType,
         operation: Operation | None = None,
         machine_id: int | None = None,
         job_id: int | None = None,
     ):
+        """Initializes the node with the given attributes.
+
+        Args:
+            node_type:
+                The type of the node. It can be one of the following:
+                - NodeType.OPERATION
+                - NodeType.MACHINE
+                - NodeType.JOB
+                - NodeType.GLOBAL
+                ...
+            operation:
+                The operation of the node. It should be provided if the
+                `node_type` is NodeType.OPERATION.
+            machine_id:
+                The id of the machine of the node. It should be provided if the
+                node_type is NodeType.MACHINE.
+            job_id:
+                The id of the job of the node. It should be provided if the
+                node_type is NodeType.JOB.
+
+        Raises:
+            JobShopLibError:
+                If the node_type is OPERATION and operation is None.
+            JobShopLibError:
+                If the node_type is MACHINE and machine_id is None.
+            JobShopLibError:
+                If the node_type is JOB and job_id is None.
+        """
         if node_type == NodeType.OPERATION and operation is None:
-            raise ValueError("Operation node must have an operation.")
+            raise JobShopLibError("Operation node must have an operation.")
 
         if node_type == NodeType.MACHINE and machine_id is None:
-            raise ValueError("Machine node must have a machine_id.")
+            raise JobShopLibError("Machine node must have a machine_id.")
 
         if node_type == NodeType.JOB and job_id is None:
-            raise ValueError("Job node must have a job_id.")
+            raise JobShopLibError("Job node must have a job_id.")
 
         self.node_type = node_type
         self._node_id: int | None = None
 
         self._operation = operation
         self._machine_id = machine_id
         self._job_id = job_id
 
     @property
     def node_id(self) -> int:
         """Returns a unique identifier for the node."""
         if self._node_id is None:
-            raise ValueError("Node has not been assigned an id.")
+            raise JobShopLibError("Node has not been assigned an id.")
         return self._node_id
 
     @node_id.setter
     def node_id(self, value: int) -> None:
         self._node_id = value
 
     @property
     def operation(self) -> Operation:
         """Returns the operation of the node.
 
         This property is mandatory for nodes of type `OPERATION`.
         """
         if self._operation is None:
-            raise ValueError("Node has no operation.")
+            raise JobShopLibError("Node has no operation.")
         return self._operation
 
     @property
     def machine_id(self) -> int:
         """Returns the `machine_id` of the node.
 
         This property is mandatory for nodes of type `MACHINE`.
         """
         if self._machine_id is None:
-            raise ValueError("Node has no `machine_id`.")
+            raise JobShopLibError("Node has no `machine_id`.")
         return self._machine_id
 
     @property
     def job_id(self) -> int:
         """Returns the `job_id` of the node.
 
         This property is mandatory for nodes of type `JOB`.
         """
         if self._job_id is None:
-            raise ValueError("Node has no `job_id`.")
+            raise JobShopLibError("Node has no `job_id`.")
         return self._job_id
 
     def __hash__(self) -> int:
         return self.node_id
 
     def __eq__(self, __value: object) -> bool:
         if isinstance(__value, Node):
```

### Comparing `job_shop_lib-0.2.1/job_shop_lib/job_shop_instance.py` & `job_shop_lib-0.3.0/job_shop_lib/job_shop_instance.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/operation.py` & `job_shop_lib-0.3.0/job_shop_lib/operation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Home of the `Operation` class."""
 
 from __future__ import annotations
 
+from job_shop_lib import JobShopLibError
+
 
 class Operation:
     """Stores machine and duration information for a job operation.
 
     Note:
         To increase performance, some solvers such as the CP-SAT solver use
         only integers to represent the operation's attributes. Should a
@@ -47,22 +49,22 @@
     def machine_id(self) -> int:
         """Returns the id of the machine associated with the operation.
 
         Raises:
             ValueError: If the operation has multiple machines in its list.
         """
         if len(self.machines) > 1:
-            raise ValueError("Operation has multiple machines.")
+            raise JobShopLibError("Operation has multiple machines.")
         return self.machines[0]
 
     @property
     def job_id(self) -> int:
         """Returns the id of the job that the operation belongs to."""
         if self._job_id is None:
-            raise ValueError("Operation has no job_id.")
+            raise JobShopLibError("Operation has no job_id.")
         return self._job_id
 
     @job_id.setter
     def job_id(self, value: int) -> None:
         self._job_id = value
 
     @property
@@ -70,15 +72,15 @@
         """Returns the position (starting at zero) of the operation in the
         job.
 
         Raises:
             ValueError: If the operation has no position_in_job.
         """
         if self._position_in_job is None:
-            raise ValueError("Operation has no position_in_job.")
+            raise JobShopLibError("Operation has no position_in_job.")
         return self._position_in_job
 
     @position_in_job.setter
     def position_in_job(self, value: int) -> None:
         self._position_in_job = value
 
     @property
@@ -91,15 +93,15 @@
         It starts at 0 and is incremented by 1 for each operation in the
         instance.
 
         Raises:
             ValueError: If the operation has no id.
         """
         if self._operation_id is None:
-            raise ValueError("Operation has no id.")
+            raise JobShopLibError("Operation has no id.")
         return self._operation_id
 
     @operation_id.setter
     def operation_id(self, value: int) -> None:
         self._operation_id = value
 
     def __hash__(self) -> int:
```

### Comparing `job_shop_lib-0.2.1/job_shop_lib/schedule.py` & `job_shop_lib-0.3.0/job_shop_lib/schedule.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/scheduled_operation.py` & `job_shop_lib-0.3.0/job_shop_lib/scheduled_operation.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/visualization/__init__.py` & `job_shop_lib-0.3.0/job_shop_lib/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/visualization/agent_task_graph.py` & `job_shop_lib-0.3.0/job_shop_lib/visualization/agent_task_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/job_shop_lib/visualization/create_gif.py` & `job_shop_lib-0.3.0/job_shop_lib/visualization/create_gif.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """Module for creating a GIF of the schedule being built by a
 dispatching rule solver."""
 
 import os
 import pathlib
 import shutil
-from typing import Callable
+from collections.abc import Callable
 
 import imageio
 import matplotlib.pyplot as plt
 from matplotlib.figure import Figure
 
 from job_shop_lib import JobShopInstance, Schedule, Operation
-from job_shop_lib.dispatching import DispatchingRuleSolver, Dispatcher
+from job_shop_lib.dispatching import (
+    DispatchingRuleSolver,
+    Dispatcher,
+    HistoryTracker,
+)
 from job_shop_lib.visualization.gantt_chart import plot_gantt_chart
 
 
 # Most of the arguments are optional with default values. There is no way to
 # reduce the number of arguments without losing functionality.
 # pylint: disable=too-many-arguments
 def create_gif(
@@ -110,15 +114,19 @@
         fig.text(
             1.25,
             0.05,
             text,
             ha="right",
             va="bottom",
             transform=ax.transAxes,
-            bbox=dict(facecolor="white", alpha=0.5, boxstyle="round,pad=0.5"),
+            bbox={
+                "facecolor": "white",
+                "alpha": 0.5,
+                "boxstyle": "round,pad=0.5",
+            },
         )
         return fig
 
     return plot_function
 
 
 def create_gantt_chart_frames(
@@ -140,30 +148,31 @@
         plot_function:
             A function that plots a Gantt chart for a schedule. It
             should take a `Schedule` object and the makespan of the schedule as
             input and return a `Figure` object.
         plot_current_time:
             Whether to plot a vertical line at the current time."""
     dispatcher = Dispatcher(instance, pruning_function=solver.pruning_function)
-    schedule = dispatcher.schedule
-    makespan = solver(instance).makespan()
-    iteration = 0
-
-    while not schedule.is_complete():
-        solver.step(dispatcher)
-        iteration += 1
+    history_tracker = HistoryTracker(dispatcher)
+    makespan = solver.solve(instance, dispatcher).makespan()
+    dispatcher.unsubscribe(history_tracker)
+    dispatcher.reset()
+    for i, scheduled_operation in enumerate(history_tracker.history, start=1):
+        dispatcher.dispatch(
+            scheduled_operation.operation, scheduled_operation.machine_id
+        )
         fig = plot_function(
-            schedule,
+            dispatcher.schedule,
             makespan,
             dispatcher.available_operations(),
         )
         current_time = (
             None if not plot_current_time else dispatcher.current_time()
         )
-        _save_frame(fig, frames_dir, iteration, current_time)
+        _save_frame(fig, frames_dir, i, current_time)
 
 
 def _save_frame(
     figure: Figure, frames_dir: str, number: int, current_time: int | None
 ) -> None:
     if current_time is not None:
         figure.gca().axvline(current_time, color="red", linestyle="--")
```

### Comparing `job_shop_lib-0.2.1/job_shop_lib/visualization/disjunctive_graph.py` & `job_shop_lib-0.3.0/job_shop_lib/visualization/disjunctive_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Optional, Callable
 import warnings
 import copy
 
 import matplotlib
 import matplotlib.pyplot as plt
 import networkx as nx
+from networkx.drawing.nx_agraph import graphviz_layout
 
 from job_shop_lib import JobShopInstance
 from job_shop_lib.graphs import (
     JobShopGraph,
     EdgeType,
     NodeType,
     Node,
@@ -61,43 +62,44 @@
             f"Disjunctive Graph Visualization: {job_shop_graph.instance.name}"
         )
     plt.title(title)
 
     # Set up the layout
     # -----------------
     if layout is None:
-        try:
-            from networkx.drawing.nx_agraph import (
-                graphviz_layout,
-            )
-
-            layout = functools.partial(
-                graphviz_layout, prog="dot", args="-Grankdir=LR"
-            )
-        except ImportError:
-            warnings.warn(
-                "Could not import graphviz_layout. "
-                + "Using spring_layout instead."
-            )
-            layout = nx.spring_layout
+        layout = functools.partial(
+            graphviz_layout, prog="dot", args="-Grankdir=LR"
+        )
 
     temp_graph = copy.deepcopy(job_shop_graph.graph)
     # Remove disjunctive edges to get a better layout
     temp_graph.remove_edges_from(
         [
             (u, v)
             for u, v, d in job_shop_graph.graph.edges(data=True)
             if d["type"] == EdgeType.DISJUNCTIVE
         ]
     )
-    pos = layout(temp_graph)  # type: ignore
+
+    try:
+        pos = layout(temp_graph)
+    except ImportError:
+        warnings.warn(
+            "Default layout requires pygraphviz http://pygraphviz.github.io/. "
+            "Using spring layout instead.",
+        )
+        pos = nx.spring_layout(temp_graph)
 
     # Draw nodes
     # ----------
-    node_colors = [_get_node_color(node) for node in job_shop_graph.nodes]
+    node_colors = [
+        _get_node_color(node)
+        for node in job_shop_graph.nodes
+        if not job_shop_graph.is_removed(node.node_id)
+    ]
 
     nx.draw_networkx_nodes(
         job_shop_graph.graph,
         pos,
         node_size=node_size,
         node_color=node_colors,
         alpha=alpha,
@@ -143,14 +145,16 @@
     labels = {}
     source_node = job_shop_graph.nodes_by_type[NodeType.SOURCE][0]
     labels[source_node] = "S"
 
     sink_node = job_shop_graph.nodes_by_type[NodeType.SINK][0]
     labels[sink_node] = "T"
     for operation_node in operation_nodes:
+        if job_shop_graph.is_removed(operation_node.node_id):
+            continue
         labels[operation_node] = (
             f"m={operation_node.operation.machine_id}\n"
             f"d={operation_node.operation.duration}"
         )
 
     nx.draw_networkx_labels(
         job_shop_graph.graph,
```

### Comparing `job_shop_lib-0.2.1/job_shop_lib/visualization/gantt_chart.py` & `job_shop_lib-0.3.0/job_shop_lib/visualization/gantt_chart.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.2.1/pyproject.toml` & `job_shop_lib-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "job-shop-lib"
-version = "0.2.1"
+version = "0.3.0"
 description = "An easy-to-use and modular Python library for the Job Shop Scheduling Problem (JSSP)"
 authors = ["Pabloo22 <pablete.arino@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "job_shop_lib"}]
 include = ["benchmarks/benchmark_instances.json"]
```

### Comparing `job_shop_lib-0.2.1/PKG-INFO` & `job_shop_lib-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: job-shop-lib
-Version: 0.2.1
+Version: 0.3.0
 Summary: An easy-to-use and modular Python library for the Job Shop Scheduling Problem (JSSP)
 License: MIT
 Author: Pabloo22
 Author-email: pablete.arino@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

