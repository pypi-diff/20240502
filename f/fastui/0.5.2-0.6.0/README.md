# Comparing `tmp/fastui-0.5.2.tar.gz` & `tmp/fastui-0.6.0.tar.gz`

## Comparing `fastui-0.5.2.tar` & `fastui-0.6.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/__init__.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/__main__.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/class_name.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/dev.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/events.py
--rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/forms.py
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/generate_typescript.py
--rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/json_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/py.typed
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/types.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/auth/__init__.py
--rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/auth/github.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/auth/shared.py
--rw-r--r--   0        0        0    10674 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/components/__init__.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/components/display.py
--rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/components/forms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/components/py.typed
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 fastui-0.5.2/fastui/components/tables.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fastui-0.5.2/requirements/all.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fastui-0.5.2/requirements/lint.in
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 fastui-0.5.2/requirements/lint.txt
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 fastui-0.5.2/requirements/pyproject.txt
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 fastui-0.5.2/requirements/render.txt
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 fastui-0.5.2/requirements/test.in
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 fastui-0.5.2/requirements/test.txt
--rw-r--r--   0        0        0    10399 2020-02-02 00:00:00.000000 fastui-0.5.2/tests/test_auth_github.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 fastui-0.5.2/tests/test_auth_shared.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 fastui-0.5.2/tests/test_components.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 fastui-0.5.2/tests/test_dev.py
--rw-r--r--   0        0        0    14360 2020-02-02 00:00:00.000000 fastui-0.5.2/tests/test_forms.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 fastui-0.5.2/tests/test_json_schema.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 fastui-0.5.2/tests/test_prebuilt_html.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 fastui-0.5.2/tests/test_tables_display.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 fastui-0.5.2/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 fastui-0.5.2/LICENSE
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 fastui-0.5.2/README.md
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 fastui-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 fastui-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/__init__.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/__main__.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/base.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/class_name.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/dev.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/events.py
+-rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/forms.py
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/generate_typescript.py
+-rw-r--r--   0        0        0    13109 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/json_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/py.typed
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/types.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/auth/__init__.py
+-rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/auth/github.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/auth/shared.py
+-rw-r--r--   0        0        0    19133 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/components/__init__.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/components/display.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/components/forms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/components/py.typed
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 fastui-0.6.0/fastui/components/tables.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fastui-0.6.0/requirements/all.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fastui-0.6.0/requirements/lint.in
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 fastui-0.6.0/requirements/lint.txt
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 fastui-0.6.0/requirements/pyproject.txt
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 fastui-0.6.0/requirements/render.txt
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 fastui-0.6.0/requirements/test.in
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 fastui-0.6.0/requirements/test.txt
+-rw-r--r--   0        0        0    10399 2020-02-02 00:00:00.000000 fastui-0.6.0/tests/test_auth_github.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 fastui-0.6.0/tests/test_auth_shared.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 fastui-0.6.0/tests/test_components.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 fastui-0.6.0/tests/test_dev.py
+-rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 fastui-0.6.0/tests/test_forms.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 fastui-0.6.0/tests/test_json_schema.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 fastui-0.6.0/tests/test_prebuilt_html.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 fastui-0.6.0/tests/test_tables_display.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 fastui-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 fastui-0.6.0/LICENSE
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 fastui-0.6.0/README.md
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 fastui-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 fastui-0.6.0/PKG-INFO
```

### Comparing `fastui-0.5.2/fastui/__init__.py` & `fastui-0.6.0/fastui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as _t
 
 import pydantic
 
 from .components import AnyComponent
 
-__version__ = '0.5.2'
+__version__ = '0.6.0'
 __all__ = 'AnyComponent', 'FastUI', 'prebuilt_html'
 
 
 class FastUI(pydantic.RootModel):
     """
     The root component of a FastUI application.
     """
@@ -19,15 +19,15 @@
     def coerce_to_list(cls, v):
         if isinstance(v, list):
             return v
         else:
             return [v]
 
 
-_PREBUILT_VERSION = '0.0.22'
+_PREBUILT_VERSION = '0.0.23'
 _PREBUILT_CDN_URL = f'https://cdn.jsdelivr.net/npm/@pydantic/fastui-prebuilt@{_PREBUILT_VERSION}/dist/assets'
 
 
 def prebuilt_html(
     *,
     title: str = '',
     api_root_url: _t.Union[str, None] = None,
```

### Comparing `fastui-0.5.2/fastui/__main__.py` & `fastui-0.6.0/fastui/__main__.py`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/fastui/class_name.py` & `fastui-0.6.0/fastui/class_name.py`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/fastui/dev.py` & `fastui-0.6.0/fastui/dev.py`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/fastui/events.py` & `fastui-0.6.0/fastui/events.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import Dict, Literal, Union
 
-from pydantic import BaseModel, Field
+from pydantic import Field
 from typing_extensions import Annotated, TypeAliasType
 
+from .base import BaseModel
+
 ContextType = TypeAliasType('ContextType', Dict[str, Union[str, int]])
 
 
 class PageEvent(BaseModel):
     name: str
-    push_path: Union[str, None] = Field(default=None, serialization_alias='pushPath')
+    push_path: Union[str, None] = None
     context: Union[ContextType, None] = None
     clear: Union[bool, None] = None
-    next_event: 'Union[AnyEvent, None]' = Field(default=None, serialization_alias='nextEvent')
+    next_event: 'Union[AnyEvent, None]' = None
     type: Literal['page'] = 'page'
 
 
 class GoToEvent(BaseModel):
     # can be a path or a full URL
     url: Union[str, None] = None
     query: Union[Dict[str, Union[str, float, None]], None] = None
```

### Comparing `fastui-0.5.2/fastui/forms.py` & `fastui-0.6.0/fastui/forms.py`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/fastui/generate_typescript.py` & `fastui-0.6.0/fastui/generate_typescript.py`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/fastui/json_schema.py` & `fastui-0.6.0/fastui/json_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 
 def json_schema_array_to_fields(
     schema: JsonSchemaArray, loc: SchemeLocation, title: _t.List[str], required: bool, defs: JsonSchemaDefs
 ) -> _t.Iterable[FormField]:
     items_schema = schema.get('items')
     if items_schema:
         items_schema, required = deference_json_schema(items_schema, defs, required)
-        for field_name in 'search_url', 'placeholder':
+        for field_name in 'search_url', 'placeholder', 'description':
             if value := schema.get(field_name):
                 items_schema[field_name] = value  # type: ignore
         if field := special_string_field(items_schema, loc_to_name(loc), title, required, True):
             yield field
             return
 
     # for fixed length tuples (min_items == max_items), where all items are required,
@@ -308,15 +308,15 @@
     """
     if ref := schema.get('$ref'):
         defs = defs or {}
         def_schema = defs[ref.rsplit('/')[-1]]
         if def_schema is None:
             raise ValueError(f'Invalid $ref "{ref}", not found in {defs}')
         else:
-            return def_schema, required
+            return def_schema.copy(), required  # clone dict to avoid attribute leakage via shared schema.
     elif any_of := schema.get('anyOf'):
         if len(any_of) == 2 and sum(s.get('type') == 'null' for s in any_of) == 1:
             # If anyOf is a single type and null, then it is optional
             not_null_schema = next(s for s in any_of if s.get('type') != 'null')
 
             # copy everything except `anyOf` across to the new schema
             # TODO is this right?
```

### Comparing `fastui-0.5.2/fastui/types.py` & `fastui-0.6.0/fastui/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typing as _t
 
 import pydantic
 import typing_extensions as _te
 from pydantic_core import core_schema
 
 
+# TODO: replace with https://docs.pydantic.dev/dev/api/types/#pydantic.types.JsonValue, maybe?
 class JsonDataSchema:
     @staticmethod
     def __get_pydantic_json_schema__(
         _core_schema: core_schema.CoreSchema, handler: pydantic.GetJsonSchemaHandler
     ) -> _t.Any:
         json_data_schema = core_schema.union_schema(
             [
```

### Comparing `fastui-0.5.2/fastui/auth/github.py` & `fastui-0.6.0/fastui/auth/github.py`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/fastui/auth/shared.py` & `fastui-0.6.0/fastui/auth/shared.py`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/fastui/components/display.py` & `fastui-0.6.0/fastui/components/display.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,62 +6,80 @@
 import pydantic
 import typing_extensions as _te
 from pydantic_core import core_schema as _core_schema
 
 from .. import class_name as _class_name
 from .. import events
 from .. import types as _types
+from ..base import BaseModel
 
 __all__ = 'DisplayMode', 'DisplayLookup', 'Display', 'Details'
 
 
 class DisplayMode(str, enum.Enum):
+    """Display mode for a value."""
+
     auto = 'auto'  # default, same as None below
     plain = 'plain'
     datetime = 'datetime'
     date = 'date'
     duration = 'duration'
     as_title = 'as_title'
     markdown = 'markdown'
     json = 'json'
     inline_code = 'inline_code'
 
 
-class DisplayBase(pydantic.BaseModel, ABC, defer_build=True):
+class DisplayBase(BaseModel, ABC, defer_build=True):
+    """Base class for display components."""
+
     mode: _t.Union[DisplayMode, None] = None
+    """Display mode for the value."""
+
     title: _t.Union[str, None] = None
-    on_click: _t.Union[events.AnyEvent, None] = pydantic.Field(default=None, serialization_alias='onClick')
+    """Title to display for the value."""
+
+    on_click: _t.Union[events.AnyEvent, None] = None
+    """Event to trigger when the value is clicked."""
 
 
 class DisplayLookup(DisplayBase, extra='forbid'):
-    """
-    Description of how to display a value looked up from data, either in a table or detail view.
-    """
+    """Description of how to display a value looked up from data, either in a table or detail view."""
 
     field: str
-    # percentage width - 0 to 100, specific to tables
-    table_width_percent: _t.Union[_te.Annotated[int, _at.Interval(ge=0, le=100)], None] = pydantic.Field(
-        default=None, serialization_alias='tableWidthPercent'
-    )
+    """Field to display."""
+
+    table_width_percent: _t.Union[_te.Annotated[int, _at.Interval(ge=0, le=100)], None] = None
+    """Percentage width - 0 to 100, specific to tables."""
 
 
 class Display(DisplayBase, extra='forbid'):
-    """
-    Description of how to display a value, either in a table or detail view.
-    """
+    """Description of how to display a value, either in a table or detail view."""
 
     value: _types.JsonData
+    """Value to display."""
+
     type: _t.Literal['Display'] = 'Display'
+    """The type of the component. Always 'Display'."""
+
 
+class Details(BaseModel, extra='forbid'):
+    """Details associated with displaying a data model."""
 
-class Details(pydantic.BaseModel, extra='forbid'):
     data: pydantic.SerializeAsAny[_types.DataModel]
+    """Data model to display."""
+
     fields: _t.Union[_t.List[DisplayLookup], None] = None
+    """Fields to display."""
+
     class_name: _class_name.ClassNameField = None
+    """Optional class name to apply to the details component."""
+
     type: _t.Literal['Details'] = 'Details'
+    """The type of the component. Always 'Details'."""
 
     @pydantic.model_validator(mode='after')
     def _fill_fields(self) -> _te.Self:
         if self.fields is None:
             self.fields = [
                 DisplayLookup(field=name, title=field.title) for name, field in self.data.model_fields.items()
             ]
```

### Comparing `fastui-0.5.2/fastui/components/tables.py` & `fastui-0.6.0/fastui/components/tables.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,26 +2,40 @@
 
 import pydantic
 import typing_extensions as _te
 from pydantic_core import core_schema as _core_schema
 
 from .. import class_name as _class_name
 from .. import types as _types
+from ..base import BaseModel
 from . import display
 
 # TODO allow dataclasses and typed dicts here too
 
 
-class Table(pydantic.BaseModel, extra='forbid'):
+class Table(BaseModel, extra='forbid'):
+    """Table component."""
+
     data: _t.Sequence[pydantic.SerializeAsAny[_types.DataModel]]
+    """Sequence of data models to display in the table."""
+
     columns: _t.Union[_t.List[display.DisplayLookup], None] = None
+    """List of columns to display in the table. If not provided, columns will be inferred from the data model."""
+
     data_model: _t.Union[_t.Type[pydantic.BaseModel], None] = pydantic.Field(default=None, exclude=True)
-    no_data_message: _t.Union[str, None] = pydantic.Field(default=None, serialization_alias='noDataMessage')
+    """Data model to use for the table. If not provided, the model will be inferred from the first data item."""
+
+    no_data_message: _t.Union[str, None] = None
+    """Message to display when there is no data."""
+
     class_name: _class_name.ClassNameField = None
+    """Optional class name to apply to the paragraph's HTML component."""
+
     type: _t.Literal['Table'] = 'Table'
+    """The type of the component. Always 'Table'."""
 
     @pydantic.model_validator(mode='after')
     def _fill_columns(self) -> _te.Self:
         if self.data_model:
             data_model_type = self.data_model
         else:
             try:
@@ -49,17 +63,31 @@
         json_schema = handler(core_schema)
         schema_def = handler.resolve_ref_schema(json_schema)
         # columns are filled by `_fill_columns`
         schema_def['required'].append('columns')
         return json_schema
 
 
-class Pagination(pydantic.BaseModel):
+class Pagination(BaseModel):
+    """Pagination component to use with tables."""
+
     page: int
-    page_size: int = pydantic.Field(serialization_alias='pageSize')
+    """The current page number."""
+
+    page_size: int
+    """The number of items per page."""
+
     total: int
+    """The total number of items."""
+
+    page_query_param: str = 'page'
+    """The query parameter to use for the page number."""
+
     class_name: _class_name.ClassNameField = None
+    """Optional class name to apply to the pagination's HTML component."""
+
     type: _t.Literal['Pagination'] = 'Pagination'
+    """The type of the component. Always 'Pagination'."""
 
     @pydantic.computed_field(alias='pageCount')
     def page_count(self) -> int:
         return (self.total - 1) // self.page_size + 1
```

### Comparing `fastui-0.5.2/requirements/pyproject.txt` & `fastui-0.6.0/requirements/pyproject.txt`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/requirements/test.txt` & `fastui-0.6.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/tests/test_auth_github.py` & `fastui-0.6.0/tests/test_auth_github.py`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/tests/test_auth_shared.py` & `fastui-0.6.0/tests/test_auth_shared.py`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/tests/test_components.py` & `fastui-0.6.0/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/tests/test_dev.py` & `fastui-0.6.0/tests/test_dev.py`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/tests/test_forms.py` & `fastui-0.6.0/tests/test_forms.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import enum
 from contextlib import asynccontextmanager
 from io import BytesIO
 from typing import List, Tuple, Union
 
 import pytest
 from fastapi import HTTPException
 from fastui import components
 from fastui.forms import FormFile, Textarea, fastui_form
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from starlette.datastructures import FormData, Headers, UploadFile
 from typing_extensions import Annotated
 
 
 class SimpleForm(BaseModel):
     name: str
     size: int = 4
@@ -465,7 +466,59 @@
                 'title': ['Text'],
                 'required': True,
                 'locked': False,
                 'type': 'FormFieldTextarea',
             }
         ],
     }
+
+
+class SelectEnum(str, enum.Enum):
+    one = 'one'
+    two = 'two'
+
+
+class FormSelectMultiple(BaseModel):
+    select_single: SelectEnum = Field(title='Select Single', description='first field')
+    select_single_2: SelectEnum = Field(title='Select Single')  # unset description to test leakage from prev. field
+    select_multiple: List[SelectEnum] = Field(title='Select Multiple', description='third field')
+
+
+def test_form_description_leakage():
+    m = components.ModelForm(model=FormSelectMultiple, submit_url='/foobar/')
+
+    assert m.model_dump(by_alias=True, exclude_none=True) == {
+        'formFields': [
+            {
+                'description': 'first field',
+                'locked': False,
+                'multiple': False,
+                'name': 'select_single',
+                'options': [{'label': 'One', 'value': 'one'}, {'label': 'Two', 'value': 'two'}],
+                'required': True,
+                'title': ['Select Single'],
+                'type': 'FormFieldSelect',
+            },
+            {
+                'locked': False,
+                'multiple': False,
+                'name': 'select_single_2',
+                'options': [{'label': 'One', 'value': 'one'}, {'label': 'Two', 'value': 'two'}],
+                'required': True,
+                'title': ['Select Single'],
+                'type': 'FormFieldSelect',
+            },
+            {
+                'description': 'third field',
+                'locked': False,
+                'multiple': True,
+                'name': 'select_multiple',
+                'options': [{'label': 'One', 'value': 'one'}, {'label': 'Two', 'value': 'two'}],
+                'required': True,
+                'title': ['Select Multiple'],
+                'type': 'FormFieldSelect',
+            },
+        ],
+        'method': 'POST',
+        'submitUrl': '/foobar/',
+        'type': 'ModelForm',
+    }
```

### Comparing `fastui-0.5.2/tests/test_json_schema.py` & `fastui-0.6.0/tests/test_json_schema.py`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/tests/test_prebuilt_html.py` & `fastui-0.6.0/tests/test_prebuilt_html.py`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/tests/test_tables_display.py` & `fastui-0.6.0/tests/test_tables_display.py`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/LICENSE` & `fastui-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/pyproject.toml` & `fastui-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastui-0.5.2/PKG-INFO` & `fastui-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fastui
-Version: 0.5.2
+Version: 0.6.0
 Summary: Build better UIs faster.
 Project-URL: Homepage, https://github.com/pydantic/FastUI
 Author-email: Samuel Colvin <s@muelcolvin.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: FastAPI
```

