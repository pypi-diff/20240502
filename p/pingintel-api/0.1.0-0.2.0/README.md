# Comparing `tmp/pingintel_api-0.1.0.tar.gz` & `tmp/pingintel_api-0.2.0.tar.gz`

## Comparing `pingintel_api-0.1.0.tar` & `pingintel_api-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pingintel_api-0.1.0/justfile
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pingintel_api-0.1.0/requirements.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pingintel_api-0.1.0/src/pingintel_api/__about__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pingintel_api-0.1.0/src/pingintel_api/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pingintel_api-0.1.0/src/pingintel_api/constants.py
--rw-r--r--   0        0        0    11223 2020-02-02 00:00:00.000000 pingintel_api-0.1.0/src/pingintel_api/sov_fixer_api_client.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 pingintel_api-0.1.0/src/pingintel_api/sovfixerapi_cmd.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pingintel_api-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pingintel_api-0.1.0/tests/tests.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 pingintel_api-0.1.0/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pingintel_api-0.1.0/LICENSE
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pingintel_api-0.1.0/README.md
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pingintel_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 pingintel_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/justfile
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/examples/fix_sov.py
+-rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/examples/test_sov.xlsx
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/src/pingintel_api/__about__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/src/pingintel_api/__init__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/src/pingintel_api/constants.py
+-rw-r--r--   0        0        0    10590 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/src/pingintel_api/sov_fixer_api_client.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/src/pingintel_api/sovfixerapi_cmd.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/tests/tests.py
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/LICENSE
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/README.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pingintel_api-0.2.0/PKG-INFO
```

### Comparing `pingintel_api-0.1.0/src/pingintel_api/constants.py` & `pingintel_api-0.2.0/src/pingintel_api/constants.py`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.1.0/src/pingintel_api/sov_fixer_api_client.py` & `pingintel_api-0.2.0/src/pingintel_api/sov_fixer_api_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,24 +71,24 @@
 
 
 class SOVFixerAPIClient:
     SOV_STATUS = c.SOV_STATUS
     SOV_RESULT_STATUS = c.SOV_RESULT_STATUS
 
     @overload
-    def __init__(self, api_url: str, token=None) -> None: ...
+    def __init__(self, api_url: str, auth_token=None) -> None: ...
 
     @overload
-    def __init__(self, environment: str = "prod", token=None) -> None: ...
+    def __init__(self, environment: str = "prod", auth_token=None) -> None: ...
 
     def __init__(
         self,
         api_url: str | None = None,
         environment: str | None = "prod",
-        token=None,
+        auth_token=None,
     ):
         if api_url is None:
             assert environment, "Need either api_url or environment."
             if environment == "prod":
                 api_url = "https://api.sovfixer.com"
             elif environment == "prod2":
                 api_url = "https://api2.sovfixer.com"
@@ -97,44 +97,44 @@
             elif environment == "local":
                 api_url = "http://api-local.sovfixer.com"
             elif environment == "local2":
                 api_url = "http://localhost:8000"
             else:
                 api_url = f"https://api-{environment}.sovfixer.com"
 
-        if token is None:
+        if auth_token is None:
             if environment in ["staging", "staging2"]:
                 serverspace = "stg"
             elif environment in ["prod", "prod2"]:
                 serverspace = "prd"
             elif environment in ["prodeu", "prodeu2"]:
                 serverspace = "prdeu"
             elif environment in ["dev", "dev2"]:
                 serverspace = "dev"
             elif environment in ["local", "local2"]:
                 serverspace = "local"
             else:
-                raise ValueError("Unknown environment and missing token.")
-            token = os.environ.get(f"PING_{serverspace}_AUTH_TOKEN".upper())
+                raise ValueError("Unknown environment and missing auth_token.")
+            auth_token = os.environ.get(f"PING_{serverspace}_AUTH_TOKEN".upper())
 
-        if token is None:
-            token = os.environ.get("SOVFIXER_AUTH_TOKEN")
-        if token is None:
+        if auth_token is None:
+            auth_token = os.environ.get("SOVFIXER_AUTH_TOKEN")
+        if auth_token is None:
             raise ValueError(
                 "Need --auth-token or SOVFIXER_AUTH_TOKEN environment variable set."
             )
         assert api_url
         self.api_url = api_url
-        self.token = token
-        self.headers = {"Authorization": f"Token {token}"}
+        self.auth_token = auth_token
         self.session = requests.Session()
         self.session.headers = {
-            "Authorization": f"Token {self.token}",
+            "Authorization": f"Token {self.auth_token}",
             "Accept-Encoding": "gzip",
         }
+        self.environment = environment if api_url is None else None
 
     def fix_sov_async_start(
         self,
         file: IO[bytes] | str,
         document_type,
         filename=None,
         callback_url=None,
@@ -177,180 +177,136 @@
             pprint.pprint(response.text)
 
         raise_for_status(response)
 
         response_data = response.json()
         sov_id = response_data["id"]
         message = response_data["message"]
-        status_url = self.api_url + f"/api/v1/sov/{sov_id}?include_progress=True"
+        status_url = self.api_url + f"/api/v1/sov/{sov_id}"
         log(
             f"+ Dispatched {sov_id}: {message}.  Now, polling for results at {status_url}."
         )
         return response_data
 
     def fix_sov_async_check_progress(self, sovid_or_start_ret) -> FixSOVResponse:
         if isinstance(sovid_or_start_ret, dict):
             sov_id = sovid_or_start_ret["id"]
         else:
             sov_id = sovid_or_start_ret
 
-        status_url = self.api_url + f"/api/v1/sov/{sov_id}?include_progress=True"
+        status_url = self.api_url + f"/api/v1/sov/{sov_id}?include_progress=true"
         # params = {"id": sov_id}
 
         response = self.session.get(status_url)
         # pprint.pprint(response.json())
         raise_for_status(response)
 
         response_data: FixSOVResponse = response.json()
         # request_status = response_data["request"]["status"]
         return response_data
 
-    def fix_sov_download(
-        self, output_ret, actually_write=False, output_path=None, environment=None
-    ):
-        return download_output(
-            output_ret,
-            session=self.session,
-            actually_write=actually_write,
-            output_path=output_path,
-            environment=environment,
-        )
+    def fix_sov_download(self, output_ret, actually_write=False, output_path=None):
+        output_url = output_ret["url"]
+        if (
+            self.environment
+            and self.environment == "local2"
+            and "api-local.sovfixer.com" in output_url
+        ):
+            output_url = output_url.replace("api-local.sovfixer.com", "localhost:8000")
+
+        output_description = output_ret["description"]
+        output_filename = output_ret["filename"]
+        if output_path is None:
+            output_path = output_filename
 
+        log(f"Requesting output from {output_url}...")
+        with self.session.get(output_url, stream=True) as response:
+            raise_for_status(response)
+            filesize_mb = int(response.headers.get("content-length", 0)) / 1024 / 1024
+            pprint.pprint(dict(response.headers))
+            log(f"  - Streaming {output_description} output ({filesize_mb:.2f} MB)...")
 
-def download_output(
-    output,
-    environment=None,
-    session=None,
-    auth_token=None,
-    actually_write=False,
-    output_path=None,
-):
-    if session is None:
-        session = requests.Session()
-        session.headers = {
-            "Authorization": f"Token {auth_token}",
-            "Accept-Encoding": "gzip",
-        }
+            if actually_write:
+                with open(output_path, "wb") as fd:
+                    for chunk in response.iter_content(chunk_size=1024 * 1024):
+                        fd.write(chunk)
+            log(f"  - Downloaded {output_description} output: {output_path}.")
+        return output_path if actually_write else None
 
-    output_url = output["url"]
-    if (
-        environment
-        and environment == "local2"
-        and "api-local.sovfixer.com" in output_url
+    def fix_sov(
+        self,
+        filename,
+        document_type: str = "SOV",
+        callback_url=None,
+        actually_write=False,
+        output_formats=None,
+        client_ref=None,
     ):
-        output_url = output_url.replace("api-local.sovfixer.com", "localhost:8000")
-
-    output_description = output["description"]
-    output_filename = output["filename"]
-    if output_path is None:
-        output_path = output_filename
-
-    log(f"Requesting output from {output_url}...")
-    with session.get(output_url, stream=True) as response:
-        raise_for_status(response)
-        filesize_mb = int(response.headers.get("content-length", 0)) / 1024 / 1024
-        pprint.pprint(dict(response.headers))
-        log(f"  - Streaming {output_description} output ({filesize_mb:.2f} MB)...")
-
-        if actually_write:
-            with open(output_path, "wb") as fd:
-                for chunk in response.iter_content(chunk_size=1024 * 1024):
-                    fd.write(chunk)
-        log(f"  - Downloaded {output_description} output: {output_path}.")
-    return output_path if actually_write else None
-
-
-def secure_filename(s):
-    return s
-
-
-def fix_sov(
-    API_URL,
-    filename,
-    document_type,
-    auth_token,
-    environment=None,
-    callback_url=None,
-    actually_write=False,
-    output_formats=None,
-    session=None,
-    client_ref=None,
-):
-    if auth_token is None:
-        auth_token = os.environ.get("SOVFIXER_AUTH_TOKEN")
-    if auth_token is None:
-        raise click.ClickException(
-            "Need --auth-token or SOVFIXER_AUTH_TOKEN environment variable set."
+        sov_fixer_client = self
+        start_response = sov_fixer_client.fix_sov_async_start(
+            filename,
+            document_type=document_type,
+            callback_url=callback_url,
+            output_formats=output_formats,
+            client_ref=client_ref,
         )
 
-    if not os.path.exists(filename):
-        raise click.ClickException("Path does not exist.")
-
-    sov_fixer_client = SOVFixerAPIClient(API_URL, auth_token)
-    start_response = sov_fixer_client.fix_sov_async_start(
-        filename,
-        document_type=document_type,
-        callback_url=callback_url,
-        output_formats=output_formats,
-        client_ref=client_ref,
-    )
-
-    while 1:
-        response_data = sov_fixer_client.fix_sov_async_check_progress(start_response)
-        # raise_for_status(response_data)
-        # pprint.pprint(response_data)
-
-        request_status = response_data["request"]["status"]
-
-        POLL_SECS = 2.5
-        if request_status == "PENDING":
-            log(
-                f"  - Has not yet been queued for processing, checking progress in {POLL_SECS}s."
+        while 1:
+            response_data = sov_fixer_client.fix_sov_async_check_progress(
+                start_response
             )
-            time.sleep(POLL_SECS)
-        elif request_status == "IN_PROGRESS":
-            log(f"  - Still in progress, checking progress in {POLL_SECS}s.")
-            time.sleep(POLL_SECS)
-        else:
-            break
+            # raise_for_status(response_data)
+            # pprint.pprint(response_data)
 
-    result_status = response_data["result"]["status"]
-    result_message = response_data["result"]["message"]
-    log(f"+ Finished with result {result_status}: {result_message}")
-
-    if result_status == "SUCCESS":
-        log("Complete!  Fetching outputs.")
-        for output in response_data["result"]["outputs"]:
-            output_url = output["url"]
-            if (
-                environment
-                and environment == "local2"
-                and "api-local.sovfixer.com" in output_url
-            ):
-                output_url = output_url.replace(
-                    "api-local.sovfixer.com", "localhost:8000"
-                )
+            request_status = response_data["request"]["status"]
+            pct_complete = response_data["request"]["pct_complete"]
+            last_status = response_data["request"]["last_health_status"]
+
+            POLL_SECS = 2.5
+            if request_status == "PENDING":
+                log("  - Has not yet been queued for processing.")
+                time.sleep(POLL_SECS)
+            elif request_status == "IN_PROGRESS":
+                log(f"  - Still in progress ({pct_complete}% complete): {last_status}")
+                time.sleep(POLL_SECS)
+            else:
+                break
 
-            output_filename = output["filename"]
+        result_status = response_data["result"]["status"]
+        result_message = response_data["result"]["message"]
+        log(f"+ Finished with result {result_status}: {result_message}")
+
+        if result_status == "SUCCESS":
+            log("Complete!  Fetching outputs.")
+            for output in response_data["result"]["outputs"]:
+                output_url = output["url"]
+                if (
+                    self.environment
+                    and self.environment == "local2"
+                    and "api-local.sovfixer.com" in output_url
+                ):
+                    output_url = output_url.replace(
+                        "api-local.sovfixer.com", "localhost:8000"
+                    )
 
-            output_path = output_filename
+                output_filename = output["filename"]
 
-            if actually_write:
-                if os.path.exists(output_path):
-                    yesno = input(
-                        f"Do you want to overwrite the existing file {output_path} [y/N]? "
-                    )
-                    if yesno.lower() != "y":
-                        continue
+                output_path = output_filename
 
-            response = sov_fixer_client.fix_sov_download(
-                output,
-                actually_write=actually_write,
-                output_path=output_path,
-                environment=environment,
-            )
-            raise_for_status(response)
-        return True
-    else:
-        log("* Parsing failed!  Raw API output:")
-        log(response_data)
-        return False
+                if actually_write:
+                    if os.path.exists(output_path):
+                        yesno = input(
+                            f"Do you want to overwrite the existing file {output_path} [y/N]? "
+                        )
+                        if yesno.lower() != "y":
+                            continue
+
+                sov_fixer_client.fix_sov_download(
+                    output,
+                    actually_write=actually_write,
+                    output_path=output_path,
+                )
+            return True
+        else:
+            log("* Parsing failed!  Raw API output:")
+            log(response_data)
+            return False
```

### Comparing `pingintel_api-0.1.0/src/pingintel_api/sovfixerapi_cmd.py` & `pingintel_api-0.2.0/src/pingintel_api/sovfixerapi_cmd.py`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.1.0/.gitignore` & `pingintel_api-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.1.0/LICENSE` & `pingintel_api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pingintel_api-0.1.0/pyproject.toml` & `pingintel_api-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "pingintel-api"
 dynamic = ["version"]
 authors = [
   { name="Scott Stafford", email="scott@pingintel.com" },
 ]
 description = "Python-based API for Ping Data Intelligence APIs"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `pingintel_api-0.1.0/PKG-INFO` & `pingintel_api-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.3
 Name: pingintel-api
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python-based API for Ping Data Intelligence APIs
 Project-URL: Homepage, https://github.com/pingintel/pingintel-api
 Project-URL: Issues, https://github.com/pingintel/pingintel-api
 Author-email: Scott Stafford <scott@pingintel.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # pingintel-api
 Python-based API for Ping Data Technology products.
 
+### Usage
 
-Usage:
+To submit an SOV to Ping SOV Fixer and poll for completion:
 
 ```python
-from pingintel_api import PingSOVFixerAPIClient
+from pingintel_api import SOVFixerAPIClient
 
-PingSOVFixerAPIClient(
-```
+api_client = SOVFixerAPIClient()
+api_client.fix_sov("test_sov.xlsx")
+```
```

