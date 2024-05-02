# Comparing `tmp/pydantic_glue-0.1.0.tar.gz` & `tmp/pydantic_glue-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_glue-0.1.0.tar", max compression
+gzip compressed data, was "pydantic_glue-0.2.0.tar", max compression
```

## Comparing `pydantic_glue-0.1.0.tar` & `pydantic_glue-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2024-04-30 20:01:37.691496 pydantic_glue-0.1.0/LICENSE
--rw-r--r--   0        0        0     2564 2024-04-30 20:01:37.691496 pydantic_glue-0.1.0/README.md
--rw-r--r--   0        0        0       65 2024-04-30 20:01:37.691496 pydantic_glue-0.1.0/pydantic_glue/__init__.py
--rw-r--r--   0        0        0      761 2024-04-30 20:01:37.691496 pydantic_glue-0.1.0/pydantic_glue/cli.py
--rw-r--r--   0        0        0     1473 2024-04-30 20:01:37.691496 pydantic_glue-0.1.0/pydantic_glue/handler.py
--rw-r--r--   0        0        0     1294 2024-04-30 20:01:37.691496 pydantic_glue-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 pydantic_glue-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-02 08:45:19.300822 pydantic_glue-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2574 2024-05-02 08:45:19.300822 pydantic_glue-0.2.0/README.md
+-rw-r--r--   0        0        0       65 2024-05-02 08:45:19.300822 pydantic_glue-0.2.0/pydantic_glue/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-02 08:45:19.300822 pydantic_glue-0.2.0/pydantic_glue/cli.py
+-rw-r--r--   0        0        0     1556 2024-05-02 08:45:19.300822 pydantic_glue-0.2.0/pydantic_glue/handler.py
+-rw-r--r--   0        0        0     1294 2024-05-02 08:45:19.300822 pydantic_glue-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 pydantic_glue-0.2.0/PKG-INFO
```

### Comparing `pydantic_glue-0.1.0/LICENSE` & `pydantic_glue-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_glue-0.1.0/README.md` & `pydantic_glue-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 pydantic-glue example.py Foo
 ```
 
 you get this JSON
 
 ```json
 {
-  "//": "Generated by j2g at 2022-05-25 12:35:55.333570. DO NOT EDIT",
+  "//": "Generated by pydantic-glue at 2022-05-25 12:35:55.333570. DO NOT EDIT",
   "columns": {
     "nums": "array<int>",
     "bars": "array<struct<name:string,age:int>>",
     "other": "string"
   }
 }
 ```
```

### Comparing `pydantic_glue-0.1.0/pydantic_glue/cli.py` & `pydantic_glue-0.2.0/pydantic_glue/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     module_file = sys.argv[1].replace(".py", "")
     class_name = sys.argv[2]
 
     sys.path.append(os.path.dirname(module_file))
 
     imported = __import__(os.path.basename(module_file))
     imported = getattr(imported, class_name)
-    schema = imported.model_json_schema()
-    schema = convert(schema)
-    schema = {k: v for (k, v) in schema}
-    schema = {
+    input_schema = json.dumps(imported.model_json_schema())
+    converted = convert(input_schema)
+    output = {
         "//": f"Generated by pydantic-glue at {datetime.now()}. DO NOT EDIT",
-        "columns": schema,
+        "columns": {k: v for (k, v) in converted},
     }
 
-    print(json.dumps(schema, indent=2))
+    print(json.dumps(output, indent=2))
```

### Comparing `pydantic_glue-0.1.0/pydantic_glue/handler.py` & `pydantic_glue-0.2.0/pydantic_glue/handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,16 +35,19 @@
 def handle_map(o: dict[str, Any]) -> str:
     t = o["additionalProperties"]
     res = dispatch(t)
     return f"map<{res}, {res}>"
 
 
 def handle_union(o: dict[str, Any]) -> str:
-    res = [dispatch(v) for v in o["anyOf"]]
-    return f"union<{','.join(res)}>"
+    types = [i for i in o["anyOf"] if i["type"] != "null"]
+    if len(types) > 1:
+        res = [dispatch(v) for v in types]
+        return f"union<{','.join(res)}>"
+    return dispatch(types[0])
 
 
 def map_dispatch(o: dict[str, Any]) -> list[tuple[str, str]]:
     return [(k, dispatch(v)) for k, v in o["properties"].items()]
 
 
 def handle_object(o: dict[str, Any]) -> str:
@@ -57,13 +60,11 @@
     return f"array<{t}>"
 
 
 def handle_root(o: dict[str, Any]) -> list[tuple[str, str]]:
     return map_dispatch(o)
 
 
-def convert(schema: dict[str, Any]) -> Union[list[Any], list[tuple[str, str]]]:
+def convert(schema: str) -> Union[list[Any], list[tuple[str, str]]]:
     if not schema:
         return []
-
-    schema = jsonref.loads(schema)
-    return handle_root(schema)
+    return handle_root(jsonref.loads(schema))
```

### Comparing `pydantic_glue-0.1.0/pyproject.toml` & `pydantic_glue-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-glue"
-version = "0.1.0"
+version = "0.2.0"
 description = "Convert pydantic model to aws glue schema for terraform"
 authors = ["Serhii Dimchenko <svdimchenko@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 pydantic-glue = "pydantic_glue.cli:cli"
```

### Comparing `pydantic_glue-0.1.0/PKG-INFO` & `pydantic_glue-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-glue
-Version: 0.1.0
+Version: 0.2.0
 Summary: Convert pydantic model to aws glue schema for terraform
 Author: Serhii Dimchenko
 Author-email: svdimchenko@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -70,15 +70,15 @@
 pydantic-glue example.py Foo
 ```
 
 you get this JSON
 
 ```json
 {
-  "//": "Generated by j2g at 2022-05-25 12:35:55.333570. DO NOT EDIT",
+  "//": "Generated by pydantic-glue at 2022-05-25 12:35:55.333570. DO NOT EDIT",
   "columns": {
     "nums": "array<int>",
     "bars": "array<struct<name:string,age:int>>",
     "other": "string"
   }
 }
 ```
```
