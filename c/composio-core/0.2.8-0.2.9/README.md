# Comparing `tmp/composio_core-0.2.8.tar.gz` & `tmp/composio_core-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.2.8.tar", last modified: Thu Apr 18 18:07:27 2024, max compression
+gzip compressed data, was "composio_core-0.2.9.tar", last modified: Thu Apr 18 18:49:37 2024, max compression
```

## Comparing `composio_core-0.2.8.tar` & `composio_core-0.2.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:27.833490 composio_core-0.2.8/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-15 07:39:40.000000 composio_core-0.2.8/MANIFEST.in
--rw-r--r--   0 karanvaidya   (501) staff       (20)      796 2024-04-18 18:07:27.833245 composio_core-0.2.8/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-15 07:39:40.000000 composio_core-0.2.8/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:27.827969 composio_core-0.2.8/composio/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      159 2024-04-15 07:39:40.000000 composio_core-0.2.8/composio/__init__.py
--rwxr-xr-x   0 karanvaidya   (501) staff       (20)    22079 2024-04-18 18:07:01.000000 composio_core-0.2.8/composio/composio_cli.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:27.830924 composio_core-0.2.8/composio/sdk/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-15 07:39:40.000000 composio_core-0.2.8/composio/sdk/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     7018 2024-04-16 18:37:25.000000 composio_core-0.2.8/composio/sdk/core.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    10226 2024-04-16 18:39:17.000000 composio_core-0.2.8/composio/sdk/enums.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    21190 2024-04-17 08:08:09.000000 composio_core-0.2.8/composio/sdk/sdk.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-15 07:39:40.000000 composio_core-0.2.8/composio/sdk/shared.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1358 2024-04-16 16:08:42.000000 composio_core-0.2.8/composio/sdk/storage.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3455 2024-04-16 17:03:02.000000 composio_core-0.2.8/composio/sdk/utils.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:27.832893 composio_core-0.2.8/composio_core.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      796 2024-04-18 18:07:27.000000 composio_core-0.2.8/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      489 2024-04-18 18:07:27.000000 composio_core-0.2.8/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-18 18:07:27.000000 composio_core-0.2.8/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-18 18:07:27.000000 composio_core-0.2.8/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      103 2024-04-18 18:07:27.000000 composio_core-0.2.8/composio_core.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-18 18:07:27.000000 composio_core-0.2.8/composio_core.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      528 2024-04-15 07:39:40.000000 composio_core-0.2.8/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)      130 2024-04-15 07:39:40.000000 composio_core-0.2.8/requirements.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-18 18:07:27.833574 composio_core-0.2.8/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1127 2024-04-18 18:07:01.000000 composio_core-0.2.8/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:37.098840 composio_core-0.2.9/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-15 07:39:40.000000 composio_core-0.2.9/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      796 2024-04-18 18:49:37.098646 composio_core-0.2.9/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-15 07:39:40.000000 composio_core-0.2.9/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:37.094983 composio_core-0.2.9/composio/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      159 2024-04-15 07:39:40.000000 composio_core-0.2.9/composio/__init__.py
+-rwxr-xr-x   0 karanvaidya   (501) staff       (20)    22112 2024-04-18 18:43:06.000000 composio_core-0.2.9/composio/composio_cli.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:37.097376 composio_core-0.2.9/composio/sdk/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-15 07:39:40.000000 composio_core-0.2.9/composio/sdk/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     7018 2024-04-16 18:37:25.000000 composio_core-0.2.9/composio/sdk/core.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    10226 2024-04-16 18:39:17.000000 composio_core-0.2.9/composio/sdk/enums.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    22118 2024-04-18 18:43:44.000000 composio_core-0.2.9/composio/sdk/sdk.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-15 07:39:40.000000 composio_core-0.2.9/composio/sdk/shared.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1358 2024-04-16 16:08:42.000000 composio_core-0.2.9/composio/sdk/storage.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3455 2024-04-16 17:03:02.000000 composio_core-0.2.9/composio/sdk/utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:37.098444 composio_core-0.2.9/composio_core.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      796 2024-04-18 18:49:37.000000 composio_core-0.2.9/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      489 2024-04-18 18:49:37.000000 composio_core-0.2.9/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-18 18:49:37.000000 composio_core-0.2.9/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-18 18:49:37.000000 composio_core-0.2.9/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      103 2024-04-18 18:49:37.000000 composio_core-0.2.9/composio_core.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-18 18:49:37.000000 composio_core-0.2.9/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      528 2024-04-15 07:39:40.000000 composio_core-0.2.9/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      130 2024-04-15 07:39:40.000000 composio_core-0.2.9/requirements.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-18 18:49:37.098876 composio_core-0.2.9/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1127 2024-04-18 18:44:03.000000 composio_core-0.2.9/setup.py
```

### Comparing `composio_core-0.2.8/PKG-INFO` & `composio_core-0.2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.2.8
+Version: 0.2.9
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.2.8/composio/composio_cli.py` & `composio_core-0.2.9/composio/composio_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,17 +332,17 @@
             console.print("\n[green]Existing connection retained. No new connection added.[/green]\n")
             return
 
     console.print(f"\n[green]> Adding integration: {integration_name.capitalize()}...[/green]\n")
     try:
         app = client.sdk.get_app(args.integration_name)
         auth_schemes = app.get('auth_schemes')
-        auth_schemes_arr = [auth_scheme.get('auth_mode') for auth_scheme in auth_schemes]
-        if len(auth_schemes_arr) > 1 and auth_schemes_arr[0] in ['API_KEY', 'BASIC', 'SNOWFLAKE']:
-            connection = entity.initiate_connection(integration_name.lower())
+        auth_modes_arr = [auth_scheme.get('auth_mode') for auth_scheme in auth_schemes]
+        if len(auth_modes_arr) > 0 and auth_modes_arr[0] in ['API_KEY', 'BASIC', 'SNOWFLAKE']:
+            connection = entity.initiate_connection_not_oauth(integration_name.lower(), auth_mode=auth_modes_arr[0])
             fields = auth_schemes[0].get('fields')
             fields_input = {}
             for field in fields:
                 if field.get('expected_from_customer', True):
                     if field.get('required', False):
                         console.print(f"[green]> Enter {field.get('displayName', field.get('name'))}: [/green]", end="")
                         value = input() or field.get('default')
```

### Comparing `composio_core-0.2.8/composio/sdk/core.py` & `composio_core-0.2.9/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.8/composio/sdk/enums.py` & `composio_core-0.2.9/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.8/composio/sdk/sdk.py` & `composio_core-0.2.9/composio/sdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,25 +329,35 @@
         
     def get_integration(self, connector_id: str) -> Integration:
         resp = self.http_client.get(f"{self.base_url}/v1/integrations/{connector_id}")
         if resp.status_code == 200:
             return Integration(self, **resp.json())
         raise Exception(f"Failed to get integration, status code: {resp.status_code}, response: {resp.text}")
         
-    def create_integration(self, app: Union[App, str], use_default = False) -> Integration:
+    def create_integration(self, app: Union[App, str], use_default = False, name: str = None, auth_mode: str = None) -> Integration:
         if isinstance(app, App):
             app = app.value
         app_details = self.get_app(app)
         app_id = app_details.get("appId")
         if app_id is None:
             raise Exception(f"App {app} does not exist for the account")
-        resp = self.http_client.post(f"{self.base_url}/v1/integrations", json={
+        req = {
             "appId": app_id,
             "useComposioAuth": use_default
-        })
+        }
+        if name:
+            req["name"] = name
+        if auth_mode:
+            req["authScheme"] = auth_mode
+            auth_schemes = app_details.get('auth_schemes')
+            for auth_scheme_iter in auth_schemes:
+                if auth_scheme_iter.get('auth_mode') == auth_mode:
+                    fields = auth_scheme_iter.get('fields')
+                    req["authConfig"] = {field.get('name'): "" for field in fields}
+        resp = self.http_client.post(f"{self.base_url}/v1/integrations", json=req)
         if resp.status_code == 200:
             return Integration(self, **resp.json())
 
         raise Exception(f"Failed to create integration, status code: {resp.status_code}, response: {resp.text}")
 
     def get_connected_account(self, connection_id: str) -> ConnectedAccount:
         resp = self.http_client.get(
@@ -522,7 +532,13 @@
                 )
                 time.sleep(0.5)
         return run_object
 
     def initiate_connection(self, app_name: Union[str, App], redirect_url: str = None):
         integration = self.client.get_default_integration(app_name)
         return integration.initiate_connection(entity_id=self.entity_id, redirect_url=redirect_url)
+
+    def initiate_connection_not_oauth(self, app_name: Union[str, App], redirect_url: str = None, auth_mode: str = None):
+        from datetime import datetime
+        timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
+        integration = self.client.create_integration(app_name, name=f"integration_{timestamp}", auth_mode=auth_mode)
+        return integration.initiate_connection(entity_id=self.entity_id, redirect_url=redirect_url)
```

### Comparing `composio_core-0.2.8/composio/sdk/storage.py` & `composio_core-0.2.9/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.8/composio/sdk/utils.py` & `composio_core-0.2.9/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.8/composio_core.egg-info/PKG-INFO` & `composio_core-0.2.9/composio_core.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.2.8
+Version: 0.2.9
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.2.8/pyproject.toml` & `composio_core-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.8/setup.py` & `composio_core-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.2.8",
+    version="0.2.9",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

