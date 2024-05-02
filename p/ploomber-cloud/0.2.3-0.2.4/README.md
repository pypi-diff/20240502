# Comparing `tmp/ploomber-cloud-0.2.3.tar.gz` & `tmp/ploomber-cloud-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomber-cloud-0.2.3.tar", last modified: Fri Apr 26 20:58:33 2024, max compression
+gzip compressed data, was "ploomber-cloud-0.2.4.tar", last modified: Thu May  2 14:11:57 2024, max compression
```

## Comparing `ploomber-cloud-0.2.3.tar` & `ploomber-cloud-0.2.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:58:33.571488 ploomber-cloud-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 20:58:33.571488 ploomber-cloud-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 20:58:33.575488 ploomber-cloud-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:58:33.567488 ploomber-cloud-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:58:33.571488 ploomber-cloud-0.2.3/src/ploomber_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:58:33.571488 ploomber-cloud-0.2.3/src/ploomber_cloud/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:58:33.571488 ploomber-cloud-0.2.3/src/ploomber_cloud/assets/vllm/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/assets/vllm/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/assets/vllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/assets/vllm/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/assets/vllm/test-vllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:58:33.571488 ploomber-cloud-0.2.3/src/ploomber_cloud/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/configurations/community.json
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/configurations/premium.json
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-26 20:58:20.000000 ploomber-cloud-0.2.3/src/ploomber_cloud/zip_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:58:33.571488 ploomber-cloud-0.2.3/src/ploomber_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-26 20:58:33.000000 ploomber-cloud-0.2.3/src/ploomber_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-26 20:58:33.000000 ploomber-cloud-0.2.3/src/ploomber_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:58:33.000000 ploomber-cloud-0.2.3/src/ploomber_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-26 20:58:33.000000 ploomber-cloud-0.2.3/src/ploomber_cloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-26 20:58:33.000000 ploomber-cloud-0.2.3/src/ploomber_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 20:58:33.000000 ploomber-cloud-0.2.3/src/ploomber_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:57.609134 ploomber-cloud-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/src/ploomber_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/src/ploomber_cloud/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/src/ploomber_cloud/assets/vllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/assets/vllm/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/assets/vllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/assets/vllm/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/assets/vllm/test-vllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/src/ploomber_cloud/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/configurations/community.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/configurations/premium.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7835 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-02 14:11:39.000000 ploomber-cloud-0.2.4/src/ploomber_cloud/zip_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:11:57.617134 ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 14:11:57.000000 ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-02 14:11:57.000000 ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:11:57.000000 ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 14:11:57.000000 ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 14:11:57.000000 ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 14:11:57.000000 ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/top_level.txt
```

### Comparing `ploomber-cloud-0.2.3/CHANGELOG.md` & `ploomber-cloud-0.2.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## 0.2.4 (2024-05-02)
+
+- [Feature] Allow deploying secrets using `secret-keys` in `ploomber-cloud.json`
+
 ## 0.2.3 (2024-04-26)
 
 - [Feature] Add `ploomber-cloud labels` for adding or deleting labels of the project.
 
 ## 0.2.2 (2024-04-26)
 
 - [Feature] Better validation when running `ploomber-cloud templates auth0`
```

### Comparing `ploomber-cloud-0.2.3/pyproject.toml` & `ploomber-cloud-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/setup.py` & `ploomber-cloud-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/api.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,15 +145,21 @@
             files = {
                 "files": (
                     "app.zip",
                     file,
                     "application/zip",
                 ),
             }
-            data = {"secrets": secrets, "template": template}
+            data = {}
+
+            if secrets:
+                data["secrets"] = secrets
+
+            if template:
+                data["template"] = template
 
             if resources:
                 data["cpu"] = resources["cpu"]
                 data["ram"] = resources["ram"]
                 data["gpu"] = resources["gpu"]
 
             if labels:
```

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/api_key.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/api_key.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/assets/vllm/requirements.txt` & `ploomber-cloud-0.2.4/src/ploomber_cloud/assets/vllm/requirements.txt`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/assets/vllm/test-vllm.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/assets/vllm/test-vllm.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/cli.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/cli.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/config.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,24 @@
         for label in self._data["labels"]:
             if not isinstance(label, str):
                 return (
                     f"'labels' must be a list of strings. "
                     f"Found invalid label: {label}.\n"
                 )
 
+    def _validate_secret_keys(self):
+        if "secret-keys" not in self._data.keys():
+            return None
+        for key in self._data["secret-keys"]:
+            if not isinstance(key, str):
+                return (
+                    f"'secret-keys' must be a list of strings. "
+                    f"Found invalid key: {key}.\n"
+                )
+
     def _validate_resources(self):
         if "resources" not in self._data.keys():
             return None
 
         error = ""
         resources = self._data["resources"]
 
@@ -65,16 +75,21 @@
 
         return error
 
     def _validate_config(self):
         """Method to validate the ploomber-cloud.json file
         for common issues"""
         KEYS_REQUIRED = {"id", "type"}
-        KEYS_OPTIONAL = {"resources", "template", "labels"}
-        TYPES = {"id": str, "type": str, "resources": dict, "template": str}
+        KEYS_OPTIONAL = {"resources", "template", "labels", "secret-keys"}
+        TYPES = {
+            "id": str,
+            "type": str,
+            "resources": dict,
+            "template": str,
+        }
 
         error = ""
 
         for key in KEYS_REQUIRED:
             if key not in self._data.keys():
                 error = f"{error}Mandatory key '{key}' is missing.\n"
 
@@ -89,14 +104,16 @@
             elif key in TYPES and not isinstance(value, TYPES[key]):
                 error = (
                     f"{error}Only {TYPES[key].__name__} "
                     f"values allowed for key '{key}'\n"
                 )
             elif key == "labels" and not isinstance(value, list):
                 error = "'labels' must be a list of strings.\n"
+            elif key == "secret-keys" and not isinstance(value, list):
+                error = "'secret-keys' must be a list of strings.\n"
             elif key == "type" and value not in VALID_PROJECT_TYPES:
                 error = (
                     f"{error}Invalid type '{value}'. "
                     f"Valid project types are: "
                     f"{pretty_print(VALID_PROJECT_TYPES)}\n"
                 )
 
@@ -104,14 +121,18 @@
         if resources_error:
             error = f"{error}{resources_error}"
 
         labels_error = self._validate_labels()
         if labels_error:
             error = f"{error}{labels_error}"
 
+        secret_keys_error = self._validate_secret_keys()
+        if secret_keys_error:
+            error = f"{error}{secret_keys_error}"
+
         if error:
             raise InvalidPloomberConfigException(
                 f"There are some issues with the ploomber-cloud.json file:\n{error}\n"
                 f"{FORCE_INIT_MESSAGE}\n"
             )
 
     def load(self):
```

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/configurations/community.json` & `ploomber-cloud-0.2.4/src/ploomber_cloud/configurations/community.json`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/configurations/premium.json` & `ploomber-cloud-0.2.4/src/ploomber_cloud/configurations/premium.json`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/constants.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/constants.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/delete.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/delete.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/deploy.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/deploy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import click
 import time
+import json
+from os import environ
 
 from ploomber_core.exceptions import modify_exceptions
 
 from ploomber_cloud.exceptions import (
     BasePloomberCloudException,
     InvalidPloomberResourcesException,
 )
@@ -128,24 +130,87 @@
             if job_status == "success":
                 click.echo(f"View your deployed app: {app_url}")
             break
 
         time.sleep(interval - (time_diff % interval))
 
 
+def generate_secrets_from_env(keys):
+    """
+    From a list of keys, read the value of each one and
+    package the key-value pairs into a JSON string.
+
+    For this to work, the secrets must be defined as
+    environment variables.
+    """
+    secrets_arr = []
+    output_message = [
+        "Adding the following secrets to the app: ",
+    ]
+
+    for key in keys:
+        value = environ.get(key)
+        if not value:
+            raise BasePloomberCloudException(
+                f"Value for key '{key}' not found. "
+                f"Set the value using 'export {key}=value' "
+                "or remove it from 'secret-keys'"
+            )
+        secrets_arr.append({"key": key, "value": value})
+        output_message.append(f"{key}, ")
+
+    click.echo("".join(output_message))
+    return json.dumps(secrets_arr)
+
+
+def check_for_secrets_in_config(secret_keys, secrets):
+    """
+    Check if secrets are defined in `.env` or `secret-keys`.
+    If defined in both, returns an error.
+
+    Parameters
+    ----------
+    secret_keys: list
+        A list of keys (strings) of environment variables to be read
+        from the current environment.
+        It is only keys/names, not the values.
+
+    secrets: JSON
+        A list of key-value pairs from .env as a JSON string.
+        If no secrets defined in .env, secrets is None.
+
+    Returns
+    ----------
+    secrets: JSON
+        A list of key-value pairs as a JSON string.
+    """
+    if secret_keys and secrets:
+        raise BasePloomberCloudException(
+            "Found 'secret-keys' section and '.env' file. "
+            "Only one method for adding secrets may be used.\n"
+            "Delete '.env' or remove 'secret-keys' from 'ploomber-cloud.json'."
+        )
+    elif secret_keys:
+        click.echo("Generating secrets from 'secret-keys' and environment variables.")
+        return generate_secrets_from_env(secret_keys)
+
+    return secrets
+
+
 @modify_exceptions
 @telemetry.log_call(log_args=True)
 def deploy(watch):
     """Deploy a project to Ploomber Cloud, requires a project to be initialized"""
 
     client = api.PloomberCloudClient()
     config = PloomberCloudConfig()
     config.load()
 
     with zip_.zip_app(verbose=True) as (path_to_zip, secrets):
+        secrets = check_for_secrets_in_config(config.data.get("secret-keys"), secrets)
         click.echo(f"Deploying project with id: {config.data['id']}...")
         try:
             output = client.deploy(
                 path_to_zip=path_to_zip,
                 project_type=config.data["type"],
                 project_id=config.data["id"],
                 secrets=secrets,
```

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/examples.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/examples.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/exceptions.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/functions.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/functions.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/github.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/github.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/init.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/init.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/io.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/io.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/labels.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/labels.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/resources.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/resources.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/templates.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/templates.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/util.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/util.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud/zip_.py` & `ploomber-cloud-0.2.4/src/ploomber_cloud/zip_.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.3/src/ploomber_cloud.egg-info/SOURCES.txt` & `ploomber-cloud-0.2.4/src/ploomber_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

