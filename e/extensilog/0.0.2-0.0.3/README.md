# Comparing `tmp/extensilog-0.0.2.tar.gz` & `tmp/extensilog-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extensilog-0.0.2.tar", last modified: Wed May  1 18:04:08 2024, max compression
+gzip compressed data, was "extensilog-0.0.3.tar", last modified: Thu May  2 18:45:35 2024, max compression
```

## Comparing `extensilog-0.0.2.tar` & `extensilog-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:04:08.395032 extensilog-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-01 18:04:02.000000 extensilog-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-01 18:04:02.000000 extensilog-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-01 18:04:08.395032 extensilog-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-01 18:04:02.000000 extensilog-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:04:08.391032 extensilog-0.0.2/extensilog/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:04:08.391032 extensilog-0.0.2/extensilog/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/connectors/base_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/connectors/extensible_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/connectors/local_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/connectors/mongo_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/connectors/postgres_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/extensilog.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-01 18:04:02.000000 extensilog-0.0.2/extensilog/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:04:08.395032 extensilog-0.0.2/extensilog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-01 18:04:08.000000 extensilog-0.0.2/extensilog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-01 18:04:08.000000 extensilog-0.0.2/extensilog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:04:08.000000 extensilog-0.0.2/extensilog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-01 18:04:08.000000 extensilog-0.0.2/extensilog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 18:04:08.000000 extensilog-0.0.2/extensilog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-01 18:04:02.000000 extensilog-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:04:08.395032 extensilog-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-01 18:04:02.000000 extensilog-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:45:35.047759 extensilog-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-02 18:45:26.000000 extensilog-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 18:45:26.000000 extensilog-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-02 18:45:35.047759 extensilog-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 18:45:26.000000 extensilog-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:45:35.047759 extensilog-0.0.3/extensilog/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-02 18:45:26.000000 extensilog-0.0.3/extensilog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:45:35.047759 extensilog-0.0.3/extensilog/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-02 18:45:26.000000 extensilog-0.0.3/extensilog/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 18:45:26.000000 extensilog-0.0.3/extensilog/connectors/base_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-02 18:45:26.000000 extensilog-0.0.3/extensilog/connectors/extensible_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-02 18:45:26.000000 extensilog-0.0.3/extensilog/connectors/local_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-02 18:45:26.000000 extensilog-0.0.3/extensilog/connectors/mongo_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-02 18:45:26.000000 extensilog-0.0.3/extensilog/connectors/postgres_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9993 2024-05-02 18:45:26.000000 extensilog-0.0.3/extensilog/extensilog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-02 18:45:26.000000 extensilog-0.0.3/extensilog/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-02 18:45:26.000000 extensilog-0.0.3/extensilog/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:45:35.047759 extensilog-0.0.3/extensilog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-02 18:45:35.000000 extensilog-0.0.3/extensilog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-02 18:45:35.000000 extensilog-0.0.3/extensilog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:45:35.000000 extensilog-0.0.3/extensilog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-02 18:45:35.000000 extensilog-0.0.3/extensilog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 18:45:35.000000 extensilog-0.0.3/extensilog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-02 18:45:26.000000 extensilog-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:45:35.047759 extensilog-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-02 18:45:26.000000 extensilog-0.0.3/setup.py
```

### Comparing `extensilog-0.0.2/LICENSE` & `extensilog-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `extensilog-0.0.2/PKG-INFO` & `extensilog-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extensilog
-Version: 0.0.2
+Version: 0.0.3
 Summary: A logger for tracking your agent workflow
 Home-page: https://github.com/Extensible-AI/extensilog/
 Author: Parth Sareen, Omkaar Kamath
 Author-email: parth@extensible.dev, omkaar@extensible.dev
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,28 +14,26 @@
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==4.3.0
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: distro==1.9.0
 Requires-Dist: dnspython==2.6.1
-Requires-Dist: fastask==0.4.6
 Requires-Dist: h11==0.14.0
 Requires-Dist: httpcore==1.0.5
 Requires-Dist: httpx==0.27.0
 Requires-Dist: idna==3.7
 Requires-Dist: openai==1.14.3
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pydantic_core==2.16.3
 Requires-Dist: pymongo==4.6.3
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: requests==2.31.0
-Requires-Dist: setuptools==69.5.1
 Requires-Dist: sniffio==1.3.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: typing_extensions==4.10.0
 Requires-Dist: urllib3==2.2.1
 
 # Extensilog 
 ## Key Features
```

### Comparing `extensilog-0.0.2/README.md` & `extensilog-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `extensilog-0.0.2/extensilog/connectors/extensible_connector.py` & `extensilog-0.0.3/extensilog/connectors/extensible_connector.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from .base_connector import BaseConnector
 import requests
 import json
 
 
 class ExtensibleConnector(BaseConnector):
-    def __init__(self):
+    def __init__(self, endpoint: str="http://127.0.0.1:5000/api/push_tasks"):
         """
         Initialize the Extensible Connector.
         """
         self.credentials = {}
-        self.endpoint = "http://127.0.0.1:5000/api/push_tasks"
+        self.endpoint = endpoint 
 
 
     def flush(self, logs: list):
         """
         Flushes the provided logs using the connector.
 
         Args:
```

### Comparing `extensilog-0.0.2/extensilog/connectors/local_connector.py` & `extensilog-0.0.3/extensilog/connectors/local_connector.py`

 * *Files identical despite different names*

### Comparing `extensilog-0.0.2/extensilog/connectors/mongo_connector.py` & `extensilog-0.0.3/extensilog/connectors/mongo_connector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pymongo import MongoClient
 from pymongo.errors import ConnectionFailure, OperationFailure
+import atexit
 
 from .base_connector import BaseConnector
 
 class MongoConnector(BaseConnector):
     def __init__(self, connection_string: str, db_name: str, collection_name: str, client: MongoClient=None):
         """
         Initialize the MongoDB Connector using a connection string.
@@ -13,23 +14,23 @@
         """
         self.db_name = db_name
         self.collection_name = collection_name
         self.client = client or MongoClient(connection_string, tlsAllowInvalidCertificates=True)
         try:
             # Verify server connectivity
             self.client.admin.command('ping')
-            print('successful')
         except ConnectionFailure as e:
             print("Failed to connect to MongoDB:", e)
         except OperationFailure as e:
             print("Authentication failed:", e)
+        atexit.register(self.close_connection)
 
-    def __del__(self):
+    def close_connection(self):
         """
-        Destructor to close the MongoDB connection when the object is deleted.
+        Close the MongoDB connection.
         """
         if self.client:
             self.client.close()
             print("MongoDB connection closed.")
 
     def flush(self, json_data):
         """
```

### Comparing `extensilog-0.0.2/extensilog/connectors/postgres_connector.py` & `extensilog-0.0.3/extensilog/connectors/postgres_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
-from logging import Logger
 import psycopg2
-from psycopg2 import OperationalError, DatabaseError
+import atexit
+from psycopg2 import OperationalError
 from extensilog.model import Task
 
 from .base_connector import BaseConnector
 
 class PostgresConnector(BaseConnector):
     def __init__(self, connection_string: str, table_name: str):
         """
@@ -18,54 +18,47 @@
         self.connection = None
         try:
             self.connection = psycopg2.connect(self.connection_string)
             self.connection.autocommit = True
             print('Connection successful')
         except OperationalError as e:
             print("Failed to connect to PostgreSQL:", e)
-    
-
-    def __del__(self):
-        """
-        Destructor method to ensure the connection is closed when the object is deleted.
-        """
-        self.close()
+        atexit.register(self.close)
 
         
     def close(self):
         """
         Close the database connection.
         """
         if self.connection:
             self.connection.close()
             print("Database connection closed.")
 
 
-    def flush(self, json_data: list):
+    def flush(self, json_data: list) -> bool:
         if not self.connection:
             print("Database connection is not established.")
             return False
 
         if not json_data:
             print("No data to insert.")
             return False
 
         tasks = [Task(**item) for item in json_data]
 
         conn = self.connection
-        cur = conn.cursor()
-
-        insert_query = """
-        INSERT INTO logs (log_id, function_name, start_time, end_time, args, result, task_id, agent_id, parent_log_id, metadata, inferred_accuracy, accuracy_reasoning)
-        VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s)
-        """
-
         try:
+            cur = conn.cursor()
+            insert_query = """
+            INSERT INTO logs (log_id, function_name, start_time, end_time, args, result, task_id, agent_id, parent_log_id, metadata, inferred_accuracy, accuracy_reasoning)
+            VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s)
+            """
             cur.executemany(insert_query, [(task.log_id, task.function_name, task.start_time, task.end_time, 
-                                        json.dumps(task.args), json.dumps(task.result), task.task_id, 
-                                        task.agent_id, task.parent_log_id, json.dumps(task.metadata), 
-                                        task.inferred_accuracy, task.accuracy_reasoning) for task in tasks])
+                                            json.dumps(task.args), json.dumps(task.result), task.task_id, 
+                                            task.agent_id, task.parent_log_id, json.dumps(task.metadata), 
+                                            task.inferred_accuracy, task.accuracy_reasoning) for task in tasks])
+            conn.commit()
+            cur.close()
+            return True
         except Exception as e:
-            Logger.error(f"Error inserting data: {e}")
-
-        conn.commit()
-        cur.close()
+            print(f"Error inserting data: {e}")
+            return False
```

### Comparing `extensilog-0.0.2/extensilog/extensilog.py` & `extensilog-0.0.3/extensilog/extensilog.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,46 +3,71 @@
 import functools
 import json
 from datetime import datetime
 from queue import Queue
 import threading
 import uuid
 import openai
+import atexit
 
 from .connectors.local_connector import LocalConnector
 from .singleton import Singleton
 
 
 thread_local_storage = threading.local()
 
 class Extensilog(metaclass=Singleton):
-    def __init__(self, client=None, log_file='./event_log.json', connector=None):
+    def __init__(self, client=None, log_file='./event_log.json', connector=None, task_flush_limit=1):
         self.client = client or openai
         self.log_file = log_file
         self.lock = threading.Lock()
         self.agent_id = str(uuid.uuid4())
         self.data_store = dict() 
-        self.connector = LocalConnector(log_file) if connector is None else connector 
+        self.connector = connector or LocalConnector(log_file)
+        self.task_flush_limit = task_flush_limit
+        self.task_flush_ids = Queue() 
+        self.task_count = 0
+        self.to_flush = []
+        atexit.register(self.__on_exit)
+
+
+    def __on_exit(self):
+        """
+        Method to ensure all remaining logs are flushed upon program interruption or shutdown.
+        """
+        with self.lock:
+            while not self.task_flush_ids.empty():
+                task_id = self.task_flush_ids.get()
+                self.__add_to_flush(task_id)
+            self.__flush_queue()
+            self.task_count = 0
+            self.data_store = dict()  # Optionally reset the data store if needed
+            print("Program interrupted. All pending logs have been flushed.")
 
 
     def log(self, track=False):
         def decorator(func):
             @functools.wraps(func)
             def wrapper(*args, **kwargs):
+                if track and hasattr(thread_local_storage, 'task_id') and len(self.data_store[thread_local_storage.task_id]['call_stack']) > 0:
+                    raise ValueError("Cannot track a top level function that is already part of a task.")
                 if not hasattr(thread_local_storage, 'task_id') or track:
                     thread_local_storage.task_id = str(uuid.uuid4())
                     with self.lock:
-                        self.data_store[thread_local_storage.task_id] = dict() 
-                        self.data_store[thread_local_storage.task_id]['queue'] = Queue()
-                        self.data_store[thread_local_storage.task_id]['client'] = self.client
-                        self.data_store[thread_local_storage.task_id]['call_stack'] = []
-                        self.data_store[thread_local_storage.task_id]['patched'] = False 
-                        self.data_store[thread_local_storage.task_id]['completion_ids'] = set()
-                        self.data_store[thread_local_storage.task_id]['last_openai_call'] = {} 
-                        self.data_store[thread_local_storage.task_id]['metadata'] = None 
+                        self.task_flush_ids.put(thread_local_storage.task_id)
+                        self.task_count += 1
+                        self.data_store[thread_local_storage.task_id] = {
+                            'queue': Queue(),
+                            'client': self.client,
+                            'call_stack': [],
+                            'patched': False,
+                            'completion_ids': set(),
+                            'last_openai_call': {},
+                            'metadata': None
+                        }
 
                 with self.lock:
                     self.data_store[thread_local_storage.task_id]['call_stack'].append((func.__name__, str(uuid.uuid4())))
 
 
                 func_args = inspect.signature(func).bind(*args, **kwargs).arguments
                 func_args_dict = self.__serialize_arguments(func_args)
@@ -176,24 +201,33 @@
         # Example modification to include full call stack in the log
         task_id = thread_local_storage.task_id
         if log_entry['function_name'] == 'openai.chat.completions.create':
             openai_id = log_entry['result']['id']
             self.data_store[task_id]['last_openai_call'][openai_id] = log_entry['log_id'] 
 
         self.data_store[task_id]['queue'].put(log_entry)
-        if len(self.data_store[task_id]['call_stack']) == 0:
-            self.__flush_queue()
-
 
-    def __flush_queue(self):
+        if len(self.data_store[task_id]['call_stack']) == 0 and self.task_count >= self.task_flush_limit:
+            # TODO: to be made non-blocking
+            removed = 0
+            while removed < self.task_flush_limit: 
+                task_id = self.task_flush_ids.get()
+                removed += 1
+                self.__add_to_flush(task_id)
+            self.task_count -= self.task_flush_limit
+            self.__flush_queue()
 
 
-        new_data = []
-        task_id = thread_local_storage.task_id
+    # TODO: add batch flushing with storing in memory
+    def __add_to_flush(self, task_id):
         while not self.data_store[task_id]['queue'].empty():
             log_entry = self.data_store[task_id]['queue'].get()
             # Skip the loop if the log id is not the last openai call
             if log_entry['function_name'] == 'openai.chat.completions.create' and self.data_store[task_id]['last_openai_call'][log_entry['result']['id']] != log_entry['log_id']:
                 continue
-            new_data.append(log_entry)
-        
-        self.connector.flush(new_data)
+            self.to_flush.append(log_entry)
+
+    
+    def __flush_queue(self):
+        if self.to_flush:
+            self.connector.flush(self.to_flush)
+            self.to_flush.clear()
```

### Comparing `extensilog-0.0.2/extensilog/singleton.py` & `extensilog-0.0.3/extensilog/singleton.py`

 * *Files identical despite different names*

### Comparing `extensilog-0.0.2/extensilog.egg-info/PKG-INFO` & `extensilog-0.0.3/extensilog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extensilog
-Version: 0.0.2
+Version: 0.0.3
 Summary: A logger for tracking your agent workflow
 Home-page: https://github.com/Extensible-AI/extensilog/
 Author: Parth Sareen, Omkaar Kamath
 Author-email: parth@extensible.dev, omkaar@extensible.dev
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,28 +14,26 @@
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==4.3.0
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: distro==1.9.0
 Requires-Dist: dnspython==2.6.1
-Requires-Dist: fastask==0.4.6
 Requires-Dist: h11==0.14.0
 Requires-Dist: httpcore==1.0.5
 Requires-Dist: httpx==0.27.0
 Requires-Dist: idna==3.7
 Requires-Dist: openai==1.14.3
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pydantic_core==2.16.3
 Requires-Dist: pymongo==4.6.3
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: requests==2.31.0
-Requires-Dist: setuptools==69.5.1
 Requires-Dist: sniffio==1.3.1
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: typing_extensions==4.10.0
 Requires-Dist: urllib3==2.2.1
 
 # Extensilog 
 ## Key Features
```

### Comparing `extensilog-0.0.2/extensilog.egg-info/SOURCES.txt` & `extensilog-0.0.3/extensilog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `extensilog-0.0.2/setup.py` & `extensilog-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     required = f.read().splitlines()
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='extensilog',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(include=['extensilog', 'extensilog.*']),
     install_requires=required,
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='Apache License 2.0',
     author='Parth Sareen, Omkaar Kamath',
     author_email='parth@extensible.dev, omkaar@extensible.dev',
```

