# Comparing `tmp/py_grpcio-1.1.1.tar.gz` & `tmp/py_grpcio-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_grpcio-1.1.1.tar", max compression
+gzip compressed data, was "py_grpcio-1.2.1.tar", max compression
```

## Comparing `py_grpcio-1.1.1.tar` & `py_grpcio-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1076 2024-05-01 13:30:07.396767 py_grpcio-1.1.1/LICENSE
--rw-r--r--   0        0        0     2836 2024-05-01 13:30:07.396767 py_grpcio-1.1.1/README.md
--rw-r--r--   0        0        0      119 2024-05-01 13:30:07.400767 py_grpcio-1.1.1/py_grpcio/__init__.py
--rw-r--r--   0        0        0      277 2024-05-01 13:30:07.400767 py_grpcio-1.1.1/py_grpcio/exceptions.py
--rw-r--r--   0        0        0     1422 2024-05-01 13:30:07.400767 py_grpcio-1.1.1/py_grpcio/interceptor.py
--rw-r--r--   0        0        0     2769 2024-05-01 13:30:07.400767 py_grpcio-1.1.1/py_grpcio/method.py
--rw-r--r--   0        0        0     3263 2024-05-01 13:30:07.400767 py_grpcio-1.1.1/py_grpcio/models.py
--rw-r--r--   0        0        0      114 2024-05-01 13:30:07.400767 py_grpcio-1.1.1/py_grpcio/proto/__init__.py
--rw-r--r--   0        0        0      483 2024-05-01 13:30:07.400767 py_grpcio-1.1.1/py_grpcio/proto/enums.py
--rw-r--r--   0        0        0     3685 2024-05-01 13:30:07.400767 py_grpcio-1.1.1/py_grpcio/proto/parser.py
--rw-r--r--   0        0        0      682 2024-05-01 13:30:07.400767 py_grpcio-1.1.1/py_grpcio/proto/templates/service.proto.template
--rw-r--r--   0        0        0     1873 2024-05-01 13:30:07.400767 py_grpcio-1.1.1/py_grpcio/server.py
--rw-r--r--   0        0        0      924 2024-05-01 13:30:07.400767 py_grpcio-1.1.1/py_grpcio/service.py
--rw-r--r--   0        0        0     2402 2024-05-01 13:30:07.400767 py_grpcio-1.1.1/py_grpcio/service_meta.py
--rw-r--r--   0        0        0      582 2024-05-01 13:30:07.400767 py_grpcio-1.1.1/py_grpcio/utils.py
--rw-r--r--   0        0        0      573 2024-05-01 13:30:07.400767 py_grpcio-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3577 1970-01-01 00:00:00.000000 py_grpcio-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2836 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/README.md
+-rw-r--r--   0        0        0      119 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/exceptions.py
+-rw-r--r--   0        0        0     1422 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/interceptor.py
+-rw-r--r--   0        0        0     2769 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/method.py
+-rw-r--r--   0        0        0     3263 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/models.py
+-rw-r--r--   0        0        0      114 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/proto/__init__.py
+-rw-r--r--   0        0        0      483 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/proto/enums.py
+-rw-r--r--   0        0        0     3685 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/proto/parser.py
+-rw-r--r--   0        0        0      682 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/proto/templates/service.proto.template
+-rw-r--r--   0        0        0     1873 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/server.py
+-rw-r--r--   0        0        0      924 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/service.py
+-rw-r--r--   0        0        0     2417 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/service_meta.py
+-rw-r--r--   0        0        0      582 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/py_grpcio/utils.py
+-rw-r--r--   0        0        0      573 2024-05-02 21:50:16.619614 py_grpcio-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3577 1970-01-01 00:00:00.000000 py_grpcio-1.2.1/PKG-INFO
```

### Comparing `py_grpcio-1.1.1/LICENSE` & `py_grpcio-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.1.1/README.md` & `py_grpcio-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.1.1/py_grpcio/interceptor.py` & `py_grpcio-1.2.1/py_grpcio/interceptor.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.1.1/py_grpcio/method.py` & `py_grpcio-1.2.1/py_grpcio/method.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.1.1/py_grpcio/models.py` & `py_grpcio-1.2.1/py_grpcio/models.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.1.1/py_grpcio/proto/parser.py` & `py_grpcio-1.2.1/py_grpcio/proto/parser.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.1.1/py_grpcio/proto/templates/service.proto.template` & `py_grpcio-1.2.1/py_grpcio/proto/templates/service.proto.template`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.1.1/py_grpcio/server.py` & `py_grpcio-1.2.1/py_grpcio/server.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.1.1/py_grpcio/service.py` & `py_grpcio-1.2.1/py_grpcio/service.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.1.1/py_grpcio/service_meta.py` & `py_grpcio-1.2.1/py_grpcio/service_meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         cls.name: str = name
         cls.methods: dict[str, Method] = {}
         cls.messages: dict[str, Type[Message]] = {}
         cls.protos: ModuleType | None = None
         cls.services: ModuleType | None = None
 
     def __getattr__(cls: 'BaseServiceMeta', attr_name: str) -> ServerMethodGRPC | Any:
-        if method := cls.methods.get(attr_name.lower()):
+        if method := cls.methods.get(camel_to_snake(string=attr_name)):
             return ServerMethodGRPC(method=method)
         return getattr(cls, attr_name)
 
     def methods_and_messages(cls: 'BaseServiceMeta') -> None:
         for method_name, target in cls.__dict__.items():
             if is_method(method=target):
                 method: Method = Method.from_target(target=target)
```

### Comparing `py_grpcio-1.1.1/py_grpcio/utils.py` & `py_grpcio-1.2.1/py_grpcio/utils.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.1.1/pyproject.toml` & `py_grpcio-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-grpcio"
-version = "1.1.1"
+version = "1.2.1"
 description = "gRPC with autogen by Pydantic models"
 authors = ["Yurii <ykolibroda@lytvynov-production.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "py_grpcio" },
 ]
```

### Comparing `py_grpcio-1.1.1/PKG-INFO` & `py_grpcio-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-grpcio
-Version: 1.1.1
+Version: 1.2.1
 Summary: gRPC with autogen by Pydantic models
 License: MIT
 Author: Yurii
 Author-email: ykolibroda@lytvynov-production.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

