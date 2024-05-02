# Comparing `tmp/ts_mock_api-0.1.1.tar.gz` & `tmp/ts_mock_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts_mock_api-0.1.1.tar", max compression
+gzip compressed data, was "ts_mock_api-0.1.2.tar", max compression
```

## Comparing `ts_mock_api-0.1.1.tar` & `ts_mock_api-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,6 @@
--rw-r--r--   0        0        0     1072 2024-01-15 08:40:07.624939 ts_mock_api-0.1.1/LICENSE
--rw-r--r--   0        0        0       32 2024-01-15 08:40:07.624939 ts_mock_api-0.1.1/README.md
--rw-r--r--   0        0        0      315 2024-01-18 15:41:18.281484 ts_mock_api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       74 2024-01-15 09:01:48.458317 ts_mock_api-0.1.1/tsmockapi/__init__.py
--rw-r--r--   0        0        0     4433 2024-01-18 15:30:29.476465 ts_mock_api-0.1.1/tsmockapi/dto/io.py
--rw-r--r--   0        0        0       14 2023-12-18 15:05:49.484843 ts_mock_api-0.1.1/tsmockapi/resources/test.json
--rw-r--r--   0        0        0      147 2023-12-18 15:05:33.816743 ts_mock_api-0.1.1/tsmockapi/settings.py
--rw-r--r--   0        0        0      793 2024-01-15 09:01:48.454318 ts_mock_api-0.1.1/tsmockapi/ts_interface.py
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 ts_mock_api-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-01-15 08:40:07.624939 ts_mock_api-0.1.2/LICENSE
+-rw-r--r--   0        0        0       32 2024-01-15 08:40:07.624939 ts_mock_api-0.1.2/README.md
+-rw-r--r--   0        0        0      323 2024-05-02 09:52:29.399798 ts_mock_api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       73 2024-05-02 08:27:48.857981 ts_mock_api-0.1.2/tsmockapi/__init__.py
+-rw-r--r--   0        0        0     6954 2024-05-02 09:43:27.338245 ts_mock_api-0.1.2/tsmockapi/ts_mock_api.py
+-rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 ts_mock_api-0.1.2/PKG-INFO
```

### Comparing `ts_mock_api-0.1.1/LICENSE` & `ts_mock_api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ts_mock_api-0.1.1/PKG-INFO` & `ts_mock_api-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: ts-mock-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
-License: MIT
 Author: ph
 Author-email: ph@tordenskjold.space
-Requires-Python: >=3.7,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: ts-interface (>=0.1.1,<0.2.0)
 Description-Content-Type: text/markdown
 
 # ts-mock
 Tordenskjold mock api
```

