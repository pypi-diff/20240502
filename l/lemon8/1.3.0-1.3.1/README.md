# Comparing `tmp/lemon8-1.3.0.tar.gz` & `tmp/lemon8-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemon8-1.3.0.tar", max compression
+gzip compressed data, was "lemon8-1.3.1.tar", max compression
```

## Comparing `lemon8-1.3.0.tar` & `lemon8-1.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1061 2024-05-02 13:10:52.689140 lemon8-1.3.0/LICENSE
--rw-r--r--   0        0        0     1315 2024-05-02 13:10:52.689140 lemon8-1.3.0/README.md
--rw-r--r--   0        0        0     3687 2024-05-02 13:10:52.709140 lemon8-1.3.0/lemon8/__main__.py
--rw-r--r--   0        0        0      133 2024-05-02 13:10:52.689140 lemon8-1.3.0/lemon8/components/__init__.py
--rw-r--r--   0        0        0      193 2024-05-02 13:10:52.689140 lemon8-1.3.0/lemon8/components/constants.py
--rw-r--r--   0        0        0    12098 2024-05-02 13:10:52.689140 lemon8-1.3.0/lemon8/components/cpu.py
--rw-r--r--   0        0        0     2825 2024-05-02 13:10:52.689140 lemon8-1.3.0/lemon8/components/display.py
--rw-r--r--   0        0        0     1644 2024-05-02 13:10:52.689140 lemon8-1.3.0/lemon8/components/keypad.py
--rw-r--r--   0        0        0      750 2024-05-02 13:10:52.689140 lemon8-1.3.0/lemon8/components/memory.py
--rw-r--r--   0        0        0     1763 2024-05-02 13:10:52.689140 lemon8-1.3.0/lemon8/components/opcode.py
--rw-r--r--   0        0        0      557 2024-05-02 13:28:29.689082 lemon8-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 lemon8-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-02 14:07:41.628947 lemon8-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1315 2024-05-02 14:07:41.628947 lemon8-1.3.1/README.md
+-rw-r--r--   0        0        0     3688 2024-05-02 16:59:20.320495 lemon8-1.3.1/lemon8/__main__.py
+-rw-r--r--   0        0        0      133 2024-05-02 14:07:41.658947 lemon8-1.3.1/lemon8/components/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-02 14:07:41.658947 lemon8-1.3.1/lemon8/components/constants.py
+-rw-r--r--   0        0        0    12098 2024-05-02 14:07:41.658947 lemon8-1.3.1/lemon8/components/cpu.py
+-rw-r--r--   0        0        0     2825 2024-05-02 14:07:41.658947 lemon8-1.3.1/lemon8/components/display.py
+-rw-r--r--   0        0        0     1644 2024-05-02 14:07:41.658947 lemon8-1.3.1/lemon8/components/keypad.py
+-rw-r--r--   0        0        0      750 2024-05-02 14:07:41.658947 lemon8-1.3.1/lemon8/components/memory.py
+-rw-r--r--   0        0        0     1763 2024-05-02 14:07:41.658947 lemon8-1.3.1/lemon8/components/opcode.py
+-rw-r--r--   0        0        0      557 2024-05-02 16:59:50.420490 lemon8-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 lemon8-1.3.1/PKG-INFO
```

### Comparing `lemon8-1.3.0/LICENSE` & `lemon8-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.0/README.md` & `lemon8-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.0/lemon8/__main__.py` & `lemon8-1.3.1/lemon8/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import logging
 
 import pygame
 
-from components import (CPU, INIT_LOC_CONSTANT, TICK, WAVE, Display, Keypad,
+from .components import (CPU, INIT_LOC_CONSTANT, TICK, WAVE, Display, Keypad,
                         Memory)
 
 logging.basicConfig(
     format="%(asctime)s:%(msecs)03d (%(levelname)s/%(module)s): %(message)s",
     level=logging.DEBUG,
     encoding="utf-8",
     datefmt="%M:%S",
```

### Comparing `lemon8-1.3.0/lemon8/components/cpu.py` & `lemon8-1.3.1/lemon8/components/cpu.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.0/lemon8/components/display.py` & `lemon8-1.3.1/lemon8/components/display.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.0/lemon8/components/keypad.py` & `lemon8-1.3.1/lemon8/components/keypad.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.0/lemon8/components/memory.py` & `lemon8-1.3.1/lemon8/components/memory.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.0/lemon8/components/opcode.py` & `lemon8-1.3.1/lemon8/components/opcode.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.0/pyproject.toml` & `lemon8-1.3.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lemon8"
-version = "1.3.0"
+version = "1.3.1"
 description = "A CHIP-8 emulator written in Python."
 authors = ["mooncell07 <80042274+mooncell07@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://mooncell07.github.io/lemon.pie/"
 
 [tool.poetry.dependencies]
```

### Comparing `lemon8-1.3.0/PKG-INFO` & `lemon8-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemon8
-Version: 1.3.0
+Version: 1.3.1
 Summary: A CHIP-8 emulator written in Python.
 License: MIT
 Author: mooncell07
 Author-email: 80042274+mooncell07@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lemon8 Version: 1.3.0 Summary: A CHIP-8 emulator
+Metadata-Version: 2.1 Name: lemon8 Version: 1.3.1 Summary: A CHIP-8 emulator
 written in Python. License: MIT Author: mooncell07 Author-email:
 80042274+mooncell07@users.noreply.github.com Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pygame (>=2.2.0,<3.0.0) Project-URL: Documentation, https://
 mooncell07.github.io/lemon.pie/ Description-Content-Type: text/markdown
                             [./docs/img/lemon.png]
```

