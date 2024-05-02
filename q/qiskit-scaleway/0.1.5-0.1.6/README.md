# Comparing `tmp/qiskit_scaleway-0.1.5.tar.gz` & `tmp/qiskit_scaleway-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_scaleway-0.1.5.tar", last modified: Tue Apr 16 12:39:04 2024, max compression
+gzip compressed data, was "qiskit_scaleway-0.1.6.tar", last modified: Thu May  2 16:06:21 2024, max compression
```

## Comparing `qiskit_scaleway-0.1.5.tar` & `qiskit_scaleway-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,26 @@
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-16 12:39:04.186541 qiskit_scaleway-0.1.5/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    11357 2024-02-29 13:51:39.000000 qiskit_scaleway-0.1.5/LICENSE
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2178 2024-04-16 12:39:04.186541 qiskit_scaleway-0.1.5/PKG-INFO
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1983 2024-04-16 12:36:19.000000 qiskit_scaleway-0.1.5/README.md
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-16 12:39:04.182541 qiskit_scaleway-0.1.5/qiskit_scaleway/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       39 2024-04-03 12:51:52.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/__init__.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-16 12:39:04.186541 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      178 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5083 2024-04-16 12:36:19.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/aer_backend.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3504 2024-04-10 09:37:46.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/aer_job.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3010 2024-04-16 12:36:19.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/qsim_backend.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     9781 2024-04-10 09:26:04.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/qsim_job.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1892 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/scaleway_backend.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2041 2024-04-10 09:26:04.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/scaleway_job.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-16 12:39:04.186541 qiskit_scaleway-0.1.5/qiskit_scaleway/primitives/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       70 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/primitives/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      740 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/primitives/aer_estimator.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      568 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/primitives/aer_sampler.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2532 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/provider.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-16 12:39:04.186541 qiskit_scaleway-0.1.5/qiskit_scaleway/utils/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       31 2024-04-03 12:51:52.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/utils/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3957 2024-04-16 12:36:19.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/utils/client.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-16 12:39:04.186541 qiskit_scaleway-0.1.5/qiskit_scaleway.egg-info/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2178 2024-04-16 12:39:04.000000 qiskit_scaleway-0.1.5/qiskit_scaleway.egg-info/PKG-INFO
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      744 2024-04-16 12:39:04.000000 qiskit_scaleway-0.1.5/qiskit_scaleway.egg-info/SOURCES.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)        1 2024-04-16 12:39:04.000000 qiskit_scaleway-0.1.5/qiskit_scaleway.egg-info/dependency_links.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      127 2024-04-16 12:39:04.000000 qiskit_scaleway-0.1.5/qiskit_scaleway.egg-info/requires.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       16 2024-04-16 12:39:04.000000 qiskit_scaleway-0.1.5/qiskit_scaleway.egg-info/top_level.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       38 2024-04-16 12:39:04.186541 qiskit_scaleway-0.1.5/setup.cfg
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      514 2024-04-16 12:37:52.000000 qiskit_scaleway-0.1.5/setup.py
+drwxr-xr-x   0 bonnie     (501) staff       (20)        0 2024-05-02 16:06:21.087203 qiskit_scaleway-0.1.6/
+-rw-r--r--   0 bonnie     (501) staff       (20)    11357 2024-03-25 15:53:04.000000 qiskit_scaleway-0.1.6/LICENSE
+-rw-r--r--   0 bonnie     (501) staff       (20)     3195 2024-05-02 16:06:21.086718 qiskit_scaleway-0.1.6/PKG-INFO
+-rw-r--r--   0 bonnie     (501) staff       (20)     2805 2024-05-02 16:05:31.000000 qiskit_scaleway-0.1.6/README.md
+drwxr-xr-x   0 bonnie     (501) staff       (20)        0 2024-05-02 16:06:21.079040 qiskit_scaleway-0.1.6/qiskit_scaleway/
+-rw-r--r--   0 bonnie     (501) staff       (20)       39 2024-04-19 13:45:11.000000 qiskit_scaleway-0.1.6/qiskit_scaleway/__init__.py
+drwxr-xr-x   0 bonnie     (501) staff       (20)        0 2024-05-02 16:06:21.084857 qiskit_scaleway-0.1.6/qiskit_scaleway/backends/
+-rw-r--r--   0 bonnie     (501) staff       (20)      178 2024-04-19 13:45:11.000000 qiskit_scaleway-0.1.6/qiskit_scaleway/backends/__init__.py
+-rw-r--r--   0 bonnie     (501) staff       (20)     5149 2024-05-02 16:05:31.000000 qiskit_scaleway-0.1.6/qiskit_scaleway/backends/aer_backend.py
+-rw-r--r--   0 bonnie     (501) staff       (20)     3504 2024-04-19 13:45:11.000000 qiskit_scaleway-0.1.6/qiskit_scaleway/backends/aer_job.py
+-rw-r--r--   0 bonnie     (501) staff       (20)     3076 2024-05-02 16:05:31.000000 qiskit_scaleway-0.1.6/qiskit_scaleway/backends/qsim_backend.py
+-rw-r--r--   0 bonnie     (501) staff       (20)     9781 2024-04-19 13:45:11.000000 qiskit_scaleway-0.1.6/qiskit_scaleway/backends/qsim_job.py
+-rw-r--r--   0 bonnie     (501) staff       (20)     2118 2024-05-02 16:05:31.000000 qiskit_scaleway-0.1.6/qiskit_scaleway/backends/scaleway_backend.py
+-rw-r--r--   0 bonnie     (501) staff       (20)     2041 2024-05-02 12:16:45.000000 qiskit_scaleway-0.1.6/qiskit_scaleway/backends/scaleway_job.py
+-rw-r--r--   0 bonnie     (501) staff       (20)     5132 2024-05-02 16:05:31.000000 qiskit_scaleway-0.1.6/qiskit_scaleway/provider.py
+drwxr-xr-x   0 bonnie     (501) staff       (20)        0 2024-05-02 16:06:21.085865 qiskit_scaleway-0.1.6/qiskit_scaleway/utils/
+-rw-r--r--   0 bonnie     (501) staff       (20)       31 2024-04-19 13:45:11.000000 qiskit_scaleway-0.1.6/qiskit_scaleway/utils/__init__.py
+-rw-r--r--   0 bonnie     (501) staff       (20)     4021 2024-05-02 16:05:31.000000 qiskit_scaleway-0.1.6/qiskit_scaleway/utils/client.py
+drwxr-xr-x   0 bonnie     (501) staff       (20)        0 2024-05-02 16:06:21.080948 qiskit_scaleway-0.1.6/qiskit_scaleway.egg-info/
+-rw-r--r--   0 bonnie     (501) staff       (20)     3195 2024-05-02 16:06:20.000000 qiskit_scaleway-0.1.6/qiskit_scaleway.egg-info/PKG-INFO
+-rw-r--r--   0 bonnie     (501) staff       (20)      619 2024-05-02 16:06:21.000000 qiskit_scaleway-0.1.6/qiskit_scaleway.egg-info/SOURCES.txt
+-rw-r--r--   0 bonnie     (501) staff       (20)        1 2024-05-02 16:06:20.000000 qiskit_scaleway-0.1.6/qiskit_scaleway.egg-info/dependency_links.txt
+-rw-r--r--   0 bonnie     (501) staff       (20)      148 2024-05-02 16:06:20.000000 qiskit_scaleway-0.1.6/qiskit_scaleway.egg-info/requires.txt
+-rw-r--r--   0 bonnie     (501) staff       (20)       16 2024-05-02 16:06:20.000000 qiskit_scaleway-0.1.6/qiskit_scaleway.egg-info/top_level.txt
+-rw-r--r--   0 bonnie     (501) staff       (20)       38 2024-05-02 16:06:21.087330 qiskit_scaleway-0.1.6/setup.cfg
+-rw-r--r--   0 bonnie     (501) staff       (20)      545 2024-05-02 16:06:14.000000 qiskit_scaleway-0.1.6/setup.py
```

### Comparing `qiskit_scaleway-0.1.5/LICENSE` & `qiskit_scaleway-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.5/PKG-INFO` & `qiskit_scaleway-0.1.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: qiskit_scaleway
-Version: 0.1.5
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Scaleway provider for Qiskit
 
 **Qiskit Scaleway** is a Python package to run quantum circuits on [Scaleway](https://www.scaleway.com/en/) infrastructure, providing access to [Aer](https://github.com/Qiskit/qiskit-aer) and [Qsim](https://github.com/quantumlib/qsim) simulators on powerful hardware (CPU and GPU).
 
 To run circuits over [Quandela](https://www.quandela.com/) backends provided by Scaleway, you must use [Perceval SDK](https://perceval.quandela.net/) through the [Scaleway provider](https://perceval.quandela.net/docs/providers.html).
 
 More info on the [Quantum service web page](https://labs.scaleway.com/en/qaas/).
@@ -21,26 +11,62 @@
 We encourage installing Scaleway provider via the pip tool (a Python package manager):
 
 ```bash
 pip install qiskit-scaleway
 ```
 
 ## Getting started
+
+To instantiate the ScalewayProvider, you need to have an access token and a project_id
+
 ```python
 from qiskit import QuantumCircuit
 from qiskit_scaleway import ScalewayProvider
 
 provider = ScalewayProvider(
     project_id="<your-scaleway-project-id>",
     secret_key="<your-scaleway-secret-key>",
 )
+```
+
+Alternatively, the Scaleway Provider can discover your access token from environment variables or from your .env file
+
+```
+export QISKIT_SCALEWAY_PROJECT_ID="project_id"
+export QISKIT_SCALEWAY_API_TOKEN="token"
+```
+
+Then you can instantiate the provider without any arguments:
+
+```python
+from qiskit import QuantumCircuit
+from qiskit_scaleway import ScalewayProvider
+
+provider = ScalewayProvider()
+```
+
+Now you can have acces to the supported backends:
+
+
+```python
+# List all operational backends
+backends = provider.backends(operational=True)
+print(backends)
+
+# List all backends with a minimum number of qbits
+backends = provider.backends(min_num_qubits=35)
+print(backends)
 
 # Retrieve a backend by providing search criteria. The search must have a single match
 backend = provider.get_backend("aer_simulation_h100")
+```
+
+Define a quantum circuit and run it
 
+```python
 # Define a quantum circuit that produces a 4-qubit GHZ state.
 qc = QuantumCircuit(4)
 qc.h(0)
 qc.cx(0, 1)
 qc.cx(0, 2)
 qc.cx(0, 3)
 qc.measure_all()
@@ -59,8 +85,7 @@
 This repository is at its early stage and is still in active development. If you are looking for a way to contribute please read [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Reach us
 We love feedback. Feel free to reach us on [Scaleway Slack community](https://slack.scaleway.com/), we are waiting for you on [#opensource](https://scaleway-community.slack.com/app_redirect?channel=opensource)..
 
 ## Licence
 [License Apache 2.0](LICENCE)
-
```

### Comparing `qiskit_scaleway-0.1.5/qiskit_scaleway/backends/aer_backend.py` & `qiskit_scaleway-0.1.6/qiskit_scaleway/backends/aer_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,23 +18,25 @@
 class AerBackend(ScalewayBackend):
     def __init__(
         self,
         provider,
         client: QaaSClient,
         backend_id: str,
         name: str,
+        availability: str,
         version: str,
         num_qubits: int,
         metadata: str,
     ):
         super().__init__(
             provider=provider,
             client=client,
             backend_id=backend_id,
             name=name,
+            availability=availability,
             version=version,
         )
 
         self._options = self._default_options()
 
         # Create Target
         self._configuration = QasmBackendConfiguration.from_dict(
```

### Comparing `qiskit_scaleway-0.1.5/qiskit_scaleway/backends/aer_job.py` & `qiskit_scaleway-0.1.6/qiskit_scaleway/backends/aer_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.5/qiskit_scaleway/backends/qsim_backend.py` & `qiskit_scaleway-0.1.6/qiskit_scaleway/backends/qsim_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 class QsimBackend(ScalewayBackend):
     def __init__(
         self,
         provider,
         client: QaaSClient,
         backend_id: str,
         name: str,
+        availability: str,
         version: str,
         num_qubits: int,
         metadata: str,
     ):
         super().__init__(
             provider=provider,
             client=client,
             backend_id=backend_id,
             name=name,
+            availability=availability,
             version=version,
         )
 
         self._options = self._default_options()
 
         # Set option validators
         self.options.set_validator("shots", (1, 10000000))
```

### Comparing `qiskit_scaleway-0.1.5/qiskit_scaleway/backends/qsim_job.py` & `qiskit_scaleway-0.1.6/qiskit_scaleway/backends/qsim_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.5/qiskit_scaleway/backends/scaleway_backend.py` & `qiskit_scaleway-0.1.6/qiskit_scaleway/backends/scaleway_backend.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,25 +10,35 @@
 class ScalewayBackend(Backend, ABC):
     def __init__(
         self,
         provider,
         client: QaaSClient,
         backend_id: str,
         name: str,
+        availability: str,
         version: str,
     ):
         super().__init__(provider=provider, backend_version=version, name=name)
 
         self._backend_id = backend_id
+        self._availability = availability
         self._client = client
 
     @property
     def id(self):
         return self._backend_id
 
+    @property
+    def availability(self):
+        return self._availability
+
+    @property
+    def num_qubits(self) -> int:
+        return self._max_qubits
+
     def start_session(
         self,
         name: str = None,
         deduplication_id: str = None,
         max_duration: Union[int, str] = None,
         max_idle_duration: Union[int, str] = None,
     ) -> str:
```

### Comparing `qiskit_scaleway-0.1.5/qiskit_scaleway/backends/scaleway_job.py` & `qiskit_scaleway-0.1.6/qiskit_scaleway/backends/scaleway_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.5/qiskit_scaleway/utils/client.py` & `qiskit_scaleway-0.1.6/qiskit_scaleway/utils/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,18 +21,20 @@
     def _api_headers(self) -> dict:
         return {"X-Auth-Token": self.__token}
 
     def _build_endpoint(self, endpoint: str) -> str:
         return f"{self.__url}{endpoint}"
 
     def list_platforms(self, name: str) -> dict:
-        assert name is not None
+        filter_by_name = ""
+        if (name):
+            filter_by_name = f"?name={name}"
 
         http_client = self._http_client()
-        endpoint = f"{self._build_endpoint(_ENDPOINT_PLATFORM)}?name={name}"
+        endpoint = f"{self._build_endpoint(_ENDPOINT_PLATFORM)}{filter_by_name}"
 
         resp = http_client.get(endpoint)
         resp.raise_for_status()
 
         return resp.json()
 
     def create_session(
```

### Comparing `qiskit_scaleway-0.1.5/qiskit_scaleway.egg-info/SOURCES.txt` & `qiskit_scaleway-0.1.6/qiskit_scaleway.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -11,12 +11,9 @@
 qiskit_scaleway/backends/__init__.py
 qiskit_scaleway/backends/aer_backend.py
 qiskit_scaleway/backends/aer_job.py
 qiskit_scaleway/backends/qsim_backend.py
 qiskit_scaleway/backends/qsim_job.py
 qiskit_scaleway/backends/scaleway_backend.py
 qiskit_scaleway/backends/scaleway_job.py
-qiskit_scaleway/primitives/__init__.py
-qiskit_scaleway/primitives/aer_estimator.py
-qiskit_scaleway/primitives/aer_sampler.py
 qiskit_scaleway/utils/__init__.py
 qiskit_scaleway/utils/client.py
```

### Comparing `qiskit_scaleway-0.1.5/setup.py` & `qiskit_scaleway-0.1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="qiskit_scaleway",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     install_requires=[
         "qiskit==1.0.2",
         "qiskit-aer==0.14.0.1",
         "randomname==0.2.1",
         "httpx==0.27.0",
         "dataclasses-json==0.6.4",
         "dataclasses==0.6",
         "pytimeparse==1.1.8",
+        "python-dotenv==1.0.1"
     ],
     long_description=description,
     long_description_content_type="text/markdown",
 )
```

