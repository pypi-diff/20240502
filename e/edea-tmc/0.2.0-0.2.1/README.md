# Comparing `tmp/edea_tmc-0.2.0.tar.gz` & `tmp/edea_tmc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edea_tmc-0.2.0.tar", last modified: Fri Feb  9 11:27:19 2024, max compression
+gzip compressed data, was "edea_tmc-0.2.1.tar", last modified: Fri Feb  9 15:06:54 2024, max compression
```

## Comparing `edea_tmc-0.2.0.tar` & `edea_tmc-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      197 2023-11-28 17:49:22.266884 edea_tmc-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-01-24 12:57:36.048781 edea_tmc-0.2.0/edea_tmc/__init__.py
--rw-r--r--   0        0        0     2673 2024-02-09 11:27:01.402736 edea_tmc-0.2.0/edea_tmc/local.py
--rw-r--r--   0        0        0     8060 2024-02-09 11:27:01.402736 edea_tmc-0.2.0/edea_tmc/remote.py
--rw-r--r--   0        0        0     2356 2024-02-09 11:27:01.402736 edea_tmc-0.2.0/edea_tmc/runner.py
--rw-r--r--   0        0        0     1335 2024-02-09 11:27:01.402736 edea_tmc-0.2.0/edea_tmc/sequencer.py
--rw-r--r--   0        0        0     2597 2024-02-09 11:27:01.402736 edea_tmc-0.2.0/edea_tmc/stepper.py
--rw-r--r--   0        0        0      820 2024-02-09 11:27:19.356199 edea_tmc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       37 2024-02-08 10:47:37.007151 edea_tmc-0.2.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2024-02-08 10:47:37.007151 edea_tmc-0.2.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2024-02-08 10:47:37.007151 edea_tmc-0.2.0/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      691 2024-02-09 10:04:53.030476 edea_tmc-0.2.0/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1164 2024-02-09 10:14:22.676610 edea_tmc-0.2.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2024-02-09 10:14:22.676610 edea_tmc-0.2.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2023-01-24 12:57:36.068783 edea_tmc-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      936 2024-02-09 11:27:01.406070 edea_tmc-0.2.0/tests/mocks.py
--rw-r--r--   0        0        0        0 2024-02-09 10:00:02.938532 edea_tmc-0.2.0/tests/test.db
--rw-r--r--   0        0        0     1874 2024-02-09 11:27:01.406070 edea_tmc-0.2.0/tests/test_local_run.py
--rw-r--r--   0        0        0     1528 2024-02-09 11:27:01.406070 edea_tmc-0.2.0/tests/test_remote_run.py
--rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 edea_tmc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      197 2023-11-28 17:49:22.266884 edea_tmc-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-01-24 12:57:36.048781 edea_tmc-0.2.1/edea_tmc/__init__.py
+-rw-r--r--   0        0        0     2807 2024-02-09 15:06:41.649323 edea_tmc-0.2.1/edea_tmc/local.py
+-rw-r--r--   0        0        0    10227 2024-02-09 15:06:41.649323 edea_tmc-0.2.1/edea_tmc/remote.py
+-rw-r--r--   0        0        0     2388 2024-02-09 15:06:41.649323 edea_tmc-0.2.1/edea_tmc/runner.py
+-rw-r--r--   0        0        0     1407 2024-02-09 15:06:41.649323 edea_tmc-0.2.1/edea_tmc/sequencer.py
+-rw-r--r--   0        0        0     2673 2024-02-09 15:06:41.652656 edea_tmc-0.2.1/edea_tmc/stepper.py
+-rw-r--r--   0        0        0     1046 2024-02-09 15:06:54.506058 edea_tmc-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-02-08 10:47:37.007151 edea_tmc-0.2.1/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2024-02-08 10:47:37.007151 edea_tmc-0.2.1/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2024-02-08 10:47:37.007151 edea_tmc-0.2.1/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      691 2024-02-09 10:04:53.030476 edea_tmc-0.2.1/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1164 2024-02-09 10:14:22.676610 edea_tmc-0.2.1/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2024-02-09 10:14:22.676610 edea_tmc-0.2.1/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2023-01-24 12:57:36.068783 edea_tmc-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      936 2024-02-09 11:27:01.406070 edea_tmc-0.2.1/tests/mocks.py
+-rw-r--r--   0        0        0        0 2024-02-09 10:00:02.938532 edea_tmc-0.2.1/tests/test.db
+-rw-r--r--   0        0        0     1874 2024-02-09 11:27:01.406070 edea_tmc-0.2.1/tests/test_local_run.py
+-rw-r--r--   0        0        0     2135 2024-02-09 12:12:37.475600 edea_tmc-0.2.1/tests/test_remote_run.py
+-rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 edea_tmc-0.2.1/PKG-INFO
```

### Comparing `edea_tmc-0.2.0/edea_tmc/local.py` & `edea_tmc-0.2.1/edea_tmc/local.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 from .runner import AbstractMeasurementRun
 from .stepper import Stepper
 
 try:
     from tqdm.auto import tqdm
 except ImportError:
-    tqdm = None
+    tqdm = None  # type: ignore
 
 try:
     import polars as pl
 except ImportError:
-    pl = None
+    pl = None  # type: ignore
 
 try:
     import pandas as pd
 except ImportError:
-    pd = None
+    pd = None  # type: ignore
 
 
 class LocalMeasurementRun(AbstractMeasurementRun):
     def __init__(self, steps: list[Any], steppers: dict[str, Stepper], filename: str, convert: bool = False):
         super().__init__(steps, steppers)
         self._file = None
         self.filename = filename.removesuffix(".ndjson") if filename.endswith(".ndjson") else filename
@@ -74,15 +74,16 @@
         with the same short_code again.
         """
 
         # 1. check if the project exists and get the project id
         run = LocalMeasurementRun(steps, steppers, filename, convert)
 
         # display a progress bar when running interactively
-        if hasattr(sys, "ps1") and tqdm:
-            steps = tqdm(steps, unit="step")
-
-        # 3. run the steps
-        for _ in steps:
-            run.step()
+        if hasattr(sys, "ps1") and tqdm is not None:
+            for _ in tqdm(steps, unit="step"):
+                run.step()
+        else:
+            # or simply run without a progress bar
+            for _ in steps:
+                run.step()
 
         return run
```

### Comparing `edea_tmc-0.2.0/edea_tmc/runner.py` & `edea_tmc-0.2.1/edea_tmc/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from typing import TypeVar, Generic, Any
 
 from .stepper import Stepper, StepResult, StepStatus
 
 try:
     import polars as pl
 except ImportError:
-    pl = None
+    pl = None  # type: ignore
 
 try:
     import pandas as pd
 except ImportError:
-    pd = None
+    pd = None  # type: ignore
 
 
 @dataclass
 class SequenceStepResult:
     conditions: dict[str, str | float]
     results: dict[str, str | float]
```

### Comparing `edea_tmc-0.2.0/edea_tmc/sequencer.py` & `edea_tmc-0.2.1/edea_tmc/sequencer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import itertools
 
 
-def condition_generator(test_parameters: dict[str, list[float | str]]) -> list[dict[str, str | float]]:
+def condition_generator(test_parameters: dict[str, list[float | str]]) -> list[dict[str, str | float | int]]:
     """
     General-purpose test condition generator.
     Takes a map of Stepper names as key with the conditions as a list of values. It will
     generate a list of set-conditions in order of the keys and values.
 
     It generates a set of conditions for each key. The values of each key are iterated
     in order and the keys from last to first.
@@ -22,14 +22,14 @@
         {"a": 2, "b": "foo", "c": 3},
         {"a": 2, "b": "foo", "c": 4},
         {"a": 2, "b": "bar", "c": 3},
         {"a": 2, "b": "bar", "c": 4},
     ]
     """
 
-    test_conditions = []
+    test_conditions: list[dict[str, str | float | int]] = []
     for idx, e in enumerate(itertools.product(*test_parameters.values())):
-        d = {"sequence_number": idx}
+        d: dict[str, str | float | int] = {"sequence_number": idx}
         for sub_index, key in enumerate(test_parameters.keys()):
             d[key] = e[sub_index]
         test_conditions.append(d)
     return test_conditions
```

### Comparing `edea_tmc-0.2.0/edea_tmc/stepper.py` & `edea_tmc-0.2.1/edea_tmc/stepper.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,39 +38,39 @@
     def setup(self, resume: bool = False):
         """
         setup the device/instrument/other based on the parameters passed
         in the class initialization. resume will
         """
         pass
 
-    def pre_step(self):
+    def pre_step(self) -> None:
         """
         pre_step will be executed before a new step is being run. this can
         e.g. be a sanity check that a value is in an expected range for the
         next step to be run.
         """
         pass
 
     def step(self, set_point: str | float) -> StepResult:
         """
         step brings the device/instrument/other to a given setpoint and returns
         a result representing success or failure. on success, post_step will be
         executed and on failure, depending on the result of the check method,
         it will be re-tried (check says it's ok) or the procedure will be aborted.
         """
-        pass
+        raise NotImplementedError("step method not implemented")
 
-    def post_step(self):
+    def post_step(self) -> None:
         """
         post_step, similar to pre_step is an additional check that will be
         executed after a step has been executed for a given set point.
         """
         pass
 
-    def teardown(self):
+    def teardown(self) -> None:
         """
         teardown will be run after a run has been finished. this should bring
         everything that needs it into a safe state and/or shut it off if
         necessary.
         """
         pass
```

### Comparing `edea_tmc-0.2.0/tests/.pytest_cache/v/cache/lastfailed` & `edea_tmc-0.2.1/tests/.pytest_cache/v/cache/lastfailed`

 * *Files identical despite different names*

### Comparing `edea_tmc-0.2.0/tests/.pytest_cache/v/cache/nodeids` & `edea_tmc-0.2.1/tests/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `edea_tmc-0.2.0/tests/mocks.py` & `edea_tmc-0.2.1/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `edea_tmc-0.2.0/tests/test_local_run.py` & `edea_tmc-0.2.1/tests/test_local_run.py`

 * *Files identical despite different names*

### Comparing `edea_tmc-0.2.0/tests/test_remote_run.py` & `edea_tmc-0.2.1/tests/test_remote_run.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 
 import httpx
 import numpy as np
 import pytest
 from httpx import ConnectError
 
-from edea_tmc.remote import MSRunner
+from edea_tmc.remote import MSRunner, AsyncMSRunner
 from edea_tmc.sequencer import condition_generator
 from tests.mocks import MockStepper, MockValueStepper
 
 
 @pytest.fixture(autouse=True)
 def edea_ms_server():
     p = subprocess.Popen(["python3", "-m", "edea_ms", "--local"])
@@ -44,7 +44,24 @@
     v1 = MockValueStepper(s1, s2)
 
     steppers = {"Mock_1": s1, "Mock_2": s2, "Value_1": v1}
 
     steps = condition_generator(test_parameters)
 
     runner.run(steps, steppers, "TR01", "TEST_DEV", "first test", )
+
+@pytest.mark.asyncio
+async def test_async_remote_measurement_run() -> None:
+    runner = AsyncMSRunner("http://127.0.0.1:8000", "X5678")
+
+    test_parameters = {"Mock_1": [3, 4, 5], "Mock_2": np.concatenate(
+        (np.linspace(0.1, 1, 9), np.linspace(0.05, 0.01, 6), (np.logspace(0, 1, 10)),)), "Value_1": ["get_value"], }
+
+    s1 = MockStepper()
+    s2 = MockStepper()
+    v1 = MockValueStepper(s1, s2)
+
+    steppers = {"Mock_1": s1, "Mock_2": s2, "Value_1": v1}
+
+    steps = condition_generator(test_parameters)
+
+    await runner.run(steps, steppers, "TR02", "TEST_DEV", "async test", )
```

