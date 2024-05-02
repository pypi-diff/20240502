# Comparing `tmp/character_encoding_utils-0.0.6.tar.gz` & `tmp/character_encoding_utils-0.0.7.tar.gz`

## Comparing `character_encoding_utils-0.0.6.tar` & `character_encoding_utils-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/requirements.txt
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/src/character_encoding_utils/__init__.py
--rw-r--r--   0        0        0     5219 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/src/character_encoding_utils/big5.py
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/src/character_encoding_utils/gb2312.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/src/character_encoding_utils/ksx1001.py
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/src/character_encoding_utils/shiftjis.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/tests/test_big5.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/tests/test_gb2312.py
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/tests/test_ksx1001.py
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/tests/test_shiftjis.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/LICENSE
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/src/character_encoding_utils/__init__.py
+-rw-r--r--   0        0        0     5219 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/src/character_encoding_utils/big5.py
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/src/character_encoding_utils/gb2312.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/src/character_encoding_utils/ksx1001.py
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/src/character_encoding_utils/shiftjis.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/tests/test_big5.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/tests/test_gb2312.py
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/tests/test_ksx1001.py
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/tests/test_shiftjis.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 character_encoding_utils-0.0.7/PKG-INFO
```

### Comparing `character_encoding_utils-0.0.6/src/character_encoding_utils/big5.py` & `character_encoding_utils-0.0.7/src/character_encoding_utils/big5.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 
 class Big5Exception(Exception):
     pass
 
 
 class Big5EncodeError(Big5Exception):
     def __init__(self, obj: str, position: int, reason: str):
+        super().__init__(f"'big5' codec can't encode character '\\u{ord(obj):x}' in position {position}: {reason}")
         self.object = obj
         self.position = position
         self.reason = reason
-        super().__init__(f"'big5' codec can't encode character '\\u{ord(obj):x}' in position {position}: {reason}")
 
 
 class Big5DecodeError(Big5Exception):
     def __init__(self, obj: bytes, position: int, reason: str):
-        self.object = obj
-        self.position = position
-        self.reason = reason
         if len(obj) <= 1:
             super().__init__(f"'big5' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
         else:
             super().__init__(f"'big5' codec can't decode bytes in position {position}-{position + len(obj) - 1}: {reason}")
+        self.object = obj
+        self.position = position
+        self.reason = reason
 
 
 def encode(cs: str) -> bytes:
     bs = bytearray()
     for position, c in enumerate(cs):
         if c == '〸':  # 0x3038
             bs.extend(b'\xa2\xcc')
```

### Comparing `character_encoding_utils-0.0.6/src/character_encoding_utils/gb2312.py` & `character_encoding_utils-0.0.7/src/character_encoding_utils/gb2312.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 
 class GB2312Exception(Exception):
     pass
 
 
 class GB2312EncodeError(GB2312Exception):
     def __init__(self, obj: str, position: int, reason: str):
+        super().__init__(f"'gb2312' codec can't encode character '\\u{ord(obj):x}' in position {position}: {reason}")
         self.object = obj
         self.position = position
         self.reason = reason
-        super().__init__(f"'gb2312' codec can't encode character '\\u{ord(obj):x}' in position {position}: {reason}")
 
 
 class GB2312DecodeError(GB2312Exception):
     def __init__(self, obj: bytes, position: int, reason: str):
-        self.object = obj
-        self.position = position
-        self.reason = reason
         if len(obj) <= 1:
             super().__init__(f"'gb2312' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
         else:
             super().__init__(f"'gb2312' codec can't decode bytes in position {position}-{position + len(obj) - 1}: {reason}")
+        self.object = obj
+        self.position = position
+        self.reason = reason
 
 
 def encode(cs: str) -> bytes:
     bs = bytearray()
     for position, c in enumerate(cs):
         try:
             bs.extend(c.encode('gb2312'))
```

### Comparing `character_encoding_utils-0.0.6/src/character_encoding_utils/ksx1001.py` & `character_encoding_utils-0.0.7/src/character_encoding_utils/ksx1001.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 
 class KSX1001Exception(Exception):
     pass
 
 
 class KSX1001EncodeError(KSX1001Exception):
     def __init__(self, obj: str, position: int, reason: str):
+        super().__init__(f"'ksx1001' codec can't encode character '\\u{ord(obj):x}' in position {position}: {reason}")
         self.object = obj
         self.position = position
         self.reason = reason
-        super().__init__(f"'ksx1001' codec can't encode character '\\u{ord(obj):x}' in position {position}: {reason}")
 
 
 class KSX1001DecodeError(KSX1001Exception):
     def __init__(self, obj: bytes, position: int, reason: str):
-        self.object = obj
-        self.position = position
-        self.reason = reason
         if len(obj) <= 1:
             super().__init__(f"'ksx1001' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
         else:
             super().__init__(f"'ksx1001' codec can't decode bytes in position {position}-{position + len(obj) - 1}: {reason}")
+        self.object = obj
+        self.position = position
+        self.reason = reason
 
 
 def encode(cs: str) -> bytes:
     bs = bytearray()
     for position, c in enumerate(cs):
         try:
             bs.extend(c.encode('ksx1001'))
```

### Comparing `character_encoding_utils-0.0.6/src/character_encoding_utils/shiftjis.py` & `character_encoding_utils-0.0.7/src/character_encoding_utils/shiftjis.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 
 class ShiftJISException(Exception):
     pass
 
 
 class ShiftJISEncodeError(ShiftJISException):
     def __init__(self, obj: str, position: int, reason: str):
+        super().__init__(f"'shift-jis' codec can't encode character '\\u{ord(obj):x}' in position {position}: {reason}")
         self.object = obj
         self.position = position
         self.reason = reason
-        super().__init__(f"'shift-jis' codec can't encode character '\\u{ord(obj):x}' in position {position}: {reason}")
 
 
 class ShiftJISDecodeError(ShiftJISException):
     def __init__(self, obj: bytes, position: int, reason: str):
-        self.object = obj
-        self.position = position
-        self.reason = reason
         if len(obj) <= 1:
             super().__init__(f"'shift-jis' codec can't decode byte 0x{obj[0]:x} in position {position}: {reason}")
         else:
             super().__init__(f"'shift-jis' codec can't decode bytes in position {position}-{position + len(obj) - 1}: {reason}")
+        self.object = obj
+        self.position = position
+        self.reason = reason
 
 
 def encode(cs: str) -> bytes:
     bs = bytearray()
     for position, c in enumerate(cs):
         if c == '\\':
             raise ShiftJISEncodeError(c, position, f"in 'shift-jis' the character '\\' is replaced with '¥'")
```

### Comparing `character_encoding_utils-0.0.6/tests/test_big5.py` & `character_encoding_utils-0.0.7/tests/test_big5.py`

 * *Files identical despite different names*

### Comparing `character_encoding_utils-0.0.6/tests/test_gb2312.py` & `character_encoding_utils-0.0.7/tests/test_gb2312.py`

 * *Files identical despite different names*

### Comparing `character_encoding_utils-0.0.6/tests/test_ksx1001.py` & `character_encoding_utils-0.0.7/tests/test_ksx1001.py`

 * *Files identical despite different names*

### Comparing `character_encoding_utils-0.0.6/tests/test_shiftjis.py` & `character_encoding_utils-0.0.7/tests/test_shiftjis.py`

 * *Files identical despite different names*

### Comparing `character_encoding_utils-0.0.6/.gitignore` & `character_encoding_utils-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `character_encoding_utils-0.0.6/LICENSE` & `character_encoding_utils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `character_encoding_utils-0.0.6/README.md` & `character_encoding_utils-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `character_encoding_utils-0.0.6/pyproject.toml` & `character_encoding_utils-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "character-encoding-utils"
-version = "0.0.6"
+version = "0.0.7"
 description = "Some character encoding utils."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `character_encoding_utils-0.0.6/PKG-INFO` & `character_encoding_utils-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: character-encoding-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Some character encoding utils.
 Project-URL: homepage, https://github.com/TakWolf/character-encoding-utils
 Project-URL: source, https://github.com/TakWolf/character-encoding-utils
 Project-URL: issues, https://github.com/TakWolf/character-encoding-utils/issues
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
```

