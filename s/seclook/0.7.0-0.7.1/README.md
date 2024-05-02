# Comparing `tmp/seclook-0.7.0.tar.gz` & `tmp/seclook-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seclook-0.7.0.tar", max compression
+gzip compressed data, was "seclook-0.7.1.tar", max compression
```

## Comparing `seclook-0.7.0.tar` & `seclook-0.7.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1068 2024-01-01 19:44:45.950259 seclook-0.7.0/LICENSE
--rw-r--r--   0        0        0     3025 2024-01-01 19:44:45.950259 seclook-0.7.0/README.md
--rw-r--r--   0        0        0      547 2024-01-01 19:44:45.950259 seclook-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/__init__.py
--rwxr-xr-x   0        0        0     2913 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/cli.py
--rw-r--r--   0        0        0     1527 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/config_helper.py
--rw-r--r--   0        0        0      710 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/find_config.py
--rw-r--r--   0        0        0        0 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/lookups/__init__.py
--rw-r--r--   0        0        0      432 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/lookups/abuseipdb_lookup.py
--rw-r--r--   0        0        0      311 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/lookups/emailrep_lookup.py
--rw-r--r--   0        0        0      382 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/lookups/greynoise_lookup.py
--rw-r--r--   0        0        0      436 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/lookups/pulsedive_lookup.py
--rw-r--r--   0        0        0      392 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/lookups/shodan_lookup.py
--rw-r--r--   0        0        0      474 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/lookups/threatfox_lookup.py
--rw-r--r--   0        0        0      371 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/lookups/virustotal_lookup.py
--rw-r--r--   0        0        0      296 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/lookups/yaraify_lookup.py
--rw-r--r--   0        0        0        0 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/openai/__init__.py
--rw-r--r--   0        0        0      816 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/openai/gpt4_summarize.py
--rw-r--r--   0        0        0        0 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/tests/__init__.py
--rw-r--r--   0        0        0      232 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/tests/test_export.py
--rw-r--r--   0        0        0      235 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/tests/test_list.py
--rw-r--r--   0        0        0      263 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/tests/test_missing_service_value.py
--rw-r--r--   0        0        0     1762 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/tests/test_missing_value.py
--rw-r--r--   0        0        0      266 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/tests/test_unknown_service.py
--rw-r--r--   0        0        0     1288 2024-01-01 19:44:45.950259 seclook-0.7.0/seclook/tests/test_valid_service_value.py
--rw-r--r--   0        0        0     3622 1970-01-01 00:00:00.000000 seclook-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-02 02:10:04.865951 seclook-0.7.1/LICENSE
+-rw-r--r--   0        0        0     3041 2024-05-02 02:10:04.865951 seclook-0.7.1/README.md
+-rw-r--r--   0        0        0      547 2024-05-02 02:10:04.869951 seclook-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/__init__.py
+-rwxr-xr-x   0        0        0     2913 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/cli.py
+-rw-r--r--   0        0        0     1527 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/config_helper.py
+-rw-r--r--   0        0        0      710 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/find_config.py
+-rw-r--r--   0        0        0        0 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/lookups/__init__.py
+-rw-r--r--   0        0        0      432 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/lookups/abuseipdb_lookup.py
+-rw-r--r--   0        0        0      311 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/lookups/emailrep_lookup.py
+-rw-r--r--   0        0        0      382 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/lookups/greynoise_lookup.py
+-rw-r--r--   0        0        0      436 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/lookups/pulsedive_lookup.py
+-rw-r--r--   0        0        0      392 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/lookups/shodan_lookup.py
+-rw-r--r--   0        0        0      474 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/lookups/threatfox_lookup.py
+-rw-r--r--   0        0        0      371 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/lookups/virustotal_lookup.py
+-rw-r--r--   0        0        0      296 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/lookups/yaraify_lookup.py
+-rw-r--r--   0        0        0        0 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/openai/__init__.py
+-rw-r--r--   0        0        0      816 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/openai/gpt4_summarize.py
+-rw-r--r--   0        0        0        0 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/tests/__init__.py
+-rw-r--r--   0        0        0      232 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/tests/test_export.py
+-rw-r--r--   0        0        0      235 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/tests/test_list.py
+-rw-r--r--   0        0        0      263 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/tests/test_missing_service_value.py
+-rw-r--r--   0        0        0     1762 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/tests/test_missing_value.py
+-rw-r--r--   0        0        0      266 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/tests/test_unknown_service.py
+-rw-r--r--   0        0        0     1288 2024-05-02 02:10:04.869951 seclook-0.7.1/seclook/tests/test_valid_service_value.py
+-rw-r--r--   0        0        0     3638 1970-01-01 00:00:00.000000 seclook-0.7.1/PKG-INFO
```

### Comparing `seclook-0.7.0/LICENSE` & `seclook-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seclook-0.7.0/README.md` & `seclook-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-[![Tests](https://github.com/ackatz/seclook/actions/workflows/ci.yml/badge.svg)](https://github.com/ackatz/seclook/actions/workflows/ci.yml)
-[![Release](https://github.com/ackatz/seclook/actions/workflows/cd.yml/badge.svg)](https://github.com/ackatz/seclook/actions/workflows/cd.yml)
+[![Tests](https://github.com/ackatz/seclook-cli/actions/workflows/ci.yml/badge.svg)](https://github.com/ackatz/seclook-cli/actions/workflows/ci.yml)
+[![Release](https://github.com/ackatz/seclook-cli/actions/workflows/cd.yml/badge.svg)](https://github.com/ackatz/seclook-cli/actions/workflows/cd.yml)
 [![Downloads](https://static.pepy.tech/badge/seclook)](https://pepy.tech/project/seclook)
 
 # seclook
 
 `seclook` is a security lookup CLI tool that allows you to query various security services on the fly. It is essentially a wrapper over the `requests` library that removes the need to manually search within Web UIs or write your own requests in Postman or cURL to query these services.
 
 You can look up information using commands like `seclook [service] [value]`, where the service can be `virustotal`, `shodan`, `emailrep`, and so on. The value is the information you're querying for and varies by service.
```

### Comparing `seclook-0.7.0/pyproject.toml` & `seclook-0.7.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seclook"
-version = "0.7.0"
+version = "0.7.1"
 description = "Simple security lookups via CLI"
 authors = ["ackatz <andrew@akatz.org>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ackatz/seclook-cli"
 
 [tool.poetry.scripts]
```

### Comparing `seclook-0.7.0/seclook/cli.py` & `seclook-0.7.1/seclook/cli.py`

 * *Files identical despite different names*

### Comparing `seclook-0.7.0/seclook/config_helper.py` & `seclook-0.7.1/seclook/config_helper.py`

 * *Files identical despite different names*

### Comparing `seclook-0.7.0/seclook/find_config.py` & `seclook-0.7.1/seclook/find_config.py`

 * *Files identical despite different names*

### Comparing `seclook-0.7.0/seclook/openai/gpt4_summarize.py` & `seclook-0.7.1/seclook/openai/gpt4_summarize.py`

 * *Files identical despite different names*

### Comparing `seclook-0.7.0/seclook/tests/test_missing_value.py` & `seclook-0.7.1/seclook/tests/test_missing_value.py`

 * *Files identical despite different names*

### Comparing `seclook-0.7.0/seclook/tests/test_valid_service_value.py` & `seclook-0.7.1/seclook/tests/test_valid_service_value.py`

 * *Files identical despite different names*

### Comparing `seclook-0.7.0/PKG-INFO` & `seclook-0.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seclook
-Version: 0.7.0
+Version: 0.7.1
 Summary: Simple security lookups via CLI
 Home-page: https://github.com/ackatz/seclook-cli
 License: MIT
 Author: ackatz
 Author-email: andrew@akatz.org
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: configparser (>=6.0.0,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-[![Tests](https://github.com/ackatz/seclook/actions/workflows/ci.yml/badge.svg)](https://github.com/ackatz/seclook/actions/workflows/ci.yml)
-[![Release](https://github.com/ackatz/seclook/actions/workflows/cd.yml/badge.svg)](https://github.com/ackatz/seclook/actions/workflows/cd.yml)
+[![Tests](https://github.com/ackatz/seclook-cli/actions/workflows/ci.yml/badge.svg)](https://github.com/ackatz/seclook-cli/actions/workflows/ci.yml)
+[![Release](https://github.com/ackatz/seclook-cli/actions/workflows/cd.yml/badge.svg)](https://github.com/ackatz/seclook-cli/actions/workflows/cd.yml)
 [![Downloads](https://static.pepy.tech/badge/seclook)](https://pepy.tech/project/seclook)
 
 # seclook
 
 `seclook` is a security lookup CLI tool that allows you to query various security services on the fly. It is essentially a wrapper over the `requests` library that removes the need to manually search within Web UIs or write your own requests in Postman or cURL to query these services.
 
 You can look up information using commands like `seclook [service] [value]`, where the service can be `virustotal`, `shodan`, `emailrep`, and so on. The value is the information you're querying for and varies by service.
```

