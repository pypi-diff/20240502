# Comparing `tmp/quantastica-qps-api-0.9.8.tar.gz` & `tmp/quantastica-qps-api-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantastica-qps-api-0.9.8.tar", last modified: Fri Mar 17 00:46:55 2023, max compression
+gzip compressed data, was "quantastica-qps-api-0.9.9.tar", last modified: Sat Mar 18 22:49:03 2023, max compression
```

## Comparing `quantastica-qps-api-0.9.8.tar` & `quantastica-qps-api-0.9.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pera       (501) staff       (20)        0 2023-03-17 00:46:55.317562 quantastica-qps-api-0.9.8/
--rw-r--r--   0 pera       (501) staff       (20)    11357 2021-12-29 09:16:07.000000 quantastica-qps-api-0.9.8/LICENSE
--rw-r--r--   0 pera       (501) staff       (20)       25 2021-12-29 09:16:07.000000 quantastica-qps-api-0.9.8/MANIFEST.in
--rw-r--r--   0 pera       (501) staff       (20)    31465 2023-03-17 00:46:55.317425 quantastica-qps-api-0.9.8/PKG-INFO
--rw-r--r--   0 pera       (501) staff       (20)    30947 2023-03-16 23:32:17.000000 quantastica-qps-api-0.9.8/README.md
-drwxr-xr-x   0 pera       (501) staff       (20)        0 2023-03-17 00:46:55.315748 quantastica-qps-api-0.9.8/quantastica/
-drwxr-xr-x   0 pera       (501) staff       (20)        0 2023-03-17 00:46:55.316686 quantastica-qps-api-0.9.8/quantastica/qps_api/
--rw-r--r--   0 pera       (501) staff       (20)       44 2021-12-29 09:16:07.000000 quantastica-qps-api-0.9.8/quantastica/qps_api/__init__.py
--rw-r--r--   0 pera       (501) staff       (20)    13554 2023-03-16 23:56:38.000000 quantastica-qps-api-0.9.8/quantastica/qps_api/qps_api.py
-drwxr-xr-x   0 pera       (501) staff       (20)        0 2023-03-17 00:46:55.317266 quantastica-qps-api-0.9.8/quantastica_qps_api.egg-info/
--rw-r--r--   0 pera       (501) staff       (20)    31465 2023-03-17 00:46:55.000000 quantastica-qps-api-0.9.8/quantastica_qps_api.egg-info/PKG-INFO
--rw-r--r--   0 pera       (501) staff       (20)      367 2023-03-17 00:46:55.000000 quantastica-qps-api-0.9.8/quantastica_qps_api.egg-info/SOURCES.txt
--rw-r--r--   0 pera       (501) staff       (20)        1 2023-03-17 00:46:55.000000 quantastica-qps-api-0.9.8/quantastica_qps_api.egg-info/dependency_links.txt
--rw-r--r--   0 pera       (501) staff       (20)       12 2023-03-17 00:46:55.000000 quantastica-qps-api-0.9.8/quantastica_qps_api.egg-info/namespace_packages.txt
--rw-r--r--   0 pera       (501) staff       (20)       22 2023-03-17 00:46:55.000000 quantastica-qps-api-0.9.8/quantastica_qps_api.egg-info/requires.txt
--rw-r--r--   0 pera       (501) staff       (20)       12 2023-03-17 00:46:55.000000 quantastica-qps-api-0.9.8/quantastica_qps_api.egg-info/top_level.txt
--rw-r--r--   0 pera       (501) staff       (20)       38 2023-03-17 00:46:55.317592 quantastica-qps-api-0.9.8/setup.cfg
--rw-r--r--   0 pera       (501) staff       (20)     1547 2023-03-17 00:44:44.000000 quantastica-qps-api-0.9.8/setup.py
+drwxr-xr-x   0 pera       (501) staff       (20)        0 2023-03-18 22:49:03.397337 quantastica-qps-api-0.9.9/
+-rw-r--r--   0 pera       (501) staff       (20)    11357 2021-12-29 09:16:07.000000 quantastica-qps-api-0.9.9/LICENSE
+-rw-r--r--   0 pera       (501) staff       (20)       25 2021-12-29 09:16:07.000000 quantastica-qps-api-0.9.9/MANIFEST.in
+-rw-r--r--   0 pera       (501) staff       (20)    31513 2023-03-18 22:49:03.397198 quantastica-qps-api-0.9.9/PKG-INFO
+-rw-r--r--   0 pera       (501) staff       (20)    30995 2023-03-18 22:31:38.000000 quantastica-qps-api-0.9.9/README.md
+drwxr-xr-x   0 pera       (501) staff       (20)        0 2023-03-18 22:49:03.395262 quantastica-qps-api-0.9.9/quantastica/
+drwxr-xr-x   0 pera       (501) staff       (20)        0 2023-03-18 22:49:03.396273 quantastica-qps-api-0.9.9/quantastica/qps_api/
+-rw-r--r--   0 pera       (501) staff       (20)       44 2021-12-29 09:16:07.000000 quantastica-qps-api-0.9.9/quantastica/qps_api/__init__.py
+-rw-r--r--   0 pera       (501) staff       (20)    13554 2023-03-16 23:56:38.000000 quantastica-qps-api-0.9.9/quantastica/qps_api/qps_api.py
+drwxr-xr-x   0 pera       (501) staff       (20)        0 2023-03-18 22:49:03.397025 quantastica-qps-api-0.9.9/quantastica_qps_api.egg-info/
+-rw-r--r--   0 pera       (501) staff       (20)    31513 2023-03-18 22:49:03.000000 quantastica-qps-api-0.9.9/quantastica_qps_api.egg-info/PKG-INFO
+-rw-r--r--   0 pera       (501) staff       (20)      367 2023-03-18 22:49:03.000000 quantastica-qps-api-0.9.9/quantastica_qps_api.egg-info/SOURCES.txt
+-rw-r--r--   0 pera       (501) staff       (20)        1 2023-03-18 22:49:03.000000 quantastica-qps-api-0.9.9/quantastica_qps_api.egg-info/dependency_links.txt
+-rw-r--r--   0 pera       (501) staff       (20)       12 2023-03-18 22:49:03.000000 quantastica-qps-api-0.9.9/quantastica_qps_api.egg-info/namespace_packages.txt
+-rw-r--r--   0 pera       (501) staff       (20)       22 2023-03-18 22:49:03.000000 quantastica-qps-api-0.9.9/quantastica_qps_api.egg-info/requires.txt
+-rw-r--r--   0 pera       (501) staff       (20)       12 2023-03-18 22:49:03.000000 quantastica-qps-api-0.9.9/quantastica_qps_api.egg-info/top_level.txt
+-rw-r--r--   0 pera       (501) staff       (20)       38 2023-03-18 22:49:03.397372 quantastica-qps-api-0.9.9/setup.cfg
+-rw-r--r--   0 pera       (501) staff       (20)     1547 2023-03-18 22:47:30.000000 quantastica-qps-api-0.9.9/setup.py
```

### Comparing `quantastica-qps-api-0.9.8/LICENSE` & `quantastica-qps-api-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quantastica-qps-api-0.9.8/PKG-INFO` & `quantastica-qps-api-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantastica-qps-api
-Version: 0.9.8
+Version: 0.9.9
 Summary: Quantastica Quantum Programming Studio API
 Home-page: https://github.com/quantastica/qps-api
 Author: Quantastica
 Author-email: support@quantastica.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -1147,14 +1147,15 @@
 - `input` String. Program source code
 
 - `source` String. Input format:
 
 	- `qasm` [OpenQASM 2.0](https://github.com/Qiskit/openqasm) source code
 	- `quil` [Quil](https://arxiv.org/abs/1608.03355) source code
 	- `qobj` [QObj](https://arxiv.org/abs/1809.03452)
+	- `ionq` [IONQ](https://docs.ionq.com/) (json)
 	- `quantum-circuit` [quantum-circuit](https://www.npmjs.com/package/quantum-circuit) object (json)
 	- `toaster` [Qubit Toaster](https://quantastica.com/#toaster) object (json)
 
 - `dest` String. Output format:
 
 	- `qiskit` [Qiskit](https://qiskit.org/documentation/)
 	- `qasm` [OpenQASM 2.0](https://github.com/Qiskit/openqasm)
```

### Comparing `quantastica-qps-api-0.9.8/README.md` & `quantastica-qps-api-0.9.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1132,14 +1132,15 @@
 - `input` String. Program source code
 
 - `source` String. Input format:
 
 	- `qasm` [OpenQASM 2.0](https://github.com/Qiskit/openqasm) source code
 	- `quil` [Quil](https://arxiv.org/abs/1608.03355) source code
 	- `qobj` [QObj](https://arxiv.org/abs/1809.03452)
+	- `ionq` [IONQ](https://docs.ionq.com/) (json)
 	- `quantum-circuit` [quantum-circuit](https://www.npmjs.com/package/quantum-circuit) object (json)
 	- `toaster` [Qubit Toaster](https://quantastica.com/#toaster) object (json)
 
 - `dest` String. Output format:
 
 	- `qiskit` [Qiskit](https://qiskit.org/documentation/)
 	- `qasm` [OpenQASM 2.0](https://github.com/Qiskit/openqasm)
```

### Comparing `quantastica-qps-api-0.9.8/quantastica/qps_api/qps_api.py` & `quantastica-qps-api-0.9.9/quantastica/qps_api/qps_api.py`

 * *Files identical despite different names*

### Comparing `quantastica-qps-api-0.9.8/quantastica_qps_api.egg-info/PKG-INFO` & `quantastica-qps-api-0.9.9/quantastica_qps_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantastica-qps-api
-Version: 0.9.8
+Version: 0.9.9
 Summary: Quantastica Quantum Programming Studio API
 Home-page: https://github.com/quantastica/qps-api
 Author: Quantastica
 Author-email: support@quantastica.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -1147,14 +1147,15 @@
 - `input` String. Program source code
 
 - `source` String. Input format:
 
 	- `qasm` [OpenQASM 2.0](https://github.com/Qiskit/openqasm) source code
 	- `quil` [Quil](https://arxiv.org/abs/1608.03355) source code
 	- `qobj` [QObj](https://arxiv.org/abs/1809.03452)
+	- `ionq` [IONQ](https://docs.ionq.com/) (json)
 	- `quantum-circuit` [quantum-circuit](https://www.npmjs.com/package/quantum-circuit) object (json)
 	- `toaster` [Qubit Toaster](https://quantastica.com/#toaster) object (json)
 
 - `dest` String. Output format:
 
 	- `qiskit` [Qiskit](https://qiskit.org/documentation/)
 	- `qasm` [OpenQASM 2.0](https://github.com/Qiskit/openqasm)
```

### Comparing `quantastica-qps-api-0.9.8/setup.py` & `quantastica-qps-api-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="quantastica-qps-api",
-    version="0.9.8",
+    version="0.9.9",
     description="Quantastica Quantum Programming Studio API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/quantastica/qps-api",
     author="Quantastica",
     author_email="support@quantastica.com",
     license="Apache License 2.0",
```

