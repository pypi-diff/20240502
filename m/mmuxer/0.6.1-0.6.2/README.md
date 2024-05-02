# Comparing `tmp/mmuxer-0.6.1.tar.gz` & `tmp/mmuxer-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmuxer-0.6.1.tar", last modified: Sun Mar 17 10:51:37 2024, max compression
+gzip compressed data, was "mmuxer-0.6.2.tar", last modified: Thu May  2 20:11:55 2024, max compression
```

## Comparing `mmuxer-0.6.1.tar` & `mmuxer-0.6.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    34523 2024-03-17 10:51:34.812287 mmuxer-0.6.1/LICENSE
--rw-r--r--   0        0        0     3579 2024-03-17 10:51:34.812287 mmuxer-0.6.1/README.md
--rw-r--r--   0        0        0       12 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/MANIFEST.in
--rw-r--r--   0        0        0       22 2024-03-17 10:51:36.364311 mmuxer-0.6.1/mmuxer/__init__.py
--rw-r--r--   0        0        0     2318 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/__main__.py
--rw-r--r--   0        0        0        0 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/cli/__init__.py
--rw-r--r--   0        0        0     3272 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/cli/folder.py
--rw-r--r--   0        0        0     1675 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/cli/run.py
--rw-r--r--   0        0        0      850 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/cli/sieve_export.py
--rw-r--r--   0        0        0     5588 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/config_state.py
--rw-r--r--   0        0        0     3268 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/mailbox.py
--rw-r--r--   0        0        0        0 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/models/__init__.py
--rw-r--r--   0        0        0     3042 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/models/action.py
--rw-r--r--   0        0        0      486 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/models/common.py
--rw-r--r--   0        0        0     4338 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/models/condition.py
--rw-r--r--   0        0        0      946 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/models/enums.py
--rw-r--r--   0        0        0     2309 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/models/rule.py
--rw-r--r--   0        0        0     1990 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/models/script.py
--rw-r--r--   0        0        0      797 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/models/settings.py
--rw-r--r--   0        0        0     4995 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/models/sieve.py
--rw-r--r--   0        0        0     3288 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/utils.py
--rw-r--r--   0        0        0     2133 2024-03-17 10:51:34.820287 mmuxer-0.6.1/mmuxer/workers.py
--rw-r--r--   0        0        0     1319 2024-03-17 10:51:37.552329 mmuxer-0.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-17 10:51:34.820287 mmuxer-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0     1477 2024-03-17 10:51:34.820287 mmuxer-0.6.1/tests/conftest.py
--rw-r--r--   0        0        0      536 2024-03-17 10:51:34.820287 mmuxer-0.6.1/tests/data/models/rules.yaml
--rw-r--r--   0        0        0    36154 2024-03-17 10:51:34.820287 mmuxer-0.6.1/tests/imap_server.py
--rw-r--r--   0        0        0      248 2024-03-17 10:51:34.820287 mmuxer-0.6.1/tests/models/test_parse_rule.py
--rw-r--r--   0        0        0     2515 2024-03-17 10:51:34.820287 mmuxer-0.6.1/tests/models/test_sieve.py
--rw-r--r--   0        0        0     1893 2024-03-17 10:51:34.820287 mmuxer-0.6.1/tests/test_actions.py
--rw-r--r--   0        0        0     1391 2024-03-17 10:51:34.820287 mmuxer-0.6.1/tests/test_condition.py
--rw-r--r--   0        0        0     2869 2024-03-17 10:51:34.820287 mmuxer-0.6.1/tests/test_utils.py
--rw-r--r--   0        0        0     4354 1970-01-01 00:00:00.000000 mmuxer-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-02 20:11:41.409973 mmuxer-0.6.2/LICENSE
+-rw-r--r--   0        0        0     3579 2024-05-02 20:11:41.409973 mmuxer-0.6.2/README.md
+-rw-r--r--   0        0        0       12 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/MANIFEST.in
+-rw-r--r--   0        0        0       22 2024-05-02 20:11:53.370069 mmuxer-0.6.2/mmuxer/__init__.py
+-rw-r--r--   0        0        0     2318 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/cli/__init__.py
+-rw-r--r--   0        0        0     3272 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/cli/folder.py
+-rw-r--r--   0        0        0     1675 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/cli/run.py
+-rw-r--r--   0        0        0      850 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/cli/sieve_export.py
+-rw-r--r--   0        0        0     5588 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/config_state.py
+-rw-r--r--   0        0        0     3268 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/mailbox.py
+-rw-r--r--   0        0        0        0 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/__init__.py
+-rw-r--r--   0        0        0     3042 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/action.py
+-rw-r--r--   0        0        0      486 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/common.py
+-rw-r--r--   0        0        0     4338 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/condition.py
+-rw-r--r--   0        0        0      946 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/enums.py
+-rw-r--r--   0        0        0     2309 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/rule.py
+-rw-r--r--   0        0        0     1990 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/script.py
+-rw-r--r--   0        0        0      797 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/settings.py
+-rw-r--r--   0        0        0     4995 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/models/sieve.py
+-rw-r--r--   0        0        0     3288 2024-05-02 20:11:41.413972 mmuxer-0.6.2/mmuxer/utils.py
+-rw-r--r--   0        0        0     2133 2024-05-02 20:11:41.417972 mmuxer-0.6.2/mmuxer/workers.py
+-rw-r--r--   0        0        0     1356 2024-05-02 20:11:55.558085 mmuxer-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/__init__.py
+-rw-r--r--   0        0        0     1477 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/conftest.py
+-rw-r--r--   0        0        0      536 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/data/models/rules.yaml
+-rw-r--r--   0        0        0    36154 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/imap_server.py
+-rw-r--r--   0        0        0      248 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/models/test_parse_rule.py
+-rw-r--r--   0        0        0     2515 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/models/test_sieve.py
+-rw-r--r--   0        0        0     1893 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/test_actions.py
+-rw-r--r--   0        0        0     1391 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/test_condition.py
+-rw-r--r--   0        0        0     2869 2024-05-02 20:11:41.417972 mmuxer-0.6.2/tests/test_utils.py
+-rw-r--r--   0        0        0     4167 1970-01-01 00:00:00.000000 mmuxer-0.6.2/PKG-INFO
```

### Comparing `mmuxer-0.6.1/LICENSE` & `mmuxer-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/README.md` & `mmuxer-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/__main__.py` & `mmuxer-0.6.2/mmuxer/__main__.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/cli/folder.py` & `mmuxer-0.6.2/mmuxer/cli/folder.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/cli/run.py` & `mmuxer-0.6.2/mmuxer/cli/run.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/cli/sieve_export.py` & `mmuxer-0.6.2/mmuxer/cli/sieve_export.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/config_state.py` & `mmuxer-0.6.2/mmuxer/config_state.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/mailbox.py` & `mmuxer-0.6.2/mmuxer/mailbox.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/models/action.py` & `mmuxer-0.6.2/mmuxer/models/action.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/models/condition.py` & `mmuxer-0.6.2/mmuxer/models/condition.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/models/enums.py` & `mmuxer-0.6.2/mmuxer/models/enums.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/models/rule.py` & `mmuxer-0.6.2/mmuxer/models/rule.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/models/script.py` & `mmuxer-0.6.2/mmuxer/models/script.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/models/settings.py` & `mmuxer-0.6.2/mmuxer/models/settings.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/models/sieve.py` & `mmuxer-0.6.2/mmuxer/models/sieve.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/utils.py` & `mmuxer-0.6.2/mmuxer/utils.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/mmuxer/workers.py` & `mmuxer-0.6.2/mmuxer/workers.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/pyproject.toml` & `mmuxer-0.6.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -7,46 +7,48 @@
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
     "typer[all]>=0.7, <0.8",
     "pydantic>2",
     "pydantic-settings",
     "pyyaml",
-    "imap-tools",
+    "imap-tools==v1.5.0",
     "certifi",
     "watchfiles >= 0.18",
     "boolean.py >= 4.0",
 ]
 classifiers = [
     "Topic :: Communications :: Email :: Filters",
 ]
 dynamic = []
-version = "0.6.1"
+version = "0.6.2"
 
 [project.license]
 text = "AGPL-3.0"
 
 [project.scripts]
 mmuxer = "mmuxer.__main__:app"
 
 [project.optional-dependencies]
-dev = [
-    "pytest >= 7.0",
-    "pre-commit >= 2.0",
-    "pytest-bg-process",
-    "pytz",
-]
 systemd = [
     "cysystemd >= 1.5.0",
 ]
 
 [tool.pdm.version]
 source = "file"
 path = "mmuxer/__init__.py"
 
+[tool.pdm.dev-dependencies]
+dev = [
+    "pytest >= 7.0",
+    "pre-commit>=3.7.0",
+    "pytest-bg-process",
+    "pytz",
+]
+
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = [
     "mmuxer*",
 ]
```

### Comparing `mmuxer-0.6.1/tests/conftest.py` & `mmuxer-0.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/tests/data/models/rules.yaml` & `mmuxer-0.6.2/tests/data/models/rules.yaml`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/tests/imap_server.py` & `mmuxer-0.6.2/tests/imap_server.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/tests/models/test_sieve.py` & `mmuxer-0.6.2/tests/models/test_sieve.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/tests/test_actions.py` & `mmuxer-0.6.2/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/tests/test_condition.py` & `mmuxer-0.6.2/tests/test_condition.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/tests/test_utils.py` & `mmuxer-0.6.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.6.1/PKG-INFO` & `mmuxer-0.6.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 Metadata-Version: 2.1
 Name: mmuxer
-Version: 0.6.1
+Version: 0.6.2
 Summary: Manage mail from your server.
 Author-Email: Mathias Millet <mathias@mmill.eu>
 License: AGPL-3.0
 Classifier: Topic :: Communications :: Email :: Filters
 Requires-Python: >=3.9
 Requires-Dist: typer[all]<0.8,>=0.7
 Requires-Dist: pydantic>2
 Requires-Dist: pydantic-settings
 Requires-Dist: pyyaml
-Requires-Dist: imap-tools
+Requires-Dist: imap-tools==v1.5.0
 Requires-Dist: certifi
 Requires-Dist: watchfiles>=0.18
 Requires-Dist: boolean.py>=4.0
-Requires-Dist: pytest>=7.0; extra == "dev"
-Requires-Dist: pre-commit>=2.0; extra == "dev"
-Requires-Dist: pytest-bg-process; extra == "dev"
-Requires-Dist: pytz; extra == "dev"
 Requires-Dist: cysystemd>=1.5.0; extra == "systemd"
-Provides-Extra: dev
 Provides-Extra: systemd
 Description-Content-Type: text/markdown
 
 # Mail Muxer
 
 ![cover](assets/cover.png)
```

