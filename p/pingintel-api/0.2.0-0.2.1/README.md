# Comparing `tmp/pingintel_api-0.2.0.tar.gz` & `tmp/pingintel_api-0.2.1.tar.gz`

## Comparing `pingintel_api-0.2.0.tar` & `pingintel_api-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/justfile
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/requirements.txt
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/examples/fix_sov.py
--rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/examples/test_sov.xlsx
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/src/pingintel_api/__about__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/src/pingintel_api/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/src/pingintel_api/constants.py
--rw-r--r--   0        0        0    10590 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/src/pingintel_api/sov_fixer_api_client.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/src/pingintel_api/sovfixerapi_cmd.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/tests/tests.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/LICENSE
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/README.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/justfile
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/requirements.txt
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/examples/fix_sov.py
+-rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/examples/test_sov.xlsx
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/src/pingintel_api/__about__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/src/pingintel_api/__init__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/src/pingintel_api/constants.py
+-rw-r--r--   0        0        0    10590 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/src/pingintel_api/sov_fixer_api_client.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/src/pingintel_api/sovfixerapi_cmd.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/tests/tests.py
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/LICENSE
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/README.md
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pingintel_api-0.2.1/PKG-INFO
```

### Comparing `pingintel_api-0.2.0/examples/test_sov.xlsx` & `pingintel_api-0.2.1/examples/test_sov.xlsx`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.2.0/src/pingintel_api/constants.py` & `pingintel_api-0.2.1/src/pingintel_api/constants.py`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.2.0/src/pingintel_api/sov_fixer_api_client.py` & `pingintel_api-0.2.1/src/pingintel_api/sov_fixer_api_client.py`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.2.0/src/pingintel_api/sovfixerapi_cmd.py` & `pingintel_api-0.2.1/src/pingintel_api/sovfixerapi_cmd.py`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.2.0/.gitignore` & `pingintel_api-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.2.0/LICENSE` & `pingintel_api-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.2.0/pyproject.toml` & `pingintel_api-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 [project]
 name = "pingintel-api"
 dynamic = ["version"]
 authors = [
   { name="Scott Stafford", email="scott@pingintel.com" },
 ]
-description = "Python-based API for Ping Data Intelligence APIs"
+description = "Python-based client to Ping Data Intelligence APIs"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/pingintel/pingintel-api"
-Issues = "https://github.com/pingintel/pingintel-api"
+Issues = "https://github.com/pingintel/pingintel-api/issues"
 
 [tool.hatch.version]
 path = "src/pingintel_api/__about__.py"
 
 [project.scripts]
 sovfixerapi = "pingintel_api.sovfixerapi_cmd:main"
```

