# Comparing `tmp/dhuodata-lib-0.2.3.tar.gz` & `tmp/dhuodata_lib-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata-lib-0.2.3.tar", last modified: Tue Apr 30 03:39:18 2024, max compression
+gzip compressed data, was "dhuodata_lib-0.2.4.tar", last modified: Wed May  1 23:06:52 2024, max compression
```

## Comparing `dhuodata-lib-0.2.3.tar` & `dhuodata_lib-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 03:39:18.168500 dhuodata-lib-0.2.3/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2528 2024-04-30 03:39:18.168500 dhuodata-lib-0.2.3/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata-lib-0.2.3/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-30 03:39:18.168500 dhuodata-lib-0.2.3/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-04-30 03:39:05.000000 dhuodata-lib-0.2.3/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 03:39:18.168500 dhuodata-lib-0.2.3/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 03:39:18.168500 dhuodata-lib-0.2.3/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     2528 2024-04-30 03:39:18.000000 dhuodata-lib-0.2.3/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-04-30 03:39:18.000000 dhuodata-lib-0.2.3/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-30 03:39:18.000000 dhuodata-lib-0.2.3/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-04-30 03:39:18.000000 dhuodata-lib-0.2.3/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-04-30 03:39:18.000000 dhuodata-lib-0.2.3/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 03:39:18.168500 dhuodata-lib-0.2.3/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata-lib-0.2.3/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata-lib-0.2.3/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     4125 2024-04-30 02:11:57.000000 dhuodata-lib-0.2.3/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata-lib-0.2.3/src/dhuolib/config.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata-lib-0.2.3/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1364 2024-04-30 03:38:55.000000 dhuodata-lib-0.2.3/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      750 2024-04-29 11:53:52.000000 dhuodata-lib-0.2.3/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata-lib-0.2.3/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-30 03:39:18.168500 dhuodata-lib-0.2.3/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     2540 2024-04-29 12:52:51.000000 dhuodata-lib-0.2.3/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-01 23:06:52.751688 dhuodata_lib-0.2.4/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-01 23:06:52.751688 dhuodata_lib-0.2.4/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.4/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-01 23:06:52.751688 dhuodata_lib-0.2.4/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-01 23:06:06.000000 dhuodata_lib-0.2.4/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-01 23:06:52.747688 dhuodata_lib-0.2.4/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-01 23:06:52.747688 dhuodata_lib-0.2.4/src/dhuodata_lib.egg-info/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-01 23:06:52.000000 dhuodata_lib-0.2.4/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-05-01 23:06:52.000000 dhuodata_lib-0.2.4/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-01 23:06:52.000000 dhuodata_lib-0.2.4/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-01 23:06:52.000000 dhuodata_lib-0.2.4/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-01 23:06:52.000000 dhuodata_lib-0.2.4/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-01 23:06:52.747688 dhuodata_lib-0.2.4/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.4/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.2.4/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     4249 2024-04-30 19:18:11.000000 dhuodata_lib-0.2.4/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata_lib-0.2.4/src/dhuolib/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.2.4/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1341 2024-04-30 19:13:45.000000 dhuodata_lib-0.2.4/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      750 2024-04-29 11:53:52.000000 dhuodata_lib-0.2.4/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.2.4/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-01 23:06:52.747688 dhuodata_lib-0.2.4/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2901 2024-05-01 23:06:51.000000 dhuodata_lib-0.2.4/tests/test_dhuolib.py
```

### Comparing `dhuodata-lib-0.2.3/PKG-INFO` & `dhuodata_lib-0.2.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
+Requires-Dist: oci==2.125.3
+Requires-Dist: pydantic==1.8.2
 Provides-Extra: interactive
+Requires-Dist: mypy==1.5.1; extra == "interactive"
+Requires-Dist: flake8==6.1.0; extra == "interactive"
+Requires-Dist: black==22.3.0; extra == "interactive"
+Requires-Dist: pytest-cov~=4.0; extra == "interactive"
+Requires-Dist: pytest~=7.0; extra == "interactive"
+Requires-Dist: twine==3.4.2; extra == "interactive"
+Requires-Dist: wheel==0.37.0; extra == "interactive"
+Requires-Dist: oci==2.125.3; extra == "interactive"
 
 # DHuO LIb
 
 ## Board
 
 ![](assets/imgs/board.png)
```

### Comparing `dhuodata-lib-0.2.3/README.md` & `dhuodata_lib-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.2.3/setup.py` & `dhuodata_lib-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.2.3",
+    version="0.2.4",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata-lib-0.2.3/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata_lib-0.2.4/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
+Requires-Dist: oci==2.125.3
+Requires-Dist: pydantic==1.8.2
 Provides-Extra: interactive
+Requires-Dist: mypy==1.5.1; extra == "interactive"
+Requires-Dist: flake8==6.1.0; extra == "interactive"
+Requires-Dist: black==22.3.0; extra == "interactive"
+Requires-Dist: pytest-cov~=4.0; extra == "interactive"
+Requires-Dist: pytest~=7.0; extra == "interactive"
+Requires-Dist: twine==3.4.2; extra == "interactive"
+Requires-Dist: wheel==0.37.0; extra == "interactive"
+Requires-Dist: oci==2.125.3; extra == "interactive"
 
 # DHuO LIb
 
 ## Board
 
 ![](assets/imgs/board.png)
```

### Comparing `dhuodata-lib-0.2.3/src/dhuolib/clients.py` & `dhuodata_lib-0.2.4/src/dhuolib/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pydantic import ValidationError
-
+import json
 from dhuolib.config import logger
 from dhuolib.services import ServiceAPIML
 from dhuolib.validations import ExperimentBody, RunExperimentBody
 
 
 class DhuolibClient:
     def __init__(self, service_endpoint=None):
@@ -21,14 +21,16 @@
                     'requirements_file': ('requirements.txt', open(experiment_params['requirements_file'], 'rb'), 'text/plain'),
                     'model_pkl_file': ('model.pkl', open(experiment_params['model_pkl_file'], 'rb'), 'application/octet-stream')
                 }
                 print(experiment_params)
             except FileNotFoundError as e:
                 logger.error(f"Error: {e}")
                 return {"error": str(e)}
+            
+            experiment_params['experiment_tags'] = json.dumps(experiment_params['experiment_tags'])
 
             response = self.service.create_experiment_by_conf_json(
                 experiment_params=experiment_params,
                 files=files)
 
             experiment = response.json()
             logger.info(
```

### Comparing `dhuodata-lib-0.2.3/src/dhuolib/predict.py` & `dhuodata_lib-0.2.4/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.2.3/src/dhuolib/services.py` & `dhuodata_lib-0.2.4/src/dhuolib/services.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     def create_experiment_by_conf_json(self, experiment_params, files):
         if experiment_params is None and isinstance(experiment_params, dict):
             raise ValueError("json_data must be a dict")
 
         response = requests.post(
             f"{self.service_endpoint}/save",
-            json={'experiment_params': experiment_params},
+            data=experiment_params,
             files=files
         )
         return response
 
     def run_experiment(self, run_params, files=None):
         if run_params is None and isinstance(run_params, str):
             raise ValueError("json_data must be a dict")
```

### Comparing `dhuodata-lib-0.2.3/src/dhuolib/validations.py` & `dhuodata_lib-0.2.4/src/dhuolib/validations.py`

 * *Files identical despite different names*

### Comparing `dhuodata-lib-0.2.3/tests/test_dhuolib.py` & `dhuodata_lib-0.2.4/tests/test_dhuolib.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,20 +5,29 @@
 
 sys.path.append("src")
 from dhuolib.clients import DhuolibClient
 
 
 class TestDhuolibUtils(unittest.TestCase):
     def setUp(self):
-        self.end_point = "http://fake-endpoint"
+        self.end_point = "http://localhost:8000"
         self.dhuolib = DhuolibClient(service_endpoint=self.end_point)
-        self.namespace = "engdb"
-        self.bucket_name = "dhuodata-mlops"
         self.file_path = "tests/files/LogisticRegression_best.pickle"
+        
+    # def test_integracao(self):
+    #     experiment_params = {
+    #         "experiment_name": "test_experiment_nlp",
+    #         "experiment_tags": {"version": "v1", "priority": "P1"},
+    #         "model_pkl_file": "tests/files/LogisticRegression_best.pickle",
+    #         "requirements_file": "tests/files/requirements.txt"
+    #     }
 
+    #     response = self.dhuolib.create_experiment(experiment_params)
+
+        
     def test_deve_lancar_excecao_com_valores_run_params_incorretos(self):
         experiment_params = {
             "experiment_name": "test_experiment",
             "experiment_tags": {"version": "v1", "priority": "P1"}
         }
         response = self.dhuolib.create_experiment(experiment_params)
         self.assertEqual(list(response.keys()), ["error"])
```

