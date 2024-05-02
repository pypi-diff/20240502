# Comparing `tmp/beta9-0.1.7.tar.gz` & `tmp/beta9-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beta9-0.1.7.tar", max compression
+gzip compressed data, was "beta9-0.1.8.tar", max compression
```

## Comparing `beta9-0.1.7.tar` & `beta9-0.1.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1149 2024-04-29 21:57:51.839903 beta9-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      586 2024-04-26 18:24:46.913842 beta9-0.1.7/src/beta9/__init__.py
--rw-r--r--   0        0        0        0 2024-01-23 23:38:59.669351 beta9-0.1.7/src/beta9/abstractions/__init__.py
--rw-r--r--   0        0        0     1799 2024-04-29 18:52:41.008869 beta9-0.1.7/src/beta9/abstractions/base/__init__.py
--rw-r--r--   0        0        0     9285 2024-04-29 18:31:09.499178 beta9-0.1.7/src/beta9/abstractions/base/runner.py
--rw-r--r--   0        0        0     3454 2024-04-29 21:53:15.666398 beta9-0.1.7/src/beta9/abstractions/container.py
--rw-r--r--   0        0        0     7314 2024-04-29 21:53:15.666604 beta9-0.1.7/src/beta9/abstractions/endpoint.py
--rw-r--r--   0        0        0     7251 2024-04-29 21:53:15.667152 beta9-0.1.7/src/beta9/abstractions/function.py
--rw-r--r--   0        0        0     4413 2024-04-29 15:50:05.673117 beta9-0.1.7/src/beta9/abstractions/image.py
--rw-r--r--   0        0        0     3237 2024-04-17 13:14:18.141834 beta9-0.1.7/src/beta9/abstractions/map.py
--rw-r--r--   0        0        0     3345 2024-04-29 15:50:05.673407 beta9-0.1.7/src/beta9/abstractions/queue.py
--rw-r--r--   0        0        0     9054 2024-04-29 21:53:15.667793 beta9-0.1.7/src/beta9/abstractions/taskqueue.py
--rw-r--r--   0        0        0     1605 2024-04-17 13:14:18.142367 beta9-0.1.7/src/beta9/abstractions/volume.py
--rw-r--r--   0        0        0      292 2024-04-15 21:13:39.880348 beta9-0.1.7/src/beta9/aio.py
--rw-r--r--   0        0        0     4839 2024-04-29 19:08:45.672170 beta9-0.1.7/src/beta9/channel.py
--rw-r--r--   0        0        0        0 2024-01-23 23:38:59.670190 beta9-0.1.7/src/beta9/cli/__init__.py
--rw-r--r--   0        0        0      669 2024-04-29 15:50:05.674161 beta9-0.1.7/src/beta9/cli/config.py
--rw-r--r--   0        0        0     2418 2024-04-29 19:06:38.918521 beta9-0.1.7/src/beta9/cli/deployment.py
--rw-r--r--   0        0        0     5582 2024-04-29 19:07:51.112717 beta9-0.1.7/src/beta9/cli/extraclick.py
--rw-r--r--   0        0        0     1810 2024-04-29 18:32:08.108950 beta9-0.1.7/src/beta9/cli/main.py
--rw-r--r--   0        0        0     3770 2024-04-29 18:40:09.512566 beta9-0.1.7/src/beta9/cli/task.py
--rw-r--r--   0        0        0     8591 2024-04-29 18:31:31.881448 beta9-0.1.7/src/beta9/cli/volume.py
--rw-r--r--   0        0        0        0 2024-04-16 19:32:37.403246 beta9-0.1.7/src/beta9/clients/__init__.py
--rw-r--r--   0        0        0     2980 2024-04-17 13:14:18.144448 beta9-0.1.7/src/beta9/clients/container/__init__.py
--rw-r--r--   0        0        0     4275 2024-04-21 18:41:12.433810 beta9-0.1.7/src/beta9/clients/endpoint/__init__.py
--rw-r--r--   0        0        0     8023 2024-04-17 13:14:18.144848 beta9-0.1.7/src/beta9/clients/function/__init__.py
--rw-r--r--   0        0        0    22783 2024-04-29 14:36:52.301336 beta9-0.1.7/src/beta9/clients/gateway/__init__.py
--rw-r--r--   0        0        0     4773 2024-04-17 13:14:18.145074 beta9-0.1.7/src/beta9/clients/image/__init__.py
--rw-r--r--   0        0        0     8003 2024-04-17 13:14:18.145188 beta9-0.1.7/src/beta9/clients/map/__init__.py
--rw-r--r--   0        0        0     8687 2024-04-17 13:14:18.145328 beta9-0.1.7/src/beta9/clients/simplequeue/__init__.py
--rw-r--r--   0        0        0    13315 2024-04-21 18:41:12.433950 beta9-0.1.7/src/beta9/clients/taskqueue/__init__.py
--rw-r--r--   0        0        0     9482 2024-04-17 13:14:18.145732 beta9-0.1.7/src/beta9/clients/volume/__init__.py
--rw-r--r--   0        0        0     4843 2024-04-29 21:33:40.077172 beta9-0.1.7/src/beta9/config.py
--rw-r--r--   0        0        0      492 2024-04-26 18:24:46.916278 beta9-0.1.7/src/beta9/env.py
--rw-r--r--   0        0        0      207 2024-01-23 23:38:59.671504 beta9-0.1.7/src/beta9/exceptions.py
--rw-r--r--   0        0        0      883 2024-04-26 18:24:46.916852 beta9-0.1.7/src/beta9/logging.py
--rw-r--r--   0        0        0        0 2024-01-23 23:38:59.671565 beta9-0.1.7/src/beta9/runner/__init__.py
--rw-r--r--   0        0        0     6364 2024-04-29 19:00:52.006511 beta9-0.1.7/src/beta9/runner/common.py
--rw-r--r--   0        0        0     2322 2024-04-29 18:32:47.793316 beta9-0.1.7/src/beta9/runner/container.py
--rw-r--r--   0        0        0     7454 2024-04-29 18:32:58.148052 beta9-0.1.7/src/beta9/runner/endpoint.py
--rw-r--r--   0        0        0     6890 2024-04-29 18:30:52.002896 beta9-0.1.7/src/beta9/runner/function.py
--rw-r--r--   0        0        0     3910 2024-04-17 13:14:18.147410 beta9-0.1.7/src/beta9/runner/serve.py
--rw-r--r--   0        0        0    12307 2024-04-29 21:53:15.668333 beta9-0.1.7/src/beta9/runner/taskqueue.py
--rw-r--r--   0        0        0     5716 2024-04-29 19:00:25.543057 beta9-0.1.7/src/beta9/sync.py
--rw-r--r--   0        0        0     3114 2024-04-29 15:50:05.676180 beta9-0.1.7/src/beta9/terminal.py
--rw-r--r--   0        0        0     1541 2024-04-29 14:36:52.302649 beta9-0.1.7/src/beta9/type.py
--rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 beta9-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1149 2024-04-30 16:23:12.920277 beta9-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      586 2024-04-29 20:55:10.787352 beta9-0.1.8/src/beta9/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-27 16:13:22.962074 beta9-0.1.8/src/beta9/abstractions/__init__.py
+-rw-r--r--   0        0        0     1799 2024-04-29 22:20:49.578255 beta9-0.1.8/src/beta9/abstractions/base/__init__.py
+-rw-r--r--   0        0        0     9817 2024-04-30 15:09:38.112071 beta9-0.1.8/src/beta9/abstractions/base/runner.py
+-rw-r--r--   0        0        0     3486 2024-04-30 15:09:38.112202 beta9-0.1.8/src/beta9/abstractions/container.py
+-rw-r--r--   0        0        0     7346 2024-04-30 15:58:19.398940 beta9-0.1.8/src/beta9/abstractions/endpoint.py
+-rw-r--r--   0        0        0     7283 2024-04-30 16:12:49.561561 beta9-0.1.8/src/beta9/abstractions/function.py
+-rw-r--r--   0        0        0     4421 2024-04-30 15:58:19.399337 beta9-0.1.8/src/beta9/abstractions/image.py
+-rw-r--r--   0        0        0     3237 2024-04-21 16:36:14.954512 beta9-0.1.8/src/beta9/abstractions/map.py
+-rw-r--r--   0        0        0     3345 2024-04-29 22:20:49.581920 beta9-0.1.8/src/beta9/abstractions/queue.py
+-rw-r--r--   0        0        0     9086 2024-04-30 15:58:19.399510 beta9-0.1.8/src/beta9/abstractions/taskqueue.py
+-rw-r--r--   0        0        0     1605 2024-04-21 16:36:14.957214 beta9-0.1.8/src/beta9/abstractions/volume.py
+-rw-r--r--   0        0        0      292 2024-01-27 16:13:22.963762 beta9-0.1.8/src/beta9/aio.py
+-rw-r--r--   0        0        0     4839 2024-04-29 22:20:49.582363 beta9-0.1.8/src/beta9/channel.py
+-rw-r--r--   0        0        0        0 2024-01-27 16:13:22.963872 beta9-0.1.8/src/beta9/cli/__init__.py
+-rw-r--r--   0        0        0      669 2024-04-29 22:20:49.582635 beta9-0.1.8/src/beta9/cli/config.py
+-rw-r--r--   0        0        0     2418 2024-04-29 22:20:49.583013 beta9-0.1.8/src/beta9/cli/deployment.py
+-rw-r--r--   0        0        0     5681 2024-04-30 15:09:38.113040 beta9-0.1.8/src/beta9/cli/extraclick.py
+-rw-r--r--   0        0        0     1810 2024-04-30 14:48:49.684633 beta9-0.1.8/src/beta9/cli/main.py
+-rw-r--r--   0        0        0     3770 2024-04-29 22:20:49.583966 beta9-0.1.8/src/beta9/cli/task.py
+-rw-r--r--   0        0        0     8591 2024-04-29 22:20:49.584340 beta9-0.1.8/src/beta9/cli/volume.py
+-rw-r--r--   0        0        0        0 2024-04-27 21:49:44.298869 beta9-0.1.8/src/beta9/clients/__init__.py
+-rw-r--r--   0        0        0     2980 2024-04-27 21:49:44.298980 beta9-0.1.8/src/beta9/clients/container/__init__.py
+-rw-r--r--   0        0        0     4275 2024-04-27 21:49:44.117994 beta9-0.1.8/src/beta9/clients/endpoint/__init__.py
+-rw-r--r--   0        0        0     8023 2024-04-27 21:49:43.256507 beta9-0.1.8/src/beta9/clients/function/__init__.py
+-rw-r--r--   0        0        0    22783 2024-04-29 20:55:10.788917 beta9-0.1.8/src/beta9/clients/gateway/__init__.py
+-rw-r--r--   0        0        0     4773 2024-04-27 21:49:42.845715 beta9-0.1.8/src/beta9/clients/image/__init__.py
+-rw-r--r--   0        0        0     8003 2024-04-27 21:49:43.051036 beta9-0.1.8/src/beta9/clients/map/__init__.py
+-rw-r--r--   0        0        0     8687 2024-04-27 21:49:43.458692 beta9-0.1.8/src/beta9/clients/simplequeue/__init__.py
+-rw-r--r--   0        0        0    13315 2024-04-27 21:49:43.930351 beta9-0.1.8/src/beta9/clients/taskqueue/__init__.py
+-rw-r--r--   0        0        0     9482 2024-04-27 21:49:43.680311 beta9-0.1.8/src/beta9/clients/volume/__init__.py
+-rw-r--r--   0        0        0     5193 2024-04-30 16:22:57.222961 beta9-0.1.8/src/beta9/config.py
+-rw-r--r--   0        0        0      492 2024-04-29 20:55:10.789359 beta9-0.1.8/src/beta9/env.py
+-rw-r--r--   0        0        0      207 2024-01-27 16:13:22.966808 beta9-0.1.8/src/beta9/exceptions.py
+-rw-r--r--   0        0        0      935 2024-04-30 16:22:57.223216 beta9-0.1.8/src/beta9/logging.py
+-rw-r--r--   0        0        0        0 2024-01-27 16:13:22.966902 beta9-0.1.8/src/beta9/runner/__init__.py
+-rw-r--r--   0        0        0     6364 2024-04-29 22:20:49.585063 beta9-0.1.8/src/beta9/runner/common.py
+-rw-r--r--   0        0        0     2322 2024-04-29 22:20:49.585267 beta9-0.1.8/src/beta9/runner/container.py
+-rw-r--r--   0        0        0     7454 2024-04-29 22:20:49.585589 beta9-0.1.8/src/beta9/runner/endpoint.py
+-rw-r--r--   0        0        0     6890 2024-04-29 22:20:49.585904 beta9-0.1.8/src/beta9/runner/function.py
+-rw-r--r--   0        0        0     3910 2024-04-21 16:36:14.986354 beta9-0.1.8/src/beta9/runner/serve.py
+-rw-r--r--   0        0        0    12307 2024-04-29 22:20:49.586188 beta9-0.1.8/src/beta9/runner/taskqueue.py
+-rw-r--r--   0        0        0     5716 2024-04-29 22:20:49.586428 beta9-0.1.8/src/beta9/sync.py
+-rw-r--r--   0        0        0     3114 2024-04-29 22:20:49.586622 beta9-0.1.8/src/beta9/terminal.py
+-rw-r--r--   0        0        0     1541 2024-04-29 20:55:10.791694 beta9-0.1.8/src/beta9/type.py
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 beta9-0.1.8/PKG-INFO
```

### Comparing `beta9-0.1.7/pyproject.toml` & `beta9-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beta9"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["beam.cloud <support@beam.cloud>"]
 packages = [
     { include = "beta9", from = "src" },
     { include = "beta9/**/*.py", from = "src" },
 ]
```

### Comparing `beta9-0.1.7/src/beta9/__init__.py` & `beta9-0.1.8/src/beta9/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/abstractions/base/__init__.py` & `beta9-0.1.8/src/beta9/abstractions/base/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/abstractions/base/runner.py` & `beta9-0.1.8/src/beta9/abstractions/base/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 FUNCTION_SERVE_STUB_TYPE = "function/serve"
 
 
 class RunnerAbstraction(BaseAbstraction):
     def __init__(
         self,
         cpu: Union[int, float, str] = 1.0,
-        memory: int = 128,
+        memory: Union[int, str] = 128,
         gpu: str = "",
         image: Image = Image(),
         concurrency: int = 1,
         max_containers: int = 1,
         keep_warm_seconds: float = 10.0,
         max_pending_tasks: int = 100,
         retries: int = 3,
@@ -61,15 +61,15 @@
         self.object_id: str = ""
         self.image_id: str = ""
         self.stub_id: str = ""
         self.handler: str = ""
         self.on_start: str = ""
         self.callback_url = callback_url or ""
         self.cpu = cpu
-        self.memory = memory
+        self.memory = self._parse_memory(memory) if isinstance(memory, str) else memory
         self.gpu = gpu
         self.volumes = volumes or []
         self.concurrency = concurrency
         self.keep_warm_seconds = keep_warm_seconds
         self.max_pending_tasks = max_pending_tasks
         self.max_containers = max_containers
         self.retries = retries
@@ -77,14 +77,26 @@
 
         if on_start is not None:
             self._map_callable_to_attr(attr="on_start", func=on_start)
 
         self._gateway_stub: Optional[GatewayServiceStub] = None
         self.syncer: FileSyncer = FileSyncer(self.gateway_stub)
 
+    def _parse_memory(self, memory_str: str) -> int:
+        """Parse memory str (with units) to megabytes."""
+
+        if memory_str.lower().endswith("mi"):
+            return int(memory_str[:-2])
+        elif memory_str.lower().endswith("gb"):
+            return int(memory_str[:-2]) * 1000
+        elif memory_str.lower().endswith("gi"):
+            return int(memory_str[:-2]) * 1024
+        else:
+            raise ValueError("Unsupported memory format")
+
     @property
     def gateway_stub(self) -> GatewayServiceStub:
         if not self._gateway_stub:
             self._gateway_stub = GatewayServiceStub(self.channel)
         return self._gateway_stub
 
     def _parse_cpu_to_millicores(self, cpu: Union[float, str]) -> int:
```

### Comparing `beta9-0.1.7/src/beta9/abstractions/container.py` & `beta9-0.1.8/src/beta9/abstractions/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 class Container(RunnerAbstraction):
     """
     Container allows you to run arbitrary commands in a remote container.
 
     Parameters:
         cpu (Union[int, float, str]):
             The number of CPU cores allocated to the container. Default is 1.0.
-        memory (int):
+        memory (Union[int, str]):
             The amount of memory allocated to the container. It should be specified in
-            megabytes (e.g., 128 for 128 megabytes). Default is 128.
+            MiB, or as a string with units (e.g. "1Gi"). Default is 128 MiB.
         gpu (Union[GpuType, str]):
             The type or name of the GPU device to be used for GPU-accelerated tasks. If not
             applicable or no GPU required, leave it empty. Default is [GpuType.NoGPU](#gputype).
         image (Union[Image, dict]):
             The container image used for the task execution. Default is [Image](#image).
         volumes (Optional[List[Volume]]):
             A list of volumes to be mounted to the container. Default is None.
@@ -47,15 +47,15 @@
             print(exit_code)
         ```
     """
 
     def __init__(
         self,
         cpu: Union[int, float, str] = 1.0,
-        memory: int = 128,
+        memory: Union[int, str] = 128,
         gpu: str = "",
         image: Image = Image(),
         volumes: Optional[List[Volume]] = None,
         name: Optional[str] = None,
     ) -> None:
         super().__init__(cpu=cpu, memory=memory, gpu=gpu, image=image, volumes=volumes)
```

### Comparing `beta9-0.1.7/src/beta9/abstractions/endpoint.py` & `beta9-0.1.8/src/beta9/abstractions/endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     """
     Decorator which allows you to create a web endpoint out of the decorated function.
     Tasks are invoked synchronously as HTTP requests.
 
     Parameters:
         cpu (Union[int, float, str]):
             The number of CPU cores allocated to the container. Default is 1.0.
-        memory (int):
+        memory (Union[int, str]):
             The amount of memory allocated to the container. It should be specified in
-            megabytes (e.g., 128 for 128 megabytes). Default is 128.
+            MiB, or as a string with units (e.g. "1Gi"). Default is 128 MiB.
         gpu (Union[GpuType, str]):
             The type or name of the GPU device to be used for GPU-accelerated tasks. If not
             applicable or no GPU required, leave it empty. Default is [GpuType.NoGPU](#gputype).
         image (Union[Image, dict]):
             The container image used for the task execution. Default is [Image](#image).
         volumes (Optional[List[Volume]]):
             A list of volumes to be mounted to the endpoint. Default is None.
@@ -76,15 +76,15 @@
             return {"result": result}
         ```
     """
 
     def __init__(
         self,
         cpu: Union[int, float, str] = 1.0,
-        memory: int = 128,
+        memory: Union[int, str] = 128,
         gpu: str = "",
         image: Image = Image(),
         timeout: int = 180,
         concurrency: int = 1,
         max_containers: int = 1,
         keep_warm_seconds: int = 300,
         max_pending_tasks: int = 100,
@@ -181,15 +181,15 @@
         try:
             async for r in self.parent.endpoint_stub.start_endpoint_serve(
                 StartEndpointServeRequest(
                     stub_id=self.parent.stub_id,
                 )
             ):
                 if r.output != "":
-                    terminal.detail(r.output.strip())
+                    terminal.detail(r.output, end="")
 
                 if r.done or r.exit_code != 0:
                     last_response = r
                     break
 
             if last_response is None or not last_response.done or last_response.exit_code != 0:
                 terminal.error("Serve container failed ☠️")
```

### Comparing `beta9-0.1.7/src/beta9/abstractions/function.py` & `beta9-0.1.8/src/beta9/abstractions/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 class Function(RunnerAbstraction):
     """
     Decorator which allows you to run the decorated function in a remote container.
 
     Parameters:
         cpu (Union[int, float, str]):
             The number of CPU cores allocated to the container. Default is 1.0.
-        memory (int):
+        memory (Union[int, str]):
             The amount of memory allocated to the container. It should be specified in
-            megabytes (e.g., 128 for 128 megabytes). Default is 128.
+            MiB, or as a string with units (e.g. "1Gi"). Default is 128 MiB.
         gpu (Union[GpuType, str]):
             The type or name of the GPU device to be used for GPU-accelerated tasks. If not
             applicable or no GPU required, leave it empty. Default is [GpuType.NoGPU](#gputype).
         image (Union[Image, dict]):
             The container image used for the task execution. Default is [Image](#image).
         timeout (Optional[int]):
             The maximum number of seconds a task can run before it times out.
@@ -63,15 +63,15 @@
             print(result)
         ```
     """
 
     def __init__(
         self,
         cpu: Union[int, float, str] = 1.0,
-        memory: int = 128,
+        memory: Union[int, str] = 128,
         gpu: str = "",
         image: Image = Image(),
         timeout: int = 3600,
         retries: int = 3,
         callback_url: Optional[str] = "",
         volumes: Optional[List[Volume]] = None,
     ) -> None:
@@ -131,15 +131,15 @@
         async for r in self.parent.function_stub.function_invoke(
             FunctionInvokeRequest(
                 stub_id=self.parent.stub_id,
                 args=args,
             )
         ):
             if r.output != "":
-                terminal.detail(r.output.strip())
+                terminal.detail(r.output, end="")
 
             if r.done or r.exit_code != 0:
                 last_response = r
                 break
 
         if last_response is None or not last_response.done or last_response.exit_code != 0:
             terminal.error("Function failed ☠️")
```

### Comparing `beta9-0.1.7/src/beta9/abstractions/image.py` & `beta9-0.1.8/src/beta9/abstractions/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                 BuildImageRequest(
                     python_packages=self.python_packages,
                     python_version=self.python_version,
                     commands=self.commands,
                     existing_image_uri=self.base_image,
                 )
             ):
-                terminal.detail(r.msg)
+                terminal.detail(r.msg, end="")
 
                 if r.done:
                     last_response = r
                     break
 
             return last_response
```

### Comparing `beta9-0.1.7/src/beta9/abstractions/map.py` & `beta9-0.1.8/src/beta9/abstractions/map.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/abstractions/queue.py` & `beta9-0.1.8/src/beta9/abstractions/queue.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/abstractions/taskqueue.py` & `beta9-0.1.8/src/beta9/abstractions/taskqueue.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     Decorator which allows you to create a task queue out of the decorated function. The tasks are executed
     asynchronously, in remote containers. You can interact with the task queue either through an API (when deployed), or directly
     in python through the .put() method.
 
     Parameters:
         cpu (Union[int, float, str]):
             The number of CPU cores allocated to the container. Default is 1.0.
-        memory (int):
+        memory (Union[int, str]):
             The amount of memory allocated to the container. It should be specified in
-            megabytes (e.g., 128 for 128 megabytes). Default is 128.
+            MiB, or as a string with units (e.g. "1Gi"). Default is 128 MiB.
         gpu (Union[GpuType, str]):
             The type or name of the GPU device to be used for GPU-accelerated tasks. If not
             applicable or no GPU required, leave it empty. Default is [GpuType.NoGPU](#gputype).
         image (Union[Image, dict]):
             The container image used for the task execution. Default is [Image](#image).
         timeout (Optional[int]):
             The maximum number of seconds a task can run before it times out.
@@ -83,15 +83,15 @@
 
         ```
     """
 
     def __init__(
         self,
         cpu: Union[int, float, str] = 1.0,
-        memory: int = 128,
+        memory: Union[int, str] = 128,
         gpu: str = "",
         image: Image = Image(),
         timeout: int = 3600,
         retries: int = 3,
         concurrency: int = 1,
         max_containers: int = 1,
         keep_warm_seconds: int = 10,
@@ -199,15 +199,15 @@
         try:
             async for r in self.parent.taskqueue_stub.start_task_queue_serve(
                 StartTaskQueueServeRequest(
                     stub_id=self.parent.stub_id,
                 )
             ):
                 if r.output != "":
-                    terminal.detail(r.output.strip())
+                    terminal.detail(r.output, end="")
 
                 if r.done or r.exit_code != 0:
                     last_response = r
                     break
 
             if last_response is None or not last_response.done or last_response.exit_code != 0:
                 terminal.error("Serve container failed ☠️")
```

### Comparing `beta9-0.1.7/src/beta9/abstractions/volume.py` & `beta9-0.1.8/src/beta9/abstractions/volume.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/channel.py` & `beta9-0.1.8/src/beta9/channel.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/cli/config.py` & `beta9-0.1.8/src/beta9/cli/config.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/cli/deployment.py` & `beta9-0.1.8/src/beta9/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/cli/extraclick.py` & `beta9-0.1.8/src/beta9/cli/extraclick.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import functools
 import inspect
+import sys
 import textwrap
 from gettext import gettext
 from typing import Any, Callable, Optional
 
 import click
 
 from ..abstractions import base as base_abstraction
@@ -105,14 +106,17 @@
                 r[command] = source
         return r
 
     def invoke(self, ctx: click.Context) -> Any:
         if ctx.protected_args:
             if group := self.sources_map.get(ctx.protected_args[0]):
                 group.invoke(ctx)
+            else:
+                print(self.get_help(ctx))
+                sys.exit(1)
         else:
             super().invoke(ctx)
 
     def format_commands(self, ctx: click.Context, formatter: click.HelpFormatter) -> None:
         """
         Extra format methods for multi methods that adds all the commands after
         the options.
```

### Comparing `beta9-0.1.7/src/beta9/cli/main.py` & `beta9-0.1.8/src/beta9/cli/main.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/cli/task.py` & `beta9-0.1.8/src/beta9/cli/task.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/cli/volume.py` & `beta9-0.1.8/src/beta9/cli/volume.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/clients/container/__init__.py` & `beta9-0.1.8/src/beta9/clients/container/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/clients/endpoint/__init__.py` & `beta9-0.1.8/src/beta9/clients/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/clients/function/__init__.py` & `beta9-0.1.8/src/beta9/clients/function/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/clients/gateway/__init__.py` & `beta9-0.1.8/src/beta9/clients/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/clients/image/__init__.py` & `beta9-0.1.8/src/beta9/clients/image/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/clients/map/__init__.py` & `beta9-0.1.8/src/beta9/clients/map/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/clients/simplequeue/__init__.py` & `beta9-0.1.8/src/beta9/clients/simplequeue/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/clients/taskqueue/__init__.py` & `beta9-0.1.8/src/beta9/clients/taskqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/clients/volume/__init__.py` & `beta9-0.1.8/src/beta9/clients/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/config.py` & `beta9-0.1.8/src/beta9/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,25 @@
 
 
 def get_config_context(name: str = DEFAULT_CONTEXT_NAME) -> ConfigContext:
     config = load_config()
     if name in config:
         return config[name]
 
+    gateway_host = os.getenv("BETA9_GATEWAY_HOST", None)
+    gateway_port = os.getenv("BETA9_GATEWAY_PORT", None)
+    token = os.getenv("BETA9_TOKEN", None)
+
+    if gateway_host and gateway_port and token:
+        return ConfigContext(
+            token=token,
+            gateway_host=gateway_host,
+            gateway_port=gateway_port,
+        )
+
     terminal.header(f"Context '{name}' does not exist. Let's try setting it up.")
     _, config = prompt_for_config_context(name=name)
     return config
 
 
 def prompt_for_config_context(
     name: Optional[str] = None,
```

### Comparing `beta9-0.1.7/src/beta9/logging.py` & `beta9-0.1.8/src/beta9/logging.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,21 +16,24 @@
     def __exit__(self, exc_type, exc_value, traceback):
         sys.stdout = sys.__stdout__
         sys.stderr = sys.__stderr__
         return False
 
     def write(self, buf: str):
         try:
-            for line in buf.rstrip().splitlines():
+            for line in buf.splitlines():
+                if line == "":
+                    continue
+
                 log_record = {
-                    "message": line,
+                    "message": f"{line}\n",
                     **self.ctx,
                 }
 
-                self.stream.write(json.dumps(log_record) + "\n")
+                self.stream.write(json.dumps(log_record))
         except BaseException:
             self.stream.write(buf)
 
     def flush(self):
         return self.stream.flush()
 
     def fileno(self) -> int:
```

### Comparing `beta9-0.1.7/src/beta9/runner/common.py` & `beta9-0.1.8/src/beta9/runner/common.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/runner/container.py` & `beta9-0.1.8/src/beta9/runner/container.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/runner/endpoint.py` & `beta9-0.1.8/src/beta9/runner/endpoint.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/runner/function.py` & `beta9-0.1.8/src/beta9/runner/function.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/runner/serve.py` & `beta9-0.1.8/src/beta9/runner/serve.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/runner/taskqueue.py` & `beta9-0.1.8/src/beta9/runner/taskqueue.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/sync.py` & `beta9-0.1.8/src/beta9/sync.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/terminal.py` & `beta9-0.1.8/src/beta9/terminal.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/src/beta9/type.py` & `beta9-0.1.8/src/beta9/type.py`

 * *Files identical despite different names*

### Comparing `beta9-0.1.7/PKG-INFO` & `beta9-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: beta9
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: beam.cloud
 Author-email: support@beam.cloud
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asgiref (>=3.7.2,<4.0.0)
 Requires-Dist: betterproto[compiler] (==2.0.0b6)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cloudpickle (>=3.0.0,<4.0.0)
 Requires-Dist: croniter (>=2.0.3,<3.0.0)
 Requires-Dist: fastapi (>=0.110.2,<0.111.0)
 Requires-Dist: grpcio (>=1.60.0,<2.0.0)
```

