# Comparing `tmp/pycrdt-0.8.8.tar.gz` & `tmp/pycrdt-0.8.9.tar.gz`

## Comparing `pycrdt-0.8.8.tar` & `pycrdt-0.8.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      179 1970-01-01 00:00:00.000000 pycrdt-0.8.8/Cargo.toml
--rw-r--r--   0      501       20     5017 2024-02-05 15:24:30.000000 pycrdt-0.8.8/.github/workflows/publish.yml
--rw-r--r--   0      501       20     1168 2024-02-05 15:24:30.000000 pycrdt-0.8.8/.github/workflows/test.yml
--rw-r--r--   0      501       20      216 2024-02-05 15:24:30.000000 pycrdt-0.8.8/.pre-commit-config.yaml
--rw-r--r--   0      501       20     1081 2024-02-05 15:24:30.000000 pycrdt-0.8.8/LICENSE
--rw-r--r--   0      501       20      719 2024-02-05 15:24:30.000000 pycrdt-0.8.8/README.md
--rw-r--r--   0      501       20     1167 2024-02-05 15:24:30.000000 pycrdt-0.8.8/docs/index.md
--rw-r--r--   0      501       20     1535 2024-02-05 15:24:30.000000 pycrdt-0.8.8/docs/install.md
--rw-r--r--   0      501       20     5986 2024-02-05 15:24:30.000000 pycrdt-0.8.8/docs/usage.md
--rw-r--r--   0      501       20       81 2024-02-05 15:24:30.000000 pycrdt-0.8.8/environment-dev.yml
--rw-r--r--   0      501       20      769 2024-02-05 15:24:30.000000 pycrdt-0.8.8/mkdocs.yml
--rw-r--r--   0      501       20      414 2024-02-05 15:24:30.000000 pycrdt-0.8.8/python/pycrdt/__init__.py
--rw-r--r--   0      501       20     6467 2024-02-05 15:24:30.000000 pycrdt-0.8.8/python/pycrdt/_pycrdt.pyi
--rw-r--r--   0      501       20     7987 2024-02-05 15:24:30.000000 pycrdt-0.8.8/python/pycrdt/array.py
--rw-r--r--   0      501       20     4750 2024-02-05 15:24:30.000000 pycrdt-0.8.8/python/pycrdt/base.py
--rw-r--r--   0      501       20     3183 2024-02-05 15:24:30.000000 pycrdt-0.8.8/python/pycrdt/doc.py
--rw-r--r--   0      501       20     5613 2024-02-05 15:24:30.000000 pycrdt-0.8.8/python/pycrdt/map.py
--rw-r--r--   0      501       20        0 2024-02-05 15:24:30.000000 pycrdt-0.8.8/python/pycrdt/py.typed
--rw-r--r--   0      501       20     5075 2024-02-05 15:24:30.000000 pycrdt-0.8.8/python/pycrdt/text.py
--rw-r--r--   0      501       20     1277 2024-02-05 15:24:30.000000 pycrdt-0.8.8/python/pycrdt/transaction.py
--rw-r--r--   0      501       20     8096 2024-02-05 15:24:30.000000 pycrdt-0.8.8/src/array.rs
--rw-r--r--   0      501       20     8588 2024-02-05 15:24:30.000000 pycrdt-0.8.8/src/doc.rs
--rw-r--r--   0      501       20      733 2024-02-05 15:24:30.000000 pycrdt-0.8.8/src/lib.rs
--rw-r--r--   0      501       20     8242 2024-02-05 15:24:30.000000 pycrdt-0.8.8/src/map.rs
--rw-r--r--   0      501       20     4786 2024-02-05 15:24:30.000000 pycrdt-0.8.8/src/text.rs
--rw-r--r--   0      501       20     1600 2024-02-05 15:24:30.000000 pycrdt-0.8.8/src/transaction.rs
--rw-r--r--   0      501       20     8782 2024-02-05 15:24:30.000000 pycrdt-0.8.8/src/type_conversions.rs
--rw-r--r--   0      501       20     5386 2024-02-05 15:24:30.000000 pycrdt-0.8.8/tests/test_array.py
--rw-r--r--   0      501       20     4106 2024-02-05 15:24:30.000000 pycrdt-0.8.8/tests/test_doc.py
--rw-r--r--   0      501       20     3665 2024-02-05 15:24:30.000000 pycrdt-0.8.8/tests/test_map.py
--rw-r--r--   0      501       20     1792 2024-02-05 15:24:30.000000 pycrdt-0.8.8/tests/test_model.py
--rw-r--r--   0      501       20     3663 2024-02-05 15:24:30.000000 pycrdt-0.8.8/tests/test_text.py
--rw-r--r--   0      501       20      860 2024-02-05 15:24:30.000000 pycrdt-0.8.8/tests/test_transaction.py
--rw-r--r--   0      501       20     2458 2024-02-05 15:24:30.000000 pycrdt-0.8.8/tests/test_ypy.py
--rw-r--r--   0      501       20    13522 2024-02-05 15:24:38.000000 pycrdt-0.8.8/Cargo.lock
--rw-r--r--   0      501       20     1440 2024-02-05 15:24:30.000000 pycrdt-0.8.8/pyproject.toml
--rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 pycrdt-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0      179 1970-01-01 00:00:00.000000 pycrdt-0.8.9/Cargo.toml
+-rw-r--r--   0      501       20     5017 2024-02-08 10:07:02.000000 pycrdt-0.8.9/.github/workflows/publish.yml
+-rw-r--r--   0      501       20     1168 2024-02-08 10:07:02.000000 pycrdt-0.8.9/.github/workflows/test.yml
+-rw-r--r--   0      501       20      215 2024-02-08 10:07:02.000000 pycrdt-0.8.9/.pre-commit-config.yaml
+-rw-r--r--   0      501       20     1081 2024-02-08 10:07:02.000000 pycrdt-0.8.9/LICENSE
+-rw-r--r--   0      501       20      719 2024-02-08 10:07:02.000000 pycrdt-0.8.9/README.md
+-rw-r--r--   0      501       20     1167 2024-02-08 10:07:02.000000 pycrdt-0.8.9/docs/index.md
+-rw-r--r--   0      501       20     1535 2024-02-08 10:07:02.000000 pycrdt-0.8.9/docs/install.md
+-rw-r--r--   0      501       20     5986 2024-02-08 10:07:02.000000 pycrdt-0.8.9/docs/usage.md
+-rw-r--r--   0      501       20       81 2024-02-08 10:07:02.000000 pycrdt-0.8.9/environment-dev.yml
+-rw-r--r--   0      501       20      769 2024-02-08 10:07:02.000000 pycrdt-0.8.9/mkdocs.yml
+-rw-r--r--   0      501       20      423 2024-02-08 10:07:02.000000 pycrdt-0.8.9/python/pycrdt/__init__.py
+-rw-r--r--   0      501       20     7989 2024-02-08 10:07:02.000000 pycrdt-0.8.9/python/pycrdt/_array.py
+-rw-r--r--   0      501       20     4752 2024-02-08 10:07:02.000000 pycrdt-0.8.9/python/pycrdt/_base.py
+-rw-r--r--   0      501       20     3185 2024-02-08 10:07:02.000000 pycrdt-0.8.9/python/pycrdt/_doc.py
+-rw-r--r--   0      501       20     5615 2024-02-08 10:07:02.000000 pycrdt-0.8.9/python/pycrdt/_map.py
+-rw-r--r--   0      501       20     6467 2024-02-08 10:07:02.000000 pycrdt-0.8.9/python/pycrdt/_pycrdt.pyi
+-rw-r--r--   0      501       20     5077 2024-02-08 10:07:02.000000 pycrdt-0.8.9/python/pycrdt/_text.py
+-rw-r--r--   0      501       20     1278 2024-02-08 10:07:02.000000 pycrdt-0.8.9/python/pycrdt/_transaction.py
+-rw-r--r--   0      501       20        0 2024-02-08 10:07:02.000000 pycrdt-0.8.9/python/pycrdt/py.typed
+-rw-r--r--   0      501       20     8096 2024-02-08 10:07:02.000000 pycrdt-0.8.9/src/array.rs
+-rw-r--r--   0      501       20     8588 2024-02-08 10:07:02.000000 pycrdt-0.8.9/src/doc.rs
+-rw-r--r--   0      501       20      733 2024-02-08 10:07:02.000000 pycrdt-0.8.9/src/lib.rs
+-rw-r--r--   0      501       20     8242 2024-02-08 10:07:02.000000 pycrdt-0.8.9/src/map.rs
+-rw-r--r--   0      501       20     4786 2024-02-08 10:07:02.000000 pycrdt-0.8.9/src/text.rs
+-rw-r--r--   0      501       20     1600 2024-02-08 10:07:02.000000 pycrdt-0.8.9/src/transaction.rs
+-rw-r--r--   0      501       20     8782 2024-02-08 10:07:02.000000 pycrdt-0.8.9/src/type_conversions.rs
+-rw-r--r--   0      501       20     5386 2024-02-08 10:07:02.000000 pycrdt-0.8.9/tests/test_array.py
+-rw-r--r--   0      501       20     4106 2024-02-08 10:07:02.000000 pycrdt-0.8.9/tests/test_doc.py
+-rw-r--r--   0      501       20     3665 2024-02-08 10:07:02.000000 pycrdt-0.8.9/tests/test_map.py
+-rw-r--r--   0      501       20     1792 2024-02-08 10:07:02.000000 pycrdt-0.8.9/tests/test_model.py
+-rw-r--r--   0      501       20     3663 2024-02-08 10:07:02.000000 pycrdt-0.8.9/tests/test_text.py
+-rw-r--r--   0      501       20      860 2024-02-08 10:07:02.000000 pycrdt-0.8.9/tests/test_transaction.py
+-rw-r--r--   0      501       20     2458 2024-02-08 10:07:02.000000 pycrdt-0.8.9/tests/test_ypy.py
+-rw-r--r--   0      501       20    13522 2024-02-08 10:07:20.000000 pycrdt-0.8.9/Cargo.lock
+-rw-r--r--   0      501       20     1440 2024-02-08 10:07:02.000000 pycrdt-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 pycrdt-0.8.9/PKG-INFO
```

### Comparing `pycrdt-0.8.8/.github/workflows/publish.yml` & `pycrdt-0.8.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/.github/workflows/test.yml` & `pycrdt-0.8.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/LICENSE` & `pycrdt-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/README.md` & `pycrdt-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/docs/index.md` & `pycrdt-0.8.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/docs/install.md` & `pycrdt-0.8.9/docs/install.md`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/docs/usage.md` & `pycrdt-0.8.9/docs/usage.md`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/mkdocs.yml` & `pycrdt-0.8.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/python/pycrdt/_pycrdt.pyi` & `pycrdt-0.8.9/python/pycrdt/_pycrdt.pyi`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/python/pycrdt/array.py` & `pycrdt-0.8.9/python/pycrdt/_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable
 
+from ._base import BaseDoc, BaseEvent, BaseType, base_types, event_types
 from ._pycrdt import Array as _Array
 from ._pycrdt import ArrayEvent as _ArrayEvent
-from .base import BaseDoc, BaseEvent, BaseType, base_types, event_types
 
 if TYPE_CHECKING:  # pragma: no cover
-    from .doc import Doc
+    from ._doc import Doc
 
 
 class Array(BaseType):
     _prelim: list | None
     _integrated: _Array | None
 
     def __init__(
```

### Comparing `pycrdt-0.8.8/python/pycrdt/base.py` & `pycrdt-0.8.9/python/pycrdt/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Type, cast
 
 from ._pycrdt import Doc as _Doc
 from ._pycrdt import Transaction as _Transaction
-from .transaction import ReadTransaction, Transaction
+from ._transaction import ReadTransaction, Transaction
 
 if TYPE_CHECKING:  # pragma: no cover
-    from .doc import Doc
+    from ._doc import Doc
 
 
 base_types: dict[Any, Type[BaseType | BaseDoc]] = {}
 event_types: dict[Any, Type[BaseEvent]] = {}
 
 
 class BaseDoc:
```

### Comparing `pycrdt-0.8.8/python/pycrdt/doc.py` & `pycrdt-0.8.9/python/pycrdt/_doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import Callable, Type, cast
 
+from ._base import BaseDoc, BaseType, base_types
 from ._pycrdt import Doc as _Doc
 from ._pycrdt import SubdocsEvent, TransactionEvent
 from ._pycrdt import Transaction as _Transaction
-from .base import BaseDoc, BaseType, base_types
-from .transaction import ReadTransaction, Transaction
+from ._transaction import ReadTransaction, Transaction
 
 
 class Doc(BaseDoc):
     def __init__(
         self,
         init: dict[str, BaseType] = {},
         *,
```

### Comparing `pycrdt-0.8.8/python/pycrdt/map.py` & `pycrdt-0.8.9/python/pycrdt/_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable
 
+from ._base import BaseDoc, BaseEvent, BaseType, base_types, event_types
 from ._pycrdt import Map as _Map
 from ._pycrdt import MapEvent as _MapEvent
-from .base import BaseDoc, BaseEvent, BaseType, base_types, event_types
 
 if TYPE_CHECKING:  # pragma: no cover
-    from .doc import Doc
+    from ._doc import Doc
 
 
 class Map(BaseType):
     _prelim: dict | None
     _integrated: _Map | None
 
     def __init__(
```

### Comparing `pycrdt-0.8.8/python/pycrdt/text.py` & `pycrdt-0.8.9/python/pycrdt/_text.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable
 
+from ._base import BaseEvent, BaseType, base_types, event_types
 from ._pycrdt import Text as _Text
 from ._pycrdt import TextEvent as _TextEvent
-from .base import BaseEvent, BaseType, base_types, event_types
 
 if TYPE_CHECKING:  # pragma: no cover
-    from .doc import Doc
+    from ._doc import Doc
 
 
 class Text(BaseType):
     _prelim: str | None
     _integrated: _Text | None
 
     def __init__(
```

### Comparing `pycrdt-0.8.8/python/pycrdt/transaction.py` & `pycrdt-0.8.9/python/pycrdt/_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from types import TracebackType
 from typing import TYPE_CHECKING
 
 from ._pycrdt import Transaction as _Transaction
 
 if TYPE_CHECKING:  # pragma: no cover
-    from .doc import Doc
+    from ._doc import Doc
 
 
 class Transaction:
     _doc: Doc
     _txn: _Transaction | None
     _nb: int
```

### Comparing `pycrdt-0.8.8/src/array.rs` & `pycrdt-0.8.9/src/array.rs`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/src/doc.rs` & `pycrdt-0.8.9/src/doc.rs`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/src/lib.rs` & `pycrdt-0.8.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/src/map.rs` & `pycrdt-0.8.9/src/map.rs`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/src/text.rs` & `pycrdt-0.8.9/src/text.rs`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/src/transaction.rs` & `pycrdt-0.8.9/src/transaction.rs`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/src/type_conversions.rs` & `pycrdt-0.8.9/src/type_conversions.rs`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/tests/test_array.py` & `pycrdt-0.8.9/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/tests/test_doc.py` & `pycrdt-0.8.9/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/tests/test_map.py` & `pycrdt-0.8.9/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/tests/test_model.py` & `pycrdt-0.8.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/tests/test_text.py` & `pycrdt-0.8.9/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/tests/test_transaction.py` & `pycrdt-0.8.9/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/tests/test_ypy.py` & `pycrdt-0.8.9/tests/test_ypy.py`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/Cargo.lock` & `pycrdt-0.8.9/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,17 @@
 name = "itoa"
 version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
 
 [[package]]
 name = "js-sys"
-version = "0.3.67"
+version = "0.3.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a1d36f1235bc969acba30b7f5990b864423a6068a10f7c90ae8f0112e3a59d1"
+checksum = "406cda4b368d531c842222cf9d2600a9a4acce8d29423695379c6868a143a9ee"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.153"
@@ -145,15 +145,15 @@
 checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pycrdt"
-version = "0.8.8"
+version = "0.8.9"
 dependencies = [
  "pyo3",
  "yrs",
 ]
 
 [[package]]
 name = "pyo3"
@@ -386,65 +386,65 @@
 name = "wasi"
 version = "0.9.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cccddf32554fecc6acb585f82a32a72e28b48f8c4c1883ddfeeeaa96f7d8e519"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.90"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1223296a201415c7fad14792dbefaace9bd52b62d33453ade1c5b5f07555406"
+checksum = "c1e124130aee3fb58c5bdd6b639a0509486b0338acaaae0c84a5124b0f588b7f"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.90"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcdc935b63408d58a32f8cc9738a0bffd8f05cc7c002086c6ef20b7312ad9dcd"
+checksum = "c9e7e1900c352b609c8488ad12639a311045f40a35491fb69ba8c12f758af70b"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.90"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e4c238561b2d428924c49815533a8b9121c664599558a5d9ec51f8a1740a999"
+checksum = "b30af9e2d358182b5c7449424f017eba305ed32a7010509ede96cdc4696c46ed"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.90"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bae1abb6806dc1ad9e560ed242107c0f6c84335f1749dd4e8ddb012ebd5e25a7"
+checksum = "642f325be6301eb8107a83d12a8ac6c1e1c54345a7ef1a9261962dfefda09e66"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.90"
+version = "0.2.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d91413b1c31d7539ba5ef2451af3f0b833a005eb27a631cec32bc0635a8602b"
+checksum = "4f186bd2dcf04330886ce82d6f33dd75a7bfcf69ecf5763b89fcde53b6ac9838"
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
```

### Comparing `pycrdt-0.8.8/pyproject.toml` & `pycrdt-0.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycrdt-0.8.8/PKG-INFO` & `pycrdt-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrdt
-Version: 0.8.8
+Version: 0.8.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

