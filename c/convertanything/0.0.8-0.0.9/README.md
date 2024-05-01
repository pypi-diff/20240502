# Comparing `tmp/convertanything-0.0.8.tar.gz` & `tmp/convertanything-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convertanything-0.0.8.tar", last modified: Wed May  1 21:54:07 2024, max compression
+gzip compressed data, was "convertanything-0.0.9.tar", last modified: Wed May  1 22:13:21 2024, max compression
```

## Comparing `convertanything-0.0.8.tar` & `convertanything-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:54:07.314558 convertanything-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 21:54:03.000000 convertanything-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-01 21:54:03.000000 convertanything-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 21:54:03.000000 convertanything-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-01 21:54:07.314558 convertanything-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-01 21:54:03.000000 convertanything-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:54:07.314558 convertanything-0.0.8/convertanything/
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-01 21:54:03.000000 convertanything-0.0.8/convertanything/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:54:07.314558 convertanything-0.0.8/convertanything.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-01 21:54:07.000000 convertanything-0.0.8/convertanything.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-01 21:54:07.000000 convertanything-0.0.8/convertanything.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:54:07.000000 convertanything-0.0.8/convertanything.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 21:54:07.000000 convertanything-0.0.8/convertanything.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 21:54:07.000000 convertanything-0.0.8/convertanything.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-01 21:54:03.000000 convertanything-0.0.8/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 21:54:03.000000 convertanything-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 21:54:03.000000 convertanything-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:54:07.314558 convertanything-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-01 21:54:03.000000 convertanything-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:13:21.270277 convertanything-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 22:13:17.000000 convertanything-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-01 22:13:17.000000 convertanything-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 22:13:17.000000 convertanything-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-01 22:13:21.270277 convertanything-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-01 22:13:17.000000 convertanything-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:13:21.266277 convertanything-0.0.9/convertanything/
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-01 22:13:17.000000 convertanything-0.0.9/convertanything/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:13:21.266277 convertanything-0.0.9/convertanything.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-01 22:13:21.000000 convertanything-0.0.9/convertanything.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-01 22:13:21.000000 convertanything-0.0.9/convertanything.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:13:21.000000 convertanything-0.0.9/convertanything.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 22:13:21.000000 convertanything-0.0.9/convertanything.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 22:13:21.000000 convertanything-0.0.9/convertanything.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-01 22:13:17.000000 convertanything-0.0.9/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 22:13:17.000000 convertanything-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 22:13:17.000000 convertanything-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 22:13:21.270277 convertanything-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-01 22:13:17.000000 convertanything-0.0.9/setup.py
```

### Comparing `convertanything-0.0.8/LICENSE` & `convertanything-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `convertanything-0.0.8/PKG-INFO` & `convertanything-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convertanything
-Version: 0.0.8
+Version: 0.0.9
 Summary: convertanything is a Python package that allows you to convert any text into a structured format according to the schema provided.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
```

### Comparing `convertanything-0.0.8/README.md` & `convertanything-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `convertanything-0.0.8/convertanything/__init__.py` & `convertanything-0.0.9/convertanything/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 from pydantic import BaseModel
-from typing import Type
+from typing import Type, get_args, get_origin, Union
 import json
 import openai
+from enum import Enum
 
 
 def convertanything(
     input_string: str,
     model: Type[BaseModel],
     api_key=None,
     server="https://api.openai.com",
     llm="gpt-3.5-turbo-16k",
 ):
     input_string = str(input_string)
     openai.base_url = f"{server}/v1/"
     openai.api_key = api_key if api_key else server
-    fields = model.model_fields
-    field_descriptions = [f"{field}: {fields[field]}" for field in fields]
+    fields = model.__annotations__
+    field_descriptions = []
+    for field, field_type in fields.items():
+        description = f"{field}: {field_type}"
+        if get_origin(field_type) == Union:
+            field_type = get_args(field_type)[0]
+        if isinstance(field_type, type) and issubclass(field_type, Enum):
+            enum_values = ", ".join([f"{e.name} = {e.value}" for e in field_type])
+            description += f" (Enum values: {enum_values})"
+        field_descriptions.append(description)
     schema = "\n".join(field_descriptions)
     prompt = f"""Act as a JSON converter that converts any text into the desired JSON format based on the schema provided. Respond only with JSON in a properly formatted markdown code block, no explanations.
 **Reformat the following information into a structured format according to the schema provided:**
 
 ## Information:
 {input_string}
```

### Comparing `convertanything-0.0.8/convertanything.egg-info/PKG-INFO` & `convertanything-0.0.9/convertanything.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convertanything
-Version: 0.0.8
+Version: 0.0.9
 Summary: convertanything is a Python package that allows you to convert any text into a structured format according to the schema provided.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
```

### Comparing `convertanything-0.0.8/example.ipynb` & `convertanything-0.0.9/example.ipynb`

 * *Files identical despite different names*

### Comparing `convertanything-0.0.8/setup.py` & `convertanything-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = f.read()
 
 with open(os.path.join(this_directory, "requirements.txt")) as f:
     requirements = f.read().splitlines()
 
 setup(
     name="convertanything",
-    version="0.0.8",
+    version="0.0.9",
     description="convertanything is a Python package that allows you to convert any text into a structured format according to the schema provided.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     packages=find_packages(),
     python_requires=">=3.10",
```

