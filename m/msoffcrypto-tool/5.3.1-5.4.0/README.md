# Comparing `tmp/msoffcrypto_tool-5.3.1.tar.gz` & `tmp/msoffcrypto_tool-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msoffcrypto_tool-5.3.1.tar", max compression
+gzip compressed data, was "msoffcrypto_tool-5.4.0.tar", max compression
```

## Comparing `msoffcrypto_tool-5.3.1.tar` & `msoffcrypto_tool-5.4.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0     2840 2024-01-18 16:24:11.390561 msoffcrypto_tool-5.3.1/LICENSE.txt
--rw-r--r--   0        0        0     9412 2024-01-18 16:24:11.390561 msoffcrypto_tool-5.3.1/README.md
--rw-r--r--   0        0        0     2813 2024-01-18 16:24:11.390561 msoffcrypto_tool-5.3.1/msoffcrypto/__init__.py
--rw-r--r--   0        0        0     3175 2024-01-18 16:24:11.390561 msoffcrypto_tool-5.3.1/msoffcrypto/__main__.py
--rw-r--r--   0        0        0      555 2024-01-18 16:24:11.390561 msoffcrypto_tool-5.3.1/msoffcrypto/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 16:24:11.390561 msoffcrypto_tool-5.3.1/msoffcrypto/format/__init__.py
--rw-r--r--   0        0        0      398 2024-01-18 16:24:11.390561 msoffcrypto_tool-5.3.1/msoffcrypto/format/base.py
--rw-r--r--   0        0        0     1669 2024-01-18 16:24:11.390561 msoffcrypto_tool-5.3.1/msoffcrypto/format/common.py
--rw-r--r--   0        0        0    15845 2024-01-18 16:24:11.394561 msoffcrypto_tool-5.3.1/msoffcrypto/format/doc97.py
--rw-r--r--   0        0        0    12060 2024-01-18 16:24:11.394561 msoffcrypto_tool-5.3.1/msoffcrypto/format/ooxml.py
--rw-r--r--   0        0        0    28423 2024-01-18 16:24:11.394561 msoffcrypto_tool-5.3.1/msoffcrypto/format/ppt97.py
--rw-r--r--   0        0        0    19142 2024-01-18 16:24:11.394561 msoffcrypto_tool-5.3.1/msoffcrypto/format/xls97.py
--rw-r--r--   0        0        0        0 2024-01-18 16:24:11.394561 msoffcrypto_tool-5.3.1/msoffcrypto/method/__init__.py
--rw-r--r--   0        0        0    22252 2024-01-18 16:24:11.394561 msoffcrypto_tool-5.3.1/msoffcrypto/method/container/ecma376_encrypted.py
--rw-r--r--   0        0        0    18589 2024-01-18 16:24:11.394561 msoffcrypto_tool-5.3.1/msoffcrypto/method/ecma376_agile.py
--rw-r--r--   0        0        0       62 2024-01-18 16:24:11.394561 msoffcrypto_tool-5.3.1/msoffcrypto/method/ecma376_extensible.py
--rw-r--r--   0        0        0     3922 2024-01-18 16:24:11.394561 msoffcrypto_tool-5.3.1/msoffcrypto/method/ecma376_standard.py
--rw-r--r--   0        0        0     3064 2024-01-18 16:24:11.394561 msoffcrypto_tool-5.3.1/msoffcrypto/method/rc4.py
--rw-r--r--   0        0        0     2512 2024-01-18 16:24:11.394561 msoffcrypto_tool-5.3.1/msoffcrypto/method/rc4_cryptoapi.py
--rw-r--r--   0        0        0     8016 2024-01-18 16:24:11.394561 msoffcrypto_tool-5.3.1/msoffcrypto/method/xor_obfuscation.py
--rw-r--r--   0        0        0     1210 2024-01-18 16:24:11.394561 msoffcrypto_tool-5.3.1/pyproject.toml
--rw-r--r--   0        0        0    10169 1970-01-01 00:00:00.000000 msoffcrypto_tool-5.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-02 05:48:37.029318 msoffcrypto_tool-5.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1705 2024-05-02 05:48:37.029318 msoffcrypto_tool-5.4.0/NOTICE.txt
+-rw-r--r--   0        0        0     9412 2024-05-02 05:48:37.029318 msoffcrypto_tool-5.4.0/README.md
+-rw-r--r--   0        0        0     2813 2024-05-02 05:48:37.029318 msoffcrypto_tool-5.4.0/msoffcrypto/__init__.py
+-rw-r--r--   0        0        0     3175 2024-05-02 05:48:37.029318 msoffcrypto_tool-5.4.0/msoffcrypto/__main__.py
+-rw-r--r--   0        0        0      555 2024-05-02 05:48:37.029318 msoffcrypto_tool-5.4.0/msoffcrypto/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 05:48:37.029318 msoffcrypto_tool-5.4.0/msoffcrypto/format/__init__.py
+-rw-r--r--   0        0        0      398 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/format/base.py
+-rw-r--r--   0        0        0     1669 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/format/common.py
+-rw-r--r--   0        0        0    15845 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/format/doc97.py
+-rw-r--r--   0        0        0    12178 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/format/ooxml.py
+-rw-r--r--   0        0        0    28423 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/format/ppt97.py
+-rw-r--r--   0        0        0    19142 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/format/xls97.py
+-rw-r--r--   0        0        0        0 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/container/__init__.py
+-rw-r--r--   0        0        0    22252 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/container/ecma376_encrypted.py
+-rw-r--r--   0        0        0    18589 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/ecma376_agile.py
+-rw-r--r--   0        0        0       62 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/ecma376_extensible.py
+-rw-r--r--   0        0        0     3922 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/ecma376_standard.py
+-rw-r--r--   0        0        0     3064 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/rc4.py
+-rw-r--r--   0        0        0     2512 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/rc4_cryptoapi.py
+-rw-r--r--   0        0        0     8016 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/msoffcrypto/method/xor_obfuscation.py
+-rw-r--r--   0        0        0     1264 2024-05-02 05:48:37.033318 msoffcrypto_tool-5.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10182 1970-01-01 00:00:00.000000 msoffcrypto_tool-5.4.0/PKG-INFO
```

### Comparing `msoffcrypto_tool-5.3.1/LICENSE.txt` & `msoffcrypto_tool-5.4.0/NOTICE.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-MIT License
-
-Copyright (c) 2015 nolze
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-----------------------------------------------------------------------
-
 This software contains derivative works from https://github.com/herumi/msoffice
 which is licensed under the BSD 3-Clause License.
 
 https://github.com/herumi/msoffice/blob/c3cdb1ea0a5285a2a1718fee2dc893fd884bdad0/COPYRIGHT
 
 Copyright (c) 2007-2015 Cybozu Labs, Inc.
 All rights reserved.
```

### Comparing `msoffcrypto_tool-5.3.1/README.md` & `msoffcrypto_tool-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.3.1/msoffcrypto/__init__.py` & `msoffcrypto_tool-5.4.0/msoffcrypto/__init__.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.3.1/msoffcrypto/__main__.py` & `msoffcrypto_tool-5.4.0/msoffcrypto/__main__.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.3.1/msoffcrypto/exceptions/__init__.py` & `msoffcrypto_tool-5.4.0/msoffcrypto/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.3.1/msoffcrypto/format/common.py` & `msoffcrypto_tool-5.4.0/msoffcrypto/format/common.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.3.1/msoffcrypto/format/doc97.py` & `msoffcrypto_tool-5.4.0/msoffcrypto/format/doc97.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.3.1/msoffcrypto/format/ooxml.py` & `msoffcrypto_tool-5.4.0/msoffcrypto/format/ooxml.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     versionMajor, versionMinor = unpack("<HH", ole.read(4))
     if versionMajor == 4 and versionMinor == 4:  # Agile
         return "agile", _parseinfo_agile(ole)
     elif versionMajor in [2, 3, 4] and versionMinor == 2:  # Standard
         return "standard", _parseinfo_standard(ole)
     elif versionMajor in [3, 4] and versionMinor == 3:  # Extensible
         raise exceptions.DecryptionError("Unsupported EncryptionInfo version (Extensible Encryption)")
+    raise exceptions.DecryptionError("Unsupported EncryptionInfo version ({}:{})".format(versionMajor, versionMinor))
 
 
 class OOXMLFile(base.BaseOfficeFile):
     """Return an OOXML file object.
 
     Examples:
         >>> with open("tests/inputs/example_password.docx", "rb") as f:
```

### Comparing `msoffcrypto_tool-5.3.1/msoffcrypto/format/ppt97.py` & `msoffcrypto_tool-5.4.0/msoffcrypto/format/ppt97.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.3.1/msoffcrypto/format/xls97.py` & `msoffcrypto_tool-5.4.0/msoffcrypto/format/xls97.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.3.1/msoffcrypto/method/container/ecma376_encrypted.py` & `msoffcrypto_tool-5.4.0/msoffcrypto/method/container/ecma376_encrypted.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.3.1/msoffcrypto/method/ecma376_agile.py` & `msoffcrypto_tool-5.4.0/msoffcrypto/method/ecma376_agile.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.3.1/msoffcrypto/method/ecma376_standard.py` & `msoffcrypto_tool-5.4.0/msoffcrypto/method/ecma376_standard.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.3.1/msoffcrypto/method/rc4.py` & `msoffcrypto_tool-5.4.0/msoffcrypto/method/rc4.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.3.1/msoffcrypto/method/rc4_cryptoapi.py` & `msoffcrypto_tool-5.4.0/msoffcrypto/method/rc4_cryptoapi.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.3.1/msoffcrypto/method/xor_obfuscation.py` & `msoffcrypto_tool-5.4.0/msoffcrypto/method/xor_obfuscation.py`

 * *Files identical despite different names*

### Comparing `msoffcrypto_tool-5.3.1/pyproject.toml` & `msoffcrypto_tool-5.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "msoffcrypto-tool"
-version = "5.3.1"
-description = "Python tool and library for decrypting MS Office files with passwords or other keys"
+version = "5.4.0"
+description = "Python tool and library for decrypting and encrypting MS Office files using a password or other keys"
 license = "MIT"
 homepage = "https://github.com/nolze/msoffcrypto-tool"
-authors = ["nolze <nolze@archlinux.us>"]
+authors = ["nolze <nolze@int3.net>"]
 readme = "README.md"
-packages = [{ include = "msoffcrypto" }]
+packages = [{ include = "msoffcrypto" }, { include = "NOTICE.txt" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 cryptography = ">=35.0"
 olefile = ">=0.46"
 
 [tool.poetry.group.dev.dependencies]
 # pytest = { version = ">=6.2.1", python = "^3.7" }
-# black = { version = "^20.8b1", python = "^3.7" }
-black = "^23.7.0"
 pytest = "^7.4.0"
-coverage = { extras = ["toml"], version = "^5.3.1" }
+coverage = { extras = ["toml"], version = "^7.5" }
 
 
 [tool.poetry.group.docs.dependencies]
-sphinx-autobuild = "^2021.3.14"
-furo = "^2023.9.10"
+sphinx-autobuild = [
+  { version = "2024.4.16", python = "^3.9" },
+  { version = "2021.3.14", python = "<=3.8" },
+]
+furo = "2024.04.27"
 myst-parser = "^2.0.0"
 sphinxcontrib-autoprogram = "^0.1.8"
 
 [tool.poetry.scripts]
 msoffcrypto-tool = 'msoffcrypto.__main__:main'
 
 [tool.black]
```

### Comparing `msoffcrypto_tool-5.3.1/PKG-INFO` & `msoffcrypto_tool-5.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: msoffcrypto-tool
-Version: 5.3.1
-Summary: Python tool and library for decrypting MS Office files with passwords or other keys
+Version: 5.4.0
+Summary: Python tool and library for decrypting and encrypting MS Office files using a password or other keys
 Home-page: https://github.com/nolze/msoffcrypto-tool
 License: MIT
 Author: nolze
-Author-email: nolze@archlinux.us
+Author-email: nolze@int3.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

