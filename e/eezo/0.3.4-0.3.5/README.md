# Comparing `tmp/eezo-0.3.4.tar.gz` & `tmp/eezo-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eezo-0.3.4.tar", last modified: Thu Apr 18 20:19:16 2024, max compression
+gzip compressed data, was "eezo-0.3.5.tar", last modified: Thu May  2 21:17:49 2024, max compression
```

## Comparing `eezo-0.3.4.tar` & `eezo-0.3.5.tar`

### file list

```diff
@@ -1,35 +1,31 @@
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-18 20:19:16.358442 eezo-0.3.4/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      914 2024-04-18 20:19:16.358329 eezo-0.3.4/PKG-INFO
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1558 2024-03-19 14:53:56.000000 eezo-0.3.4/README.md
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-18 20:19:16.355774 eezo-0.3.4/eezo/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       86 2024-04-18 09:35:35.000000 eezo-0.3.4/eezo/__init__.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-18 20:19:16.356762 eezo-0.3.4/eezo/agent/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       52 2024-04-17 18:38:28.000000 eezo-0.3.4/eezo/agent/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     8043 2024-04-18 07:45:30.000000 eezo-0.3.4/eezo/agent/agent.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     2948 2024-04-18 07:26:56.000000 eezo-0.3.4/eezo/agent/agents.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)    13674 2024-04-18 20:17:35.000000 eezo-0.3.4/eezo/async_client.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)    14633 2024-04-18 20:17:55.000000 eezo-0.3.4/eezo/client.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)    12603 2024-04-18 20:14:27.000000 eezo-0.3.4/eezo/connector.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      355 2024-04-17 22:28:24.000000 eezo-0.3.4/eezo/errors.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-18 20:19:16.357410 eezo-0.3.4/eezo/interface/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      106 2024-04-10 17:54:01.000000 eezo-0.3.4/eezo/interface/__init__.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-18 20:19:16.358183 eezo-0.3.4/eezo/interface/components/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      329 2024-03-19 12:03:08.000000 eezo-0.3.4/eezo/interface/components/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1743 2024-03-19 12:03:08.000000 eezo-0.3.4/eezo/interface/components/chart.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      159 2024-03-19 12:03:08.000000 eezo-0.3.4/eezo/interface/components/component.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      243 2024-03-19 12:03:08.000000 eezo-0.3.4/eezo/interface/components/image.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      246 2024-03-19 12:03:08.000000 eezo-0.3.4/eezo/interface/components/text.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      283 2024-03-19 12:03:08.000000 eezo-0.3.4/eezo/interface/components/youtube_video.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     4073 2024-04-18 09:09:39.000000 eezo-0.3.4/eezo/interface/interface.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     5276 2024-04-18 09:16:48.000000 eezo-0.3.4/eezo/interface/interface_async.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     4502 2024-04-17 22:58:05.000000 eezo-0.3.4/eezo/interface/message.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     3509 2024-04-18 09:46:52.000000 eezo-0.3.4/eezo/state.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     3700 2024-04-18 09:40:44.000000 eezo-0.3.4/eezo/state_async.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-18 20:19:16.356305 eezo-0.3.4/eezo.egg-info/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      914 2024-04-18 20:19:16.000000 eezo-0.3.4/eezo.egg-info/PKG-INFO
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      680 2024-04-18 20:19:16.000000 eezo-0.3.4/eezo.egg-info/SOURCES.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)        1 2024-04-18 20:19:16.000000 eezo-0.3.4/eezo.egg-info/dependency_links.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      367 2024-04-18 20:19:16.000000 eezo-0.3.4/eezo.egg-info/requires.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)        5 2024-04-18 20:19:16.000000 eezo-0.3.4/eezo.egg-info/top_level.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       38 2024-04-18 20:19:16.358474 eezo-0.3.4/setup.cfg
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1601 2024-04-18 20:19:08.000000 eezo-0.3.4/setup.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-05-02 21:17:49.096594 eezo-0.3.5/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      914 2024-05-02 21:17:49.096472 eezo-0.3.5/PKG-INFO
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1453 2024-05-02 20:59:24.000000 eezo-0.3.5/README.md
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-05-02 21:17:49.092076 eezo-0.3.5/eezo/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       35 2024-04-30 12:43:00.000000 eezo-0.3.5/eezo/__init__.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-05-02 21:17:49.093529 eezo-0.3.5/eezo/agent/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       52 2024-04-17 18:38:28.000000 eezo-0.3.5/eezo/agent/__init__.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     8043 2024-04-18 07:45:30.000000 eezo-0.3.5/eezo/agent/agent.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     2948 2024-04-18 07:26:56.000000 eezo-0.3.5/eezo/agent/agents.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)    23220 2024-05-02 20:51:44.000000 eezo-0.3.5/eezo/client.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      355 2024-04-17 22:28:24.000000 eezo-0.3.5/eezo/errors.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-05-02 21:17:49.094349 eezo-0.3.5/eezo/interface/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       62 2024-04-30 12:43:58.000000 eezo-0.3.5/eezo/interface/__init__.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-05-02 21:17:49.096159 eezo-0.3.5/eezo/interface/components/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      329 2024-03-19 12:03:08.000000 eezo-0.3.5/eezo/interface/components/__init__.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1743 2024-03-19 12:03:08.000000 eezo-0.3.5/eezo/interface/components/chart.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      159 2024-03-19 12:03:08.000000 eezo-0.3.5/eezo/interface/components/component.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      338 2024-04-23 10:54:16.000000 eezo-0.3.5/eezo/interface/components/image.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      343 2024-04-23 10:54:12.000000 eezo-0.3.5/eezo/interface/components/text.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      388 2024-04-23 10:54:07.000000 eezo-0.3.5/eezo/interface/components/youtube_video.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     4205 2024-05-02 20:51:35.000000 eezo-0.3.5/eezo/interface/interface.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     4502 2024-04-17 22:58:05.000000 eezo-0.3.5/eezo/interface/message.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     3499 2024-04-30 13:09:32.000000 eezo-0.3.5/eezo/state.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-05-02 21:17:49.092860 eezo-0.3.5/eezo.egg-info/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      914 2024-05-02 21:17:49.000000 eezo-0.3.5/eezo.egg-info/PKG-INFO
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      587 2024-05-02 21:17:49.000000 eezo-0.3.5/eezo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)        1 2024-05-02 21:17:49.000000 eezo-0.3.5/eezo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      367 2024-05-02 21:17:49.000000 eezo-0.3.5/eezo.egg-info/requires.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)        5 2024-05-02 21:17:49.000000 eezo-0.3.5/eezo.egg-info/top_level.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       38 2024-05-02 21:17:49.096634 eezo-0.3.5/setup.cfg
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1601 2024-05-02 21:17:44.000000 eezo-0.3.5/setup.py
```

### Comparing `eezo-0.3.4/PKG-INFO` & `eezo-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eezo
-Version: 0.3.4
+Version: 0.3.5
 Summary: Eezo enables you to build and supervise your AI agent workforces.
 Home-page: UNKNOWN
 Author: Daniel Schoenbohm
 Author-email: daniel@eezo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `eezo-0.3.4/README.md` & `eezo-0.3.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -53,22 +53,14 @@
 pip install -r requirements.txt
 ```
 
 ## Testing
 
 Ensure everything is set up correctly by running the tests.
 
-### Asynchronous Client
-
-Run the asynchronous client tests with:
-
-```sh
-python test_async_client.py
-```
-
 ### Synchronous Client
 
 Run the synchronous client tests with:
 
 ```sh
 python test_client.py
 ```
```

### Comparing `eezo-0.3.4/eezo/agent/agent.py` & `eezo-0.3.5/eezo/agent/agent.py`

 * *Files identical despite different names*

### Comparing `eezo-0.3.4/eezo/agent/agents.py` & `eezo-0.3.5/eezo/agent/agents.py`

 * *Files identical despite different names*

### Comparing `eezo-0.3.4/eezo/client.py` & `eezo-0.3.5/eezo/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from .errors import AuthorizationError, RequestError, ResourceNotFoundError
 from typing import Optional, Callable, Dict, List, Any
 from requests.packages.urllib3.util.retry import Retry
 from watchdog.events import FileSystemEventHandler
+from .interface.interface import Interface
 from requests.adapters import HTTPAdapter
 from .interface.interface import Message
 from watchdog.observers import Observer
-from .connector import Connector
 from .agent import Agents, Agent
 
 import concurrent.futures
+import socketio
 import requests
 import logging
 import sys
+import time
+import uuid
+import traceback
 import os
 
 from .state import StateProxy
 
 SERVER = "https://api-service-bofkvbi4va-ey.a.run.app"
 if os.environ.get("EEZO_DEV_MODE") == "True":
     print("Running in dev mode")
@@ -38,14 +42,42 @@
 
 class RestartHandler(FileSystemEventHandler):
     def on_modified(self, event):
         if event.src_path.endswith(".py"):
             os.execl(sys.executable, sys.executable, *sys.argv)
 
 
+class JobCompleted:
+    def __init__(
+        self,
+        job_id: str,
+        result: Dict,
+        success: bool,
+        error=None,
+        traceback=None,
+        error_tag=None,
+    ):
+        self.result = result
+        self.job_id = job_id
+        self.success = success
+        self.error = error
+        self.traceback = traceback
+        self.error_tag = error_tag
+
+    def to_dict(self):
+        return {
+            "result": self.result,
+            "job_id": self.job_id,
+            "success": self.success,
+            "error": self.error,
+            "traceback": self.traceback,
+            "error_tag": self.error_tag,
+        }
+
+
 class Client:
     def __init__(self, api_key: Optional[str] = None, logger: bool = False) -> None:
         """Initialize the Client with an optional API key and a logger flag.
 
         Args:
             api_key (Optional[str]): The API key for authentication. If None, it defaults to the EEZO_API_KEY environment variable.
             logger (bool): Flag to enable logging.
@@ -60,27 +92,31 @@
         )
         self.observer = Observer()
         self.api_key: str = (
             api_key if api_key is not None else os.getenv("EEZO_API_KEY")
         )
         self.logger: bool = logger
         if self.logger:
-            logging.basicConfig(level=logging.INFO)
+            logging.basicConfig(level=logging.INFO, format="%(asctime)s %(message)s")
         self.state_was_loaded = False
-        self.user_id: Optional[str] = os.environ.get("EEZO_USER_ID")
-        self.token: Optional[str] = os.environ.get("EEZO_TOKEN")
+        self.user_id: Optional[str] = os.environ.get("EEZO_USER_ID", None)
+        self.auth_token: Optional[str] = os.environ.get("EEZO_TOKEN", None)
+        self.job_responses: Dict[str, str] = {}
+        self.run_loop = True
+        self.sio: Optional[socketio.Client] = None
+        self.emit_buffer: List[Dict] = []
 
         self.session = self._configure_session()
 
-        if not self.user_id or not self.token:
-            self.user_id, self.token = self._request(
-                "POST", AUTH_URL, {"api_key": self.api_key}
-            )
+        if not self.user_id or not self.auth_token:
+            result = self._request("POST", AUTH_URL, {"api_key": self.api_key})
+            self.user_id = result.get("user_id")
+            self.auth_token = result.get("token")
             os.environ["EEZO_USER_ID"] = self.user_id
-            os.environ["EEZO_TOKEN"] = self.token
+            os.environ["EEZO_TOKEN"] = self.auth_token
         else:
             logging.info("Already authenticated")
 
         if not self.api_key:
             raise ValueError("Eezo api_key is required")
 
         self._state_proxy: StateProxy = StateProxy(self)
@@ -113,44 +149,242 @@
         Returns:
             Callable: The decorator function.
         """
 
         def decorator(func: Callable) -> Callable:
             if not callable(func):
                 raise TypeError(f"Expected a callable, got {type(func)} instead")
-            self.connector_functions[connector_id] = func
+            self.add_connector(connector_id, func)
             return func
 
         return decorator
 
+    def add_connector(self, connector_id: str, func: Callable) -> None:
+        """Add a connector function to the client.
+
+        Args:
+            connector_id (str): The identifier for the connector.
+            func (Callable): The connector function to add.
+        """
+        self.connector_functions[connector_id] = func
+
+    def __run(self, skill_id: str, current_job_id: str, **kwargs):
+        """Invoke a skill and get the result."""
+        if not skill_id:
+            raise ValueError("skill_id is required")
+
+        job_id = str(uuid.uuid4())
+        self.sio.emit(
+            "invoke_skill",
+            {
+                "new_job_id": job_id,
+                "skill_id": skill_id,
+                "skill_payload": kwargs,
+                "job_id": current_job_id,
+            },
+        )
+
+        while True:
+            if job_id in self.job_responses:
+                response = self.job_responses.pop(job_id)
+
+                if not response.get("success", True):
+                    logging.info(
+                        f"<< Sub Job {response['id']} failed:\n{response['traceback']}."
+                    )
+                    raise Exception(response["error"])
+
+                logging.info(f"<< Sub Job {job_id} \033[32mcompleted\033[0m.")
+                return response["result"]
+            else:
+                time.sleep(1)
+
+    def __emit_safe(self, event: str, connector_id: str, data: Dict) -> None:
+        if self.sio.connected:
+            self.sio.emit(event, data)
+        else:
+            logging.info(
+                f"Connection down. Buffering data for '{event}' for connector {connector_id}."
+            )
+            self.emit_buffer.append(
+                {
+                    "data": data,
+                    "event": event,
+                    "connector_id": connector_id,
+                    "job_id": data["job_id"],
+                }
+            )
+
+    def __execute_job(self, job_obj):
+        job_id, connector_id, payload = (
+            job_obj["job_id"],
+            job_obj["connector_id"],
+            job_obj["job_payload"],
+        )
+        logging.info(f"<< Job {job_id} received for agent {connector_id}: {payload}")
+        # Create an interface object that the connector function can use to interact with the Eezo server
+
+        i: Interface = Interface(
+            job_id=job_id,
+            user_id=self.user_id,
+            api_key=self.api_key,
+            cb_send_message=lambda p: self.__emit_safe(
+                "direct_message", connector_id, p
+            ),
+            cb_run=self.__run,
+        )
+
+        def execute():
+            try:
+                self.__emit_safe(
+                    "confirm_job_request",
+                    connector_id,
+                    {"connector_id": connector_id, "job_id": job_id},
+                )
+
+                try:
+                    result = self.connector_functions[connector_id](i, **payload)
+                except Exception as e:
+                    logging.info(
+                        f" ✖ Agent {connector_id} failed processing job {job_id}:\n{traceback.format_exc()}"
+                    )
+                    job_completed = JobCompleted(
+                        job_id=job_id,
+                        result=None,
+                        success=False,
+                        error=str(e),
+                        traceback=str(traceback.format_exc()),
+                        error_tag="Connector Error",
+                    ).to_dict()
+                    self.__emit_safe("job_completed", connector_id, job_completed)
+
+                    return
+
+                job_completed = JobCompleted(job_id, result, True).to_dict()
+
+                self.__emit_safe("job_completed", connector_id, job_completed)
+            except Exception as e:
+                logging.info(
+                    f" ✖ Client error while connector {connector_id} was processing job {job_id}:\n{traceback.format_exc()}"
+                )
+                job_completed = JobCompleted(
+                    job_id=job_id,
+                    result=None,
+                    success=False,
+                    error=str(e),
+                    traceback=str(traceback.format_exc()),
+                    error_tag="Client Error",
+                ).to_dict()
+                self.__emit_safe("job_completed", connector_id, job_completed)
+
+        self.executor.submit(execute)
+
     def connect(self) -> None:
         """Connect to the Eezo server and start the client. This involves scheduling
         tasks in a thread pool executor and handling responses."""
         try:
             self.observer.schedule(RestartHandler(), ".", recursive=False)
             self.observer.start()
-            self.futures = []
-            self.job_responses: Dict[str, str] = {}
 
-            for connector_id, func in self.connector_functions.items():
-                c = Connector(
-                    self.api_key, connector_id, func, self.job_responses, self.logger
+            self.sio = socketio.Client(
+                reconnection_attempts=0,
+                reconnection_delay_max=10,
+                reconnection_delay=1,
+                engineio_logger=False,
+                logger=False,
+            )
+
+            @self.sio.event
+            def connect():
+                connector_ids = list(self.connector_functions.keys())
+                self.sio.emit(
+                    "authenticate",
+                    {
+                        "token": self.auth_token,
+                        "cids": connector_ids,
+                        "key": self.api_key,
+                    },
                 )
-                c.authenticate()
-                self.futures.append(self.executor.submit(c.connect))
 
-            for future in self.futures:
-                future.result()
+            if not self.auth_token:
+                raise Exception("Not authenticated")
+
+            def auth_error(message: str):
+                logging.info(f" ✖ Authentication failed: {message}")
+                self.run_loop = False
+
+            # Both functions have to address the right connector
+            self.sio.on("job_request", lambda p: self.__execute_job(p))
+
+            self.sio.on(
+                "job_response", lambda p: self.job_responses.update({p["id"]: p})
+            )
+
+            self.sio.on("token_expired", lambda: self.authenticate())
+            self.sio.on("auth_error", auth_error)
+
+            def connector_online(payload):
+                logging.info(
+                    f" ✔ Agent {payload['connector_id']} \033[32mconnected\033[0m"
+                )
+
+                # Check for buffered messages for this connector
+                removed_items = []
+                for item in self.emit_buffer:
+                    if item["connector_id"] == payload["connector_id"]:
+                        logging.info(
+                            f">> Sending buffered message for job {item['job_id']} to '{item['event']}'"
+                        )
+                        self.sio.emit(item["event"], item["data"])
+                        removed_items.append(item)
+
+                for item in removed_items:
+                    self.emit_buffer.remove(item)
+
+            self.sio.on("connector_online", connector_online)
+
+            def disconnect():
+                for connector_id in self.connector_functions:
+                    logging.info(f" ✖ Agent {connector_id} \033[31mdisconnected\033[0m")
+
+            self.sio.on("disconnect", lambda: disconnect())
+
+            while self.run_loop:
+                try:
+                    self.sio.connect(SERVER)
+                    self.sio.wait()
+                except socketio.exceptions.ConnectionError as e:
+                    if self.run_loop:
+                        if self.logger:
+                            logging.info(
+                                f" ✖ Failed to connect to Eezo server with error: {e}"
+                            )
+                            logging.info("   Retrying to connect...")
+                        time.sleep(5)
+                    else:
+                        break
+                except KeyboardInterrupt:
+                    self.run_loop = False
+                    break
+                except Exception as e:
+                    if self.run_loop:
+                        if self.logger:
+                            logging.info(
+                                f" ✖ Failed to connect to Eezo server with error: {e}"
+                            )
+                            logging.info("   Retrying to connect...")
+                        time.sleep(5)
+                    else:
+                        break
+
+                self.sio.disconnect()
 
         except KeyboardInterrupt:
             pass
         finally:
-            for future in self.futures:
-                future.cancel()
-            self.executor.shutdown(wait=False)
             self.observer.stop()
 
     def _request(
         self, method: str, endpoint: str, payload: Optional[Dict[str, Any]] = None
     ) -> Dict[str, Any]:
         """
         Sends an HTTP request to the given endpoint with the provided payload and returns the response.
@@ -164,39 +398,43 @@
         the API key for authorization. It also provides comprehensive error handling, raising more
         specific exceptions depending on the encountered HTTP error.
         """
         if payload is None:
             payload = {}
         payload["api_key"] = self.api_key
         try:
-            response = self.session.request(method, endpoint, json=payload)
+            response = self.session.request(method, endpoint, json=payload, timeout=10)
             # Raises HTTPError for bad responses
             response.raise_for_status()
             logging.info(f"Request to {endpoint} successful \033[32m200\033[0m")
             return response.json()
         except requests.exceptions.HTTPError as e:
             status = e.response.status_code
+            error_message = e.response.text
             if status in [401, 403]:
                 logging.error(
                     "Eezo \033[31mauthorization error\033[0m. Check your API key."
                 )
                 raise AuthorizationError(
                     "Authorization error. Check your API key."
                 ) from e
             elif status == 404:
                 if endpoint in {READ_STATE_ENDPOINT, UPDATE_STATE_ENDPOINT}:
                     return self.create_state(self.user_id)
                 else:
-                    logging.error(f"Eezo \033[31mresource not found\033[0m: {endpoint}")
-                    raise ResourceNotFoundError(f"Not found: {endpoint}") from e
+                    logging.error(f"Resource not found: \033[31m{error_message}\033[0m")
+                    raise ResourceNotFoundError(error_message) from e
             else:
                 logging.error(
-                    f"Eezo \033[31mrequest error\033[0m: {e.response.content}"
+                    f"Unexpected error: \033[31m{error_message} (status code: {status})\033[0m"
                 )
                 raise RequestError(f"Unexpected error: {e.response.content}") from e
+        except Exception as e:
+            logging.error(f"Unexpected error: \033[31m{e}\033[0m")
+            raise RequestError(f"Unexpected error: {e}") from e
 
     def new_message(
         self, eezo_id: str, thread_id: str, context: str = "direct_message"
     ) -> Message:
         """Create and return a new message object configured to notify on updates.
 
         Args:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eezo-0.3.4/eezo/interface/components/chart.py` & `eezo-0.3.5/eezo/interface/components/chart.py`

 * *Files identical despite different names*

### Comparing `eezo-0.3.4/eezo/interface/interface.py` & `eezo-0.3.5/eezo/interface/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,36 +66,40 @@
             raise Exception("Please create a message first")
 
         message_obj = self.message.to_dict()
         self.send_message(
             {
                 "message_id": message_obj["id"],
                 "interface": message_obj["interface"],
+                "job_id": self.job_id,
             }
         )
 
     def get_thread(self, nr: int = 5, to_string: bool = False) -> Any:
         """
         Retrieves and returns a thread of messages, with a limit on the number of messages.
 
         Args:
             nr: The number of messages to retrieve from the thread. Defaults to 5.
             to_string: A boolean flag indicating whether to convert the messages to a string. Defaults to False.
 
         The method delegates the operation to the `_run` callback, providing the required parameters.
         """
         return self._run(
-            skill_id="s_get_thread", nr_of_messages=nr, to_string=to_string
+            skill_id="s_get_thread",
+            current_job_id=self.job_id,
+            nr_of_messages=nr,
+            to_string=to_string,
         )
 
     def invoke(self, agent_id: str, **kwargs: Any) -> Any:
         """
         Invokes an agent or skill and returns its result.
 
         Args:
             agent_id: A string identifier of the agent or skill to be invoked.
             **kwargs: A variable number of keyword arguments that are passed to the agent or skill.
 
         This method utilizes the `_run` callback to execute the agent or skill identified by `agent_id`
         with the given keyword arguments.
         """
-        return self._run(skill_id=agent_id, **kwargs)
+        return self._run(skill_id=agent_id, current_job_id=self.job_id, **kwargs)
```

### Comparing `eezo-0.3.4/eezo/interface/message.py` & `eezo-0.3.5/eezo/interface/message.py`

 * *Files identical despite different names*

### Comparing `eezo-0.3.4/eezo/state.py` & `eezo-0.3.5/eezo/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             self._state = result
             self.client.state_was_loaded = True
         else:
             logging.error("Failed to load state.")
 
     def __getitem__(self, key: str) -> Any:
         """Get an item from the state by key."""
-        return self._state.get(key, None)
+        return self._state[key]
 
     def __setitem__(self, key: str, value: Any) -> None:
         """Set an item in the state."""
         self._state[key] = value
 
     def __delitem__(self, key: str) -> None:
         """Remove an item from the state by key if it exists."""
```

### Comparing `eezo-0.3.4/eezo.egg-info/PKG-INFO` & `eezo-0.3.5/eezo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eezo
-Version: 0.3.4
+Version: 0.3.5
 Summary: Eezo enables you to build and supervise your AI agent workforces.
 Home-page: UNKNOWN
 Author: Daniel Schoenbohm
 Author-email: daniel@eezo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `eezo-0.3.4/eezo.egg-info/SOURCES.txt` & `eezo-0.3.5/eezo.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 README.md
 setup.py
 eezo/__init__.py
-eezo/async_client.py
 eezo/client.py
-eezo/connector.py
 eezo/errors.py
 eezo/state.py
-eezo/state_async.py
 eezo.egg-info/PKG-INFO
 eezo.egg-info/SOURCES.txt
 eezo.egg-info/dependency_links.txt
 eezo.egg-info/requires.txt
 eezo.egg-info/top_level.txt
 eezo/agent/__init__.py
 eezo/agent/agent.py
 eezo/agent/agents.py
 eezo/interface/__init__.py
 eezo/interface/interface.py
-eezo/interface/interface_async.py
 eezo/interface/message.py
 eezo/interface/components/__init__.py
 eezo/interface/components/chart.py
 eezo/interface/components/component.py
 eezo/interface/components/image.py
 eezo/interface/components/text.py
 eezo/interface/components/youtube_video.py
```

### Comparing `eezo-0.3.4/setup.py` & `eezo-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="eezo",
-    version="0.3.4",
+    version="0.3.5",
     description="Eezo enables you to build and supervise your AI agent workforces.",
     author="Daniel Schoenbohm",
     author_email="daniel@eezo.ai",
     packages=find_packages(),
     install_requires=[
         "aiohttp==3.9.3",
         "aiosignal==1.3.1",
```

