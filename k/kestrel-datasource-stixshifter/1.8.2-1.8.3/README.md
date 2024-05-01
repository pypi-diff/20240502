# Comparing `tmp/kestrel_datasource_stixshifter-1.8.2.tar.gz` & `tmp/kestrel_datasource_stixshifter-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kestrel_datasource_stixshifter-1.8.2.tar", last modified: Mon Apr 22 18:07:20 2024, max compression
+gzip compressed data, was "kestrel_datasource_stixshifter-1.8.3.tar", last modified: Wed May  1 23:18:14 2024, max compression
```

## Comparing `kestrel_datasource_stixshifter-1.8.2.tar` & `kestrel_datasource_stixshifter-1.8.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:07:20.301728 kestrel_datasource_stixshifter-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-04-22 18:07:20.301728 kestrel_datasource_stixshifter-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 18:07:20.301728 kestrel_datasource_stixshifter-1.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:07:20.297728 kestrel_datasource_stixshifter-1.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:07:20.297728 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:07:20.301728 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/worker/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/worker/transmitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:07:20.301728 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-04-22 18:07:20.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-22 18:07:20.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:07:20.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-22 18:07:20.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-22 18:07:20.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 18:07:20.000000 kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:07:20.301728 kestrel_datasource_stixshifter-1.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/tests/test_command_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/tests/test_stixshifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/tests/test_stixshifter_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-22 18:07:09.000000 kestrel_datasource_stixshifter-1.8.2/tests/test_stixshifter_translator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:18:14.159149 kestrel_datasource_stixshifter-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-05-01 23:18:14.159149 kestrel_datasource_stixshifter-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 23:18:14.159149 kestrel_datasource_stixshifter-1.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:18:14.155149 kestrel_datasource_stixshifter-1.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:18:14.155149 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/subquery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:18:14.159149 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/worker/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/worker/transmitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:18:14.159149 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-05-01 23:18:14.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-01 23:18:14.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 23:18:14.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-01 23:18:14.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-01 23:18:14.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-01 23:18:14.000000 kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:18:14.159149 kestrel_datasource_stixshifter-1.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/tests/test_command_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/tests/test_stixshifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/tests/test_stixshifter_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-01 23:18:03.000000 kestrel_datasource_stixshifter-1.8.3/tests/test_stixshifter_translator.py
```

### Comparing `kestrel_datasource_stixshifter-1.8.2/PKG-INFO` & `kestrel_datasource_stixshifter-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kestrel_datasource_stixshifter
-Version: 1.8.2
+Version: 1.8.3
 Summary: Kestrel STIX-shifter Datasource Interface
 Maintainer-email: Xiaokui Shu <xiaokui.shu@ibm.com>, Paul Coccoli <pcoccoli@us.ibm.com>
 License: Apache 2.0 License
 Project-URL: Homepage, https://github.com/opencybersecurityalliance/kestrel-lang
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Project-URL: Repository, https://github.com/opencybersecurityalliance/kestrel-lang.git
 Keywords: kestrel,datasource,interface,STIX-shifter
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: kestrel_core>=1.8.1
-Requires-Dist: lxml>=5.2.1
+Requires-Dist: lxml==4.9.4
 Requires-Dist: requests>=2.31.0
 Requires-Dist: nest-asyncio>=1.6.0
 Requires-Dist: stix-shifter==7.0.6
 Requires-Dist: stix-shifter-utils==7.0.6
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: stix-shifter-modules-elastic-ecs; extra == "test"
```

### Comparing `kestrel_datasource_stixshifter-1.8.2/README.rst` & `kestrel_datasource_stixshifter-1.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.2/pyproject.toml` & `kestrel_datasource_stixshifter-1.8.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 68.2.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kestrel_datasource_stixshifter"
-version = "1.8.2"
+version = "1.8.3"
 description = "Kestrel STIX-shifter Datasource Interface"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "Apache 2.0 License"}
 maintainers = [
     {name = "Xiaokui Shu", email = "xiaokui.shu@ibm.com"},
     {name = "Paul Coccoli", email = "pcoccoli@us.ibm.com"},
@@ -24,15 +24,15 @@
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
 ]
 
 dependencies = [
     "kestrel_core>=1.8.1",
-    "lxml>=5.2.1",
+    "lxml==4.9.4", # Python 3.8 on mac error >5.0.0; stackoverflow #75442675
     "requests>=2.31.0",
     "nest-asyncio>=1.6.0",
     "stix-shifter==7.0.6",
     "stix-shifter-utils==7.0.6",
 ]
 
 [project.optional-dependencies]
```

### Comparing `kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/config.py` & `kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 PROFILE_PATH_DEFAULT = CONFIG_DIR_DEFAULT / "stixshifter.yaml"
 PROFILE_PATH_ENV_VAR = "KESTREL_STIXSHIFTER_CONFIG"
 STIXSHIFTER_DEBUG_ENV_VAR = "KESTREL_STIXSHIFTER_DEBUG"  # debug mode for stix-shifter if the environment variable exists
 ENV_VAR_PREFIX = "STIXSHIFTER_"
 RETRIEVAL_BATCH_SIZE = 2000
 SINGLE_BATCH_TIMEOUT = 60
+SUBQUERY_TIME_WINDOW_IN_SECONDS = 0  # if >0, then segment START/STOP into this Windows Size to file multiple subqueries
 COOL_DOWN_AFTER_TRANSMISSION = 0
 ALLOW_DEV_CONNECTOR = False
 VERIFY_CERT = True
 FAST_TRANSLATE_CONNECTORS = []  # Suggested: ["qradar", "elastic_ecs"]
 
 
 _logger = logging.getLogger(__name__)
@@ -180,22 +181,31 @@
             "verify_cert",
             bool,
             VERIFY_CERT,
             connection,
             profile_name,
         )
 
+        subquery_time_window = _extract_param_from_connection_config(
+            "subquery_time_window",
+            int,
+            SUBQUERY_TIME_WINDOW_IN_SECONDS,
+            connection,
+            profile_name,
+        )
+
     return (
         connector_name,
         connection,
         configuration,
         retrieval_batch_size,
         cool_down_after_transmission,
         allow_dev_connector,
         verify_cert,
+        subquery_time_window,
     )
 
 
 def load_profiles():
     config = load_user_config(PROFILE_PATH_ENV_VAR, PROFILE_PATH_DEFAULT)
     if config and "profiles" in config:
         _logger.debug(f"stix-shifter profiles found in config file")
```

### Comparing `kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/connector.py` & `kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/connector.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/diagnosis.py` & `kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/diagnosis.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             self.connector_name,
             self.connection_dict,
             self.configuration_dict,
             self.retrieval_batch_size,
             self.cool_down_after_transmission,
             self.allow_dev_connector,
             self.verify_cert,
+            self.subquery_time_window,
         ) = get_datasource_from_profiles(datasource_name, self.profiles)
         self.if_fast_translation = (
             self.connector_name in self.kestrel_options["fast_translate"]
         )
         set_stixshifter_logging_level()
 
     def diagnose_config(self):
@@ -46,14 +47,18 @@
             deepcopy(self.configuration_dict), "*"
         )
 
         print()
         print("#### Kestrel specific config")
         print(f"retrieval batch size: {self.retrieval_batch_size}")
         print(f"cool down after transmission: {self.cool_down_after_transmission}")
+        print(f"allow unverified connector: {self.allow_dev_connector}")
+        print(f"verify SSL or not: {self.verify_cert}")
+        print(f"split query into subquery: {bool(self.subquery_time_window)}")
+        print(f"subquery with time window (in seconds): {self.subquery_time_window}")
         print(f"enable fast translation: {self.if_fast_translation}")
 
         print()
         print("#### Config to be passed to stix-shifter")
         print(f"connector name: {self.connector_name}")
         print(
             "connection object [ref: https://github.com/opencybersecurityalliance/stix-shifter/blob/develop/OVERVIEW.md#connection]:"
```

### Comparing `kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/interface.py` & `kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
                     port: 9200
                     indices: host101
                     options:  # use any of this section when needed
                         verify_cert: false  # allow invalid/expired/self-signed certificate
                         retrieval_batch_size: 10000  # set to 10000 to match default Elasticsearch page size; Kestrel default across connectors: 2000
                         single_batch_timeout: 120  # increase it if hit 60 seconds (Kestrel default) timeout error for each batch of retrieval
                         cool_down_after_transmission: 2  # seconds to cool down between data source API calls, required by some API such as sentinelone; Kestrel default: 0
+                        subquery_time_window: 3600 # split each query into multiple subqueries with smaller time windows specified here in seconds; Kestrel default: 0 (not split query)
                         allow_dev_connector: True  # do not check version of a connector to allow custom/testing connector installed with any version; Kestrel default: False
                         dialects:  # more info: https://github.com/opencybersecurityalliance/stix-shifter/tree/develop/stix_shifter_modules/elastic_ecs#dialects
                           - beats  # need it if the index is created by Filebeat/Winlogbeat/*beat
                 config:
                     auth:
                         id: VuaCfGcBCdbkQm-e5aOx
                         api_key: ui2lp2axTNmsyakw9tvNnw
```

### Comparing `kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/multiproc.py` & `kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/multiproc.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/query.py` & `kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from multiprocessing import Queue
 
 from kestrel.datasource import ReturnFromStore
 from kestrel.utils import mkdtemp
 from kestrel.exceptions import DataSourceError, DataSourceManagerInternalError
 from kestrel_datasource_stixshifter.connector import setup_connector_module
 from kestrel_datasource_stixshifter import multiproc
+from kestrel_datasource_stixshifter.subquery import split_subquery_by_time_window
 from kestrel_datasource_stixshifter.config import (
     get_datasource_from_profiles,
     load_options,
     load_profiles,
     set_stixshifter_logging_level,
 )
 
@@ -59,86 +60,96 @@
     # so it always needs to be created
     cache_dir = mkdtemp()
     query_id = cache_dir.name
 
     _logger.debug(f"prepare query with ID: {query_id}")
 
     num_records = 0
-    profile_limit = limit
+    limit_per_profile = limit
 
     for profile in profiles:
         if limit:
             if num_records >= limit:
                 break
             if num_records > 0:
-                profile_limit = limit - num_records
+                limit_per_profile = limit - num_records
         _logger.debug(f"entering stix-shifter data source: {profile}")
-        _logger.debug(f"profile = {profile}, profile_limit = {profile_limit}")
+        _logger.debug(f"profile = {profile}, limit_per_profile = {limit_per_profile}")
         # STIX-shifter will alter the config objects, thus making them not reusable.
         # So only give STIX-shifter a copy of the configs.
         # Check `modernize` functions in the `stix_shifter_utils` for details.
         (
             connector_name,
             connection_dict,
             configuration_dict,
             retrieval_batch_size,
             cool_down_after_transmission,
             allow_dev_connector,
             verify_cert,
+            subquery_time_window,
         ) = map(
             copy.deepcopy, get_datasource_from_profiles(profile, config["profiles"])
         )
 
         setup_connector_module(connector_name, allow_dev_connector)
 
         if _logger.isEnabledFor(logging.DEBUG):
             data_path_striped = "".join(filter(str.isalnum, profile))
             cache_data_path_prefix = str(cache_dir / data_path_striped)
         else:
             cache_data_path_prefix = None
 
         observation_metadata = gen_observation_metadata(connector_name, query_id)
 
-        dsl = translate_query(
-            connector_name, observation_metadata, pattern, connection_dict
-        )
+        for pattern in split_subquery_by_time_window(pattern, subquery_time_window):
 
-        raw_records_queue = Queue()
-        translated_data_queue = Queue()
+            if limit_per_profile:
+                if num_records >= limit_per_profile:
+                    _logger.debug("do not execute subquery due to limit return reached")
+                    break
+                if num_records > 0:
+                    limit_per_profile = limit_per_profile - num_records
 
-        exceptions = []
+            dsl = translate_query(
+                connector_name, observation_metadata, pattern, connection_dict
+            )
 
-        with multiproc.translate(
-            connector_name,
-            observation_metadata,
-            connection_dict.get("options", {}),
-            cache_data_path_prefix,
-            connector_name in config["options"]["fast_translate"],
-            raw_records_queue,
-            translated_data_queue,
-            config["options"]["translation_workers_count"],
-        ):
-            with multiproc.transmit(
+            raw_records_queue = Queue()
+            translated_data_queue = Queue()
+
+            exceptions = []
+
+            with multiproc.translate(
                 connector_name,
-                connection_dict,
-                configuration_dict,
-                retrieval_batch_size,
-                config["options"]["translation_workers_count"],
-                cool_down_after_transmission,
-                verify_cert,
-                dsl["queries"],
+                observation_metadata,
+                connection_dict.get("options", {}),
+                cache_data_path_prefix,
+                connector_name in config["options"]["fast_translate"],
                 raw_records_queue,
-                profile_limit,
+                translated_data_queue,
+                config["options"]["translation_workers_count"],
             ):
-                for result in multiproc.read_translated_results(
-                    translated_data_queue,
+                with multiproc.transmit(
+                    connector_name,
+                    connection_dict,
+                    configuration_dict,
+                    retrieval_batch_size,
                     config["options"]["translation_workers_count"],
+                    cool_down_after_transmission,
+                    verify_cert,
+                    dsl["queries"],
+                    raw_records_queue,
+                    limit_per_profile,
                 ):
-                    num_records += get_num_objects(result)
-                    ingest(result, observation_metadata, query_id, store)
+                    for result in multiproc.read_translated_results(
+                        translated_data_queue,
+                        config["options"]["translation_workers_count"],
+                    ):
+                        num_records += get_num_objects(result)
+                        ingest(result, observation_metadata, query_id, store)
 
     return ReturnFromStore(query_id)
 
 
 @typechecked
 def gen_observation_metadata(connector_name: str, query_id: str):
     return {
```

### Comparing `kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/worker/translator.py` & `kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/worker/translator.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/worker/transmitter.py` & `kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/worker/transmitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,17 +188,24 @@
                         True,
                         result_batch["data"],
                         result_retrieval_offset,
                         None,
                     )
 
                     # prepare for next round retrieval
-                    result_retrieval_offset += len(result_batch["data"])
+                    result_len = len(result_batch["data"])
+                    result_retrieval_offset += result_len
+
+                    if result_len < batch_size:
+                        has_remaining_results = False
+
                     if "metadata" in result_batch:
                         metadata = result_batch["metadata"]
+                    else:
+                        has_remaining_results = False
 
                     if self.limit:
                         if result_retrieval_offset >= self.limit:
                             has_remaining_results = False
                         else:
                             batch_size = self.limit - result_retrieval_offset
                             if batch_size > self.retrieval_batch_size:
```

### Comparing `kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter/worker/utils.py` & `kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter/worker/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter.egg-info/PKG-INFO` & `kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: kestrel_datasource_stixshifter
-Version: 1.8.2
+Version: 1.8.3
 Summary: Kestrel STIX-shifter Datasource Interface
 Maintainer-email: Xiaokui Shu <xiaokui.shu@ibm.com>, Paul Coccoli <pcoccoli@us.ibm.com>
 License: Apache 2.0 License
 Project-URL: Homepage, https://github.com/opencybersecurityalliance/kestrel-lang
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Project-URL: Repository, https://github.com/opencybersecurityalliance/kestrel-lang.git
 Keywords: kestrel,datasource,interface,STIX-shifter
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: kestrel_core>=1.8.1
-Requires-Dist: lxml>=5.2.1
+Requires-Dist: lxml==4.9.4
 Requires-Dist: requests>=2.31.0
 Requires-Dist: nest-asyncio>=1.6.0
 Requires-Dist: stix-shifter==7.0.6
 Requires-Dist: stix-shifter-utils==7.0.6
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: stix-shifter-modules-elastic-ecs; extra == "test"
```

### Comparing `kestrel_datasource_stixshifter-1.8.2/src/kestrel_datasource_stixshifter.egg-info/SOURCES.txt` & `kestrel_datasource_stixshifter-1.8.3/src/kestrel_datasource_stixshifter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/kestrel_datasource_stixshifter/cli.py
 src/kestrel_datasource_stixshifter/config.py
 src/kestrel_datasource_stixshifter/connector.py
 src/kestrel_datasource_stixshifter/diagnosis.py
 src/kestrel_datasource_stixshifter/interface.py
 src/kestrel_datasource_stixshifter/multiproc.py
 src/kestrel_datasource_stixshifter/query.py
+src/kestrel_datasource_stixshifter/subquery.py
 src/kestrel_datasource_stixshifter.egg-info/PKG-INFO
 src/kestrel_datasource_stixshifter.egg-info/SOURCES.txt
 src/kestrel_datasource_stixshifter.egg-info/dependency_links.txt
 src/kestrel_datasource_stixshifter.egg-info/entry_points.txt
 src/kestrel_datasource_stixshifter.egg-info/requires.txt
 src/kestrel_datasource_stixshifter.egg-info/top_level.txt
 src/kestrel_datasource_stixshifter/worker/__init__.py
```

### Comparing `kestrel_datasource_stixshifter-1.8.2/tests/test_command_get.py` & `kestrel_datasource_stixshifter-1.8.3/tests/test_command_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,19 +162,16 @@
                      START 2019-01-01T00:00:00Z STOP 2023-01-01T00:00:00Z
                      LIMIT 15
                """
 
         s.execute(stmt)
         v = s.get_variable("var")
 
-        # The extended graph [ipv4-addr:value = '127.0.0.1'] is recognized and
-        # merged to prefetch query, resultsing in limited (32) processes. If
-        # not used by prefetch, the total number of process records prefetched
-        # is 240.
-        assert len(v) == 28
+        # HOST1 returns 26, which is larger than 15
+        assert len(v) == 26
         for i in range(len(v)):
             assert v[i]["type"] == "process"
             assert v[i]["name"] in [
                 "powershell.exe",
                 "(unknown)",
                 "explorer.exe",
                 "firefox.exe",
```

### Comparing `kestrel_datasource_stixshifter-1.8.2/tests/test_stixshifter.py` & `kestrel_datasource_stixshifter-1.8.3/tests/test_stixshifter.py`

 * *Files 13% similar despite different names*

```diff
@@ -75,14 +75,15 @@
             indices: host101
             options:
                 retrieval_batch_size: 10000
                 single_batch_timeout: 120
                 cool_down_after_transmission: 5
                 allow_dev_connector: True
                 verify_cert: false
+                subquery_time_window: 600
                 dialects:
                     - beats
         config:
             auth:
                 id: profileB
                 api_key: xxxxxx
 """
@@ -103,36 +104,38 @@
 """
         s.execute(stmt)
 
         s.data_source_manager.list_data_sources_from_scheme("stixshifter")
 
         ss_config = s.config["datasources"]["kestrel_datasource_stixshifter"]
         ss_profiles = ss_config["profiles"]
-        connector_name, connection, configuration, retrieval_batch_size, cool_down_after_transmission, allow_dev_connector, verify_cert = get_datasource_from_profiles("host101", ss_profiles)
+        connector_name, connection, configuration, retrieval_batch_size, cool_down_after_transmission, allow_dev_connector, verify_cert, subquery_time_window = get_datasource_from_profiles("host101", ss_profiles)
         assert connector_name == "elastic_ecs"
         assert configuration["auth"]["id"] == "profileA"
         assert configuration["auth"]["api_key"] == "qwer"
         assert connection["options"]["timeout"] == 60
         assert connection["options"]["result_limit"] == 2000 * 2
         assert retrieval_batch_size == 2000
         assert cool_down_after_transmission == 0
         assert verify_cert == True
+        assert subquery_time_window == 0
 
         with open(profile_file, "w") as pf:
             pf.write(profileB)
 
         s.data_source_manager.list_data_sources_from_scheme("stixshifter")
 
         # need to refresh the pointers since the dict is updated
         ss_profiles = ss_config["profiles"]
-        connector_name, connection, configuration, retrieval_batch_size, cool_down_after_transmission, allow_dev_connector, verify_cert = get_datasource_from_profiles("host101", ss_profiles)
+        connector_name, connection, configuration, retrieval_batch_size, cool_down_after_transmission, allow_dev_connector, verify_cert, subquery_time_window = get_datasource_from_profiles("host101", ss_profiles)
         assert connector_name == "elastic_ecs"
         assert configuration["auth"]["id"] == "profileB"
         assert configuration["auth"]["api_key"] == "xxxxxx"
         assert connection["options"]["timeout"] == 120
         assert connection["options"]["result_limit"] == 10000 * 2
         assert retrieval_batch_size == 10000
         assert cool_down_after_transmission == 5
         assert allow_dev_connector == True
         assert verify_cert == False
+        assert subquery_time_window == 600
 
     del os.environ["KESTREL_STIXSHIFTER_CONFIG"]
```

### Comparing `kestrel_datasource_stixshifter-1.8.2/tests/test_stixshifter_diagnosis.py` & `kestrel_datasource_stixshifter-1.8.3/tests/test_stixshifter_diagnosis.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 def test_cli(stixshifter_profile_lab101):
     expected_output = """
 ## Diagnose: config verification
 
 #### Kestrel specific config
 retrieval batch size: 2000
 cool down after transmission: 0
+allow unverified connector: False
+verify SSL or not: True
+split query into subquery: False
+subquery with time window (in seconds): 0
 enable fast translation: False
 
 #### Config to be passed to stix-shifter
 connector name: stix_bundle
 connection object [ref: https://github.com/opencybersecurityalliance/stix-shifter/blob/develop/OVERVIEW.md#connection]:
 {
     "host": "https://github.com/opencybersecurityalliance/data-bucket-kestrel/blob/main/stix-bundles/lab101.json?raw=true",
@@ -74,15 +78,15 @@
 ## Diagnose: stix-shifter query execution: <=5 batch(s)
 
 #### data retrieval results:
 one batch retrieved: 533 entries
 """
 
     result = subprocess.run(
-        args=[STIX_SHIFTER_DIAG, "lab101"],
+        args=[STIX_SHIFTER_DIAG, "--start=2000-01-01T00:00:00.000Z", "--stop=3000-01-01T00:00:00.000Z", "lab101"],
         universal_newlines=True,
         stdout=subprocess.PIPE,
     )
 
     result_lines = result.stdout.splitlines()
     result_lines = [x for x in result_lines if x]
     expected_lines = expected_output.splitlines()
@@ -94,14 +98,18 @@
 def test_cli_ecs(stixshifter_profile_ecs):
     expected_output = """
 ## Diagnose: config verification
 
 #### Kestrel specific config
 retrieval batch size: 2000
 cool down after transmission: 0
+allow unverified connector: False
+verify SSL or not: True
+split query into subquery: False
+subquery with time window (in seconds): 0
 enable fast translation: False
 
 #### Config to be passed to stix-shifter
 connector name: elastic_ecs
 connection object [ref: https://github.com/opencybersecurityalliance/stix-shifter/blob/develop/OVERVIEW.md#connection]:
 {
     "host": "elastic.securitylog.company.com",
```

### Comparing `kestrel_datasource_stixshifter-1.8.2/tests/test_stixshifter_translator.py` & `kestrel_datasource_stixshifter-1.8.3/tests/test_stixshifter_translator.py`

 * *Files identical despite different names*

