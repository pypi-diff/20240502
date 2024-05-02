# Comparing `tmp/worker_dispatcher-0.0.3.tar.gz` & `tmp/worker_dispatcher-1.0.0.tar.gz`

## Comparing `worker_dispatcher-0.0.3.tar` & `worker_dispatcher-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.3/src/worker_dispatcher/__init__.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.3/src/worker_dispatcher/worker_dispatcher.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.3/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.3/LICENSE
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.3/README.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 worker_dispatcher-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/img/introduction.planuml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/src/worker_dispatcher/__init__.py
+-rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/src/worker_dispatcher/worker_dispatcher.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8366 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.0/PKG-INFO
```

### Comparing `worker_dispatcher-0.0.3/.github/workflows/python-publish.yml` & `worker_dispatcher-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `worker_dispatcher-0.0.3/.gitignore` & `worker_dispatcher-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `worker_dispatcher-0.0.3/LICENSE` & `worker_dispatcher-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `worker_dispatcher-0.0.3/README.md` & `worker_dispatcher-1.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -21,19 +21,27 @@
 
 ---
 
 OUTLINE
 -------
 
 - [Demonstration](#demonstration)
+- [Introduction](#introduction)
 - [Installation](#installation)
 - [Usage](#usage)
     - [Option](#option)
         - [callbacks.process](#callbacksprocess)
         - [callbacks.task](#callbackstask)
+    - [Other Methods](#other-methods)
+        - [get_results()](#get_results)
+        - [get_logs()](#get_logs)
+        - [get_result_info()](#get_result_info)
+        - [get_tps()](#get_tps)
+    - [Scenarios](#scenarios)
+        - [Stress Test](#stress-test)
 
 ---
 
 DEMONSTRATION
 -------------
 
 Use 20 theads concurrently to dispatch tasks for HTTP reqeusts
@@ -79,25 +87,36 @@
             'multiprocessing': True
         }
     })
 ```
 
 ---
 
-## INSTALLATION
+INTRODUCTION
+------------
+
+This library helps to efficiently consume tasks by using multiple threading or processing and returns all results jointly.
+
+![Introduction](https://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/yidas/python-worker-dispatcher/main/img/introduction.planuml&v=1)
+
+---
+
+INSTALLATION
+------------
 
 To install the current release:
 
 ```shell
 $ pip install worker-dispatcher
 ```
 
 ---
 
-## USAGE
+USAGE
+-----
 
 By calling the `start()` methid with the configuration parameter, the package will begin dispatching tasks while managing threading or processing based on the provided settings. Once the tasks are completed, the package will return all the results.
 
 An example configuration setting with all options is as follows:
 
 ```python
 import worker_dispatcher 
@@ -109,58 +128,129 @@
         'callback': your_function_name_for_each_task,
         'config': {'your_config': 'your_value'},
         'result_callback': your_function_name_for_each_result,
     },
     'worker': {
         'number': 8,
         'per_second': 0,                # If greater than 0, the specified number of workers run forcefully at set intervals.
+        'cumulative': False,            # Cumulative mode for per_second method.
         'multiprocessing': False
     }
 })
 ```
 
 ### Options
 
 |Option            |Type     |Deafult      |Description|
 |:--               |:--      |:--          |:--        |
-|debug             |boolean  |False        |Debug mode |
+|debug             |bool     |False        |Debug mode |
 |task.list         |multitype|list         |The tasks for dispatching to each worker. *<br>- List: Each value will be passed as a parameter to your callback function. <br>- Integer: The number of tasks to be generated.|
 |[task.callback](#taskcallback)             |callable |(sample)          |The callback function called by each worker runs|
 |task.config       |multitype|list         |The custom variable to be passed to the callback function|
 |[task.result_callback](#taskresultcallback) |callable |Null          |The callback function called when each task processes the result|
-|worker.number     |integer  |(auto)       |The number of workers to fork. <br>(The default value is the number of local CPU cores)|
+|worker.number     |int      |(auto)       |The number of workers to fork. <br>(The default value is the number of local CPU cores)|
 |worker.per_second |float    |0            |If greater than 0, the specified number of workers run forcefully at set intervals.|
+|worker.cumulative |bool     |False        |Cumulative mode for per_second method.|
 |worker.multiprocessing                     |boolean  |False        |Use multi-processing instead of the default multi-threading |
 
 
 #### task.callback
 
 The callback function called by each worker runs
 
 ```python
 callback_function (id: int=None, config=None, task=None)
 ```
 
 |Argument          |Type     |Deafult      |Description|
 |:--               |:--      |:--          |:--        |
-|id                |integer  |(auto)       |The sequence number generated by each task starting from 1|
+|id                |int      |(auto)       |The sequence number generated by each task starting from 1|
 |config            |multitype|{}           |The custom variable to be passed to the callback function|
 |task              |multitype|(custom)     |Each value from the `task.list`|
 
 
-#### task.result_allback
+#### task.result_callback
 
 The callback function called when each task processes the result
 
 ```python
 result_callback_function (id: int=None, config=None, result=None, log: dict=None)
 ```
 
 |Argument          |Type     |Deafult      |Description|
 |:--               |:--      |:--          |:--        |
-|id                |integer  |(auto)       |The sequence number generated by each task starting from 1|
+|id                |int      |(auto)       |The sequence number generated by each task starting from 1|
 |config            |multitype|{}           |The custom variable to be passed to the callback function|
 |result            |multitype|(custom)     |Each value returned back from `task.callback`|
-|log               |dict     |(auto)       |Each log containing the result of each task processed by the worker <br>- task_id <br>- started_at <br>- ended_at <br>- duration <br>- result|
+|log               |dict     |(auto)       |Reference: [get_logs()](#get_logs)|
+
+
+### Other Methods
+
+- #### get_results()
+    Get all results in list type after completing `start()`
+
+- #### get_logs()
+    Get all logs in list type after completing `start()`
+
+    Each log is of type dict, containing the results of every task processed by the worker:
+    - task_id 
+    - started_at 
+    - ended_at 
+    - duration 
+    - result
+
+- #### get_result_info()
+    Get a dict with the whole spending time and started/ended timestamps after completing `start()`
+
+- #### get_tps()
+    Get TPS report in dict type after completing `start()` or by passing a list data.
+  ```python
+  def get_tps(logs: dict=None, debug: bool=False, peak_duration: float=0) -> dict:
+  ```
+  The log dict matches that of the [get_logs()](#get_logs), each `result` of a log will be considered valid if it meets one of the following conditions:
+  - It is a `requests.Response` object with a status code of 200
+  - It is a valid value other than the aforementioned object
+
+### Scenarios
+
+#### Stress Test
+
+Perform a stress test scenario with 10 requests per second.
+
+```python
+import worker_dispatcher, requests
+
+def each_task(id, config, task):
+    response = None
+    try:
+        response = requests.get(config['my_endpoint'], timeout=(5, 10))
+    except requests.exceptions.RequestException as e:
+        print("An error occurred:", e)
+    return response
+
+responses = worker_dispatcher.start({
+    'task': {
+        'list': 5000,
+        'callback': each_task,
+        'config': {
+            'my_endpoint': 'https://your.name/api'
+        },
+    },
+    'worker': {
+        'number': 10,
+        'per_second': 1
+    }
+})
+
+print(worker_dispatcher.get_logs())
+print(worker_dispatcher.get_tps())
+```
+
+
+
+
+
+
```

### Comparing `worker_dispatcher-0.0.3/pyproject.toml` & `worker_dispatcher-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "worker_dispatcher"
-version = "0.0.3"
+version = "1.0.0"
 authors = [
   { name="Nick Tsai", email="myintaer@gmail.com" },
 ]
-description = "Developing"
+description = "A flexible task dispatcher for Python with multiple threading or processing control"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/yidas/python-worker-dispatcher"
-Issues = "https://github.com/yidas/python-worker-dispatcher/issues"
+Issues = "https://github.com/yidas/python-worker-dispatcher/issues"
```

### Comparing `worker_dispatcher-0.0.3/PKG-INFO` & `worker_dispatcher-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: worker_dispatcher
-Version: 0.0.3
-Summary: Developing
+Version: 1.0.0
+Summary: A flexible task dispatcher for Python with multiple threading or processing control
 Project-URL: Homepage, https://github.com/yidas/python-worker-dispatcher
 Project-URL: Issues, https://github.com/yidas/python-worker-dispatcher/issues
 Author-email: Nick Tsai <myintaer@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -35,19 +35,27 @@
 
 ---
 
 OUTLINE
 -------
 
 - [Demonstration](#demonstration)
+- [Introduction](#introduction)
 - [Installation](#installation)
 - [Usage](#usage)
     - [Option](#option)
         - [callbacks.process](#callbacksprocess)
         - [callbacks.task](#callbackstask)
+    - [Other Methods](#other-methods)
+        - [get_results()](#get_results)
+        - [get_logs()](#get_logs)
+        - [get_result_info()](#get_result_info)
+        - [get_tps()](#get_tps)
+    - [Scenarios](#scenarios)
+        - [Stress Test](#stress-test)
 
 ---
 
 DEMONSTRATION
 -------------
 
 Use 20 theads concurrently to dispatch tasks for HTTP reqeusts
@@ -93,25 +101,36 @@
             'multiprocessing': True
         }
     })
 ```
 
 ---
 
-## INSTALLATION
+INTRODUCTION
+------------
+
+This library helps to efficiently consume tasks by using multiple threading or processing and returns all results jointly.
+
+![Introduction](https://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/yidas/python-worker-dispatcher/main/img/introduction.planuml&v=1)
+
+---
+
+INSTALLATION
+------------
 
 To install the current release:
 
 ```shell
 $ pip install worker-dispatcher
 ```
 
 ---
 
-## USAGE
+USAGE
+-----
 
 By calling the `start()` methid with the configuration parameter, the package will begin dispatching tasks while managing threading or processing based on the provided settings. Once the tasks are completed, the package will return all the results.
 
 An example configuration setting with all options is as follows:
 
 ```python
 import worker_dispatcher 
@@ -123,58 +142,129 @@
         'callback': your_function_name_for_each_task,
         'config': {'your_config': 'your_value'},
         'result_callback': your_function_name_for_each_result,
     },
     'worker': {
         'number': 8,
         'per_second': 0,                # If greater than 0, the specified number of workers run forcefully at set intervals.
+        'cumulative': False,            # Cumulative mode for per_second method.
         'multiprocessing': False
     }
 })
 ```
 
 ### Options
 
 |Option            |Type     |Deafult      |Description|
 |:--               |:--      |:--          |:--        |
-|debug             |boolean  |False        |Debug mode |
+|debug             |bool     |False        |Debug mode |
 |task.list         |multitype|list         |The tasks for dispatching to each worker. *<br>- List: Each value will be passed as a parameter to your callback function. <br>- Integer: The number of tasks to be generated.|
 |[task.callback](#taskcallback)             |callable |(sample)          |The callback function called by each worker runs|
 |task.config       |multitype|list         |The custom variable to be passed to the callback function|
 |[task.result_callback](#taskresultcallback) |callable |Null          |The callback function called when each task processes the result|
-|worker.number     |integer  |(auto)       |The number of workers to fork. <br>(The default value is the number of local CPU cores)|
+|worker.number     |int      |(auto)       |The number of workers to fork. <br>(The default value is the number of local CPU cores)|
 |worker.per_second |float    |0            |If greater than 0, the specified number of workers run forcefully at set intervals.|
+|worker.cumulative |bool     |False        |Cumulative mode for per_second method.|
 |worker.multiprocessing                     |boolean  |False        |Use multi-processing instead of the default multi-threading |
 
 
 #### task.callback
 
 The callback function called by each worker runs
 
 ```python
 callback_function (id: int=None, config=None, task=None)
 ```
 
 |Argument          |Type     |Deafult      |Description|
 |:--               |:--      |:--          |:--        |
-|id                |integer  |(auto)       |The sequence number generated by each task starting from 1|
+|id                |int      |(auto)       |The sequence number generated by each task starting from 1|
 |config            |multitype|{}           |The custom variable to be passed to the callback function|
 |task              |multitype|(custom)     |Each value from the `task.list`|
 
 
-#### task.result_allback
+#### task.result_callback
 
 The callback function called when each task processes the result
 
 ```python
 result_callback_function (id: int=None, config=None, result=None, log: dict=None)
 ```
 
 |Argument          |Type     |Deafult      |Description|
 |:--               |:--      |:--          |:--        |
-|id                |integer  |(auto)       |The sequence number generated by each task starting from 1|
+|id                |int      |(auto)       |The sequence number generated by each task starting from 1|
 |config            |multitype|{}           |The custom variable to be passed to the callback function|
 |result            |multitype|(custom)     |Each value returned back from `task.callback`|
-|log               |dict     |(auto)       |Each log containing the result of each task processed by the worker <br>- task_id <br>- started_at <br>- ended_at <br>- duration <br>- result|
+|log               |dict     |(auto)       |Reference: [get_logs()](#get_logs)|
+
+
+### Other Methods
+
+- #### get_results()
+    Get all results in list type after completing `start()`
+
+- #### get_logs()
+    Get all logs in list type after completing `start()`
+
+    Each log is of type dict, containing the results of every task processed by the worker:
+    - task_id 
+    - started_at 
+    - ended_at 
+    - duration 
+    - result
+
+- #### get_result_info()
+    Get a dict with the whole spending time and started/ended timestamps after completing `start()`
+
+- #### get_tps()
+    Get TPS report in dict type after completing `start()` or by passing a list data.
+  ```python
+  def get_tps(logs: dict=None, debug: bool=False, peak_duration: float=0) -> dict:
+  ```
+  The log dict matches that of the [get_logs()](#get_logs), each `result` of a log will be considered valid if it meets one of the following conditions:
+  - It is a `requests.Response` object with a status code of 200
+  - It is a valid value other than the aforementioned object
+
+### Scenarios
+
+#### Stress Test
+
+Perform a stress test scenario with 10 requests per second.
+
+```python
+import worker_dispatcher, requests
+
+def each_task(id, config, task):
+    response = None
+    try:
+        response = requests.get(config['my_endpoint'], timeout=(5, 10))
+    except requests.exceptions.RequestException as e:
+        print("An error occurred:", e)
+    return response
+
+responses = worker_dispatcher.start({
+    'task': {
+        'list': 5000,
+        'callback': each_task,
+        'config': {
+            'my_endpoint': 'https://your.name/api'
+        },
+    },
+    'worker': {
+        'number': 10,
+        'per_second': 1
+    }
+})
+
+print(worker_dispatcher.get_logs())
+print(worker_dispatcher.get_tps())
+```
+
+
+
+
+
+
```

