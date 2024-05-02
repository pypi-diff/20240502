# Comparing `tmp/strideutils-0.3.1.tar.gz` & `tmp/strideutils-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strideutils-0.3.1.tar", max compression
+gzip compressed data, was "strideutils-0.3.2.tar", max compression
```

## Comparing `strideutils-0.3.1.tar` & `strideutils-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1835 2024-05-01 21:30:08.059850 strideutils-0.3.1/README.md
--rw-r--r--   0        0        0     1045 2024-05-01 21:30:08.063850 strideutils-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      373 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/Makefile
--rw-r--r--   0        0        0        0 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/__init__.py
--rw-r--r--   0        0        0     5408 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/coingecko.py
--rw-r--r--   0        0        0     5673 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/config_examples/strideutils_config.yaml.example
--rw-r--r--   0        0        0      443 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/config_examples/strideutils_secrets.yaml.example
--rw-r--r--   0        0        0     1270 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/cryptography.py
--rw-r--r--   0        0        0     1835 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/exec_tx.py
--rw-r--r--   0        0        0     1664 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/invariant_helpers.py
--rw-r--r--   0        0        0     1551 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/run_safely.py
--rw-r--r--   0        0        0     6793 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/sheets_connector.py
--rw-r--r--   0        0        0     1512 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/slack_connector.py
--rw-r--r--   0        0        0     5642 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/stride_alerts.py
--rw-r--r--   0        0        0    12894 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/stride_config.py
--rw-r--r--   0        0        0    31030 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/stride_requests.py
--rw-r--r--   0        0        0     2438 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/stride_upstash.py
--rw-r--r--   0        0        0     1064 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils/twilio_connector.py
--rw-r--r--   0        0        0        0 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils-stubs/__init__.pyi
--rw-r--r--   0        0        0      257 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils-stubs/coingecko.pyi
--rw-r--r--   0        0        0      139 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils-stubs/cryptography.pyi
--rw-r--r--   0        0        0      511 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils-stubs/exec_tx.pyi
--rw-r--r--   0        0        0      237 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils-stubs/invariant_helpers.pyi
--rw-r--r--   0        0        0      290 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils-stubs/run_safely.pyi
--rw-r--r--   0        0        0      803 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils-stubs/sheets_connector.pyi
--rw-r--r--   0        0        0      242 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils-stubs/slack_connector.pyi
--rw-r--r--   0        0        0      987 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils-stubs/stride_alerts.pyi
--rw-r--r--   0        0        0     4591 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils-stubs/stride_config.pyi
--rw-r--r--   0        0        0     3977 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils-stubs/stride_requests.pyi
--rw-r--r--   0        0        0      419 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils-stubs/stride_upstash.pyi
--rw-r--r--   0        0        0      245 2024-05-01 21:30:08.063850 strideutils-0.3.1/strideutils-stubs/twilio_connector.pyi
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 strideutils-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1835 2024-05-02 19:04:33.769974 strideutils-0.3.2/README.md
+-rw-r--r--   0        0        0     1045 2024-05-02 19:04:33.769974 strideutils-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      373 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/Makefile
+-rw-r--r--   0        0        0        0 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/__init__.py
+-rw-r--r--   0        0        0     5408 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/coingecko.py
+-rw-r--r--   0        0        0     5673 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/config_examples/strideutils_config.yaml.example
+-rw-r--r--   0        0        0      443 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/config_examples/strideutils_secrets.yaml.example
+-rw-r--r--   0        0        0     1270 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/cryptography.py
+-rw-r--r--   0        0        0     1835 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/exec_tx.py
+-rw-r--r--   0        0        0     1664 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/invariant_helpers.py
+-rw-r--r--   0        0        0     1551 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/run_safely.py
+-rw-r--r--   0        0        0     6793 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/sheets_connector.py
+-rw-r--r--   0        0        0     1594 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/slack_connector.py
+-rw-r--r--   0        0        0     5642 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/stride_alerts.py
+-rw-r--r--   0        0        0    12894 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/stride_config.py
+-rw-r--r--   0        0        0    31030 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/stride_requests.py
+-rw-r--r--   0        0        0     2438 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/stride_upstash.py
+-rw-r--r--   0        0        0     1064 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils/twilio_connector.py
+-rw-r--r--   0        0        0        0 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils-stubs/__init__.pyi
+-rw-r--r--   0        0        0      257 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils-stubs/coingecko.pyi
+-rw-r--r--   0        0        0      139 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils-stubs/cryptography.pyi
+-rw-r--r--   0        0        0      511 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils-stubs/exec_tx.pyi
+-rw-r--r--   0        0        0      237 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils-stubs/invariant_helpers.pyi
+-rw-r--r--   0        0        0      290 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils-stubs/run_safely.pyi
+-rw-r--r--   0        0        0      803 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils-stubs/sheets_connector.pyi
+-rw-r--r--   0        0        0      242 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils-stubs/slack_connector.pyi
+-rw-r--r--   0        0        0      987 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils-stubs/stride_alerts.pyi
+-rw-r--r--   0        0        0     4591 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils-stubs/stride_config.pyi
+-rw-r--r--   0        0        0     3977 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils-stubs/stride_requests.pyi
+-rw-r--r--   0        0        0      419 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils-stubs/stride_upstash.pyi
+-rw-r--r--   0        0        0      245 2024-05-02 19:04:33.769974 strideutils-0.3.2/strideutils-stubs/twilio_connector.pyi
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 strideutils-0.3.2/PKG-INFO
```

### Comparing `strideutils-0.3.1/README.md` & `strideutils-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/pyproject.toml` & `strideutils-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strideutils"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 include = ["strideutils", "strideutils-stubs"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `strideutils-0.3.1/strideutils/coingecko.py` & `strideutils-0.3.2/strideutils/coingecko.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils/config_examples/strideutils_config.yaml.example` & `strideutils-0.3.2/strideutils/config_examples/strideutils_config.yaml.example`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils/cryptography.py` & `strideutils-0.3.2/strideutils/cryptography.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils/exec_tx.py` & `strideutils-0.3.2/strideutils/exec_tx.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils/invariant_helpers.py` & `strideutils-0.3.2/strideutils/invariant_helpers.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils/run_safely.py` & `strideutils-0.3.2/strideutils/run_safely.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils/sheets_connector.py` & `strideutils-0.3.2/strideutils/sheets_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils/slack_connector.py` & `strideutils-0.3.2/strideutils/slack_connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from typing import List, Optional, Union
 
 from slack_sdk import WebClient
 from slack_sdk.errors import SlackApiError
 
 from strideutils.stride_config import config
 
@@ -23,14 +24,15 @@
     if txt is an array, this will post each element of the array as a thread
 
     Args:
       username: Rename stridebot
     """
     client = WebClient(token=token)
     channel = config.slack_channels.get(channel.replace('#', ''), channel)
+    channel = os.environ.get('SLACK_CHANNEL_OVERRIDE', default=channel)
 
     # Listify
     messages = [txt] if type(txt) is str else txt
 
     # thread ts keeps track of the latest thread ID so we can keep replying in-thread
     thread_ts = None or thread_ts
     for msg in messages:
```

### Comparing `strideutils-0.3.1/strideutils/stride_alerts.py` & `strideutils-0.3.2/strideutils/stride_alerts.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils/stride_config.py` & `strideutils-0.3.2/strideutils/stride_config.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils/stride_requests.py` & `strideutils-0.3.2/strideutils/stride_requests.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils/stride_upstash.py` & `strideutils-0.3.2/strideutils/stride_upstash.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils/twilio_connector.py` & `strideutils-0.3.2/strideutils/twilio_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils-stubs/sheets_connector.pyi` & `strideutils-0.3.2/strideutils-stubs/sheets_connector.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils-stubs/stride_alerts.pyi` & `strideutils-0.3.2/strideutils-stubs/stride_alerts.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils-stubs/stride_config.pyi` & `strideutils-0.3.2/strideutils-stubs/stride_config.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/strideutils-stubs/stride_requests.pyi` & `strideutils-0.3.2/strideutils-stubs/stride_requests.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.1/PKG-INFO` & `strideutils-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strideutils
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

