# Comparing `tmp/skytable_py-0.1.1.tar.gz` & `tmp/skytable_py-0.1.2.tar.gz`

## Comparing `skytable_py-0.1.1.tar` & `skytable_py-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 skytable_py-0.1.1/run_tests.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 skytable_py-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 skytable_py-0.1.1/src/skytable_py/__init__.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 skytable_py-0.1.1/src/skytable_py/config.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 skytable_py-0.1.1/src/skytable_py/connection.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 skytable_py-0.1.1/src/skytable_py/exception.py
--rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 skytable_py-0.1.1/src/skytable_py/protocol.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 skytable_py-0.1.1/src/skytable_py/query.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 skytable_py-0.1.1/src/skytable_py/response.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 skytable_py-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 skytable_py-0.1.1/tests/test_config.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 skytable_py-0.1.1/tests/test_encoding.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 skytable_py-0.1.1/tests/test_protocol.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 skytable_py-0.1.1/tests/test_query.py
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 skytable_py-0.1.1/tests/test_response.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 skytable_py-0.1.1/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 skytable_py-0.1.1/LICENSE
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 skytable_py-0.1.1/README.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 skytable_py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 skytable_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 skytable_py-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 skytable_py-0.1.2/run_tests.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 skytable_py-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 skytable_py-0.1.2/src/skytable_py/__init__.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 skytable_py-0.1.2/src/skytable_py/config.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 skytable_py-0.1.2/src/skytable_py/connection.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 skytable_py-0.1.2/src/skytable_py/exception.py
+-rw-r--r--   0        0        0     8927 2020-02-02 00:00:00.000000 skytable_py-0.1.2/src/skytable_py/protocol.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 skytable_py-0.1.2/src/skytable_py/query.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 skytable_py-0.1.2/src/skytable_py/response.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 skytable_py-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 skytable_py-0.1.2/tests/test_config.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 skytable_py-0.1.2/tests/test_encoding.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 skytable_py-0.1.2/tests/test_protocol.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 skytable_py-0.1.2/tests/test_query.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 skytable_py-0.1.2/tests/test_response.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 skytable_py-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 skytable_py-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 skytable_py-0.1.2/README.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 skytable_py-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 skytable_py-0.1.2/PKG-INFO
```

### Comparing `skytable_py-0.1.1/run_tests.py` & `skytable_py-0.1.2/run_tests.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.1/.github/workflows/test.yml` & `skytable_py-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.1/src/skytable_py/__init__.py` & `skytable_py-0.1.2/src/skytable_py/__init__.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.1/src/skytable_py/config.py` & `skytable_py-0.1.2/src/skytable_py/config.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.1/src/skytable_py/connection.py` & `skytable_py-0.1.2/src/skytable_py/connection.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.1/src/skytable_py/exception.py` & `skytable_py-0.1.2/src/skytable_py/exception.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.1/src/skytable_py/protocol.py` & `skytable_py-0.1.2/src/skytable_py/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Union
+from typing import Union, List
 from .exception import ProtocolException
 from .response import Value, UInt8, UInt16, UInt32, UInt64, SInt8, SInt16, SInt32, SInt64, Float32, Float64, Empty, \
     ErrorCode, Row, Response
 
 
 class Protocol:
     def __init__(self, buffer=bytes()) -> None:
@@ -141,24 +141,36 @@
                 return Value(SInt64(integer))
         else:
             self.__decrement()  # move back to type symbol
             if is_negative:
                 self.__decrement()  # move back to starting position of this integer
 
     def parse_float(self, type_symbol: int) -> Union[None, Value]:
+        if self.__is_eof():
+            self.__decrement()  # move back to type symbol
+            return None
+        is_negative = False
+        if self.__step() == ord('-'):
+            is_negative = True
+        else:
+            self.__decrement()  # move back to float starting position since there is no '-'
         whole = self.parse_next_int(stop_symbol='.')
         if whole:
             decimal = self.parse_next_int()
             if decimal:
                 full_float = float(f"{whole}.{decimal}")
+                if is_negative:
+                    full_float = -full_float
                 if type_symbol == 10:
                     return Value(Float32(full_float))
                 else:
                     return Value(Float64(full_float))
         self.__decrement()  # type symbol
+        if is_negative:
+            self.__decrement()
 
     def parse_error_code(self) -> Union[None, ErrorCode]:
         if self.__remaining() < 2:
             self.__decrement()  # type symbol
         else:
             a, b = self.__buf()
             self.__increment_cursor_by(2)
@@ -192,15 +204,15 @@
             if column:
                 columns.append(column)
             else:
                 self._cursor = cursor_start
                 return None
         return Row(columns)
 
-    def parse_rows(self) -> Union[None, list[Row]]:
+    def parse_rows(self) -> Union[None, List[Row]]:
         cursor_start = self._cursor - 1
         row_count = self.parse_next_int()
         rows = []
         while len(rows) != row_count:
             row = self.parse_row()
             if row:
                 rows.append(row)
```

### Comparing `skytable_py-0.1.1/src/skytable_py/query.py` & `skytable_py-0.1.2/src/skytable_py/query.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.1/src/skytable_py/response.py` & `skytable_py-0.1.2/src/skytable_py/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
-from typing import Union
+from typing import Union, List
 from .exception import ClientException
 
 
 @dataclass
 class UInt8:
     inner: int
 
@@ -132,43 +132,43 @@
     def __eq__(self, other):
         if isinstance(other, Value):
             return self.data() == other.data()
         return False
 
 
 class Row:
-    def __init__(self, values: list[Value]) -> None:
+    def __init__(self, values: List[Value]) -> None:
         self.columns = values
 
     def __eq__(self, other):
         if isinstance(other, Row):
             return self.columns == other.columns
         return False
 
 
 @dataclass
 class ErrorCode:
     inner: int
 
 
 class Response:
-    def __init__(self, resp: Union[Empty, Value, Row, list[Row], ErrorCode]):
+    def __init__(self, resp: Union[Empty, Value, Row, List[Row], ErrorCode]):
         self.data = resp
 
     def is_empty(self) -> bool:
         return isinstance(self.data, Empty)
 
     def value(self) -> Union[None, Value]:
         if isinstance(self.data, Value):
             return self.data
 
     def row(self) -> Union[None, Row]:
         if isinstance(self.data, Row):
             return self.data
 
-    def rows(self) -> Union[None, list[Row]]:
+    def rows(self) -> Union[None, List[Row]]:
         if isinstance(self.data, list):
             return self.data
 
     def error(self) -> Union[None, int]:
         if isinstance(self.data, ErrorCode):
             return self.data.inner
```

### Comparing `skytable_py-0.1.1/tests/__init__.py` & `skytable_py-0.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.1/tests/test_config.py` & `skytable_py-0.1.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.1/tests/test_encoding.py` & `skytable_py-0.1.2/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.1/tests/test_protocol.py` & `skytable_py-0.1.2/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.1/tests/test_query.py` & `skytable_py-0.1.2/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.1/tests/test_response.py` & `skytable_py-0.1.2/tests/test_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,14 +55,18 @@
         self.assertEquals(Response(Value(SInt32(-1))).value().repr.inner, -1)
         self.assertEquals(Response(Value(SInt64(-1))).value().repr.inner, -1)
         # float
         self.assertEquals(Response(Value(Float32(3.141592654))
                                    ).value().repr.inner, 3.141592654)
         self.assertEquals(Response(Value(Float64(3.141592654))
                                    ).value().repr.inner, 3.141592654)
+        self.assertEquals(Response(Value(Float32(-3.141592654))
+                                   ).value().repr.inner, -3.141592654)
+        self.assertEquals(Response(Value(Float64(-3.141592654))
+                                   ).value().repr.inner, -3.141592654)
         # simple collections
         self.assertEquals(Response(Value(b"bytes")).value().repr, b"bytes")
         self.assertEquals(Response(Value("string")).value().repr, "string")
         # complex collections
         self.assertEquals(Response(Value([Value(b"bytes"), Value("string")])).value(
         ).repr, [Value(b"bytes"), Value("string")])
         # server error
```

### Comparing `skytable_py-0.1.1/LICENSE` & `skytable_py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.1/README.md` & `skytable_py-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `skytable_py-0.1.1/pyproject.toml` & `skytable_py-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "skytable-py"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name = "Sayan Nandan", email = "nandansayan@outlook.com" }]
 description = "Official Skytable client library for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `skytable_py-0.1.1/PKG-INFO` & `skytable_py-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: skytable-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Official Skytable client library for Python
 Project-URL: Homepage, https://github.com/skytable/skytable-py
 Project-URL: Issues, https://github.com/skytable/skytable-py/issues
 Author-email: Sayan Nandan <nandansayan@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

