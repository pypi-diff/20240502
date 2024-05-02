# Comparing `tmp/fastapi_code_generator-0.4.4.tar.gz` & `tmp/fastapi_code_generator-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_code_generator-0.4.4.tar", max compression
+gzip compressed data, was "fastapi_code_generator-0.5.0.tar", max compression
```

## Comparing `fastapi_code_generator-0.4.4.tar` & `fastapi_code_generator-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1068 2023-09-07 16:22:07.402356 fastapi_code_generator-0.4.4/LICENSE
--rw-r--r--   0        0        0    21202 2023-09-07 16:22:07.402356 fastapi_code_generator-0.4.4/README.md
--rw-r--r--   0        0        0        0 2023-09-07 16:22:07.402356 fastapi_code_generator-0.4.4/fastapi_code_generator/__init__.py
--rw-r--r--   0        0        0     9136 2023-09-07 16:22:07.402356 fastapi_code_generator-0.4.4/fastapi_code_generator/__main__.py
--rw-r--r--   0        0        0       11 2023-09-07 16:22:07.402356 fastapi_code_generator-0.4.4/fastapi_code_generator/modular_template/dependencies.jinja2
--rw-r--r--   0        0        0      461 2023-09-07 16:22:07.402356 fastapi_code_generator-0.4.4/fastapi_code_generator/modular_template/main.jinja2
--rw-r--r--   0        0        0     1064 2023-09-07 16:22:07.402356 fastapi_code_generator-0.4.4/fastapi_code_generator/modular_template/routers.jinja2
--rw-r--r--   0        0        0    17645 2023-09-07 16:22:07.402356 fastapi_code_generator-0.4.4/fastapi_code_generator/parser.py
--rw-r--r--   0        0        0     1128 2023-09-07 16:22:07.402356 fastapi_code_generator-0.4.4/fastapi_code_generator/template/main.jinja2
--rw-r--r--   0        0        0      178 2023-09-07 16:22:07.402356 fastapi_code_generator-0.4.4/fastapi_code_generator/visitor.py
--rw-r--r--   0        0        0     1232 2023-09-07 16:22:07.402356 fastapi_code_generator-0.4.4/fastapi_code_generator/visitors/imports.py
--rw-r--r--   0        0        0      449 2023-09-07 16:22:07.402356 fastapi_code_generator-0.4.4/fastapi_code_generator/visitors/operations.py
--rw-r--r--   0        0        0     2199 2023-09-07 16:22:49.139078 fastapi_code_generator-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    22469 1970-01-01 00:00:00.000000 fastapi_code_generator-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-02 15:42:23.282862 fastapi_code_generator-0.5.0/LICENSE
+-rw-r--r--   0        0        0    21202 2024-05-02 15:42:23.282862 fastapi_code_generator-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 15:42:23.282862 fastapi_code_generator-0.5.0/fastapi_code_generator/__init__.py
+-rw-r--r--   0        0        0     9188 2024-05-02 15:42:23.282862 fastapi_code_generator-0.5.0/fastapi_code_generator/__main__.py
+-rw-r--r--   0        0        0       11 2024-05-02 15:42:23.282862 fastapi_code_generator-0.5.0/fastapi_code_generator/modular_template/dependencies.jinja2
+-rw-r--r--   0        0        0      461 2024-05-02 15:42:23.282862 fastapi_code_generator-0.5.0/fastapi_code_generator/modular_template/main.jinja2
+-rw-r--r--   0        0        0     1064 2024-05-02 15:42:23.282862 fastapi_code_generator-0.5.0/fastapi_code_generator/modular_template/routers.jinja2
+-rw-r--r--   0        0        0    19145 2024-05-02 15:42:23.282862 fastapi_code_generator-0.5.0/fastapi_code_generator/parser.py
+-rw-r--r--   0        0        0     1128 2024-05-02 15:42:23.282862 fastapi_code_generator-0.5.0/fastapi_code_generator/template/main.jinja2
+-rw-r--r--   0        0        0      178 2024-05-02 15:42:23.282862 fastapi_code_generator-0.5.0/fastapi_code_generator/visitor.py
+-rw-r--r--   0        0        0     1232 2024-05-02 15:42:23.282862 fastapi_code_generator-0.5.0/fastapi_code_generator/visitors/imports.py
+-rw-r--r--   0        0        0      449 2024-05-02 15:42:23.282862 fastapi_code_generator-0.5.0/fastapi_code_generator/visitors/operations.py
+-rw-r--r--   0        0        0     2199 2024-05-02 15:42:39.618909 fastapi_code_generator-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    22516 1970-01-01 00:00:00.000000 fastapi_code_generator-0.5.0/PKG-INFO
```

### Comparing `fastapi_code_generator-0.4.4/LICENSE` & `fastapi_code_generator-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_code_generator-0.4.4/README.md` & `fastapi_code_generator-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_code_generator-0.4.4/fastapi_code_generator/__main__.py` & `fastapi_code_generator-0.5.0/fastapi_code_generator/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         return generate_code(
             input_name,
             input_text,
             encoding,
             output_dir,
             template_dir,
             model_path,
-            enum_field_as_literal,
+            enum_field_as_literal,  # type: ignore[arg-type]
             custom_visitors=custom_visitors,
             disable_timestamp=disable_timestamp,
             generate_routers=generate_routers,
             specify_tags=specify_tags,
         )
     return generate_code(
         input_name,
@@ -127,15 +127,15 @@
     if generate_routers:
         Path(output_dir / "routers").mkdir(parents=True, exist_ok=True)
     if not template_dir:
         template_dir = (
             BUILTIN_MODULAR_TEMPLATE_DIR if generate_routers else BUILTIN_TEMPLATE_DIR
         )
     if enum_field_as_literal:
-        parser = OpenAPIParser(input_text, enum_field_as_literal=enum_field_as_literal)
+        parser = OpenAPIParser(input_text, enum_field_as_literal=enum_field_as_literal)  # type: ignore[arg-type]
     else:
         parser = OpenAPIParser(input_text)
     with chdir(output_dir):
         models = parser.parse()
     output = output_dir / model_path
     if not models:
         # if no models (schemas), just generate an empty model file.
```

### Comparing `fastapi_code_generator-0.4.4/fastapi_code_generator/modular_template/routers.jinja2` & `fastapi_code_generator-0.5.0/fastapi_code_generator/modular_template/routers.jinja2`

 * *Files identical despite different names*

### Comparing `fastapi_code_generator-0.4.4/fastapi_code_generator/parser.py` & `fastapi_code_generator-0.5.0/fastapi_code_generator/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,33 +21,33 @@
 
 import stringcase
 from datamodel_code_generator import (
     DefaultPutDict,
     LiteralType,
     OpenAPIScope,
     PythonVersion,
-    cached_property,
     snooper_to_methods,
 )
 from datamodel_code_generator.imports import Import, Imports
 from datamodel_code_generator.model import DataModel, DataModelFieldBase
 from datamodel_code_generator.model import pydantic as pydantic_model
-from datamodel_code_generator.model.pydantic import DataModelField
+from datamodel_code_generator.model.pydantic import CustomRootType, DataModelField
 from datamodel_code_generator.parser.jsonschema import JsonSchemaObject
 from datamodel_code_generator.parser.openapi import MediaObject
 from datamodel_code_generator.parser.openapi import OpenAPIParser as OpenAPIModelParser
 from datamodel_code_generator.parser.openapi import (
     ParameterLocation,
     ParameterObject,
     ReferenceObject,
     RequestBodyObject,
     ResponseObject,
 )
 from datamodel_code_generator.types import DataType, DataTypeManager, StrictTypes
-from pydantic import BaseModel
+from datamodel_code_generator.util import cached_property
+from pydantic import BaseModel, ValidationInfo
 
 RE_APPLICATION_JSON_PATTERN: Pattern[str] = re.compile(r'^application/.*json$')
 
 
 class CachedPropertyModel(BaseModel):
     class Config:
         arbitrary_types_allowed = True
@@ -68,15 +68,15 @@
 
 class UsefulStr(str):
     @classmethod
     def __get_validators__(cls) -> Any:
         yield cls.validate
 
     @classmethod
-    def validate(cls, v: Any) -> Any:
+    def validate(cls, v: Any, info: ValidationInfo) -> Any:
         return cls(v)
 
     @property
     def snakecase(self) -> str:
         return stringcase.snakecase(self)
 
     @property
@@ -87,16 +87,16 @@
     def camelcase(self) -> str:
         return stringcase.camelcase(self)
 
 
 class Argument(CachedPropertyModel):
     name: UsefulStr
     type_hint: UsefulStr
-    default: Optional[UsefulStr]
-    default_value: Optional[UsefulStr]
+    default: Optional[UsefulStr] = None
+    default_value: Optional[UsefulStr] = None
     required: bool
 
     def __str__(self) -> str:
         return self.argument
 
     @cached_property
     def argument(self) -> str:
@@ -104,28 +104,28 @@
             return f'{self.name}: {self.type_hint}'
         return f'{self.name}: {self.type_hint} = {self.default}'
 
 
 class Operation(CachedPropertyModel):
     method: UsefulStr
     path: UsefulStr
-    operationId: Optional[UsefulStr]
-    description: Optional[str]
-    summary: Optional[str]
+    operationId: Optional[UsefulStr] = None
+    description: Optional[str] = None
+    summary: Optional[str] = None
     parameters: List[Dict[str, Any]] = []
     responses: Dict[UsefulStr, Any] = {}
     deprecated: bool = False
     imports: List[Import] = []
     security: Optional[List[Dict[str, List[str]]]] = None
-    tags: Optional[List[str]]
+    tags: Optional[List[str]] = []
     arguments: str = ''
     snake_case_arguments: str = ''
     request: Optional[Argument] = None
     response: str = ''
-    additional_responses: Dict[str, Dict[str, str]] = {}
+    additional_responses: Dict[Union[str, int], Dict[str, str]] = {}
     return_type: str = ''
 
     @cached_property
     def type(self) -> UsefulStr:
         """
         backwards compatibility
         """
@@ -241,24 +241,30 @@
     def parse_info(self) -> Optional[Dict[str, Any]]:
         result = self.raw_obj.get('info', {}).copy()
         servers = self.raw_obj.get('servers')
         if servers:
             result['servers'] = servers
         return result or None
 
-    def parse_parameters(self, parameters: ParameterObject, path: List[str]) -> None:
-        super().parse_parameters(parameters, path)
-        self._temporary_operation['_parameters'].append(parameters)
+    def parse_all_parameters(
+        self,
+        name: str,
+        parameters: List[Union[ReferenceObject, ParameterObject]],
+        path: List[str],
+    ) -> None:
+        super().parse_all_parameters(name, parameters, path)
+        self._temporary_operation['_parameters'].extend(parameters)
 
     def get_parameter_type(
         self,
-        parameters: ParameterObject,
+        parameters: Union[ReferenceObject, ParameterObject],
         snake_case: bool,
         path: List[str],
     ) -> Optional[Argument]:
+        parameters = self.resolve_object(parameters, ParameterObject)
         orig_name = parameters.name
         if snake_case:
             name = stringcase.snakecase(parameters.name)
         else:
             name = parameters.name
 
         schema: Optional[JsonSchemaObject] = None
@@ -270,15 +276,18 @@
                 schema = JsonSchemaObject.parse_obj(ref_model)
             else:
                 schema = content.schema_
             break
         if not data_type:
             if not schema:
                 schema = parameters.schema_
+            if schema is None:
+                raise RuntimeError("schema is None")  # pragma: no cover
             data_type = self.parse_schema(name, schema, [*path, name])
+            data_type = self._collapse_root_model(data_type)
         if not schema:
             return None
 
         field = DataModelField(
             name=name,
             data_type=data_type,
             required=parameters.required or parameters.in_ == ParameterLocation.path,
@@ -286,24 +295,26 @@
 
         if orig_name != name:
             if parameters.in_:
                 param_is = parameters.in_.value.lower().capitalize()
                 self.imports_for_fastapi.append(
                     Import(from_='fastapi', import_=param_is)
                 )
-                default: Optional[
-                    str
-                ] = f"{param_is}({'...' if field.required else repr(schema.default)}, alias='{orig_name}')"
+                default: Optional[str] = (
+                    f"{param_is}({'...' if field.required else repr(schema.default)}, alias='{orig_name}')"
+                )
         else:
             default = repr(schema.default) if schema.has_default else None
         self.imports_for_fastapi.append(field.imports)
         self.data_types.append(field.data_type)
+        if field.name is None:
+            raise RuntimeError("field.name is None")  # pragma: no cover
         return Argument(
-            name=field.name,
-            type_hint=field.type_hint,
+            name=UsefulStr(field.name),
+            type_hint=UsefulStr(field.type_hint),
             default=default,  # type: ignore
             default_value=schema.default,
             required=field.required,
         )
 
     def get_arguments(self, snake_case: bool, path: List[str]) -> str:
         return ", ".join(
@@ -357,19 +368,20 @@
                 if RE_APPLICATION_JSON_PATTERN.match(media_type):
                     if isinstance(media_obj.schema_, ReferenceObject):
                         data_type = self.get_ref_data_type(media_obj.schema_.ref)
                     else:
                         data_type = self.parse_schema(
                             name, media_obj.schema_, [*path, media_type]
                         )
+                    data_type = self._collapse_root_model(data_type)
                     arguments.append(
                         # TODO: support multiple body
                         Argument(
                             name='body',  # type: ignore
-                            type_hint=data_type.type_hint,
+                            type_hint=UsefulStr(data_type.type_hint),
                             required=request_body.required,
                         )
                     )
                     self.data_types.append(data_type)
                 elif media_type == 'application/x-www-form-urlencoded':
                     arguments.append(
                         # TODO: support form with `Form()`
@@ -402,25 +414,26 @@
                         )
                     )
                     self.imports_for_fastapi.append(
                         Import.from_full_path("fastapi.UploadFile")
                     )
         self._temporary_operation['_request'] = arguments[0] if arguments else None
 
-    def parse_responses(
+    def parse_responses(  # type: ignore[override]
         self,
         name: str,
         responses: Dict[str, Union[ResponseObject, ReferenceObject]],
         path: List[str],
-    ) -> Dict[str, Dict[str, DataType]]:
-        data_types = super().parse_responses(name, responses, path)
+    ) -> Dict[Union[str, int], Dict[str, DataType]]:
+        data_types = super().parse_responses(name, responses, path)  # type: ignore[arg-type]
         status_code_200 = data_types.get('200')
         if status_code_200:
             data_type = list(status_code_200.values())[0]
             if data_type:
+                data_type = self._collapse_root_model(data_type)
                 self.data_types.append(data_type)
         else:
             data_type = DataType(type='None')
         type_hint = data_type.type_hint  # TODO: change to lazy loading
         self._temporary_operation['response'] = type_hint
         return_types = {type_hint: data_type}
         for status_code, additional_responses in data_types.items():
@@ -462,7 +475,28 @@
 
         self.operations[resolved_path] = Operation(
             **raw_operation,
             **self._temporary_operation,
             path=f'/{path_name}',  # type: ignore
             method=method,  # type: ignore
         )
+
+    def _collapse_root_model(self, data_type: DataType) -> DataType:
+        reference = data_type.reference
+        import functools
+
+        if not (
+            reference
+            and (
+                len(reference.children) == 1
+                or functools.reduce(lambda a, b: a == b, reference.children)
+            )
+        ):
+            return data_type
+        source = reference.source
+        if not isinstance(source, CustomRootType):
+            return data_type
+        data_type.remove_reference()
+        data_type = source.fields[0].data_type
+        if source in self.results:
+            self.results.remove(source)
+        return data_type
```

### Comparing `fastapi_code_generator-0.4.4/fastapi_code_generator/template/main.jinja2` & `fastapi_code_generator-0.5.0/fastapi_code_generator/template/main.jinja2`

 * *Files identical despite different names*

### Comparing `fastapi_code_generator-0.4.4/fastapi_code_generator/visitors/imports.py` & `fastapi_code_generator-0.5.0/fastapi_code_generator/visitors/imports.py`

 * *Files identical despite different names*

### Comparing `fastapi_code_generator-0.4.4/pyproject.toml` & `fastapi_code_generator-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-code-generator"
-version = "0.4.4"
+version = "0.5.0"
 description = ""
 authors = ["Koudai Aono <koxudaxi@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/koxudaxi/fastapi-code-generator"
 repository = "https://github.com/koxudaxi/fastapi-code-generator"
 
@@ -24,37 +24,37 @@
 vcs = "git"
 pattern = "^(?P<base>\\d+\\.\\d+\\.\\d+)(-?((?P<stage>[a-zA-Z]+)\\.?(?P<revision>\\d+)?))?$"
 
 [tool.poetry.scripts]
 fastapi-codegen = "fastapi_code_generator.__main__:app"
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
+python = "^3.8.0"
 typer = {extras = ["all"], version = ">=0.2.1,<0.10.0"}
-datamodel-code-generator =  {extras = ["http"], version = "0.16.1"}
+datamodel-code-generator =  {extras = ["http"], version = "0.25.6"}
 stringcase = "^1.2.0"
 PySnooper = ">=0.4.1,<1.2.0"
 jinja2 = ">=2.11.2,<4.0.0"
-pydantic = "^1.5.1"
+pydantic = "^2.0"
 typed-ast = [
     {version = ">=1.5.0", python = ">=3.9.8"},
     {version = ">=1.4.2", python = "<3.9.8"},
 ]
 
 #mkdocs = {version = "1.1.2", optional = true}
 #mkdocs-material = {version = "5.2.3", optional = true}
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.4"
+pytest = "^8.2"
 pytest-cov = "*"
 pytest-mock = "*"
-mypy = "*"
-freezegun = "^1.2.2"
-black = "23.3.0"
-isort = "==5.11.4"
+mypy = "^1.10"
+freezegun = "^1.5"
+black = "24.4.2"
+isort = "==5.13.2"
 
 #[tool.poetry.extras]
 
 #docs = ["mkdocs", "mkdocs-material"]
 
 [tool.black]
 line-length = 88
```

### Comparing `fastapi_code_generator-0.4.4/PKG-INFO` & `fastapi_code_generator-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: fastapi-code-generator
-Version: 0.4.4
+Version: 0.5.0
 Summary: 
 Home-page: https://github.com/koxudaxi/fastapi-code-generator
 License: MIT
 Author: Koudai Aono
 Author-email: koxudaxi@gmail.com
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: PySnooper (>=0.4.1,<1.2.0)
-Requires-Dist: datamodel-code-generator[http] (==0.16.1)
+Requires-Dist: datamodel-code-generator[http] (==0.25.6)
 Requires-Dist: jinja2 (>=2.11.2,<4.0.0)
-Requires-Dist: pydantic (>=1.5.1,<2.0.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: stringcase (>=1.2.0,<2.0.0)
 Requires-Dist: typed-ast (>=1.4.2) ; python_full_version < "3.9.8"
 Requires-Dist: typed-ast (>=1.5.0) ; python_full_version >= "3.9.8"
 Requires-Dist: typer[all] (>=0.2.1,<0.10.0)
 Project-URL: Repository, https://github.com/koxudaxi/fastapi-code-generator
 Description-Content-Type: text/markdown
```

