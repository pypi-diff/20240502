# Comparing `tmp/drf_serializer_dumps-1.0.1.tar.gz` & `tmp/drf_serializer_dumps-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_serializer_dumps-1.0.1.tar", last modified: Mon Apr 29 21:14:03 2024, max compression
+gzip compressed data, was "drf_serializer_dumps-1.0.2.tar", last modified: Thu May  2 16:33:18 2024, max compression
```

## Comparing `drf_serializer_dumps-1.0.1.tar` & `drf_serializer_dumps-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:14:03.618229 drf_serializer_dumps-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:14:03.610229 drf_serializer_dumps-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:14:03.614230 drf_serializer_dumps-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-29 21:14:03.618229 drf_serializer_dumps-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12285 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 21:14:03.618229 drf_serializer_dumps-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:14:03.610229 drf_serializer_dumps-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:14:03.614230 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9949 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:14:03.614230 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-29 21:14:03.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-29 21:14:03.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 21:14:03.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 21:14:03.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-29 21:14:03.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 21:14:03.000000 drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:14:03.614230 drf_serializer_dumps-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/tests/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-29 21:13:58.000000 drf_serializer_dumps-1.0.1/tests/test_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:18.094249 drf_serializer_dumps-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:18.086249 drf_serializer_dumps-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:18.090249 drf_serializer_dumps-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11660 2024-05-02 16:33:18.094249 drf_serializer_dumps-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12378 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:33:18.094249 drf_serializer_dumps-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:18.086249 drf_serializer_dumps-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:18.090249 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:18.090249 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11660 2024-05-02 16:33:18.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-02 16:33:18.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:33:18.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 16:33:18.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-02 16:33:18.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 16:33:18.000000 drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:18.090249 drf_serializer_dumps-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/tests/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-02 16:33:13.000000 drf_serializer_dumps-1.0.2/tests/test_decorators.py
```

### Comparing `drf_serializer_dumps-1.0.1/.editorconfig` & `drf_serializer_dumps-1.0.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.1/.github/workflows/publish-to-pypi.yml` & `drf_serializer_dumps-1.0.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.1/.pre-commit-config.yaml` & `drf_serializer_dumps-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.1/CONTRIBUTING.md` & `drf_serializer_dumps-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.1/LICENSE` & `drf_serializer_dumps-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.1/PKG-INFO` & `drf_serializer_dumps-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf_serializer_dumps
-Version: 1.0.1
+Version: 1.0.2
 Summary: Decorator for creating dict based on the drf serializer class for swagger
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,14 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Documentation, https://github.com/Friskes/drf-serializer-dumps
 Project-URL: Repository, https://github.com/Friskes/drf-serializer-dumps
 Project-URL: Changelog, https://github.com/Friskes/drf-serializer-dumps/releases/
 Project-URL: Bug Reports, https://github.com/Friskes/drf-serializer-dumps/issues
 Keywords: Django,DRF,Spectacular,Swagger
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `drf_serializer_dumps-1.0.1/README.md` & `drf_serializer_dumps-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.1/pyproject.toml` & `drf_serializer_dumps-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     "pytest>=7.0.1",
     "mypy>=1.10.0",
     "pytest-cov>=5.0.0",
 ]
 
 
 [project.urls]
+"Documentation" = "https://github.com/Friskes/drf-serializer-dumps"  # Home-page in pip show
 "Repository" = "https://github.com/Friskes/drf-serializer-dumps"
 "Changelog" = "https://github.com/Friskes/drf-serializer-dumps/releases/"
 "Bug Reports" = "https://github.com/Friskes/drf-serializer-dumps/issues"
 
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=8"]
```

### Comparing `drf_serializer_dumps-1.0.1/src/drf_serializer_dumps/decorators.py` & `drf_serializer_dumps-1.0.2/src/drf_serializer_dumps/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 from rest_framework import serializers
 
 if TYPE_CHECKING:
     from collections import OrderedDict
 
     from drf_spectacular.utils import _SerializerType
 
+try:
+    from types import UnionType  # type: ignore[attr-defined]
+except ImportError:
+    UnionType = Union
+
 __all__ = ('serializer_dumps',)
 
 _uuid = uuid4()
 _now = timezone.now()
 
 
 def serializer_dumps(
@@ -148,16 +153,16 @@
 
         # annotation = inspect.signature(method).return_annotation
         # annotation = None if annotation is inspect._empty else annotation
 
         annotation = get_type_hints(method).get('return')
 
         # origin = get_origin(annotation)
-        # if origin is Union or origin is type(Union):
-        if get_origin(annotation) in (Union, type(Union)):
+        # if origin is Union or origin is UnionType:
+        if get_origin(annotation) in (Union, UnionType):
             annotation = get_args(annotation)[0]
 
         type_value = type_mapping.get(open_api_type)
         if type_value is None:
             type_value = type_mapping.get(annotation)
 
         return type_value, annotation
@@ -214,20 +219,20 @@
                     else:
                         example_val[field_name] = type_value
                         print(
                             f'Обнаружена неизвестная аннотация: "{annotation.__name__}" '
                             f'у поля: "{field_name}".'
                         )
                 else:
-                    if issubclass(annotation, serializers.Serializer):
+                    if annotation is not None and issubclass(annotation, serializers.Serializer):
                         example_val[field_name] = _walk_fields_recursively(annotation, exclude_fields)
                     else:
                         example_val[field_name] = None
                         print(
-                            f'Обнаружена неизвестная аннотация: "{annotation.__name__}" '
+                            f'Обнаружена неизвестная аннотация: "{type(annotation).__name__}" '
                             f'Для поля: "{field_name}" было установлено значение "None".'
                         )
             else:
                 example_val[field_name] = None
                 print(
                     f'Обнаружено неизвестное поле: "{type(field_instance).__name__}" '
                     f'Для поля: "{field_name}" было установлено значение "None".'
```

### Comparing `drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/PKG-INFO` & `drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf_serializer_dumps
-Version: 1.0.1
+Version: 1.0.2
 Summary: Decorator for creating dict based on the drf serializer class for swagger
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,14 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: Documentation, https://github.com/Friskes/drf-serializer-dumps
 Project-URL: Repository, https://github.com/Friskes/drf-serializer-dumps
 Project-URL: Changelog, https://github.com/Friskes/drf-serializer-dumps/releases/
 Project-URL: Bug Reports, https://github.com/Friskes/drf-serializer-dumps/issues
 Keywords: Django,DRF,Spectacular,Swagger
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `drf_serializer_dumps-1.0.1/src/drf_serializer_dumps.egg-info/SOURCES.txt` & `drf_serializer_dumps-1.0.2/src/drf_serializer_dumps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.1/tests/test_decorators.py` & `drf_serializer_dumps-1.0.2/tests/test_decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # pytest -s ./tests
 def test_serializer_dumps() -> None:
     """"""
     result = serializer_dumps(PersonSerializer1, exclude_fields=['age'])
     assert result == {
         'name': 'string',
         'birthday': ANY,
+        'field_without_annotation': None,
         'height': 1,
         'weight': 1,
         'cars': [{'car_name': 'string', 'car_price': 1}],
         'house': {'address': 'string'},
     }
 
 
@@ -29,14 +30,15 @@
 
 def test_renew_type_value() -> None:
     """"""
     expected = {
         'name': 'string',
         'age': 1,
         'birthday': ANY,
+        'field_without_annotation': None,
         'height': 1,
         'weight': 1,
         'cars': [{'car_name': 'string', 'car_price': 1}],
         'house': {'address': 'string'},
     }
 
     result1 = serializer_dumps(PersonSerializer1, renew_type_value=True)
```

