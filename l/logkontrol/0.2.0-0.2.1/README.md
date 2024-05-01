# Comparing `tmp/logkontrol-0.2.0.tar.gz` & `tmp/logkontrol-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logkontrol-0.2.0.tar", last modified: Wed May  1 18:16:52 2024, max compression
+gzip compressed data, was "logkontrol-0.2.1.tar", last modified: Wed May  1 18:28:49 2024, max compression
```

## Comparing `logkontrol-0.2.0.tar` & `logkontrol-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 18:16:52.826857 logkontrol-0.2.0/
--rw-r--r--   0 rsp       (1000) wheel      (998)      468 2024-04-30 22:54:33.000000 logkontrol-0.2.0/LICENSE
--rw-r--r--   0 rsp       (1000) wheel      (998)     1101 2024-04-30 22:54:36.000000 logkontrol-0.2.0/LICENSE_PYYAML.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)     3694 2024-05-01 18:16:52.826857 logkontrol-0.2.0/PKG-INFO
--rw-r--r--   0 rsp       (1000) wheel      (998)     3100 2024-05-01 05:01:50.000000 logkontrol-0.2.0/README.md
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 18:16:52.826857 logkontrol-0.2.0/logkontrol/
--rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-04-30 03:27:11.000000 logkontrol-0.2.0/logkontrol/__init__.py
--rw-r--r--   0 rsp       (1000) wheel      (998)    12915 2024-05-01 18:12:44.000000 logkontrol-0.2.0/logkontrol/logkontrol.py
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 18:16:52.826857 logkontrol-0.2.0/logkontrol.egg-info/
--rw-r--r--   0 rsp       (1000) wheel      (998)     3694 2024-05-01 18:16:52.000000 logkontrol-0.2.0/logkontrol.egg-info/PKG-INFO
--rw-r--r--   0 rsp       (1000) wheel      (998)      534 2024-05-01 18:16:52.000000 logkontrol-0.2.0/logkontrol.egg-info/SOURCES.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)        1 2024-05-01 18:16:52.000000 logkontrol-0.2.0/logkontrol.egg-info/dependency_links.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)        7 2024-05-01 18:16:52.000000 logkontrol-0.2.0/logkontrol.egg-info/requires.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)       11 2024-05-01 18:16:52.000000 logkontrol-0.2.0/logkontrol.egg-info/top_level.txt
--rw-r--r--   0 rsp       (1000) wheel      (998)      672 2024-05-01 18:11:29.000000 logkontrol-0.2.0/pyproject.toml
--rw-r--r--   0 rsp       (1000) wheel      (998)       38 2024-05-01 18:16:52.830190 logkontrol-0.2.0/setup.cfg
-drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 18:16:52.826857 logkontrol-0.2.0/tests/
--rw-r--r--   0 rsp       (1000) wheel      (998)     2603 2024-05-01 18:06:57.000000 logkontrol-0.2.0/tests/test_init_logging.py
--rw-r--r--   0 rsp       (1000) wheel      (998)     2305 2024-05-01 18:06:19.000000 logkontrol-0.2.0/tests/test_initialize_log_file.py
--rw-r--r--   0 rsp       (1000) wheel      (998)     1947 2024-05-01 18:07:21.000000 logkontrol-0.2.0/tests/test_load_logging_config.py
--rw-r--r--   0 rsp       (1000) wheel      (998)     2491 2024-05-01 18:07:58.000000 logkontrol-0.2.0/tests/test_log_function_call.py
--rw-r--r--   0 rsp       (1000) wheel      (998)     2624 2024-05-01 18:08:40.000000 logkontrol-0.2.0/tests/test_log_json_content.py
--rw-r--r--   0 rsp       (1000) wheel      (998)     2369 2024-05-01 18:09:13.000000 logkontrol-0.2.0/tests/test_log_message.py
--rw-r--r--   0 rsp       (1000) wheel      (998)     2328 2024-05-01 18:09:45.000000 logkontrol-0.2.0/tests/test_log_variable.py
--rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-05-01 14:26:29.000000 logkontrol-0.2.0/tests/test_logkontrol.py
--rw-r--r--   0 rsp       (1000) wheel      (998)      833 2024-05-01 18:09:53.000000 logkontrol-0.2.0/tests/test_truncate_string.py
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 18:28:49.743810 logkontrol-0.2.1/
+-rw-r--r--   0 rsp       (1000) wheel      (998)      468 2024-04-30 22:54:33.000000 logkontrol-0.2.1/LICENSE
+-rw-r--r--   0 rsp       (1000) wheel      (998)     1101 2024-04-30 22:54:36.000000 logkontrol-0.2.1/LICENSE_PYYAML.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)     3737 2024-05-01 18:28:49.743810 logkontrol-0.2.1/PKG-INFO
+-rw-r--r--   0 rsp       (1000) wheel      (998)     3143 2024-05-01 18:21:49.000000 logkontrol-0.2.1/README.md
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 18:28:49.743810 logkontrol-0.2.1/logkontrol/
+-rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-04-30 03:27:11.000000 logkontrol-0.2.1/logkontrol/__init__.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)    12915 2024-05-01 18:12:44.000000 logkontrol-0.2.1/logkontrol/logkontrol.py
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 18:28:49.743810 logkontrol-0.2.1/logkontrol.egg-info/
+-rw-r--r--   0 rsp       (1000) wheel      (998)     3737 2024-05-01 18:28:49.000000 logkontrol-0.2.1/logkontrol.egg-info/PKG-INFO
+-rw-r--r--   0 rsp       (1000) wheel      (998)      534 2024-05-01 18:28:49.000000 logkontrol-0.2.1/logkontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)        1 2024-05-01 18:28:49.000000 logkontrol-0.2.1/logkontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)        7 2024-05-01 18:28:49.000000 logkontrol-0.2.1/logkontrol.egg-info/requires.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)       11 2024-05-01 18:28:49.000000 logkontrol-0.2.1/logkontrol.egg-info/top_level.txt
+-rw-r--r--   0 rsp       (1000) wheel      (998)      672 2024-05-01 18:28:43.000000 logkontrol-0.2.1/pyproject.toml
+-rw-r--r--   0 rsp       (1000) wheel      (998)       38 2024-05-01 18:28:49.743810 logkontrol-0.2.1/setup.cfg
+drwxr-sr-x   0 rsp       (1000) wheel      (998)        0 2024-05-01 18:28:49.743810 logkontrol-0.2.1/tests/
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2603 2024-05-01 18:06:57.000000 logkontrol-0.2.1/tests/test_init_logging.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2305 2024-05-01 18:06:19.000000 logkontrol-0.2.1/tests/test_initialize_log_file.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     1947 2024-05-01 18:07:21.000000 logkontrol-0.2.1/tests/test_load_logging_config.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2491 2024-05-01 18:07:58.000000 logkontrol-0.2.1/tests/test_log_function_call.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2624 2024-05-01 18:08:40.000000 logkontrol-0.2.1/tests/test_log_json_content.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2369 2024-05-01 18:09:13.000000 logkontrol-0.2.1/tests/test_log_message.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)     2328 2024-05-01 18:09:45.000000 logkontrol-0.2.1/tests/test_log_variable.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)        0 2024-05-01 14:26:29.000000 logkontrol-0.2.1/tests/test_logkontrol.py
+-rw-r--r--   0 rsp       (1000) wheel      (998)      833 2024-05-01 18:09:53.000000 logkontrol-0.2.1/tests/test_truncate_string.py
```

### Comparing `logkontrol-0.2.0/LICENSE_PYYAML.txt` & `logkontrol-0.2.1/LICENSE_PYYAML.txt`

 * *Files identical despite different names*

### Comparing `logkontrol-0.2.0/PKG-INFO` & `logkontrol-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logkontrol
-Version: 0.2.0
+Version: 0.2.1
 Summary: Custom file logging system for Python applications
 Author-email: voidfemme <rosemkatt@gmail.com>
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Homepage, https://github.com/voidfemme/logkontrol
 Project-URL: Bug_Tracker, https://github.com/voidfemme/logkontrol/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -42,26 +42,27 @@
 ```
 
 ## Usage
 
 Here's a quick example to get you started with LogKontrol:
 
 ```python
-from logkontrol.logkontrol import init_logging, log_message
+from logkontrol.logkontrol import LogKonfig, log_message
 
 # Initialize the logging system
-init_logging()
+log_konfig = LogKonfig()
+log_konfig.init_logging()
 
 # Log a simple message
 log_message('general', 'Hello, world!')
 ```
 
 ## Configuration
 
-LogKontrol is highly customizable through a simple YAML configuration file. Here's the default configuration:
+LogKontrol is highly customizable through a simple YAML configuration file. Here's an example configuration:
 
 ```yaml
 log_file_paths:
   general: 'logs/general.log'
   errors: 'logs/errors.log'
   debug: 'logs/debug.log'
 log_format: '[{timestamp}] [{level}] {message}'
@@ -69,15 +70,15 @@
 log_level: 'INFO'
 console_output: True
 ```
 
 Or, specify a different configuration file during initialization:
 
 ```python
-init_logging(config_file_path='path/to/your/config.yaml')
+log_konfig.init_logging(config_file_path='path/to/your/config.yaml')
 ```
 
 To add your own logging categories, simply add a new entry under 'log_file_paths' in the
 YAML file. For example, to add an audit trail log, you might add:
 
 ```yaml
 audit: 'logs/audit.log'
```

### Comparing `logkontrol-0.2.0/README.md` & `logkontrol-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,26 +26,27 @@
 ```
 
 ## Usage
 
 Here's a quick example to get you started with LogKontrol:
 
 ```python
-from logkontrol.logkontrol import init_logging, log_message
+from logkontrol.logkontrol import LogKonfig, log_message
 
 # Initialize the logging system
-init_logging()
+log_konfig = LogKonfig()
+log_konfig.init_logging()
 
 # Log a simple message
 log_message('general', 'Hello, world!')
 ```
 
 ## Configuration
 
-LogKontrol is highly customizable through a simple YAML configuration file. Here's the default configuration:
+LogKontrol is highly customizable through a simple YAML configuration file. Here's an example configuration:
 
 ```yaml
 log_file_paths:
   general: 'logs/general.log'
   errors: 'logs/errors.log'
   debug: 'logs/debug.log'
 log_format: '[{timestamp}] [{level}] {message}'
@@ -53,15 +54,15 @@
 log_level: 'INFO'
 console_output: True
 ```
 
 Or, specify a different configuration file during initialization:
 
 ```python
-init_logging(config_file_path='path/to/your/config.yaml')
+log_konfig.init_logging(config_file_path='path/to/your/config.yaml')
 ```
 
 To add your own logging categories, simply add a new entry under 'log_file_paths' in the
 YAML file. For example, to add an audit trail log, you might add:
 
 ```yaml
 audit: 'logs/audit.log'
```

### Comparing `logkontrol-0.2.0/logkontrol/logkontrol.py` & `logkontrol-0.2.1/logkontrol/logkontrol.py`

 * *Files identical despite different names*

### Comparing `logkontrol-0.2.0/logkontrol.egg-info/PKG-INFO` & `logkontrol-0.2.1/logkontrol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logkontrol
-Version: 0.2.0
+Version: 0.2.1
 Summary: Custom file logging system for Python applications
 Author-email: voidfemme <rosemkatt@gmail.com>
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Homepage, https://github.com/voidfemme/logkontrol
 Project-URL: Bug_Tracker, https://github.com/voidfemme/logkontrol/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -42,26 +42,27 @@
 ```
 
 ## Usage
 
 Here's a quick example to get you started with LogKontrol:
 
 ```python
-from logkontrol.logkontrol import init_logging, log_message
+from logkontrol.logkontrol import LogKonfig, log_message
 
 # Initialize the logging system
-init_logging()
+log_konfig = LogKonfig()
+log_konfig.init_logging()
 
 # Log a simple message
 log_message('general', 'Hello, world!')
 ```
 
 ## Configuration
 
-LogKontrol is highly customizable through a simple YAML configuration file. Here's the default configuration:
+LogKontrol is highly customizable through a simple YAML configuration file. Here's an example configuration:
 
 ```yaml
 log_file_paths:
   general: 'logs/general.log'
   errors: 'logs/errors.log'
   debug: 'logs/debug.log'
 log_format: '[{timestamp}] [{level}] {message}'
@@ -69,15 +70,15 @@
 log_level: 'INFO'
 console_output: True
 ```
 
 Or, specify a different configuration file during initialization:
 
 ```python
-init_logging(config_file_path='path/to/your/config.yaml')
+log_konfig.init_logging(config_file_path='path/to/your/config.yaml')
 ```
 
 To add your own logging categories, simply add a new entry under 'log_file_paths' in the
 YAML file. For example, to add an audit trail log, you might add:
 
 ```yaml
 audit: 'logs/audit.log'
```

### Comparing `logkontrol-0.2.0/logkontrol.egg-info/SOURCES.txt` & `logkontrol-0.2.1/logkontrol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logkontrol-0.2.0/pyproject.toml` & `logkontrol-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "logkontrol"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name = "voidfemme", email = "rosemkatt@gmail.com" }
 ]
 description = "Custom file logging system for Python applications"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `logkontrol-0.2.0/tests/test_init_logging.py` & `logkontrol-0.2.1/tests/test_init_logging.py`

 * *Files identical despite different names*

### Comparing `logkontrol-0.2.0/tests/test_initialize_log_file.py` & `logkontrol-0.2.1/tests/test_initialize_log_file.py`

 * *Files identical despite different names*

### Comparing `logkontrol-0.2.0/tests/test_load_logging_config.py` & `logkontrol-0.2.1/tests/test_load_logging_config.py`

 * *Files identical despite different names*

### Comparing `logkontrol-0.2.0/tests/test_log_function_call.py` & `logkontrol-0.2.1/tests/test_log_function_call.py`

 * *Files identical despite different names*

### Comparing `logkontrol-0.2.0/tests/test_log_json_content.py` & `logkontrol-0.2.1/tests/test_log_json_content.py`

 * *Files identical despite different names*

### Comparing `logkontrol-0.2.0/tests/test_log_message.py` & `logkontrol-0.2.1/tests/test_log_message.py`

 * *Files identical despite different names*

### Comparing `logkontrol-0.2.0/tests/test_log_variable.py` & `logkontrol-0.2.1/tests/test_log_variable.py`

 * *Files identical despite different names*

### Comparing `logkontrol-0.2.0/tests/test_truncate_string.py` & `logkontrol-0.2.1/tests/test_truncate_string.py`

 * *Files identical despite different names*

