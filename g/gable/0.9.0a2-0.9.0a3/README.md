# Comparing `tmp/gable-0.9.0a2.tar.gz` & `tmp/gable-0.9.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gable-0.9.0a2.tar", max compression
+gzip compressed data, was "gable-0.9.0a3.tar", max compression
```

## Comparing `gable-0.9.0a2.tar` & `gable-0.9.0a3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2550 2024-01-17 22:32:40.198630 gable-0.9.0a2/README.md
--rw-r--r--   0        0        0        0 2023-12-04 23:31:13.219816 gable-0.9.0a2/gable/__init__.py
--rw-r--r--   0        0        0     1614 2023-12-04 23:31:13.219874 gable-0.9.0a2/gable/cli.py
--rw-r--r--   0        0        0     5566 2024-02-29 00:06:18.452402 gable-0.9.0a2/gable/client.py
--rw-r--r--   0        0        0        0 2023-12-04 23:31:13.219954 gable-0.9.0a2/gable/commands/__init__.py
--rw-r--r--   0        0        0     2316 2024-02-29 00:06:18.452672 gable-0.9.0a2/gable/commands/auth.py
--rw-r--r--   0        0        0     3083 2024-02-29 00:06:18.453121 gable-0.9.0a2/gable/commands/contract.py
--rw-r--r--   0        0        0    23337 2024-02-29 00:06:18.453565 gable-0.9.0a2/gable/commands/data_asset.py
--rw-r--r--   0        0        0     1806 2024-02-29 00:06:18.454205 gable-0.9.0a2/gable/commands/debug.py
--rw-r--r--   0        0        0      711 2024-02-29 00:06:18.454634 gable-0.9.0a2/gable/commands/ping.py
--rw-r--r--   0        0        0        0 2023-12-04 23:31:13.220281 gable-0.9.0a2/gable/helpers/__init__.py
--rw-r--r--   0        0        0     2471 2024-02-29 00:06:18.454852 gable-0.9.0a2/gable/helpers/auth.py
--rw-r--r--   0        0        0     5760 2024-02-07 18:23:08.377989 gable-0.9.0a2/gable/helpers/bundler.py
--rw-r--r--   0        0        0     4376 2024-02-29 00:06:18.455319 gable-0.9.0a2/gable/helpers/check.py
--rw-r--r--   0        0        0     4389 2024-02-16 19:16:34.822820 gable-0.9.0a2/gable/helpers/contract.py
--rw-r--r--   0        0        0    11747 2024-02-29 00:06:18.455821 gable-0.9.0a2/gable/helpers/data_asset.py
--rw-r--r--   0        0        0      143 2023-12-04 23:31:13.220520 gable-0.9.0a2/gable/helpers/emoji.py
--rw-r--r--   0        0        0      274 2023-12-04 23:31:13.220570 gable-0.9.0a2/gable/helpers/jsonpickle.py
--rw-r--r--   0        0        0     3576 2023-12-04 23:31:13.220633 gable-0.9.0a2/gable/helpers/logging.py
--rw-r--r--   0        0        0     1774 2023-12-04 23:31:13.220681 gable-0.9.0a2/gable/helpers/multi_option.py
--rw-r--r--   0        0        0     4444 2024-02-27 21:20:29.612686 gable-0.9.0a2/gable/helpers/npm.py
--rw-r--r--   0        0        0     2241 2024-02-13 21:39:00.639651 gable-0.9.0a2/gable/helpers/repo_interactions.py
--rw-r--r--   0        0        0      176 2023-12-04 23:31:13.220766 gable-0.9.0a2/gable/helpers/shell_output.py
--rw-r--r--   0        0        0    35876 2024-02-27 19:03:49.099658 gable-0.9.0a2/gable/openapi.py
--rw-r--r--   0        0        0    22496 2024-02-27 19:03:29.837674 gable-0.9.0a2/gable/options.py
--rw-r--r--   0        0        0        0 2023-12-04 23:31:13.220900 gable-0.9.0a2/gable/readers/__init__.py
--rw-r--r--   0        0        0      479 2023-12-04 23:31:13.220945 gable-0.9.0a2/gable/readers/constants.py
--rw-r--r--   0        0        0    12995 2024-01-22 21:51:35.886372 gable-0.9.0a2/gable/readers/dbapi.py
--rw-r--r--   0        0        0      256 2023-12-04 23:31:13.221038 gable-0.9.0a2/gable/readers/file.py
--rw-r--r--   0        0        0     3472 2023-12-04 23:31:13.221085 gable-0.9.0a2/gable/readers/mysql.py
--rw-r--r--   0        0        0     1694 2023-12-04 23:31:13.221135 gable-0.9.0a2/gable/readers/postgres.py
--rw-r--r--   0        0        0     1912 2024-02-29 00:07:28.779920 gable-0.9.0a2/pyproject.toml
--rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 gable-0.9.0a2/PKG-INFO
+-rw-r--r--   0        0        0     2550 2024-01-17 22:32:40.198630 gable-0.9.0a3/README.md
+-rw-r--r--   0        0        0        0 2023-12-04 23:31:13.219816 gable-0.9.0a3/gable/__init__.py
+-rw-r--r--   0        0        0     1614 2023-12-04 23:31:13.219874 gable-0.9.0a3/gable/cli.py
+-rw-r--r--   0        0        0     5566 2024-02-29 00:06:18.452402 gable-0.9.0a3/gable/client.py
+-rw-r--r--   0        0        0        0 2023-12-04 23:31:13.219954 gable-0.9.0a3/gable/commands/__init__.py
+-rw-r--r--   0        0        0     2316 2024-02-29 00:06:18.452672 gable-0.9.0a3/gable/commands/auth.py
+-rw-r--r--   0        0        0     3083 2024-02-29 00:06:18.453121 gable-0.9.0a3/gable/commands/contract.py
+-rw-r--r--   0        0        0    23327 2024-02-29 02:09:11.311876 gable-0.9.0a3/gable/commands/data_asset.py
+-rw-r--r--   0        0        0     1806 2024-02-29 00:06:18.454205 gable-0.9.0a3/gable/commands/debug.py
+-rw-r--r--   0        0        0      711 2024-02-29 00:06:18.454634 gable-0.9.0a3/gable/commands/ping.py
+-rw-r--r--   0        0        0        0 2023-12-04 23:31:13.220281 gable-0.9.0a3/gable/helpers/__init__.py
+-rw-r--r--   0        0        0     2471 2024-02-29 00:06:18.454852 gable-0.9.0a3/gable/helpers/auth.py
+-rw-r--r--   0        0        0     5760 2024-02-07 18:23:08.377989 gable-0.9.0a3/gable/helpers/bundler.py
+-rw-r--r--   0        0        0     4376 2024-02-29 00:06:18.455319 gable-0.9.0a3/gable/helpers/check.py
+-rw-r--r--   0        0        0     4389 2024-02-16 19:16:34.822820 gable-0.9.0a3/gable/helpers/contract.py
+-rw-r--r--   0        0        0    11775 2024-02-29 02:04:03.641201 gable-0.9.0a3/gable/helpers/data_asset.py
+-rw-r--r--   0        0        0      143 2023-12-04 23:31:13.220520 gable-0.9.0a3/gable/helpers/emoji.py
+-rw-r--r--   0        0        0      274 2023-12-04 23:31:13.220570 gable-0.9.0a3/gable/helpers/jsonpickle.py
+-rw-r--r--   0        0        0     3576 2023-12-04 23:31:13.220633 gable-0.9.0a3/gable/helpers/logging.py
+-rw-r--r--   0        0        0     1774 2023-12-04 23:31:13.220681 gable-0.9.0a3/gable/helpers/multi_option.py
+-rw-r--r--   0        0        0     4426 2024-03-01 00:49:26.076602 gable-0.9.0a3/gable/helpers/npm.py
+-rw-r--r--   0        0        0     2241 2024-02-13 21:39:00.639651 gable-0.9.0a3/gable/helpers/repo_interactions.py
+-rw-r--r--   0        0        0      176 2023-12-04 23:31:13.220766 gable-0.9.0a3/gable/helpers/shell_output.py
+-rw-r--r--   0        0        0    35876 2024-02-27 19:03:49.099658 gable-0.9.0a3/gable/openapi.py
+-rw-r--r--   0        0        0    22496 2024-02-27 19:03:29.837674 gable-0.9.0a3/gable/options.py
+-rw-r--r--   0        0        0        0 2023-12-04 23:31:13.220900 gable-0.9.0a3/gable/readers/__init__.py
+-rw-r--r--   0        0        0      479 2023-12-04 23:31:13.220945 gable-0.9.0a3/gable/readers/constants.py
+-rw-r--r--   0        0        0    12995 2024-01-22 21:51:35.886372 gable-0.9.0a3/gable/readers/dbapi.py
+-rw-r--r--   0        0        0      256 2023-12-04 23:31:13.221038 gable-0.9.0a3/gable/readers/file.py
+-rw-r--r--   0        0        0     3472 2023-12-04 23:31:13.221085 gable-0.9.0a3/gable/readers/mysql.py
+-rw-r--r--   0        0        0     1694 2023-12-04 23:31:13.221135 gable-0.9.0a3/gable/readers/postgres.py
+-rw-r--r--   0        0        0     1912 2024-03-01 07:13:20.445001 gable-0.9.0a3/pyproject.toml
+-rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 gable-0.9.0a3/PKG-INFO
```

### Comparing `gable-0.9.0a2/README.md` & `gable-0.9.0a3/README.md`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/cli.py` & `gable-0.9.0a3/gable/cli.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/client.py` & `gable-0.9.0a3/gable/client.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/commands/auth.py` & `gable-0.9.0a3/gable/commands/auth.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/commands/contract.py` & `gable-0.9.0a3/gable/commands/contract.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/commands/data_asset.py` & `gable-0.9.0a3/gable/commands/data_asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,19 +294,18 @@
             ctx.obj.client,
         )
     elif source_type == SourceType.TYPESCRIPT.value:
         if not library:
             raise click.ClickException(
                 f"{EMOJI.RED_X.value} Missing required options for Typescript project registration. You can use the --debug or --trace flags for more details."
             )
-        event_names = gather_typescript_asset_data(library, ctx.obj.client)
-        formatted_event_names = "\n".join(event_names)
-        logger.info(
-            f"{EMOJI.GREEN_CHECK.value} The following events were detected: \n{formatted_event_names}"
-        )
+        events = gather_typescript_asset_data(library, ctx.obj.client)
+        logger.info(f"{EMOJI.GREEN_CHECK.value} The following events were detected:")
+        for event in events:
+            logger.info(f"{event['eventName']} - {event['type']}\n")
         if not dry_run:
             logger.info(
                 f"{EMOJI.YELLOW_WARNING.value} Registration for Typescript sources is not supported at this time. Please contact Gable for more information."
             )
         return
     else:
         raise NotImplementedError(f"Unknown source type: {source_type}")
```

### Comparing `gable-0.9.0a2/gable/commands/debug.py` & `gable-0.9.0a3/gable/commands/debug.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/commands/ping.py` & `gable-0.9.0a3/gable/commands/ping.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/helpers/auth.py` & `gable-0.9.0a3/gable/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/helpers/bundler.py` & `gable-0.9.0a3/gable/helpers/bundler.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/helpers/check.py` & `gable-0.9.0a3/gable/helpers/check.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/helpers/contract.py` & `gable-0.9.0a3/gable/helpers/contract.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/helpers/data_asset.py` & `gable-0.9.0a3/gable/helpers/data_asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,19 +300,21 @@
     project_repo = get_git_repo_info(project_root + "/" + emitter_file_path)
 
     source_names = [f"{project_repo['gitSSHRepo']}" for x in sca_result_list]
     schema_contents = [json.dumps(x) for x in sca_result_list]
     return source_names, schema_contents
 
 
-def gather_typescript_asset_data(library: str, client: GableClient) -> List[str]:
+def gather_typescript_asset_data(
+    library: str, client: GableClient
+) -> List[dict[str, str]]:
     prepare_npm_environment(client)
     # Run SCA, get back the results
     sca_results = run_sca_typescript(library)
-    sca_results_list = cast(list[str], json.loads(sca_results))
+    sca_results_list = cast(list[dict[str, str]], json.loads(sca_results))
     return sca_results_list
 
 
 def prepare_npm_environment(client: GableClient) -> None:
     # Verify node is installed
     check_node_installed()
```

### Comparing `gable-0.9.0a2/gable/helpers/logging.py` & `gable-0.9.0a3/gable/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/helpers/multi_option.py` & `gable-0.9.0a3/gable/helpers/multi_option.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/helpers/npm.py` & `gable-0.9.0a3/gable/helpers/npm.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from loguru import logger
 
 BASE_NPX_CMD = [
     "npx",
     "-y",
     "-q",
     "@gable-eng/sca",
-    "typescript",
 ]
 
 
 def check_node_installed():
     try:
         result = subprocess.run(
             ["node", "--version"], check=True, stdout=subprocess.PIPE, text=True
```

### Comparing `gable-0.9.0a2/gable/helpers/repo_interactions.py` & `gable-0.9.0a3/gable/helpers/repo_interactions.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/openapi.py` & `gable-0.9.0a3/gable/openapi.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/options.py` & `gable-0.9.0a3/gable/options.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/readers/dbapi.py` & `gable-0.9.0a3/gable/readers/dbapi.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/readers/mysql.py` & `gable-0.9.0a3/gable/readers/mysql.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/gable/readers/postgres.py` & `gable-0.9.0a3/gable/readers/postgres.py`

 * *Files identical despite different names*

### Comparing `gable-0.9.0a2/pyproject.toml` & `gable-0.9.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gable"
-version = "0.9.0a2"
+version = "0.9.0a3"
 description = "Command line interface to interact with Gable API"
 authors = ["Gable.ai <engineers@gable.ai>"]
 readme = "README.md"
 packages = [{include = "gable"}]
 # By default Poetry excludes all files and directories listed in .gitignore,
 # so we need to override this for the generated openapi file
 include = ["gable/openapi.py"]
```

### Comparing `gable-0.9.0a2/PKG-INFO` & `gable-0.9.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gable
-Version: 0.9.0a2
+Version: 0.9.0a3
 Summary: Command line interface to interact with Gable API
 Author: Gable.ai
 Author-email: engineers@gable.ai
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

