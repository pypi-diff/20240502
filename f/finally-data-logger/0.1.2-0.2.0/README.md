# Comparing `tmp/finally_data_logger-0.1.2.tar.gz` & `tmp/finally_data_logger-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finally_data_logger-0.1.2.tar", last modified: Sat Aug 12 19:23:16 2023, max compression
+gzip compressed data, was "finally_data_logger-0.2.0.tar", last modified: Thu May  2 08:39:45 2024, max compression
```

## Comparing `finally_data_logger-0.1.2.tar` & `finally_data_logger-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 amir      (1000) amir      (1000)        0 2023-08-12 19:23:16.783395 finally_data_logger-0.1.2/
--rw-rw-r--   0 amir      (1000) amir      (1000)     2696 2023-08-12 19:23:16.783395 finally_data_logger-0.1.2/PKG-INFO
--rw-rw-r--   0 amir      (1000) amir      (1000)     2049 2023-08-12 08:12:56.000000 finally_data_logger-0.1.2/README.md
--rw-rw-r--   0 amir      (1000) amir      (1000)       38 2023-08-12 19:23:16.783395 finally_data_logger-0.1.2/setup.cfg
--rw-rw-r--   0 amir      (1000) amir      (1000)     1197 2023-08-12 08:13:49.000000 finally_data_logger-0.1.2/setup.py
-drwxrwxr-x   0 amir      (1000) amir      (1000)        0 2023-08-12 19:23:16.779395 finally_data_logger-0.1.2/src/
-drwxrwxr-x   0 amir      (1000) amir      (1000)        0 2023-08-12 19:23:16.783395 finally_data_logger-0.1.2/src/finally_data_logger/
--rw-rw-r--   0 amir      (1000) amir      (1000)       43 2023-08-11 07:50:52.000000 finally_data_logger-0.1.2/src/finally_data_logger/__init__.py
-drwxrwxr-x   0 amir      (1000) amir      (1000)        0 2023-08-12 19:23:16.783395 finally_data_logger-0.1.2/src/finally_data_logger/client/
--rw-rw-r--   0 amir      (1000) amir      (1000)        0 2023-07-06 07:01:46.000000 finally_data_logger-0.1.2/src/finally_data_logger/client/__init__.py
--rw-rw-r--   0 amir      (1000) amir      (1000)     3043 2023-08-11 09:28:59.000000 finally_data_logger-0.1.2/src/finally_data_logger/client/data_logger.py
-drwxrwxr-x   0 amir      (1000) amir      (1000)        0 2023-08-12 19:23:16.783395 finally_data_logger-0.1.2/src/finally_data_logger/server/
--rw-rw-r--   0 amir      (1000) amir      (1000)        0 2023-07-06 07:01:46.000000 finally_data_logger-0.1.2/src/finally_data_logger/server/__init__.py
--rw-rw-r--   0 amir      (1000) amir      (1000)     5472 2023-08-11 09:54:08.000000 finally_data_logger-0.1.2/src/finally_data_logger/server/finally_data_logger_server.py
-drwxrwxr-x   0 amir      (1000) amir      (1000)        0 2023-08-12 19:23:16.783395 finally_data_logger-0.1.2/src/finally_data_logger.egg-info/
--rw-rw-r--   0 amir      (1000) amir      (1000)     2696 2023-08-12 19:23:16.000000 finally_data_logger-0.1.2/src/finally_data_logger.egg-info/PKG-INFO
--rw-rw-r--   0 amir      (1000) amir      (1000)      557 2023-08-12 19:23:16.000000 finally_data_logger-0.1.2/src/finally_data_logger.egg-info/SOURCES.txt
--rw-rw-r--   0 amir      (1000) amir      (1000)        1 2023-08-12 19:23:16.000000 finally_data_logger-0.1.2/src/finally_data_logger.egg-info/dependency_links.txt
--rw-rw-r--   0 amir      (1000) amir      (1000)       97 2023-08-12 19:23:16.000000 finally_data_logger-0.1.2/src/finally_data_logger.egg-info/entry_points.txt
--rw-rw-r--   0 amir      (1000) amir      (1000)       28 2023-08-12 19:23:16.000000 finally_data_logger-0.1.2/src/finally_data_logger.egg-info/requires.txt
--rw-rw-r--   0 amir      (1000) amir      (1000)       20 2023-08-12 19:23:16.000000 finally_data_logger-0.1.2/src/finally_data_logger.egg-info/top_level.txt
-drwxrwxr-x   0 amir      (1000) amir      (1000)        0 2023-08-12 19:23:16.783395 finally_data_logger-0.1.2/tests/
--rw-rw-r--   0 amir      (1000) amir      (1000)     1030 2023-08-11 09:20:51.000000 finally_data_logger-0.1.2/tests/test_data_logger.py
+drwxrwxr-x   0 amir      (1000) amir      (1000)        0 2024-05-02 08:39:45.713490 finally_data_logger-0.2.0/
+-rw-rw-r--   0 amir      (1000) amir      (1000)     2949 2024-05-02 08:39:45.713490 finally_data_logger-0.2.0/PKG-INFO
+-rw-rw-r--   0 amir      (1000) amir      (1000)     2303 2024-04-30 11:10:02.000000 finally_data_logger-0.2.0/README.md
+-rw-rw-r--   0 amir      (1000) amir      (1000)       38 2024-05-02 08:39:45.713490 finally_data_logger-0.2.0/setup.cfg
+-rw-rw-r--   0 amir      (1000) amir      (1000)     1196 2024-05-02 08:38:14.000000 finally_data_logger-0.2.0/setup.py
+drwxrwxr-x   0 amir      (1000) amir      (1000)        0 2024-05-02 08:39:45.709490 finally_data_logger-0.2.0/src/
+drwxrwxr-x   0 amir      (1000) amir      (1000)        0 2024-05-02 08:39:45.713490 finally_data_logger-0.2.0/src/finally_data_logger/
+-rw-rw-r--   0 amir      (1000) amir      (1000)       43 2023-08-11 07:50:52.000000 finally_data_logger-0.2.0/src/finally_data_logger/__init__.py
+drwxrwxr-x   0 amir      (1000) amir      (1000)        0 2024-05-02 08:39:45.713490 finally_data_logger-0.2.0/src/finally_data_logger/client/
+-rw-rw-r--   0 amir      (1000) amir      (1000)        0 2023-07-06 07:01:46.000000 finally_data_logger-0.2.0/src/finally_data_logger/client/__init__.py
+-rw-rw-r--   0 amir      (1000) amir      (1000)     3043 2023-08-11 09:28:59.000000 finally_data_logger-0.2.0/src/finally_data_logger/client/data_logger.py
+drwxrwxr-x   0 amir      (1000) amir      (1000)        0 2024-05-02 08:39:45.713490 finally_data_logger-0.2.0/src/finally_data_logger/server/
+-rw-rw-r--   0 amir      (1000) amir      (1000)        0 2023-07-06 07:01:46.000000 finally_data_logger-0.2.0/src/finally_data_logger/server/__init__.py
+-rw-rw-r--   0 amir      (1000) amir      (1000)     5937 2024-04-30 15:41:13.000000 finally_data_logger-0.2.0/src/finally_data_logger/server/finally_data_logger_server.py
+drwxrwxr-x   0 amir      (1000) amir      (1000)        0 2024-05-02 08:39:45.713490 finally_data_logger-0.2.0/src/finally_data_logger.egg-info/
+-rw-rw-r--   0 amir      (1000) amir      (1000)     2949 2024-05-02 08:39:45.000000 finally_data_logger-0.2.0/src/finally_data_logger.egg-info/PKG-INFO
+-rw-rw-r--   0 amir      (1000) amir      (1000)      557 2024-05-02 08:39:45.000000 finally_data_logger-0.2.0/src/finally_data_logger.egg-info/SOURCES.txt
+-rw-rw-r--   0 amir      (1000) amir      (1000)        1 2024-05-02 08:39:45.000000 finally_data_logger-0.2.0/src/finally_data_logger.egg-info/dependency_links.txt
+-rw-rw-r--   0 amir      (1000) amir      (1000)       97 2024-05-02 08:39:45.000000 finally_data_logger-0.2.0/src/finally_data_logger.egg-info/entry_points.txt
+-rw-rw-r--   0 amir      (1000) amir      (1000)       28 2024-05-02 08:39:45.000000 finally_data_logger-0.2.0/src/finally_data_logger.egg-info/requires.txt
+-rw-rw-r--   0 amir      (1000) amir      (1000)       20 2024-05-02 08:39:45.000000 finally_data_logger-0.2.0/src/finally_data_logger.egg-info/top_level.txt
+drwxrwxr-x   0 amir      (1000) amir      (1000)        0 2024-05-02 08:39:45.713490 finally_data_logger-0.2.0/tests/
+-rw-rw-r--   0 amir      (1000) amir      (1000)     1030 2023-08-11 09:20:51.000000 finally_data_logger-0.2.0/tests/test_data_logger.py
```

### Comparing `finally_data_logger-0.1.2/PKG-INFO` & `finally_data_logger-0.2.0/src/finally_data_logger.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: finally_data_logger
-Version: 0.1.2
+Name: finally-data-logger
+Version: 0.2.0
 Summary: A simple data logging server and client.
 Home-page: https://github.com/arbasli2/FinallyDataLogger
 Author: arbasli
 Author-email: arbasli2@gmail.com
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -35,31 +35,36 @@
 ## Quick Start
 
 ### Starting the server
 
 From the command line:
 
 ```bash
-finally_data_logger_server --port 5000 --dir /path/to/storage/directory
+finallydatalogger --port 5000 --dir /path/to/storage/directory
+# to make it visible on the network
+finallydatalogger --host 0.0.0.0 --port 5000 --dir /path/to/storage/directory
 ```
 
 ### Using the client
 
 In your Python script:
 
 ```python
+import numpy as np
 from finally_data_logger import DataLogger
 
-logger = DataLogger(port=5000)
+logger = DataLogger(port=5000) #  DataLogger(server_url="http://192.168.x.x", port=5000)
 
 # Log some data
+img = np.random.rand(10,10)
+# a packet of data is stored in the form of a dictionary
 data = {
     "name": "test1",
     "duration": 0.3,
-    "image": your_numpy_image
+    "image": img
 }
 response = logger.log_data(data)
 print(response)
 
 # Fetch data
 criteria = {'name': 'test*'}
 results = logger.get_data(criteria, fetch_blob=True)
```

### Comparing `finally_data_logger-0.1.2/README.md` & `finally_data_logger-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -18,31 +18,36 @@
 ## Quick Start
 
 ### Starting the server
 
 From the command line:
 
 ```bash
-finally_data_logger_server --port 5000 --dir /path/to/storage/directory
+finallydatalogger --port 5000 --dir /path/to/storage/directory
+# to make it visible on the network
+finallydatalogger --host 0.0.0.0 --port 5000 --dir /path/to/storage/directory
 ```
 
 ### Using the client
 
 In your Python script:
 
 ```python
+import numpy as np
 from finally_data_logger import DataLogger
 
-logger = DataLogger(port=5000)
+logger = DataLogger(port=5000) #  DataLogger(server_url="http://192.168.x.x", port=5000)
 
 # Log some data
+img = np.random.rand(10,10)
+# a packet of data is stored in the form of a dictionary
 data = {
     "name": "test1",
     "duration": 0.3,
-    "image": your_numpy_image
+    "image": img
 }
 response = logger.log_data(data)
 print(response)
 
 # Fetch data
 criteria = {'name': 'test*'}
 results = logger.get_data(criteria, fetch_blob=True)
```

### Comparing `finally_data_logger-0.1.2/setup.py` & `finally_data_logger-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name="finally_data_logger",
-    version="0.1.2",
+    version="0.2.0",
     description="A simple data logging server and client.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="arbasli",
     author_email="arbasli2@gmail.com",
     url="https://github.com/arbasli2/FinallyDataLogger",
     packages=find_packages(where="src"),
@@ -21,15 +21,15 @@
     ],
     entry_points={
         "console_scripts": [
             "finallydatalogger = finally_data_logger.server.finally_data_logger_server:main",
         ],
     },
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `finally_data_logger-0.1.2/src/finally_data_logger/client/data_logger.py` & `finally_data_logger-0.2.0/src/finally_data_logger/client/data_logger.py`

 * *Files identical despite different names*

### Comparing `finally_data_logger-0.1.2/src/finally_data_logger/server/finally_data_logger_server.py` & `finally_data_logger-0.2.0/src/finally_data_logger/server/finally_data_logger_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import argparse
 from flask import Flask, request, jsonify, send_from_directory
 from tinydb import TinyDB, Query
 import os
 import base64
 import uuid
 import shutil
+import copy
 
 app = Flask(__name__)
 
 # db = TinyDB("data.json")
 # db = None
 
 
 def save_blob(base64_data):
     """Save blob data and return the blob filepath."""
     binary_data = base64.b64decode(base64_data.encode())
     filename = f"{str(uuid.uuid4())}_{hash(binary_data)}.blob"
     filepath = os.path.join(BLOB_DIR, filename)
     with open(filepath, "wb") as f:
         f.write(binary_data)
-    return filepath
+    return filename
 
 
 def handle_blob_for_dict(data_dict, original_dict=None):
     """Handle blob data in a dictionary."""
     for key, value in data_dict.items():
         if isinstance(value, dict) and value.get("type") == "blob":
             filepath = save_blob(value["data"])
@@ -37,14 +38,15 @@
                     and original_blob_info.get("type") == "blob"
                 ):
                     os.remove(original_blob_info["filepath"])
 
 
 def convert_blob_file_to_base64(filepath):
     """Convert blob file to a base64 encoded string."""
+    filepath = os.path.join(BLOB_DIR, filepath)
     with open(filepath, "rb") as f:
         binary_data = f.read()
     return base64.b64encode(binary_data).decode()
 
 
 def handle_blobs_in_fetched_data(data, fetch_blob):
     """Replace blob references with a dictionary containing type and base64 encoded content in fetched data."""
@@ -87,14 +89,17 @@
 
         if query:
             query &= current_condition
         else:
             query = current_condition
 
     results = db.search(query)
+    results = copy.deepcopy(
+        results
+    )  # Avoid modifying the original data on the database (in memory part of the db. the orginal file is not modified)
     handle_blobs_in_fetched_data(results, fetch_blob)
     return jsonify(results)
 
 
 @app.route("/modify_data/<entry_id>", methods=["PUT"])
 def modify_data(entry_id):
     modifications = request.json
@@ -157,23 +162,31 @@
 def main():
     global db, BLOB_DIR
     parser = argparse.ArgumentParser(description="Start the FinallyDataLogger server.")
     parser.add_argument(
         "--dir", type=str, default="./data", help="Directory for data storage."
     )
     parser.add_argument(
+        "--host",
+        type=str,
+        default="localhost",
+        help="Host address to run the server on.",
+    )
+    parser.add_argument(
         "--port", type=int, default=5000, help="Port number to run the server on."
     )
 
     args = parser.parse_args()
 
-    BLOB_DIR = os.path.join(args.dir, "blobs")
+    BLOB_DIR = os.path.join(os.getcwd(), args.dir, "blobs")
+    print("BLOB_DIR: ", BLOB_DIR)
     db_path = os.path.join(args.dir, "data.json")
     if not os.path.exists(BLOB_DIR):
         os.makedirs(BLOB_DIR)
     db = TinyDB(db_path)
 
-    app.run(port=args.port)
+    app.run(host=args.host, port=args.port)
+    # app.run(port=args.port)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `finally_data_logger-0.1.2/src/finally_data_logger.egg-info/PKG-INFO` & `finally_data_logger-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: finally-data-logger
-Version: 0.1.2
+Name: finally_data_logger
+Version: 0.2.0
 Summary: A simple data logging server and client.
 Home-page: https://github.com/arbasli2/FinallyDataLogger
 Author: arbasli
 Author-email: arbasli2@gmail.com
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -35,31 +35,36 @@
 ## Quick Start
 
 ### Starting the server
 
 From the command line:
 
 ```bash
-finally_data_logger_server --port 5000 --dir /path/to/storage/directory
+finallydatalogger --port 5000 --dir /path/to/storage/directory
+# to make it visible on the network
+finallydatalogger --host 0.0.0.0 --port 5000 --dir /path/to/storage/directory
 ```
 
 ### Using the client
 
 In your Python script:
 
 ```python
+import numpy as np
 from finally_data_logger import DataLogger
 
-logger = DataLogger(port=5000)
+logger = DataLogger(port=5000) #  DataLogger(server_url="http://192.168.x.x", port=5000)
 
 # Log some data
+img = np.random.rand(10,10)
+# a packet of data is stored in the form of a dictionary
 data = {
     "name": "test1",
     "duration": 0.3,
-    "image": your_numpy_image
+    "image": img
 }
 response = logger.log_data(data)
 print(response)
 
 # Fetch data
 criteria = {'name': 'test*'}
 results = logger.get_data(criteria, fetch_blob=True)
```

### Comparing `finally_data_logger-0.1.2/src/finally_data_logger.egg-info/SOURCES.txt` & `finally_data_logger-0.2.0/src/finally_data_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finally_data_logger-0.1.2/tests/test_data_logger.py` & `finally_data_logger-0.2.0/tests/test_data_logger.py`

 * *Files identical despite different names*

