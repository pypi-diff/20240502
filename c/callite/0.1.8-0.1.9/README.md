# Comparing `tmp/callite-0.1.8.tar.gz` & `tmp/callite-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callite-0.1.8.tar", max compression
+gzip compressed data, was "callite-0.1.9.tar", max compression
```

## Comparing `callite-0.1.8.tar` & `callite-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     2774 2024-04-22 12:10:31.006206 callite-0.1.8/README.md
--rw-r--r--   0        0        0      190 2024-04-22 12:10:31.010206 callite-0.1.8/callite/__init__.py
--rw-r--r--   0        0        0       50 2024-04-22 12:10:31.010206 callite-0.1.8/callite/client/__init__.py
--rw-r--r--   0        0        0     2685 2024-04-22 12:10:31.010206 callite-0.1.8/callite/client/rpc_client.py
--rw-r--r--   0        0        0      176 2024-04-22 12:10:31.010206 callite-0.1.8/callite/rpctypes/__init__.py
--rw-r--r--   0        0        0      311 2024-04-22 12:10:31.010206 callite-0.1.8/callite/rpctypes/message_base.py
--rw-r--r--   0        0        0      833 2024-04-22 12:10:31.010206 callite-0.1.8/callite/rpctypes/request.py
--rw-r--r--   0        0        0      541 2024-04-22 12:10:31.010206 callite-0.1.8/callite/rpctypes/response.py
--rw-r--r--   0        0        0      267 2024-04-22 12:10:31.010206 callite-0.1.8/callite/rpctypes/rpc_exception.py
--rw-r--r--   0        0        0       82 2024-04-22 12:10:31.010206 callite-0.1.8/callite/server/__init__.py
--rw-r--r--   0        0        0     4202 2024-04-22 12:10:31.010206 callite-0.1.8/callite/server/rpc_server.py
--rw-r--r--   0        0        0       62 2024-04-22 12:10:31.010206 callite-0.1.8/callite/shared/__init__.py
--rw-r--r--   0        0        0      657 2024-04-22 12:10:31.010206 callite-0.1.8/callite/shared/redis_connection.py
--rw-r--r--   0        0        0      432 2024-04-22 12:10:31.010206 callite-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 callite-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-02 16:02:34.159564 callite-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2708 2024-05-02 16:02:34.159564 callite-0.1.9/README.md
+-rw-r--r--   0        0        0      190 2024-05-02 16:02:34.159564 callite-0.1.9/callite/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-02 16:02:34.159564 callite-0.1.9/callite/client/__init__.py
+-rw-r--r--   0        0        0     2685 2024-05-02 16:02:34.159564 callite-0.1.9/callite/client/rpc_client.py
+-rw-r--r--   0        0        0      176 2024-05-02 16:02:34.159564 callite-0.1.9/callite/rpctypes/__init__.py
+-rw-r--r--   0        0        0      311 2024-05-02 16:02:34.159564 callite-0.1.9/callite/rpctypes/message_base.py
+-rw-r--r--   0        0        0      833 2024-05-02 16:02:34.159564 callite-0.1.9/callite/rpctypes/request.py
+-rw-r--r--   0        0        0      541 2024-05-02 16:02:34.159564 callite-0.1.9/callite/rpctypes/response.py
+-rw-r--r--   0        0        0      267 2024-05-02 16:02:34.159564 callite-0.1.9/callite/rpctypes/rpc_exception.py
+-rw-r--r--   0        0        0       82 2024-05-02 16:02:34.159564 callite-0.1.9/callite/server/__init__.py
+-rw-r--r--   0        0        0     4202 2024-05-02 16:02:34.159564 callite-0.1.9/callite/server/rpc_server.py
+-rw-r--r--   0        0        0       62 2024-05-02 16:02:34.159564 callite-0.1.9/callite/shared/__init__.py
+-rw-r--r--   0        0        0      657 2024-05-02 16:02:34.159564 callite-0.1.9/callite/shared/redis_connection.py
+-rw-r--r--   0        0        0      513 2024-05-02 16:02:34.159564 callite-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3227 1970-01-01 00:00:00.000000 callite-0.1.9/PKG-INFO
```

### Comparing `callite-0.1.8/README.md` & `callite-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 ```python
 from callite.server import RPCService
 
 
 class Main:
     def __init__(self):
-        self.service = "service"
-        self.redis_url = "redis://redis:6379/0"
-        self.rpc_service = RPCService(self.redis_url, self.service)
+        service = "service"
+        redis_url = "redis://redis:6379/0"
+        self.rpc_service = RPCService(redis_url, service)
 
     def run(self):
         @self.rpc_service.register
         def healthcheck():
             return "OK"
 
         self.rpc_service.run_forever()
@@ -53,33 +53,30 @@
 ```python
 import time
 from callite.client.rpc_client import RPCClient
 
 
 class Healthcheck():
     def __init__(self):
-        self.status = "OK"
         self.r = RPCClient("redis://redis:6379/0", "service")
 
     def get_status(self):
         start = time.perf_counter()
-        self.status = self.r.execute('healthcheck')
+        status = self.r.execute('healthcheck')
         end = time.perf_counter()
         print(f"Healthcheck took {end - start:0.4f} seconds")
-        return self.status
+        return status
 
     def check(self):
         return self.get_status()
 
 
 if __name__ == "__main__":
     Healthcheck().check()
 ```
 
 You can pass arguments and keyword arguments to the `execute` method as follows:
 
 ```python
-self.status = self.r.execute('healthcheck', [True], {'a': 1, 'b': 2})
+response = self.r.execute('foo', [True], {'paramX': 1, 'paramY': 2})
 ```
-
-This setup allows for efficient communication between components of a distributed system, promoting modularity and scalability.
-```
+This setup allows for efficient communication between components of a distributed system, promoting modularity and scalability.
```

### Comparing `callite-0.1.8/callite/client/rpc_client.py` & `callite-0.1.9/callite/client/rpc_client.py`

 * *Files identical despite different names*

### Comparing `callite-0.1.8/callite/rpctypes/request.py` & `callite-0.1.9/callite/rpctypes/request.py`

 * *Files identical despite different names*

### Comparing `callite-0.1.8/callite/rpctypes/response.py` & `callite-0.1.9/callite/rpctypes/response.py`

 * *Files identical despite different names*

### Comparing `callite-0.1.8/callite/server/rpc_server.py` & `callite-0.1.9/callite/server/rpc_server.py`

 * *Files identical despite different names*

### Comparing `callite-0.1.8/callite/shared/redis_connection.py` & `callite-0.1.9/callite/shared/redis_connection.py`

 * *Files identical despite different names*

### Comparing `callite-0.1.8/PKG-INFO` & `callite-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: callite
-Version: 0.1.8
+Version: 0.1.9
 Summary: Slim Redis RPC implementation
+Home-page: https://www.gri.ai
 License: MIT
 Author: Emrah Gozcu
 Author-email: gozcu@gri.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: redis (>=5.0.3,<6.0.0)
+Project-URL: Repository, https://github.com/gri-ai/callite
 Description-Content-Type: text/markdown
 
 # Callite
 
 callite is a lightweight Remote Procedure Call (RPC) implementation over Redis, designed to facilitate communication between different components of a distributed system. It minimizes dependencies and offers a simple yet effective solution for decoupling complex systems, thus alleviating potential library conflicts.
 
 ## Setting up Callite
@@ -35,17 +37,17 @@
 
 ```python
 from callite.server import RPCService
 
 
 class Main:
     def __init__(self):
-        self.service = "service"
-        self.redis_url = "redis://redis:6379/0"
-        self.rpc_service = RPCService(self.redis_url, self.service)
+        service = "service"
+        redis_url = "redis://redis:6379/0"
+        self.rpc_service = RPCService(redis_url, service)
 
     def run(self):
         @self.rpc_service.register
         def healthcheck():
             return "OK"
 
         self.rpc_service.run_forever()
@@ -69,33 +71,30 @@
 ```python
 import time
 from callite.client.rpc_client import RPCClient
 
 
 class Healthcheck():
     def __init__(self):
-        self.status = "OK"
         self.r = RPCClient("redis://redis:6379/0", "service")
 
     def get_status(self):
         start = time.perf_counter()
-        self.status = self.r.execute('healthcheck')
+        status = self.r.execute('healthcheck')
         end = time.perf_counter()
         print(f"Healthcheck took {end - start:0.4f} seconds")
-        return self.status
+        return status
 
     def check(self):
         return self.get_status()
 
 
 if __name__ == "__main__":
     Healthcheck().check()
 ```
 
 You can pass arguments and keyword arguments to the `execute` method as follows:
 
 ```python
-self.status = self.r.execute('healthcheck', [True], {'a': 1, 'b': 2})
+response = self.r.execute('foo', [True], {'paramX': 1, 'paramY': 2})
 ```
-
 This setup allows for efficient communication between components of a distributed system, promoting modularity and scalability.
-```
```

