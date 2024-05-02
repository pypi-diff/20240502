# Comparing `tmp/morphdb_utils-0.1.8.tar.gz` & `tmp/morphdb_utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphdb_utils-0.1.8.tar", max compression
+gzip compressed data, was "morphdb_utils-0.1.9.tar", max compression
```

## Comparing `morphdb_utils-0.1.8.tar` & `morphdb_utils-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      139 2024-03-18 04:21:28.042602 morphdb_utils-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-03-16 10:09:51.538940 morphdb_utils-0.1.8/morphdb_utils/__init__.py
--rw-r--r--   0        0        0     6133 2024-03-20 15:19:50.014817 morphdb_utils-0.1.8/morphdb_utils/api.py
--rw-r--r--   0        0        0      414 2024-03-19 10:30:59.983235 morphdb_utils-0.1.8/morphdb_utils/logging.py
--rw-r--r--   0        0        0      565 2024-03-18 04:19:45.556474 morphdb_utils-0.1.8/morphdb_utils/type.py
--rw-r--r--   0        0        0      608 2024-03-20 15:20:14.597970 morphdb_utils-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 morphdb_utils-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      139 2024-03-18 04:21:28.042602 morphdb_utils-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 15:36:31.683538 morphdb_utils-0.1.9/morphdb_utils/__init__.py
+-rw-r--r--   0        0        0     6187 2024-03-20 15:30:29.715941 morphdb_utils-0.1.9/morphdb_utils/api.py
+-rw-r--r--   0        0        0      414 2024-03-20 15:30:32.932377 morphdb_utils-0.1.9/morphdb_utils/logging.py
+-rw-r--r--   0        0        0        0 2024-03-20 15:27:58.647939 morphdb_utils-0.1.9/morphdb_utils/py.typed
+-rw-r--r--   0        0        0      565 2024-03-18 04:19:45.556474 morphdb_utils-0.1.9/morphdb_utils/type.py
+-rw-r--r--   0        0        0      608 2024-03-20 15:42:33.752555 morphdb_utils-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 morphdb_utils-0.1.9/PKG-INFO
```

### Comparing `morphdb_utils-0.1.8/morphdb_utils/api.py` & `morphdb_utils-0.1.9/morphdb_utils/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,22 +88,27 @@
             value = row["value"][field]["kind"]
             case_type = value["$case"]
             parsed_row[field] = parse_value(case_type, value)
         parsed_rows.append(parsed_row)
     return pd.DataFrame.from_dict(parsed_rows)
 
 
-def ref(
-    reference: str,
+
+def _execute_sql_impl(
+    sql: str,
+    connection_slug: str | None = None,
+    database_id: str | None = None,
     base_url: str | None = None,
     team_slug: str | None = None,
     authorization: str | None = None,
-    notebook_id: str | None = None
-) -> [str, str | None]:
+    notebook_id: str | None = None,
+) -> pd.DataFrame:
     config_from_env = _read_configuration_from_env()
+    if database_id is None:
+        database_id = config_from_env["database_id"]
     if base_url is None:
         base_url = config_from_env["base_url"]
     if team_slug is None:
         team_slug = config_from_env["team_slug"]
     if authorization is None:
         authorization = config_from_env["authorization"]
     if notebook_id is None:
@@ -112,54 +117,50 @@
     headers = {
         "teamSlug": team_slug,
         "Authorization": authorization,
     }
 
     url_sql = urllib.parse.urljoin(
         _canonicalize_base_url(base_url),
-        f"/canvas/{notebook_id}/cell-name/{reference}",
+        f"/{database_id}/sql/python",
     )
-    response = requests.get(url_sql, headers=headers, verify=True)
-    if response.status_code != 200:
-        raise MorphApiError(response.text)
-    response_body = response.json()
-
-    if response_body["cellType"] != "sql":
-        raise MorphApiError(f"Cell {reference} is not a SQL cell")
 
-    sql = response_body["code"]
-    connection_slug = None
-    if response_body["connectionType"] == "external":
-        connection_slug = response_body["connectionSlug"]
-    return {
-        "sql": sql,
-        "connection_slug": connection_slug
+    request = {
+        "sql": sql
     }
+    if connection_slug is not None:
+        request["connectionSlug"] = connection_slug
 
+    response = requests.post(url_sql, headers=headers, json=request, verify=True)
+    if response.status_code != 200:
+        raise MorphApiError(response.text)
 
-def execute_sql(*args, **kwargs):
-    if args and isinstance(args[0], dict):
-        ref_dict = args[0]
-        return _execute_sql_impl(**ref_dict, **kwargs)
-    else:
-        return _execute_sql_impl(*args, **kwargs)
+    try:
+        response_body = response.json()
+        structured_response_body = SqlResultResponse(
+            headers=response_body["headers"], rows=response_body["rows"]
+        )
+        df = _convert_sql_engine_response(structured_response_body)
+        return df
+    except Exception as e:
+        raise MorphApiError(f"{e}")
 
 
-def _execute_sql_impl(
-    sql: str,
-    connection_slug: str | None = None,
-    database_id: str | None = None,
+
+def ref(
+    reference: str,
     base_url: str | None = None,
     team_slug: str | None = None,
     authorization: str | None = None,
-    notebook_id: str | None = None,
-) -> pd.DataFrame:
+    notebook_id: str | None = None
+) -> {
+    "sql": str,
+    "connection_slug": str | None
+}:
     config_from_env = _read_configuration_from_env()
-    if database_id is None:
-        database_id = config_from_env["database_id"]
     if base_url is None:
         base_url = config_from_env["base_url"]
     if team_slug is None:
         team_slug = config_from_env["team_slug"]
     if authorization is None:
         authorization = config_from_env["authorization"]
     if notebook_id is None:
@@ -168,29 +169,33 @@
     headers = {
         "teamSlug": team_slug,
         "Authorization": authorization,
     }
 
     url_sql = urllib.parse.urljoin(
         _canonicalize_base_url(base_url),
-        f"/{database_id}/sql/python",
+        f"/canvas/{notebook_id}/cell-name/{reference}",
     )
+    response = requests.get(url_sql, headers=headers, verify=True)
+    if response.status_code != 200:
+        raise MorphApiError(response.text)
+    response_body = response.json()
 
-    request = {
-        "sql": sql
+    if response_body["cellType"] != "sql":
+        raise MorphApiError(f"Cell {reference} is not a SQL cell")
+
+    sql = response_body["code"]
+    connection_slug = None
+    if response_body["connectionType"] == "external":
+        connection_slug = response_body["connectionSlug"]
+    return {
+        "sql": sql,
+        "connection_slug": connection_slug
     }
-    if connection_slug is not None:
-        request["connectionSlug"] = connection_slug
 
-    response = requests.post(url_sql, headers=headers, json=request, verify=True)
-    if response.status_code != 200:
-        raise MorphApiError(response.text)
 
-    try:
-        response_body = response.json()
-        structured_response_body = SqlResultResponse(
-            headers=response_body["headers"], rows=response_body["rows"]
-        )
-        df = _convert_sql_engine_response(structured_response_body)
-        return df
-    except Exception as e:
-        raise MorphApiError(f"{e}")
+def execute_sql(*args, **kwargs) -> pd.DataFrame:
+    if args and isinstance(args[0], dict):
+        ref_dict = args[0]
+        return _execute_sql_impl(**ref_dict, **kwargs)
+    else:
+        return _execute_sql_impl(*args, **kwargs)
```

### Comparing `morphdb_utils-0.1.8/morphdb_utils/type.py` & `morphdb_utils-0.1.9/morphdb_utils/type.py`

 * *Files identical despite different names*

### Comparing `morphdb_utils-0.1.8/pyproject.toml` & `morphdb_utils-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "morphdb-utils"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["shibatanaoto <naoto.shibata510@gmail.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `morphdb_utils-0.1.8/PKG-INFO` & `morphdb_utils-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphdb-utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: shibatanaoto
 Author-email: naoto.shibata510@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

