# Comparing `tmp/huffify-0.1.1.tar.gz` & `tmp/huffify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huffify-0.1.1.tar", max compression
+gzip compressed data, was "huffify-0.2.0.tar", max compression
```

## Comparing `huffify-0.1.1.tar` & `huffify-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-04-20 16:45:06.233524 huffify-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2024-04-20 16:45:06.233524 huffify-0.1.1/README.md
--rw-r--r--   0        0        0      846 2024-04-20 16:45:06.233524 huffify-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       65 2024-04-20 16:45:06.233524 huffify-0.1.1/src/huffify/__init__.py
--rw-r--r--   0        0        0      654 2024-04-20 16:45:06.233524 huffify-0.1.1/src/huffify/abstract.py
--rw-r--r--   0        0        0      111 2024-04-20 16:45:06.233524 huffify-0.1.1/src/huffify/annotations.py
--rw-r--r--   0        0        0     2691 2024-04-20 16:45:06.233524 huffify-0.1.1/src/huffify/encoders.py
--rw-r--r--   0        0        0      765 2024-04-20 16:45:06.233524 huffify-0.1.1/src/huffify/fileManger.py
--rw-r--r--   0        0        0      909 2024-04-20 16:45:06.233524 huffify-0.1.1/src/huffify/heapNodes.py
--rw-r--r--   0        0        0     2578 2024-04-20 16:45:06.233524 huffify-0.1.1/src/huffify/huffify.py
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 huffify-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-02 11:34:38.852537 huffify-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2314 2024-05-02 11:34:38.852537 huffify-0.2.0/README.md
+-rw-r--r--   0        0        0      885 2024-05-02 11:34:38.856537 huffify-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      101 2024-05-02 11:34:38.856537 huffify-0.2.0/src/huffify/__init__.py
+-rw-r--r--   0        0        0      699 2024-05-02 11:34:38.856537 huffify-0.2.0/src/huffify/abstract.py
+-rw-r--r--   0        0        0      111 2024-05-02 11:34:38.856537 huffify-0.2.0/src/huffify/annotations.py
+-rw-r--r--   0        0        0     2691 2024-05-02 11:34:38.856537 huffify-0.2.0/src/huffify/encoders.py
+-rw-r--r--   0        0        0     1191 2024-05-02 11:34:38.856537 huffify-0.2.0/src/huffify/fileManger.py
+-rw-r--r--   0        0        0      909 2024-05-02 11:34:38.856537 huffify-0.2.0/src/huffify/heapNodes.py
+-rw-r--r--   0        0        0     3445 2024-05-02 11:34:38.856537 huffify-0.2.0/src/huffify/huffify.py
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 huffify-0.2.0/PKG-INFO
```

### Comparing `huffify-0.1.1/LICENSE` & `huffify-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `huffify-0.1.1/pyproject.toml` & `huffify-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huffify"
-version = "0.1.1"
+version = "0.2.0"
 description = "Simple Huffman algotithm implementation"
 authors = ["munwriter <glebvysokov3@gmail.com>"]
 keywords = ["huffman", "compression", "encoding", "decoding"]
 repository = "https://github.com/munwriter/Huffify"
 license = "MIT"
 readme = "README.md"
 
@@ -13,14 +13,15 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 black = "^23.12.1"
 mypy = "^1.8.0"
 isort = "^5.13.2"
 ruff = "^0.3.5"
+pytest-cov = "^5.0.0"
 
 [tool.mypy]
 python_version = "3.12"
 strict = false
 mypy_path = "./src"
 exclude = "tests"
 
@@ -38,8 +39,9 @@
 line-length=95
 target-version = "py312"
 show-fixes = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-exclude = "/tests"
+exclude = "/tests"
+include = "/src"
```

### Comparing `huffify-0.1.1/src/huffify/abstract.py` & `huffify-0.2.0/src/huffify/abstract.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 
 
-class PersistenceManager(metaclass=ABCMeta):
+class IPersistenceManager(metaclass=ABCMeta):
+    @staticmethod
     @abstractmethod
-    def save(self, data):
+    def save(path, encoded_data):
         pass
 
+    @staticmethod
     @abstractmethod
-    def load(self):
+    def load(path):
         pass
 
 
 @dataclass
 class INode(metaclass=ABCMeta):
     char: str
     freq: int
```

### Comparing `huffify-0.1.1/src/huffify/encoders.py` & `huffify-0.2.0/src/huffify/encoders.py`

 * *Files identical despite different names*

### Comparing `huffify-0.1.1/src/huffify/fileManger.py` & `huffify-0.2.0/src/huffify/fileManger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 import pickle
+from pathlib import Path
 
-from huffify.abstract import PersistenceManager
+from huffify.abstract import IPersistenceManager
 from huffify.annotations import FinalDataSet
 
 
-class Pickelifier(PersistenceManager):
+class PickleFileManager:
     def __init__(
         self,
-        input_path: str = "input.txt",
-        output_path: str = "output.txt",
+        input_path: str | Path = "input.txt",
+        output_path: str | Path = "output.txt",
         encoding: str = "utf-8",
     ) -> None:
         self.input_path = input_path
         self.output_path = output_path
         self.encoding = encoding
 
     def save(self, encoded_data: FinalDataSet) -> None:
         with open(self.output_path, "wb", encoding=self.encoding) as f:
             pickle.dump(encoded_data, f)
 
     def load(self) -> FinalDataSet:
         with open(self.output_path, "rb", encoding=self.encoding) as f:
             data: FinalDataSet = pickle.load(f)
         return data
+
+
+class Picklefier(IPersistenceManager):
+    @staticmethod
+    def save(path: str | Path, encoded_data: FinalDataSet) -> None:
+        with open(path, "wb") as f:
+            pickle.dump(encoded_data, f, pickle.HIGHEST_PROTOCOL)
+
+    @staticmethod
+    def load(path: str | Path) -> FinalDataSet:
+        with open(path, "rb") as f:
+            data: FinalDataSet = pickle.load(f)
+        return data
```

### Comparing `huffify-0.1.1/src/huffify/heapNodes.py` & `huffify-0.2.0/src/huffify/heapNodes.py`

 * *Files identical despite different names*

### Comparing `huffify-0.1.1/src/huffify/huffify.py` & `huffify-0.2.0/src/huffify/huffify.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 import heapq
 from collections import Counter
+from pathlib import Path
 from typing import Type
 
-from huffify.abstract import IEncoder, INode
+from huffify.abstract import IEncoder, INode, IPersistenceManager
 from huffify.annotations import FinalDataSet
 from huffify.encoders import MVPEncoder
+from huffify.fileManger import Picklefier
 from huffify.heapNodes import Node
 
 
 class HuffmanCodec:
     def __init__(
         self,
         node: Type[INode] = Node,
         encoder: Type[IEncoder] = MVPEncoder,
     ) -> None:
         self.__HeapNode = node
         self.encoder: IEncoder = encoder()
 
-    def _define_char_frequency(self, message: str) -> Counter[str]:
+    @staticmethod
+    def __define_char_frequency(message: str) -> Counter[str]:
         return Counter(message)
 
-    def print_encoding_table(self, message: str) -> None:
+    def print_encoding_table(self, message: str, reverse: bool = False) -> None:
         # TODO add sys.stout
         encoding_table = self._get_encoding_table(message)
-        encoding_table = dict(sorted(encoding_table.items(), key=lambda x: (len(x[1]), x[1])))
-        [print(_) for _ in self._format(encoding_table)]
+        encoding_table = dict(
+            sorted(encoding_table.items(), key=lambda x: (len(x[1]), x[1]), reverse=reverse)
+        )
+        [print(_) for _ in HuffmanCodec.__format(encoding_table)]
 
-    def _format(self, encoding_table: dict[str, str]) -> list[str]:
+    @staticmethod
+    def __format(encoding_table: dict[str, str]) -> list[str]:
         if not encoding_table:
             return []
         lines: list[str] = []
         for char, code in encoding_table.items():
             lines.append(f'"{char}" {code}')
         return lines
 
     def _get_encoding_table(self, message: str) -> dict[str, str]:
         if len(message) == 1:
             return {char: "1" for char in message}
-        chars_frequency = self._define_char_frequency(message)
+        chars_frequency = HuffmanCodec.__define_char_frequency(message)
         heap = [self.__HeapNode(key, chars_frequency[key]) for key in chars_frequency]
         heapq.heapify(heap)
         encoding_table = {char: "" for char in message}
         while len(heap) > 1:
             low = heapq.heappop(heap)
             hight = heapq.heappop(heap)
             for i in hight.char:
@@ -64,7 +70,27 @@
 
     def decode(self, encoded_data: FinalDataSet) -> str:
         encoding_table, encoded_message = encoded_data.get("table"), encoded_data.get(
             "message"
         )
         decoded_message = self.encoder.decode_string(encoding_table, encoded_message)
         return decoded_message
+
+
+class Huffify(HuffmanCodec):
+    def __init__(
+        self,
+        node: Type[INode] = Node,
+        encoder: Type[IEncoder] = MVPEncoder,
+        file_manager: Type[IPersistenceManager] = Picklefier,
+    ) -> None:
+        super().__init__(node, encoder)
+        self.file_manager: IPersistenceManager = file_manager()
+
+    def save(self, path: str | Path, message: str) -> None:
+        encoded_dataset = self.encode(message)
+        self.file_manager.save(path, encoded_dataset)
+
+    def load(self, path: str | Path) -> str:
+        encoded_dataset = self.file_manager.load(path)
+        decoded_message = self.decode(encoded_dataset)
+        return decoded_message
```

