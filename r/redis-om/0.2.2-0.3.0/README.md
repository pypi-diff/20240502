# Comparing `tmp/redis_om-0.2.2.tar.gz` & `tmp/redis_om-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_om-0.2.2.tar", max compression
+gzip compressed data, was "redis_om-0.3.0.tar", max compression
```

## Comparing `redis_om-0.2.2.tar` & `redis_om-0.3.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1071 2024-03-26 18:34:32.079290 redis_om-0.2.2/LICENSE
--rw-r--r--   0        0        0    13124 2024-03-26 18:34:32.079290 redis_om-0.2.2/README.md
--rw-r--r--   0        0        0      463 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/__init__.py
--rw-r--r--   0        0        0      806 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/_compat.py
--rw-r--r--   0        0        0       35 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/async_redis.py
--rw-r--r--   0        0        0      751 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/checks.py
--rw-r--r--   0        0        0      524 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/connections.py
--rw-r--r--   0        0        0      223 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/model/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/model/cli/__init__.py
--rw-r--r--   0        0        0      448 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/model/cli/migrate.py
--rw-r--r--   0        0        0     6513 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/model/encoders.py
--rw-r--r--   0        0        0        0 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/model/migrations/__init__.py
--rw-r--r--   0        0        0     5204 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/model/migrations/migrator.py
--rw-r--r--   0        0        0    70128 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/model/model.py
--rw-r--r--   0        0        0     2230 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/model/query_resolver.py
--rw-r--r--   0        0        0     2246 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/model/render_tree.py
--rw-r--r--   0        0        0      855 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/model/token_escaper.py
--rw-r--r--   0        0        0       13 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/sync_redis.py
--rw-r--r--   0        0        0      234 2024-03-26 18:34:32.079290 redis_om-0.2.2/aredis_om/util.py
--rw-r--r--   0        0        0     3717 2024-03-26 18:34:32.079290 redis_om-0.2.2/docs/connections.md
--rw-r--r--   0        0        0     6704 2024-03-26 18:34:32.079290 redis_om-0.2.2/docs/errors.md
--rw-r--r--   0        0        0     7510 2024-03-26 18:34:32.079290 redis_om-0.2.2/docs/fastapi_integration.md
--rw-r--r--   0        0        0    21897 2024-03-26 18:34:32.079290 redis_om-0.2.2/docs/getting_started.md
--rw-r--r--   0        0        0      973 2024-03-26 18:34:32.079290 redis_om-0.2.2/docs/index.md
--rw-r--r--   0        0        0    11595 2024-03-26 18:34:32.079290 redis_om-0.2.2/docs/models.md
--rw-r--r--   0        0        0     1674 2024-03-26 18:34:32.079290 redis_om-0.2.2/docs/redis_modules.md
--rw-r--r--   0        0        0     3688 2024-03-26 18:34:32.079290 redis_om-0.2.2/docs/validation.md
--rw-r--r--   0        0        0     3577 2024-03-26 18:34:32.079290 redis_om-0.2.2/images/logo.svg
--rw-r--r--   0        0        0     1931 2024-03-26 18:34:32.503298 redis_om-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      462 2024-03-26 18:35:20.792195 redis_om-0.2.2/redis_om/__init__.py
--rw-r--r--   0        0        0      806 2024-03-26 18:35:20.792195 redis_om-0.2.2/redis_om/_compat.py
--rw-r--r--   0        0        0       35 2024-03-26 18:35:20.792195 redis_om-0.2.2/redis_om/async_redis.py
--rw-r--r--   0        0        0      714 2024-03-26 18:35:20.792195 redis_om-0.2.2/redis_om/checks.py
--rw-r--r--   0        0        0      524 2024-03-26 18:35:20.792195 redis_om-0.2.2/redis_om/connections.py
--rw-r--r--   0        0        0      223 2024-03-26 18:35:20.796195 redis_om-0.2.2/redis_om/model/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 18:35:20.852196 redis_om-0.2.2/redis_om/model/cli/__init__.py
--rw-r--r--   0        0        0      446 2024-03-26 18:35:20.852196 redis_om-0.2.2/redis_om/model/cli/migrate.py
--rw-r--r--   0        0        0     6513 2024-03-26 18:35:20.800195 redis_om-0.2.2/redis_om/model/encoders.py
--rw-r--r--   0        0        0        0 2024-03-26 18:35:20.852196 redis_om-0.2.2/redis_om/model/migrations/__init__.py
--rw-r--r--   0        0        0     5101 2024-03-26 18:35:20.856196 redis_om-0.2.2/redis_om/model/migrations/migrator.py
--rw-r--r--   0        0        0    69803 2024-03-26 18:35:20.852196 redis_om-0.2.2/redis_om/model/model.py
--rw-r--r--   0        0        0     2229 2024-03-26 18:35:20.804195 redis_om-0.2.2/redis_om/model/query_resolver.py
--rw-r--r--   0        0        0     2246 2024-03-26 18:35:20.800195 redis_om-0.2.2/redis_om/model/render_tree.py
--rw-r--r--   0        0        0      855 2024-03-26 18:35:20.800195 redis_om-0.2.2/redis_om/model/token_escaper.py
--rw-r--r--   0        0        0       13 2024-03-26 18:35:20.792195 redis_om-0.2.2/redis_om/sync_redis.py
--rw-r--r--   0        0        0      228 2024-03-26 18:35:20.792195 redis_om-0.2.2/redis_om/util.py
--rw-r--r--   0        0        0    14677 1970-01-01 00:00:00.000000 redis_om-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-02 14:37:48.558696 redis_om-0.3.0/LICENSE
+-rw-r--r--   0        0        0    13159 2024-05-02 14:37:48.558696 redis_om-0.3.0/README.md
+-rw-r--r--   0        0        0      463 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/__init__.py
+-rw-r--r--   0        0        0     2995 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/_compat.py
+-rw-r--r--   0        0        0       35 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/async_redis.py
+-rw-r--r--   0        0        0      751 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/checks.py
+-rw-r--r--   0        0        0      524 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/connections.py
+-rw-r--r--   0        0        0      223 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/cli/__init__.py
+-rw-r--r--   0        0        0      448 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/cli/migrate.py
+-rw-r--r--   0        0        0     6544 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/encoders.py
+-rw-r--r--   0        0        0        0 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/migrations/__init__.py
+-rw-r--r--   0        0        0     5204 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/migrations/migrator.py
+-rw-r--r--   0        0        0    77675 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/model.py
+-rw-r--r--   0        0        0     2230 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/query_resolver.py
+-rw-r--r--   0        0        0     2246 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/render_tree.py
+-rw-r--r--   0        0        0      855 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/model/token_escaper.py
+-rw-r--r--   0        0        0       13 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/sync_redis.py
+-rw-r--r--   0        0        0      234 2024-05-02 14:37:48.558696 redis_om-0.3.0/aredis_om/util.py
+-rw-r--r--   0        0        0     3717 2024-05-02 14:37:48.558696 redis_om-0.3.0/docs/connections.md
+-rw-r--r--   0        0        0     6704 2024-05-02 14:37:48.558696 redis_om-0.3.0/docs/errors.md
+-rw-r--r--   0        0        0     7510 2024-05-02 14:37:48.558696 redis_om-0.3.0/docs/fastapi_integration.md
+-rw-r--r--   0        0        0    21897 2024-05-02 14:37:48.558696 redis_om-0.3.0/docs/getting_started.md
+-rw-r--r--   0        0        0      973 2024-05-02 14:37:48.558696 redis_om-0.3.0/docs/index.md
+-rw-r--r--   0        0        0    11595 2024-05-02 14:37:48.558696 redis_om-0.3.0/docs/models.md
+-rw-r--r--   0        0        0     1674 2024-05-02 14:37:48.562696 redis_om-0.3.0/docs/redis_modules.md
+-rw-r--r--   0        0        0     3688 2024-05-02 14:37:48.562696 redis_om-0.3.0/docs/validation.md
+-rw-r--r--   0        0        0     3577 2024-05-02 14:37:48.562696 redis_om-0.3.0/images/logo.svg
+-rw-r--r--   0        0        0     1931 2024-05-02 14:37:48.986699 redis_om-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      462 2024-05-02 14:38:20.770891 redis_om-0.3.0/redis_om/__init__.py
+-rw-r--r--   0        0        0     2995 2024-05-02 14:38:20.774891 redis_om-0.3.0/redis_om/_compat.py
+-rw-r--r--   0        0        0       35 2024-05-02 14:38:20.770891 redis_om-0.3.0/redis_om/async_redis.py
+-rw-r--r--   0        0        0      714 2024-05-02 14:38:20.770891 redis_om-0.3.0/redis_om/checks.py
+-rw-r--r--   0        0        0      524 2024-05-02 14:38:20.770891 redis_om-0.3.0/redis_om/connections.py
+-rw-r--r--   0        0        0      223 2024-05-02 14:38:20.782891 redis_om-0.3.0/redis_om/model/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 14:38:20.838892 redis_om-0.3.0/redis_om/model/cli/__init__.py
+-rw-r--r--   0        0        0      446 2024-05-02 14:38:20.838892 redis_om-0.3.0/redis_om/model/cli/migrate.py
+-rw-r--r--   0        0        0     6544 2024-05-02 14:38:20.778891 redis_om-0.3.0/redis_om/model/encoders.py
+-rw-r--r--   0        0        0        0 2024-05-02 14:38:20.842892 redis_om-0.3.0/redis_om/model/migrations/__init__.py
+-rw-r--r--   0        0        0     5101 2024-05-02 14:38:20.842892 redis_om-0.3.0/redis_om/model/migrations/migrator.py
+-rw-r--r--   0        0        0    77350 2024-05-02 14:38:20.834892 redis_om-0.3.0/redis_om/model/model.py
+-rw-r--r--   0        0        0     2229 2024-05-02 14:38:20.774891 redis_om-0.3.0/redis_om/model/query_resolver.py
+-rw-r--r--   0        0        0     2246 2024-05-02 14:38:20.838892 redis_om-0.3.0/redis_om/model/render_tree.py
+-rw-r--r--   0        0        0      855 2024-05-02 14:38:20.774891 redis_om-0.3.0/redis_om/model/token_escaper.py
+-rw-r--r--   0        0        0       13 2024-05-02 14:38:20.766891 redis_om-0.3.0/redis_om/sync_redis.py
+-rw-r--r--   0        0        0      228 2024-05-02 14:38:20.770891 redis_om-0.3.0/redis_om/util.py
+-rw-r--r--   0        0        0    14712 1970-01-01 00:00:00.000000 redis_om-0.3.0/PKG-INFO
```

### Comparing `redis_om-0.2.2/LICENSE` & `redis_om-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/README.md` & `redis_om-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 class Customer(HashModel):
     first_name: str
     last_name: str
     email: EmailStr
     join_date: datetime.date
     age: int
-    bio: Optional[str]
+    bio: Optional[str] = None
 ```
 
 Now that we have a `Customer` model, let's use it to save customer data to Redis.
 
 ```python
 import datetime
 from typing import Optional
@@ -120,15 +120,15 @@
 
 class Customer(HashModel):
     first_name: str
     last_name: str
     email: EmailStr
     join_date: datetime.date
     age: int
-    bio: Optional[str]
+    bio: Optional[str] = None
 
 
 # First, we create a new `Customer` object:
 andrew = Customer(
     first_name="Andrew",
     last_name="Brookins",
     email="andrew.brookins@example.com",
@@ -175,15 +175,15 @@
 
 class Customer(HashModel):
     first_name: str
     last_name: str
     email: EmailStr
     join_date: datetime.date
     age: int
-    bio: Optional[str]
+    bio: Optional[str] = None
 
 
 try:
     Customer(
         first_name="Andrew",
         last_name="Brookins",
         email="Not an email address!",
@@ -233,15 +233,15 @@
 
 class Customer(HashModel):
     first_name: str
     last_name: str = Field(index=True)
     email: EmailStr
     join_date: datetime.date
     age: int = Field(index=True)
-    bio: Optional[str]
+    bio: Optional[str] = None
 
 
 # Now, if we use this model with a Redis deployment that has the
 # RediSearch module installed, we can run queries like the following.
 
 # Before running queries, we need to run migrations to set up the
 # indexes that Redis OM will use. You can also use the `migrate`
@@ -283,15 +283,15 @@
     Field,
     Migrator,
 )
 
 
 class Address(EmbeddedJsonModel):
     address_line_1: str
-    address_line_2: Optional[str]
+    address_line_2: Optional[str] = None
     city: str = Field(index=True)
     state: str = Field(index=True)
     country: str
     postal_code: str = Field(index=True)
 
 
 class Customer(JsonModel):
```

### Comparing `redis_om-0.2.2/aredis_om/checks.py` & `redis_om-0.3.0/aredis_om/checks.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/aredis_om/connections.py` & `redis_om-0.3.0/aredis_om/connections.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/aredis_om/model/encoders.py` & `redis_om-0.3.0/aredis_om/model/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     sqlalchemy_safe: bool = True,
 ) -> Any:
     if include is not None and not isinstance(include, (set, dict)):
         include = set(include)
     if exclude is not None and not isinstance(exclude, (set, dict)):
         exclude = set(exclude)
 
-    if isinstance(obj, BaseModel):
+    if isinstance(obj, BaseModel) and hasattr(obj, "__config__"):
         encoder = getattr(obj.__config__, "json_encoders", {})
         if custom_encoder:
             encoder.update(custom_encoder)
         obj_dict = obj.dict(
             include=include,  # type: ignore # in Pydantic
             exclude=exclude,  # type: ignore # in Pydantic
             by_alias=by_alias,
```

### Comparing `redis_om-0.2.2/aredis_om/model/migrations/migrator.py` & `redis_om-0.3.0/aredis_om/model/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/aredis_om/model/model.py` & `redis_om-0.3.0/aredis_om/model/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
-    no_type_check,
 )
+from typing import get_args as typing_get_args, no_type_check
 
 from more_itertools import ichunked
 from redis.commands.json.path import Path
 from redis.exceptions import ResponseError
 from typing_extensions import Protocol, get_args, get_origin
 from ulid import ULID
 
@@ -71,14 +71,25 @@
 # someone has accidentally passed in the field separator with string value of a
 # multi-value field lookup, like a IN or NOT_IN.
 DEFAULT_REDISEARCH_FIELD_SEPARATOR = ","
 
 ERRORS_URL = "https://github.com/redis/redis-om-python/blob/main/docs/errors.md"
 
 
+def get_outer_type(field):
+    if hasattr(field, "outer_type_"):
+        return field.outer_type_
+    elif isinstance(field.annotation, type) or is_supported_container_type(
+        field.annotation
+    ):
+        return field.annotation
+    else:
+        return field.annotation.__args__[0]
+
+
 class RedisModelError(Exception):
     """Raised when a problem exists in the definition of a RedisModel."""
 
 
 class QuerySyntaxError(Exception):
     """Raised when a query is constructed improperly."""
 
@@ -102,15 +113,17 @@
     LIKE = 12
     ALL = 13
 
     def __str__(self):
         return str(self.name)
 
 
-ExpressionOrModelField = Union["Expression", "NegatedExpression", ModelField]
+ExpressionOrModelField = Union[
+    "Expression", "NegatedExpression", ModelField, PydanticFieldInfo
+]
 
 
 def embedded(cls):
     """
     Mark a model as embedded to avoid creating multiple indexes if the model is
     only ever used embedded within other models.
     """
@@ -126,23 +139,26 @@
 
 
 def validate_model_fields(model: Type["RedisModel"], field_values: Dict[str, Any]):
     for field_name in field_values.keys():
         if "__" in field_name:
             obj = model
             for sub_field in field_name.split("__"):
+                if not isinstance(obj, ModelMeta) and hasattr(obj, "field"):
+                    obj = getattr(obj, "field").annotation
+
                 if not hasattr(obj, sub_field):
                     raise QuerySyntaxError(
                         f"The update path {field_name} contains a field that does not "
                         f"exist on {model.__name__}. The field is: {sub_field}"
                     )
                 obj = getattr(obj, sub_field)
             return
 
-        if field_name not in model.__fields__:
+        if field_name not in model.__fields__:  # type: ignore
             raise QuerySyntaxError(
                 f"The field {field_name} does not exist on the model {model.__name__}"
             )
 
 
 def decode_redis_value(
     obj: Union[List[bytes], Dict[bytes, bytes], bytes], encoding: str
@@ -327,28 +343,31 @@
 
     def __rshift__(self, other: Any) -> Expression:
         return Expression(
             left=self.field, op=Operators.NOT_IN, right=other, parents=self.parents
         )
 
     def __getattr__(self, item):
-        if is_supported_container_type(self.field.outer_type_):
-            embedded_cls = get_args(self.field.outer_type_)
+        if item.startswith("__"):
+            raise AttributeError("cannot invoke __getattr__ with reserved field")
+        outer_type = outer_type_or_annotation(self.field)
+        if is_supported_container_type(outer_type):
+            embedded_cls = get_args(outer_type)
             if not embedded_cls:
                 raise QuerySyntaxError(
                     "In order to query on a list field, you must define "
                     "the contents of the list with a type annotation, like: "
                     f"orders: List[Order]. Docs: {ERRORS_URL}#E1"
                 )
             embedded_cls = embedded_cls[0]
             attr = getattr(embedded_cls, item)
         else:
-            attr = getattr(self.field.outer_type_, item)
+            attr = getattr(outer_type, item)
         if isinstance(attr, self.__class__):
-            new_parent = (self.field.name, self.field.outer_type_)
+            new_parent = (self.field.alias, outer_type)
             if new_parent not in attr.parents:
                 attr.parents.append(new_parent)
             new_parents = list(set(self.parents) - set(attr.parents))
             if new_parents:
                 attr.parents = new_parents + attr.parents
         return attr
 
@@ -470,42 +489,60 @@
         return params
 
     def validate_sort_fields(self, sort_fields: List[str]):
         for sort_field in sort_fields:
             field_name = sort_field.lstrip("-")
             if self.knn and field_name == self.knn.score_field:
                 continue
-            if field_name not in self.model.__fields__:
+            if field_name not in self.model.__fields__:  # type: ignore
                 raise QueryNotSupportedError(
                     f"You tried sort by {field_name}, but that field "
                     f"does not exist on the model {self.model}"
                 )
             field_proxy = getattr(self.model, field_name)
-            if not getattr(field_proxy.field.field_info, "sortable", False):
+            if isinstance(field_proxy.field, FieldInfo) or isinstance(
+                field_proxy.field, PydanticFieldInfo
+            ):
+                field_info = field_proxy.field
+            else:
+                field_info = field_proxy.field.field_info
+
+            if not getattr(field_info, "sortable", False):
                 raise QueryNotSupportedError(
                     f"You tried sort by {field_name}, but {self.model} does "
                     f"not define that field as sortable. Docs: {ERRORS_URL}#E2"
                 )
         return sort_fields
 
     @staticmethod
-    def resolve_field_type(field: ModelField, op: Operators) -> RediSearchFieldTypes:
-        if getattr(field.field_info, "primary_key", None) is True:
+    def resolve_field_type(
+        field: Union[ModelField, PydanticFieldInfo], op: Operators
+    ) -> RediSearchFieldTypes:
+        field_info: Union[FieldInfo, ModelField, PydanticFieldInfo]
+
+        if not hasattr(field, "field_info"):
+            field_info = field
+        else:
+            field_info = field.field_info
+        if getattr(field_info, "primary_key", None) is True:
             return RediSearchFieldTypes.TAG
         elif op is Operators.LIKE:
-            fts = getattr(field.field_info, "full_text_search", None)
+            fts = getattr(field_info, "full_text_search", None)
             if fts is not True:  # Could be PydanticUndefined
                 raise QuerySyntaxError(
-                    f"You tried to do a full-text search on the field '{field.name}', "
+                    f"You tried to do a full-text search on the field '{field.alias}', "
                     f"but the field is not indexed for full-text search. Use the "
                     f"full_text_search=True option. Docs: {ERRORS_URL}#E3"
                 )
             return RediSearchFieldTypes.TEXT
 
-        field_type = field.outer_type_
+        field_type = outer_type_or_annotation(field)
+
+        if not isinstance(field_type, type):
+            field_type = field_type.__origin__
 
         # TODO: GEO fields
         container_type = get_origin(field_type)
 
         if is_supported_container_type(container_type):
             # NOTE: A list of strings, like:
             #
@@ -647,15 +684,15 @@
                 expanded_value = cls.expand_tag_value(value)
                 result += "(@{field_name}:{{{expanded_value}}})".format(
                     field_name=field_name, expanded_value=expanded_value
                 )
             elif op is Operators.NOT_IN:
                 # TODO: Implement NOT_IN, test this...
                 expanded_value = cls.expand_tag_value(value)
-                result += "-(@{field_name}):{{{expanded_value}}}".format(
+                result += "-(@{field_name}:{{{expanded_value}}})".format(
                     field_name=field_name, expanded_value=expanded_value
                 )
 
         return result
 
     def resolve_redisearch_pagination(self):
         """Resolve pagination options for a query."""
@@ -725,14 +762,23 @@
             field_name = expression.left.name
             field_info = expression.left.field_info
             if not field_info or not getattr(field_info, "index", None):
                 raise QueryNotSupportedError(
                     f"You tried to query by a field ({field_name}) "
                     f"that isn't indexed. Docs: {ERRORS_URL}#E6"
                 )
+        elif isinstance(expression.left, FieldInfo):
+            field_type = cls.resolve_field_type(expression.left, expression.op)
+            field_name = expression.left.alias
+            field_info = expression.left
+            if not field_info or not getattr(field_info, "index", None):
+                raise QueryNotSupportedError(
+                    f"You tried to query by a field ({field_name}) "
+                    f"that isn't indexed. Docs: {ERRORS_URL}#E6"
+                )
         else:
             raise QueryNotSupportedError(
                 "A query expression should start with either a field "
                 f"or an expression enclosed in parentheses. Docs: {ERRORS_URL}#E7"
             )
 
         right = expression.right
@@ -1096,35 +1142,35 @@
         return " ".join([f"VECTOR {self.algorithm.name} {len(attr)}"] + attr)
 
 
 def Field(
     default: Any = Undefined,
     *,
     default_factory: Optional[NoArgAnyCallable] = None,
-    alias: str = None,
-    title: str = None,
-    description: str = None,
+    alias: Optional[str] = None,
+    title: Optional[str] = None,
+    description: Optional[str] = None,
     exclude: Union[
         AbstractSet[Union[int, str]], Mapping[Union[int, str], Any], Any
     ] = None,
     include: Union[
         AbstractSet[Union[int, str]], Mapping[Union[int, str], Any], Any
     ] = None,
-    const: bool = None,
-    gt: float = None,
-    ge: float = None,
-    lt: float = None,
-    le: float = None,
-    multiple_of: float = None,
-    min_items: int = None,
-    max_items: int = None,
-    min_length: int = None,
-    max_length: int = None,
+    const: Optional[bool] = None,
+    gt: Optional[float] = None,
+    ge: Optional[float] = None,
+    lt: Optional[float] = None,
+    le: Optional[float] = None,
+    multiple_of: Optional[float] = None,
+    min_items: Optional[int] = None,
+    max_items: Optional[int] = None,
+    min_length: Optional[int] = None,
+    max_length: Optional[int] = None,
     allow_mutation: bool = True,
-    regex: str = None,
+    regex: Optional[str] = None,
     primary_key: bool = False,
     sortable: Union[bool, UndefinedType] = Undefined,
     index: Union[bool, UndefinedType] = Undefined,
     full_text_search: Union[bool, UndefinedType] = Undefined,
     vector_options: Optional[VectorFieldOptions] = None,
     schema_extra: Optional[Dict[str, Any]] = None,
 ) -> Any:
@@ -1152,15 +1198,14 @@
         primary_key=primary_key,
         sortable=sortable,
         index=index,
         full_text_search=full_text_search,
         vector_options=vector_options,
         **current_schema_extra,
     )
-    field_info._validate()
     return field_info
 
 
 @dataclasses.dataclass
 class PrimaryKey:
     name: str
     field: ModelField
@@ -1228,29 +1273,50 @@
                 f"{new_class.__name__}Meta", (DefaultMeta,), dict(DefaultMeta.__dict__)
             )
             new_class.Meta = new_class._meta
 
         # Create proxies for each model field so that we can use the field
         # in queries, like Model.get(Model.field_name == 1)
         for field_name, field in new_class.__fields__.items():
+            if not isinstance(field, FieldInfo):
+                for base_candidate in bases:
+                    if hasattr(base_candidate, field_name):
+                        inner_field = getattr(base_candidate, field_name)
+                        if hasattr(inner_field, "field") and isinstance(
+                            getattr(inner_field, "field"), FieldInfo
+                        ):
+                            field.metadata.append(getattr(inner_field, "field"))
+                            field = getattr(inner_field, "field")
+
+            if not field.alias:
+                field.alias = field_name
             setattr(new_class, field_name, ExpressionProxy(field, []))
             annotation = new_class.get_annotations().get(field_name)
             if annotation:
                 new_class.__annotations__[field_name] = Union[
                     annotation, ExpressionProxy
                 ]
             else:
                 new_class.__annotations__[field_name] = ExpressionProxy
             # Check if this is our FieldInfo version with extended ORM metadata.
-            if isinstance(field.field_info, FieldInfo):
-                if field.field_info.primary_key:
+            field_info = None
+            if hasattr(field, "field_info") and isinstance(field.field_info, FieldInfo):
+                field_info = field.field_info
+            elif field_name in attrs and isinstance(
+                attrs.__getitem__(field_name), FieldInfo
+            ):
+                field_info = attrs.__getitem__(field_name)
+                field.field_info = field_info
+
+            if field_info is not None:
+                if field_info.primary_key:
                     new_class._meta.primary_key = PrimaryKey(
                         name=field_name, field=field
                     )
-                if field.field_info.vector_options:
+                if field_info.vector_options:
                     score_attr = f"_{field_name}_score"
                     setattr(new_class, score_attr, None)
                     new_class.__annotations__[score_attr] = Union[float, None]
 
         if not getattr(new_class._meta, "global_key_prefix", None):
             new_class._meta.global_key_prefix = getattr(
                 base_meta, "global_key_prefix", ""
@@ -1286,14 +1352,25 @@
         if abc.ABC not in bases and not getattr(new_class._meta, "embedded", False):
             key = f"{new_class.__module__}.{new_class.__qualname__}"
             model_registry[key] = new_class
 
         return new_class
 
 
+def outer_type_or_annotation(field):
+    if hasattr(field, "outer_type_"):
+        return field.outer_type_
+    elif not hasattr(field.annotation, "__args__"):
+        if not isinstance(field.annotation, type):
+            raise AttributeError(f"could not extract outer type from field {field}")
+        return field.annotation
+    else:
+        return field.annotation.__args__[0]
+
+
 class RedisModel(BaseModel, abc.ABC, metaclass=ModelMeta):
     pk: Optional[str] = Field(default=None, primary_key=True)
 
     Meta = DefaultMeta
 
     class Config:
         orm_mode = True
@@ -1306,15 +1383,18 @@
 
     def __lt__(self, other):
         """Default sort: compare primary key of models."""
         return self.key() < other.key()
 
     def key(self):
         """Return the Redis key for this model."""
-        pk = getattr(self, self._meta.primary_key.field.name)
+        if hasattr(self._meta.primary_key.field, "name"):
+            pk = getattr(self, self._meta.primary_key.field.name)
+        else:
+            pk = getattr(self, self._meta.primary_key.name)
         return self.make_primary_key(pk)
 
     @classmethod
     async def _delete(cls, db, *pks):
         return await db.delete(*pks)
 
     @classmethod
@@ -1345,24 +1425,37 @@
         db = self._get_db(pipeline)
 
         # TODO: Wrap any Redis response errors in a custom exception?
         await db.expire(self.key(), num_seconds)
 
     @validator("pk", always=True, allow_reuse=True)
     def validate_pk(cls, v):
-        if not v:
+        if not v or isinstance(v, ExpressionProxy):
             v = cls._meta.primary_key_creator_cls().create_pk()
         return v
 
     @classmethod
     def validate_primary_key(cls):
         """Check for a primary key. We need one (and only one)."""
         primary_keys = 0
         for name, field in cls.__fields__.items():
-            if getattr(field.field_info, "primary_key", None):
+            if not hasattr(field, "field_info"):
+                if (
+                    not isinstance(field, FieldInfo)
+                    and hasattr(field, "metadata")
+                    and len(field.metadata) > 0
+                    and isinstance(field.metadata[0], FieldInfo)
+                ):
+                    field_info = field.metadata[0]
+                else:
+                    field_info = field
+            else:
+                field_info = field.field_info
+
+            if getattr(field_info, "primary_key", None):
                 primary_keys += 1
         if primary_keys == 0:
             raise RedisModelError("You must define a primary key for the model")
         elif primary_keys == 2:
             cls.__fields__.pop("pk")
         elif primary_keys > 2:
             raise RedisModelError("You must define only one primary key for a model")
@@ -1486,48 +1579,72 @@
 
     @classmethod
     def redisearch_schema(cls):
         raise NotImplementedError
 
     def check(self):
         """Run all validations."""
-        *_, validation_error = validate_model(self.__class__, self.__dict__)
-        if validation_error:
-            raise validation_error
+        from pydantic.version import VERSION as PYDANTIC_VERSION
+
+        PYDANTIC_V2 = PYDANTIC_VERSION.startswith("2.")
+        if not PYDANTIC_V2:
+            *_, validation_error = validate_model(self.__class__, self.__dict__)
+            if validation_error:
+                raise validation_error
 
 
 class HashModel(RedisModel, abc.ABC):
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
 
+        if hasattr(cls, "__annotations__"):
+            for name, field_type in cls.__annotations__.items():
+                origin = get_origin(field_type)
+                for typ in (Set, Mapping, List):
+                    if isinstance(origin, type) and issubclass(origin, typ):
+                        raise RedisModelError(
+                            f"HashModels cannot index set, list,"
+                            f" or mapping fields. Field: {name}"
+                        )
+                if isinstance(field_type, type) and issubclass(field_type, RedisModel):
+                    raise RedisModelError(
+                        f"HashModels cannot index embedded model fields. Field: {name}"
+                    )
+                elif isinstance(field_type, type) and dataclasses.is_dataclass(
+                    field_type
+                ):
+                    raise RedisModelError(
+                        f"HashModels cannot index dataclass fields. Field: {name}"
+                    )
+
         for name, field in cls.__fields__.items():
-            origin = get_origin(field.outer_type_)
+            outer_type = outer_type_or_annotation(field)
+            origin = get_origin(outer_type)
             if origin:
                 for typ in (Set, Mapping, List):
                     if issubclass(origin, typ):
                         raise RedisModelError(
                             f"HashModels cannot index set, list,"
                             f" or mapping fields. Field: {name}"
                         )
 
-            if issubclass(field.outer_type_, RedisModel):
+            if issubclass(outer_type, RedisModel):
                 raise RedisModelError(
                     f"HashModels cannot index embedded model fields. Field: {name}"
                 )
-            elif dataclasses.is_dataclass(field.outer_type_):
+            elif dataclasses.is_dataclass(outer_type):
                 raise RedisModelError(
                     f"HashModels cannot index dataclass fields. Field: {name}"
                 )
 
     async def save(
         self: "Model", pipeline: Optional[redis.client.Pipeline] = None
     ) -> "Model":
         self.check()
         db = self._get_db(pipeline)
-
         document = jsonable_encoder(self.dict())
         # TODO: Wrap any Redis response errors in a custom exception?
         await db.hset(self.key(), mapping=document)
         return self
 
     @classmethod
     async def all_pks(cls):  # type: ignore
@@ -1590,46 +1707,55 @@
 
     @classmethod
     def schema_for_fields(cls):
         schema_parts = []
 
         for name, field in cls.__fields__.items():
             # TODO: Merge this code with schema_for_type()?
-            _type = field.outer_type_
+            _type = outer_type_or_annotation(field)
             is_subscripted_type = get_origin(_type)
 
-            if getattr(field.field_info, "primary_key", None):
+            if (
+                not isinstance(field, FieldInfo)
+                and hasattr(field, "metadata")
+                and len(field.metadata) > 0
+                and isinstance(field.metadata[0], FieldInfo)
+            ):
+                field = field.metadata[0]
+
+            if not hasattr(field, "field_info"):
+                field_info = field
+            else:
+                field_info = field.field_info
+
+            if getattr(field_info, "primary_key", None):
                 if issubclass(_type, str):
                     redisearch_field = (
                         f"{name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR}"
                     )
                 else:
-                    redisearch_field = cls.schema_for_type(
-                        name, _type, field.field_info
-                    )
+                    redisearch_field = cls.schema_for_type(name, _type, field_info)
                 schema_parts.append(redisearch_field)
-            elif getattr(field.field_info, "index", None) is True:
-                schema_parts.append(cls.schema_for_type(name, _type, field.field_info))
+            elif getattr(field_info, "index", None) is True:
+                schema_parts.append(cls.schema_for_type(name, _type, field_info))
             elif is_subscripted_type:
                 # Ignore subscripted types (usually containers!) that we don't
                 # support, for the purposes of indexing.
                 if not is_supported_container_type(_type):
                     continue
 
                 embedded_cls = get_args(_type)
                 if not embedded_cls:
                     # TODO: Test if this can really happen.
                     log.warning("Model %s defined an empty list field: %s", cls, name)
                     continue
                 embedded_cls = embedded_cls[0]
-                schema_parts.append(
-                    cls.schema_for_type(name, embedded_cls, field.field_info)
-                )
+                schema_parts.append(cls.schema_for_type(name, embedded_cls, field_info))
             elif issubclass(_type, RedisModel):
-                schema_parts.append(cls.schema_for_type(name, _type, field.field_info))
+                schema_parts.append(cls.schema_for_type(name, _type, field_info))
         return schema_parts
 
     @classmethod
     def schema_for_type(cls, name, typ: Any, field_info: PydanticFieldInfo):
         # TODO: Import parent logic from JsonModel to deal with lists, so that
         #  a List[int] gets indexed as TAG instead of NUMERICAL.
         # TODO: Raise error if user embeds a model field or list and makes it
@@ -1756,19 +1882,50 @@
         schema_parts = [schema_prefix] + cls.schema_for_fields()
         return " ".join(schema_parts)
 
     @classmethod
     def schema_for_fields(cls):
         schema_parts = []
         json_path = "$"
-
+        fields = dict()
         for name, field in cls.__fields__.items():
-            _type = field.outer_type_
+            fields[name] = field
+        for name, field in cls.__dict__.items():
+            if isinstance(field, FieldInfo):
+                if not field.annotation:
+                    field.annotation = cls.__annotations__.get(name)
+                fields[name] = field
+        for name, field in cls.__annotations__.items():
+            if name in fields:
+                continue
+            fields[name] = PydanticFieldInfo.from_annotation(field)
+
+        for name, field in fields.items():
+            _type = get_outer_type(field)
+            if (
+                not isinstance(field, FieldInfo)
+                and hasattr(field, "metadata")
+                and len(field.metadata) > 0
+                and isinstance(field.metadata[0], FieldInfo)
+            ):
+                field = field.metadata[0]
+
+            if hasattr(field, "field_info"):
+                field_info = field.field_info
+            else:
+                field_info = field
+            if getattr(field_info, "primary_key", None):
+                if issubclass(_type, str):
+                    redisearch_field = f"$.{name} AS {name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR}"
+                else:
+                    redisearch_field = cls.schema_for_type(name, _type, field_info)
+                schema_parts.append(redisearch_field)
+                continue
             schema_parts.append(
-                cls.schema_for_type(json_path, name, "", _type, field.field_info)
+                cls.schema_for_type(json_path, name, "", _type, field_info)
             )
         return schema_parts
 
     @classmethod
     def schema_for_type(
         cls,
         json_path: str,
@@ -1839,14 +1996,25 @@
                 field_info,
                 parent_type=field_type,
             )
         elif field_is_model:
             name_prefix = f"{name_prefix}_{name}" if name_prefix else name
             sub_fields = []
             for embedded_name, field in typ.__fields__.items():
+                if hasattr(field, "field_info"):
+                    field_info = field.field_info
+                elif (
+                    hasattr(field, "metadata")
+                    and len(field.metadata) > 0
+                    and isinstance(field.metadata[0], FieldInfo)
+                ):
+                    field_info = field.metadata[0]
+                else:
+                    field_info = field
+
                 if parent_is_container_type:
                     # We'll store this value either as a JavaScript array, so
                     # the correct JSONPath expression is to refer directly to
                     # attribute names after the container notation, e.g.
                     # orders[*].created_date.
                     path = json_path
                 else:
@@ -1855,16 +2023,17 @@
                     # order.address.street_line_1.
                     path = f"{json_path}.{name}"
                 sub_fields.append(
                     cls.schema_for_type(
                         path,
                         embedded_name,
                         name_prefix,
-                        field.outer_type_,
-                        field.field_info,
+                        # field.annotation,
+                        get_outer_type(field),
+                        field_info,
                         parent_type=typ,
                     )
                 )
             return " ".join(filter(None, sub_fields))
         # NOTE: This is the termination point for recursion. We've descended
         # into models and lists until we found an actual value to index.
         elif should_index:
@@ -1880,14 +2049,20 @@
             full_text_search = getattr(field_info, "full_text_search", False)
             sortable_tag_error = RedisModelError(
                 "In this Preview release, TAG fields cannot "
                 f"be marked as sortable. Problem field: {name}. "
                 "See docs: TODO"
             )
 
+            # For more complicated compound validators (e.g. PositiveInt), we might get a _GenericAlias rather than
+            # a proper type, we can pull the type information from the origin of the first argument.
+            if not isinstance(typ, type):
+                type_args = typing_get_args(field_info.annotation)
+                typ = type_args[0].__origin__
+
             # TODO: GEO field
             if is_vector and vector_options:
                 schema = f"{path} AS {index_field_name} {vector_options.schema}"
             elif parent_is_container_type or parent_is_model_in_container:
                 if typ is not str:
                     raise RedisModelError(
                         "In this Preview release, list and tuple fields can only "
```

### Comparing `redis_om-0.2.2/aredis_om/model/query_resolver.py` & `redis_om-0.3.0/aredis_om/model/query_resolver.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/aredis_om/model/render_tree.py` & `redis_om-0.3.0/aredis_om/model/render_tree.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/aredis_om/model/token_escaper.py` & `redis_om-0.3.0/aredis_om/model/token_escaper.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/docs/connections.md` & `redis_om-0.3.0/docs/connections.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/docs/errors.md` & `redis_om-0.3.0/docs/errors.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/docs/fastapi_integration.md` & `redis_om-0.3.0/docs/fastapi_integration.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/docs/getting_started.md` & `redis_om-0.3.0/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/docs/index.md` & `redis_om-0.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/docs/models.md` & `redis_om-0.3.0/docs/models.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/docs/redis_modules.md` & `redis_om-0.3.0/docs/redis_modules.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/docs/validation.md` & `redis_om-0.3.0/docs/validation.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/images/logo.svg` & `redis_om-0.3.0/images/logo.svg`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/pyproject.toml` & `redis_om-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redis-om"
-version = "0.2.2"
+version = "0.3.0"
 description = "Object mappings, and more, for Redis."
 authors = [ "Redis OSS <oss@redis.com>" ]
 maintainers = [ "Redis OSS <oss@redis.com>" ]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/redis/redis-om-python"
 classifiers = [
@@ -29,28 +29,28 @@
   [tool.poetry.urls]
   Code = "https://github.com/redis/redis-om-python"
   "Issue tracker" = "https://github.com/redis/redis-om-python/issues"
 
   [tool.poetry.dependencies]
   python = ">=3.8,<4.0"
   redis = ">=3.5.3,<6.0.0"
-  pydantic = ">=1.10.2,<2.5.0"
+  pydantic = ">=1.10.2,<3.0.0"
   click = "^8.0.1"
   types-redis = ">=3.5.9,<5.0.0"
   python-ulid = "^1.0.3"
   typing-extensions = "^4.4.0"
   hiredis = "^2.2.3"
   more-itertools = ">=8.14,<11.0"
 
     [tool.poetry.dependencies.setuptools]
     version = "^69.2.0"
     markers = "python_version >= '3.12'"
 
   [tool.poetry.dev-dependencies]
-  mypy = "^0.982"
+  mypy = "^1.9.0"
   pytest = "^8.0.2"
   ipdb = "^0.13.9"
   black = "^24.2"
   isort = "^5.9.3"
   flake8 = "^5.0.4"
   bandit = "^1.7.4"
   coverage = "^7.1"
```

### Comparing `redis_om-0.2.2/redis_om/checks.py` & `redis_om-0.3.0/redis_om/checks.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/redis_om/connections.py` & `redis_om-0.3.0/redis_om/connections.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/redis_om/model/encoders.py` & `redis_om-0.3.0/redis_om/model/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     sqlalchemy_safe: bool = True,
 ) -> Any:
     if include is not None and not isinstance(include, (set, dict)):
         include = set(include)
     if exclude is not None and not isinstance(exclude, (set, dict)):
         exclude = set(exclude)
 
-    if isinstance(obj, BaseModel):
+    if isinstance(obj, BaseModel) and hasattr(obj, "__config__"):
         encoder = getattr(obj.__config__, "json_encoders", {})
         if custom_encoder:
             encoder.update(custom_encoder)
         obj_dict = obj.dict(
             include=include,  # type: ignore # in Pydantic
             exclude=exclude,  # type: ignore # in Pydantic
             by_alias=by_alias,
```

### Comparing `redis_om-0.2.2/redis_om/model/migrations/migrator.py` & `redis_om-0.3.0/redis_om/model/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/redis_om/model/model.py` & `redis_om-0.3.0/redis_om/model/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
-    no_type_check,
 )
+from typing import get_args as typing_get_args, no_type_check
 
 from more_itertools import ichunked
 from redis.commands.json.path import Path
 from redis.exceptions import ResponseError
 from typing_extensions import Protocol, get_args, get_origin
 from ulid import ULID
 
@@ -71,14 +71,25 @@
 # someone has accidentally passed in the field separator with string value of a
 # multi-value field lookup, like a IN or NOT_IN.
 DEFAULT_REDISEARCH_FIELD_SEPARATOR = ","
 
 ERRORS_URL = "https://github.com/redis/redis-om-python/blob/main/docs/errors.md"
 
 
+def get_outer_type(field):
+    if hasattr(field, "outer_type_"):
+        return field.outer_type_
+    elif isinstance(field.annotation, type) or is_supported_container_type(
+        field.annotation
+    ):
+        return field.annotation
+    else:
+        return field.annotation.__args__[0]
+
+
 class RedisModelError(Exception):
     """Raised when a problem exists in the definition of a RedisModel."""
 
 
 class QuerySyntaxError(Exception):
     """Raised when a query is constructed improperly."""
 
@@ -102,15 +113,17 @@
     LIKE = 12
     ALL = 13
 
     def __str__(self):
         return str(self.name)
 
 
-ExpressionOrModelField = Union["Expression", "NegatedExpression", ModelField]
+ExpressionOrModelField = Union[
+    "Expression", "NegatedExpression", ModelField, PydanticFieldInfo
+]
 
 
 def embedded(cls):
     """
     Mark a model as embedded to avoid creating multiple indexes if the model is
     only ever used embedded within other models.
     """
@@ -126,23 +139,26 @@
 
 
 def validate_model_fields(model: Type["RedisModel"], field_values: Dict[str, Any]):
     for field_name in field_values.keys():
         if "__" in field_name:
             obj = model
             for sub_field in field_name.split("__"):
+                if not isinstance(obj, ModelMeta) and hasattr(obj, "field"):
+                    obj = getattr(obj, "field").annotation
+
                 if not hasattr(obj, sub_field):
                     raise QuerySyntaxError(
                         f"The update path {field_name} contains a field that does not "
                         f"exist on {model.__name__}. The field is: {sub_field}"
                     )
                 obj = getattr(obj, sub_field)
             return
 
-        if field_name not in model.__fields__:
+        if field_name not in model.__fields__:  # type: ignore
             raise QuerySyntaxError(
                 f"The field {field_name} does not exist on the model {model.__name__}"
             )
 
 
 def decode_redis_value(
     obj: Union[List[bytes], Dict[bytes, bytes], bytes], encoding: str
@@ -327,28 +343,31 @@
 
     def __rshift__(self, other: Any) -> Expression:
         return Expression(
             left=self.field, op=Operators.NOT_IN, right=other, parents=self.parents
         )
 
     def __getattr__(self, item):
-        if is_supported_container_type(self.field.outer_type_):
-            embedded_cls = get_args(self.field.outer_type_)
+        if item.startswith("__"):
+            raise AttributeError("cannot invoke __getattr__ with reserved field")
+        outer_type = outer_type_or_annotation(self.field)
+        if is_supported_container_type(outer_type):
+            embedded_cls = get_args(outer_type)
             if not embedded_cls:
                 raise QuerySyntaxError(
                     "In order to query on a list field, you must define "
                     "the contents of the list with a type annotation, like: "
                     f"orders: List[Order]. Docs: {ERRORS_URL}#E1"
                 )
             embedded_cls = embedded_cls[0]
             attr = getattr(embedded_cls, item)
         else:
-            attr = getattr(self.field.outer_type_, item)
+            attr = getattr(outer_type, item)
         if isinstance(attr, self.__class__):
-            new_parent = (self.field.name, self.field.outer_type_)
+            new_parent = (self.field.alias, outer_type)
             if new_parent not in attr.parents:
                 attr.parents.append(new_parent)
             new_parents = list(set(self.parents) - set(attr.parents))
             if new_parents:
                 attr.parents = new_parents + attr.parents
         return attr
 
@@ -470,42 +489,60 @@
         return params
 
     def validate_sort_fields(self, sort_fields: List[str]):
         for sort_field in sort_fields:
             field_name = sort_field.lstrip("-")
             if self.knn and field_name == self.knn.score_field:
                 continue
-            if field_name not in self.model.__fields__:
+            if field_name not in self.model.__fields__:  # type: ignore
                 raise QueryNotSupportedError(
                     f"You tried sort by {field_name}, but that field "
                     f"does not exist on the model {self.model}"
                 )
             field_proxy = getattr(self.model, field_name)
-            if not getattr(field_proxy.field.field_info, "sortable", False):
+            if isinstance(field_proxy.field, FieldInfo) or isinstance(
+                field_proxy.field, PydanticFieldInfo
+            ):
+                field_info = field_proxy.field
+            else:
+                field_info = field_proxy.field.field_info
+
+            if not getattr(field_info, "sortable", False):
                 raise QueryNotSupportedError(
                     f"You tried sort by {field_name}, but {self.model} does "
                     f"not define that field as sortable. Docs: {ERRORS_URL}#E2"
                 )
         return sort_fields
 
     @staticmethod
-    def resolve_field_type(field: ModelField, op: Operators) -> RediSearchFieldTypes:
-        if getattr(field.field_info, "primary_key", None) is True:
+    def resolve_field_type(
+        field: Union[ModelField, PydanticFieldInfo], op: Operators
+    ) -> RediSearchFieldTypes:
+        field_info: Union[FieldInfo, ModelField, PydanticFieldInfo]
+
+        if not hasattr(field, "field_info"):
+            field_info = field
+        else:
+            field_info = field.field_info
+        if getattr(field_info, "primary_key", None) is True:
             return RediSearchFieldTypes.TAG
         elif op is Operators.LIKE:
-            fts = getattr(field.field_info, "full_text_search", None)
+            fts = getattr(field_info, "full_text_search", None)
             if fts is not True:  # Could be PydanticUndefined
                 raise QuerySyntaxError(
-                    f"You tried to do a full-text search on the field '{field.name}', "
+                    f"You tried to do a full-text search on the field '{field.alias}', "
                     f"but the field is not indexed for full-text search. Use the "
                     f"full_text_search=True option. Docs: {ERRORS_URL}#E3"
                 )
             return RediSearchFieldTypes.TEXT
 
-        field_type = field.outer_type_
+        field_type = outer_type_or_annotation(field)
+
+        if not isinstance(field_type, type):
+            field_type = field_type.__origin__
 
         # TODO: GEO fields
         container_type = get_origin(field_type)
 
         if is_supported_container_type(container_type):
             # NOTE: A list of strings, like:
             #
@@ -647,15 +684,15 @@
                 expanded_value = cls.expand_tag_value(value)
                 result += "(@{field_name}:{{{expanded_value}}})".format(
                     field_name=field_name, expanded_value=expanded_value
                 )
             elif op is Operators.NOT_IN:
                 # TODO: Implement NOT_IN, test this...
                 expanded_value = cls.expand_tag_value(value)
-                result += "-(@{field_name}):{{{expanded_value}}}".format(
+                result += "-(@{field_name}:{{{expanded_value}}})".format(
                     field_name=field_name, expanded_value=expanded_value
                 )
 
         return result
 
     def resolve_redisearch_pagination(self):
         """Resolve pagination options for a query."""
@@ -725,14 +762,23 @@
             field_name = expression.left.name
             field_info = expression.left.field_info
             if not field_info or not getattr(field_info, "index", None):
                 raise QueryNotSupportedError(
                     f"You tried to query by a field ({field_name}) "
                     f"that isn't indexed. Docs: {ERRORS_URL}#E6"
                 )
+        elif isinstance(expression.left, FieldInfo):
+            field_type = cls.resolve_field_type(expression.left, expression.op)
+            field_name = expression.left.alias
+            field_info = expression.left
+            if not field_info or not getattr(field_info, "index", None):
+                raise QueryNotSupportedError(
+                    f"You tried to query by a field ({field_name}) "
+                    f"that isn't indexed. Docs: {ERRORS_URL}#E6"
+                )
         else:
             raise QueryNotSupportedError(
                 "A query expression should start with either a field "
                 f"or an expression enclosed in parentheses. Docs: {ERRORS_URL}#E7"
             )
 
         right = expression.right
@@ -1096,35 +1142,35 @@
         return " ".join([f"VECTOR {self.algorithm.name} {len(attr)}"] + attr)
 
 
 def Field(
     default: Any = Undefined,
     *,
     default_factory: Optional[NoArgAnyCallable] = None,
-    alias: str = None,
-    title: str = None,
-    description: str = None,
+    alias: Optional[str] = None,
+    title: Optional[str] = None,
+    description: Optional[str] = None,
     exclude: Union[
         AbstractSet[Union[int, str]], Mapping[Union[int, str], Any], Any
     ] = None,
     include: Union[
         AbstractSet[Union[int, str]], Mapping[Union[int, str], Any], Any
     ] = None,
-    const: bool = None,
-    gt: float = None,
-    ge: float = None,
-    lt: float = None,
-    le: float = None,
-    multiple_of: float = None,
-    min_items: int = None,
-    max_items: int = None,
-    min_length: int = None,
-    max_length: int = None,
+    const: Optional[bool] = None,
+    gt: Optional[float] = None,
+    ge: Optional[float] = None,
+    lt: Optional[float] = None,
+    le: Optional[float] = None,
+    multiple_of: Optional[float] = None,
+    min_items: Optional[int] = None,
+    max_items: Optional[int] = None,
+    min_length: Optional[int] = None,
+    max_length: Optional[int] = None,
     allow_mutation: bool = True,
-    regex: str = None,
+    regex: Optional[str] = None,
     primary_key: bool = False,
     sortable: Union[bool, UndefinedType] = Undefined,
     index: Union[bool, UndefinedType] = Undefined,
     full_text_search: Union[bool, UndefinedType] = Undefined,
     vector_options: Optional[VectorFieldOptions] = None,
     schema_extra: Optional[Dict[str, Any]] = None,
 ) -> Any:
@@ -1152,15 +1198,14 @@
         primary_key=primary_key,
         sortable=sortable,
         index=index,
         full_text_search=full_text_search,
         vector_options=vector_options,
         **current_schema_extra,
     )
-    field_info._validate()
     return field_info
 
 
 @dataclasses.dataclass
 class PrimaryKey:
     name: str
     field: ModelField
@@ -1228,29 +1273,50 @@
                 f"{new_class.__name__}Meta", (DefaultMeta,), dict(DefaultMeta.__dict__)
             )
             new_class.Meta = new_class._meta
 
         # Create proxies for each model field so that we can use the field
         # in queries, like Model.get(Model.field_name == 1)
         for field_name, field in new_class.__fields__.items():
+            if not isinstance(field, FieldInfo):
+                for base_candidate in bases:
+                    if hasattr(base_candidate, field_name):
+                        inner_field = getattr(base_candidate, field_name)
+                        if hasattr(inner_field, "field") and isinstance(
+                            getattr(inner_field, "field"), FieldInfo
+                        ):
+                            field.metadata.append(getattr(inner_field, "field"))
+                            field = getattr(inner_field, "field")
+
+            if not field.alias:
+                field.alias = field_name
             setattr(new_class, field_name, ExpressionProxy(field, []))
             annotation = new_class.get_annotations().get(field_name)
             if annotation:
                 new_class.__annotations__[field_name] = Union[
                     annotation, ExpressionProxy
                 ]
             else:
                 new_class.__annotations__[field_name] = ExpressionProxy
             # Check if this is our FieldInfo version with extended ORM metadata.
-            if isinstance(field.field_info, FieldInfo):
-                if field.field_info.primary_key:
+            field_info = None
+            if hasattr(field, "field_info") and isinstance(field.field_info, FieldInfo):
+                field_info = field.field_info
+            elif field_name in attrs and isinstance(
+                attrs.__getitem__(field_name), FieldInfo
+            ):
+                field_info = attrs.__getitem__(field_name)
+                field.field_info = field_info
+
+            if field_info is not None:
+                if field_info.primary_key:
                     new_class._meta.primary_key = PrimaryKey(
                         name=field_name, field=field
                     )
-                if field.field_info.vector_options:
+                if field_info.vector_options:
                     score_attr = f"_{field_name}_score"
                     setattr(new_class, score_attr, None)
                     new_class.__annotations__[score_attr] = Union[float, None]
 
         if not getattr(new_class._meta, "global_key_prefix", None):
             new_class._meta.global_key_prefix = getattr(
                 base_meta, "global_key_prefix", ""
@@ -1286,14 +1352,25 @@
         if abc.ABC not in bases and not getattr(new_class._meta, "embedded", False):
             key = f"{new_class.__module__}.{new_class.__qualname__}"
             model_registry[key] = new_class
 
         return new_class
 
 
+def outer_type_or_annotation(field):
+    if hasattr(field, "outer_type_"):
+        return field.outer_type_
+    elif not hasattr(field.annotation, "__args__"):
+        if not isinstance(field.annotation, type):
+            raise AttributeError(f"could not extract outer type from field {field}")
+        return field.annotation
+    else:
+        return field.annotation.__args__[0]
+
+
 class RedisModel(BaseModel, abc.ABC, metaclass=ModelMeta):
     pk: Optional[str] = Field(default=None, primary_key=True)
 
     Meta = DefaultMeta
 
     class Config:
         orm_mode = True
@@ -1306,15 +1383,18 @@
 
     def __lt__(self, other):
         """Default sort: compare primary key of models."""
         return self.key() < other.key()
 
     def key(self):
         """Return the Redis key for this model."""
-        pk = getattr(self, self._meta.primary_key.field.name)
+        if hasattr(self._meta.primary_key.field, "name"):
+            pk = getattr(self, self._meta.primary_key.field.name)
+        else:
+            pk = getattr(self, self._meta.primary_key.name)
         return self.make_primary_key(pk)
 
     @classmethod
     def _delete(cls, db, *pks):
         return db.delete(*pks)
 
     @classmethod
@@ -1345,24 +1425,37 @@
         db = self._get_db(pipeline)
 
         # TODO: Wrap any Redis response errors in a custom exception?
         db.expire(self.key(), num_seconds)
 
     @validator("pk", always=True, allow_reuse=True)
     def validate_pk(cls, v):
-        if not v:
+        if not v or isinstance(v, ExpressionProxy):
             v = cls._meta.primary_key_creator_cls().create_pk()
         return v
 
     @classmethod
     def validate_primary_key(cls):
         """Check for a primary key. We need one (and only one)."""
         primary_keys = 0
         for name, field in cls.__fields__.items():
-            if getattr(field.field_info, "primary_key", None):
+            if not hasattr(field, "field_info"):
+                if (
+                    not isinstance(field, FieldInfo)
+                    and hasattr(field, "metadata")
+                    and len(field.metadata) > 0
+                    and isinstance(field.metadata[0], FieldInfo)
+                ):
+                    field_info = field.metadata[0]
+                else:
+                    field_info = field
+            else:
+                field_info = field.field_info
+
+            if getattr(field_info, "primary_key", None):
                 primary_keys += 1
         if primary_keys == 0:
             raise RedisModelError("You must define a primary key for the model")
         elif primary_keys == 2:
             cls.__fields__.pop("pk")
         elif primary_keys > 2:
             raise RedisModelError("You must define only one primary key for a model")
@@ -1486,48 +1579,72 @@
 
     @classmethod
     def redisearch_schema(cls):
         raise NotImplementedError
 
     def check(self):
         """Run all validations."""
-        *_, validation_error = validate_model(self.__class__, self.__dict__)
-        if validation_error:
-            raise validation_error
+        from pydantic.version import VERSION as PYDANTIC_VERSION
+
+        PYDANTIC_V2 = PYDANTIC_VERSION.startswith("2.")
+        if not PYDANTIC_V2:
+            *_, validation_error = validate_model(self.__class__, self.__dict__)
+            if validation_error:
+                raise validation_error
 
 
 class HashModel(RedisModel, abc.ABC):
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
 
+        if hasattr(cls, "__annotations__"):
+            for name, field_type in cls.__annotations__.items():
+                origin = get_origin(field_type)
+                for typ in (Set, Mapping, List):
+                    if isinstance(origin, type) and issubclass(origin, typ):
+                        raise RedisModelError(
+                            f"HashModels cannot index set, list,"
+                            f" or mapping fields. Field: {name}"
+                        )
+                if isinstance(field_type, type) and issubclass(field_type, RedisModel):
+                    raise RedisModelError(
+                        f"HashModels cannot index embedded model fields. Field: {name}"
+                    )
+                elif isinstance(field_type, type) and dataclasses.is_dataclass(
+                    field_type
+                ):
+                    raise RedisModelError(
+                        f"HashModels cannot index dataclass fields. Field: {name}"
+                    )
+
         for name, field in cls.__fields__.items():
-            origin = get_origin(field.outer_type_)
+            outer_type = outer_type_or_annotation(field)
+            origin = get_origin(outer_type)
             if origin:
                 for typ in (Set, Mapping, List):
                     if issubclass(origin, typ):
                         raise RedisModelError(
                             f"HashModels cannot index set, list,"
                             f" or mapping fields. Field: {name}"
                         )
 
-            if issubclass(field.outer_type_, RedisModel):
+            if issubclass(outer_type, RedisModel):
                 raise RedisModelError(
                     f"HashModels cannot index embedded model fields. Field: {name}"
                 )
-            elif dataclasses.is_dataclass(field.outer_type_):
+            elif dataclasses.is_dataclass(outer_type):
                 raise RedisModelError(
                     f"HashModels cannot index dataclass fields. Field: {name}"
                 )
 
     def save(
         self: "Model", pipeline: Optional[redis.client.Pipeline] = None
     ) -> "Model":
         self.check()
         db = self._get_db(pipeline)
-
         document = jsonable_encoder(self.dict())
         # TODO: Wrap any Redis response errors in a custom exception?
         db.hset(self.key(), mapping=document)
         return self
 
     @classmethod
     def all_pks(cls):  # type: ignore
@@ -1590,46 +1707,55 @@
 
     @classmethod
     def schema_for_fields(cls):
         schema_parts = []
 
         for name, field in cls.__fields__.items():
             # TODO: Merge this code with schema_for_type()?
-            _type = field.outer_type_
+            _type = outer_type_or_annotation(field)
             is_subscripted_type = get_origin(_type)
 
-            if getattr(field.field_info, "primary_key", None):
+            if (
+                not isinstance(field, FieldInfo)
+                and hasattr(field, "metadata")
+                and len(field.metadata) > 0
+                and isinstance(field.metadata[0], FieldInfo)
+            ):
+                field = field.metadata[0]
+
+            if not hasattr(field, "field_info"):
+                field_info = field
+            else:
+                field_info = field.field_info
+
+            if getattr(field_info, "primary_key", None):
                 if issubclass(_type, str):
                     redisearch_field = (
                         f"{name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR}"
                     )
                 else:
-                    redisearch_field = cls.schema_for_type(
-                        name, _type, field.field_info
-                    )
+                    redisearch_field = cls.schema_for_type(name, _type, field_info)
                 schema_parts.append(redisearch_field)
-            elif getattr(field.field_info, "index", None) is True:
-                schema_parts.append(cls.schema_for_type(name, _type, field.field_info))
+            elif getattr(field_info, "index", None) is True:
+                schema_parts.append(cls.schema_for_type(name, _type, field_info))
             elif is_subscripted_type:
                 # Ignore subscripted types (usually containers!) that we don't
                 # support, for the purposes of indexing.
                 if not is_supported_container_type(_type):
                     continue
 
                 embedded_cls = get_args(_type)
                 if not embedded_cls:
                     # TODO: Test if this can really happen.
                     log.warning("Model %s defined an empty list field: %s", cls, name)
                     continue
                 embedded_cls = embedded_cls[0]
-                schema_parts.append(
-                    cls.schema_for_type(name, embedded_cls, field.field_info)
-                )
+                schema_parts.append(cls.schema_for_type(name, embedded_cls, field_info))
             elif issubclass(_type, RedisModel):
-                schema_parts.append(cls.schema_for_type(name, _type, field.field_info))
+                schema_parts.append(cls.schema_for_type(name, _type, field_info))
         return schema_parts
 
     @classmethod
     def schema_for_type(cls, name, typ: Any, field_info: PydanticFieldInfo):
         # TODO: Import parent logic from JsonModel to deal with lists, so that
         #  a List[int] gets indexed as TAG instead of NUMERICAL.
         # TODO: Raise error if user embeds a model field or list and makes it
@@ -1756,19 +1882,50 @@
         schema_parts = [schema_prefix] + cls.schema_for_fields()
         return " ".join(schema_parts)
 
     @classmethod
     def schema_for_fields(cls):
         schema_parts = []
         json_path = "$"
-
+        fields = dict()
         for name, field in cls.__fields__.items():
-            _type = field.outer_type_
+            fields[name] = field
+        for name, field in cls.__dict__.items():
+            if isinstance(field, FieldInfo):
+                if not field.annotation:
+                    field.annotation = cls.__annotations__.get(name)
+                fields[name] = field
+        for name, field in cls.__annotations__.items():
+            if name in fields:
+                continue
+            fields[name] = PydanticFieldInfo.from_annotation(field)
+
+        for name, field in fields.items():
+            _type = get_outer_type(field)
+            if (
+                not isinstance(field, FieldInfo)
+                and hasattr(field, "metadata")
+                and len(field.metadata) > 0
+                and isinstance(field.metadata[0], FieldInfo)
+            ):
+                field = field.metadata[0]
+
+            if hasattr(field, "field_info"):
+                field_info = field.field_info
+            else:
+                field_info = field
+            if getattr(field_info, "primary_key", None):
+                if issubclass(_type, str):
+                    redisearch_field = f"$.{name} AS {name} TAG SEPARATOR {SINGLE_VALUE_TAG_FIELD_SEPARATOR}"
+                else:
+                    redisearch_field = cls.schema_for_type(name, _type, field_info)
+                schema_parts.append(redisearch_field)
+                continue
             schema_parts.append(
-                cls.schema_for_type(json_path, name, "", _type, field.field_info)
+                cls.schema_for_type(json_path, name, "", _type, field_info)
             )
         return schema_parts
 
     @classmethod
     def schema_for_type(
         cls,
         json_path: str,
@@ -1839,14 +1996,25 @@
                 field_info,
                 parent_type=field_type,
             )
         elif field_is_model:
             name_prefix = f"{name_prefix}_{name}" if name_prefix else name
             sub_fields = []
             for embedded_name, field in typ.__fields__.items():
+                if hasattr(field, "field_info"):
+                    field_info = field.field_info
+                elif (
+                    hasattr(field, "metadata")
+                    and len(field.metadata) > 0
+                    and isinstance(field.metadata[0], FieldInfo)
+                ):
+                    field_info = field.metadata[0]
+                else:
+                    field_info = field
+
                 if parent_is_container_type:
                     # We'll store this value either as a JavaScript array, so
                     # the correct JSONPath expression is to refer directly to
                     # attribute names after the container notation, e.g.
                     # orders[*].created_date.
                     path = json_path
                 else:
@@ -1855,16 +2023,17 @@
                     # order.address.street_line_1.
                     path = f"{json_path}.{name}"
                 sub_fields.append(
                     cls.schema_for_type(
                         path,
                         embedded_name,
                         name_prefix,
-                        field.outer_type_,
-                        field.field_info,
+                        # field.annotation,
+                        get_outer_type(field),
+                        field_info,
                         parent_type=typ,
                     )
                 )
             return " ".join(filter(None, sub_fields))
         # NOTE: This is the termination point for recursion. We've descended
         # into models and lists until we found an actual value to index.
         elif should_index:
@@ -1880,14 +2049,20 @@
             full_text_search = getattr(field_info, "full_text_search", False)
             sortable_tag_error = RedisModelError(
                 "In this Preview release, TAG fields cannot "
                 f"be marked as sortable. Problem field: {name}. "
                 "See docs: TODO"
             )
 
+            # For more complicated compound validators (e.g. PositiveInt), we might get a _GenericAlias rather than
+            # a proper type, we can pull the type information from the origin of the first argument.
+            if not isinstance(typ, type):
+                type_args = typing_get_args(field_info.annotation)
+                typ = type_args[0].__origin__
+
             # TODO: GEO field
             if is_vector and vector_options:
                 schema = f"{path} AS {index_field_name} {vector_options.schema}"
             elif parent_is_container_type or parent_is_model_in_container:
                 if typ is not str:
                     raise RedisModelError(
                         "In this Preview release, list and tuple fields can only "
```

### Comparing `redis_om-0.2.2/redis_om/model/query_resolver.py` & `redis_om-0.3.0/redis_om/model/query_resolver.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/redis_om/model/render_tree.py` & `redis_om-0.3.0/redis_om/model/render_tree.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/redis_om/model/token_escaper.py` & `redis_om-0.3.0/redis_om/model/token_escaper.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.2.2/PKG-INFO` & `redis_om-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-om
-Version: 0.2.2
+Version: 0.3.0
 Summary: Object mappings, and more, for Redis.
 Home-page: https://github.com/redis/redis-om-python
 License: BSD-3-Clause
 Author: Redis OSS
 Author-email: oss@redis.com
 Maintainer: Redis OSS
 Maintainer-email: oss@redis.com
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database
 Requires-Dist: click (>=8.0.1,<9.0.0)
 Requires-Dist: hiredis (>=2.2.3,<3.0.0)
 Requires-Dist: more-itertools (>=8.14,<11.0)
-Requires-Dist: pydantic (>=1.10.2,<2.5.0)
+Requires-Dist: pydantic (>=1.10.2,<3.0.0)
 Requires-Dist: python-ulid (>=1.0.3,<2.0.0)
 Requires-Dist: redis (>=3.5.3,<6.0.0)
 Requires-Dist: setuptools (>=69.2.0,<70.0.0) ; python_version >= "3.12"
 Requires-Dist: types-redis (>=3.5.9,<5.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Code, https://github.com/redis/redis-om-python
 Project-URL: Issue tracker, https://github.com/redis/redis-om-python/issues
@@ -138,15 +138,15 @@
 
 class Customer(HashModel):
     first_name: str
     last_name: str
     email: EmailStr
     join_date: datetime.date
     age: int
-    bio: Optional[str]
+    bio: Optional[str] = None
 ```
 
 Now that we have a `Customer` model, let's use it to save customer data to Redis.
 
 ```python
 import datetime
 from typing import Optional
@@ -158,15 +158,15 @@
 
 class Customer(HashModel):
     first_name: str
     last_name: str
     email: EmailStr
     join_date: datetime.date
     age: int
-    bio: Optional[str]
+    bio: Optional[str] = None
 
 
 # First, we create a new `Customer` object:
 andrew = Customer(
     first_name="Andrew",
     last_name="Brookins",
     email="andrew.brookins@example.com",
@@ -213,15 +213,15 @@
 
 class Customer(HashModel):
     first_name: str
     last_name: str
     email: EmailStr
     join_date: datetime.date
     age: int
-    bio: Optional[str]
+    bio: Optional[str] = None
 
 
 try:
     Customer(
         first_name="Andrew",
         last_name="Brookins",
         email="Not an email address!",
@@ -271,15 +271,15 @@
 
 class Customer(HashModel):
     first_name: str
     last_name: str = Field(index=True)
     email: EmailStr
     join_date: datetime.date
     age: int = Field(index=True)
-    bio: Optional[str]
+    bio: Optional[str] = None
 
 
 # Now, if we use this model with a Redis deployment that has the
 # RediSearch module installed, we can run queries like the following.
 
 # Before running queries, we need to run migrations to set up the
 # indexes that Redis OM will use. You can also use the `migrate`
@@ -321,15 +321,15 @@
     Field,
     Migrator,
 )
 
 
 class Address(EmbeddedJsonModel):
     address_line_1: str
-    address_line_2: Optional[str]
+    address_line_2: Optional[str] = None
     city: str = Field(index=True)
     state: str = Field(index=True)
     country: str
     postal_code: str = Field(index=True)
 
 
 class Customer(JsonModel):
```

