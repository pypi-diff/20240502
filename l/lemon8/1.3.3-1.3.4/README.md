# Comparing `tmp/lemon8-1.3.3.tar.gz` & `tmp/lemon8-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemon8-1.3.3.tar", max compression
+gzip compressed data, was "lemon8-1.3.4.tar", max compression
```

## Comparing `lemon8-1.3.3.tar` & `lemon8-1.3.4.tar`

### file list

```diff
@@ -1,16 +1,27 @@
--rw-r--r--   0        0        0     1061 2024-05-02 14:07:41.628947 lemon8-1.3.3/LICENSE
--rw-r--r--   0        0        0     1315 2024-05-02 14:07:41.628947 lemon8-1.3.3/README.md
--rw-r--r--   0        0        0     3688 2024-05-02 17:11:00.670400 lemon8-1.3.3/lemon8/__main__.py
--rw-r--r--   0        0        0    22170 2024-05-02 14:07:41.638947 lemon8-1.3.3/lemon8/beep.mp3
--rw-r--r--   0        0        0       80 2024-05-02 14:07:41.638947 lemon8-1.3.3/lemon8/bin/FONT
--rw-r--r--   0        0        0      132 2024-05-02 14:07:41.638947 lemon8-1.3.3/lemon8/bin/ibm.ch8
--rw-r--r--   0        0        0      133 2024-05-02 14:07:41.658947 lemon8-1.3.3/lemon8/components/__init__.py
--rw-r--r--   0        0        0      193 2024-05-02 14:07:41.658947 lemon8-1.3.3/lemon8/components/constants.py
--rw-r--r--   0        0        0    12098 2024-05-02 17:13:20.040382 lemon8-1.3.3/lemon8/components/cpu.py
--rw-r--r--   0        0        0     2814 2024-05-02 17:12:48.640387 lemon8-1.3.3/lemon8/components/display.py
--rw-r--r--   0        0        0     1644 2024-05-02 14:07:41.658947 lemon8-1.3.3/lemon8/components/keypad.py
--rw-r--r--   0        0        0      750 2024-05-02 14:07:41.658947 lemon8-1.3.3/lemon8/components/memory.py
--rw-r--r--   0        0        0     1763 2024-05-02 14:07:41.658947 lemon8-1.3.3/lemon8/components/opcode.py
--rw-r--r--   0        0        0    40076 2024-05-02 17:08:24.900421 lemon8-1.3.3/lemon8/lemon.png
--rw-r--r--   0        0        0      557 2024-05-02 17:13:08.190384 lemon8-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 lemon8-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-02 14:07:41.628947 lemon8-1.3.4/LICENSE
+-rw-r--r--   0        0        0     1315 2024-05-02 14:07:41.628947 lemon8-1.3.4/README.md
+-rw-r--r--   0        0        0     3688 2024-05-02 17:33:07.960216 lemon8-1.3.4/lemon8/__main__.py
+-rw-r--r--   0        0        0    22170 2024-05-02 14:07:41.638947 lemon8-1.3.4/lemon8/beep.mp3
+-rw-r--r--   0        0        0       80 2024-05-02 14:07:41.638947 lemon8-1.3.4/lemon8/bin/FONT
+-rw-r--r--   0        0        0      132 2024-05-02 14:07:41.638947 lemon8-1.3.4/lemon8/bin/ibm.ch8
+-rw-r--r--   0        0        0      133 2024-05-02 14:07:41.658947 lemon8-1.3.4/lemon8/components/__init__.py
+-rw-r--r--   0        0        0      260 2024-05-02 13:14:11.199127 lemon8-1.3.4/lemon8/components/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      337 2024-05-02 17:00:27.180486 lemon8-1.3.4/lemon8/components/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      346 2024-05-02 13:14:11.199127 lemon8-1.3.4/lemon8/components/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0      391 2024-05-02 17:00:27.190486 lemon8-1.3.4/lemon8/components/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0        0        0    13300 2024-05-02 13:14:11.199127 lemon8-1.3.4/lemon8/components/__pycache__/cpu.cpython-310.pyc
+-rw-r--r--   0        0        0    21353 2024-05-02 17:32:51.070218 lemon8-1.3.4/lemon8/components/__pycache__/cpu.cpython-311.pyc
+-rw-r--r--   0        0        0     3266 2024-05-02 13:14:11.199127 lemon8-1.3.4/lemon8/components/__pycache__/display.cpython-310.pyc
+-rw-r--r--   0        0        0     5014 2024-05-02 17:32:51.070218 lemon8-1.3.4/lemon8/components/__pycache__/display.cpython-311.pyc
+-rw-r--r--   0        0        0     3159 2024-05-02 17:00:27.330486 lemon8-1.3.4/lemon8/components/__pycache__/keypad.cpython-311.pyc
+-rw-r--r--   0        0        0     1714 2024-05-02 17:00:27.330486 lemon8-1.3.4/lemon8/components/__pycache__/memory.cpython-311.pyc
+-rw-r--r--   0        0        0     3383 2024-05-02 17:00:27.330486 lemon8-1.3.4/lemon8/components/__pycache__/opcode.cpython-311.pyc
+-rw-r--r--   0        0        0      193 2024-05-02 14:07:41.658947 lemon8-1.3.4/lemon8/components/constants.py
+-rw-r--r--   0        0        0    12155 2024-05-02 17:32:47.890218 lemon8-1.3.4/lemon8/components/cpu.py
+-rw-r--r--   0        0        0     2871 2024-05-02 17:32:05.700224 lemon8-1.3.4/lemon8/components/display.py
+-rw-r--r--   0        0        0     1644 2024-05-02 14:07:41.658947 lemon8-1.3.4/lemon8/components/keypad.py
+-rw-r--r--   0        0        0      750 2024-05-02 14:07:41.658947 lemon8-1.3.4/lemon8/components/memory.py
+-rw-r--r--   0        0        0     1763 2024-05-02 14:07:41.658947 lemon8-1.3.4/lemon8/components/opcode.py
+-rw-r--r--   0        0        0    40076 2024-05-02 17:08:24.900421 lemon8-1.3.4/lemon8/lemon.png
+-rw-r--r--   0        0        0      557 2024-05-02 17:33:13.230215 lemon8-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 lemon8-1.3.4/PKG-INFO
```

### Comparing `lemon8-1.3.3/LICENSE` & `lemon8-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.3/README.md` & `lemon8-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.3/lemon8/__main__.py` & `lemon8-1.3.4/lemon8/__main__.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.3/lemon8/beep.mp3` & `lemon8-1.3.4/lemon8/beep.mp3`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.3/lemon8/components/cpu.py` & `lemon8-1.3.4/lemon8/components/cpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import typing as t
 from random import randint
-
+import importlib.resources as ir
 import pygame
 
 from .constants import COLUMNS, CROSS, INIT_LOC_CONSTANT, ROWS
 from .display import Display
 from .keypad import Keypad
 from .memory import Memory
 from .opcode import Opcode
@@ -59,15 +59,15 @@
             halt (bool): Flag to check if the CPU is halted.
             sync (bool): Flag to sync the display with the timer.
         """
         # devices
         self.display = display
         self.memory = memory
         self.keypad = keypad
-        self.sound: pygame.mixer.Sound = pygame.mixer.Sound("beep.mp3")
+        self.sound: pygame.mixer.Sound = pygame.mixer.Sound(ir.open_binary("lemon8","beep.mp3"))
         self.op: Opcode = Opcode(inst=0x0000)
 
         # registers
         self.V: t.List[int] = [0] * 16
         self.I: int = 0
         self.DT: int = 0
         self.ST: int = 0
```

### Comparing `lemon8-1.3.3/lemon8/components/display.py` & `lemon8-1.3.4/lemon8/components/display.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import typing as t
 
 import pygame
-
+import importlib.resources as ir
 from .constants import COLORS, COLUMNS, ROWS
 
 pygame.init()
-
-img = pygame.image.load("lemon.png")
+img = pygame.image.load(ir.open_binary("lemon8", "lemon.png"))
 __all__ = ("Display",)
 
 
 class Display:
     """
     Object for handling creation, rendering and deletion of the emulator
     window.
```

### Comparing `lemon8-1.3.3/lemon8/components/keypad.py` & `lemon8-1.3.4/lemon8/components/keypad.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.3/lemon8/components/memory.py` & `lemon8-1.3.4/lemon8/components/memory.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.3/lemon8/components/opcode.py` & `lemon8-1.3.4/lemon8/components/opcode.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.3/lemon8/lemon.png` & `lemon8-1.3.4/lemon8/lemon.png`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.3/pyproject.toml` & `lemon8-1.3.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lemon8"
-version = "1.3.3"
+version = "1.3.4"
 description = "A CHIP-8 emulator written in Python."
 authors = ["mooncell07 <80042274+mooncell07@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://mooncell07.github.io/lemon.pie/"
 
 [tool.poetry.dependencies]
```

### Comparing `lemon8-1.3.3/PKG-INFO` & `lemon8-1.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemon8
-Version: 1.3.3
+Version: 1.3.4
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
-Metadata-Version: 2.1 Name: lemon8 Version: 1.3.3 Summary: A CHIP-8 emulator
+Metadata-Version: 2.1 Name: lemon8 Version: 1.3.4 Summary: A CHIP-8 emulator
 written in Python. License: MIT Author: mooncell07 Author-email:
 80042274+mooncell07@users.noreply.github.com Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pygame (>=2.2.0,<3.0.0) Project-URL: Documentation, https://
 mooncell07.github.io/lemon.pie/ Description-Content-Type: text/markdown
                             [./docs/img/lemon.png]
```

