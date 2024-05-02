# Comparing `tmp/lemon8-1.3.8.tar.gz` & `tmp/lemon8-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemon8-1.3.8.tar", max compression
+gzip compressed data, was "lemon8-1.3.9.tar", max compression
```

## Comparing `lemon8-1.3.8.tar` & `lemon8-1.3.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1061 2024-05-02 14:07:41.628947 lemon8-1.3.8/LICENSE
--rw-r--r--   0        0        0     3688 2024-05-02 17:33:07.960216 lemon8-1.3.8/lemon8/__main__.py
--rw-r--r--   0        0        0    22170 2024-05-02 14:07:41.638947 lemon8-1.3.8/lemon8/beep.mp3
--rw-r--r--   0        0        0       80 2024-05-02 14:07:41.638947 lemon8-1.3.8/lemon8/bin/FONT
--rw-r--r--   0        0        0      132 2024-05-02 14:07:41.638947 lemon8-1.3.8/lemon8/bin/ibm.ch8
--rw-r--r--   0        0        0      133 2024-05-02 14:07:41.658947 lemon8-1.3.8/lemon8/components/__init__.py
--rw-r--r--   0        0        0      260 2024-05-02 13:14:11.199127 lemon8-1.3.8/lemon8/components/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      337 2024-05-02 17:00:27.180486 lemon8-1.3.8/lemon8/components/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      346 2024-05-02 13:14:11.199127 lemon8-1.3.8/lemon8/components/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0      391 2024-05-02 17:00:27.190486 lemon8-1.3.8/lemon8/components/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0        0        0    13300 2024-05-02 13:14:11.199127 lemon8-1.3.8/lemon8/components/__pycache__/cpu.cpython-310.pyc
--rw-r--r--   0        0        0    21353 2024-05-02 17:32:51.070218 lemon8-1.3.8/lemon8/components/__pycache__/cpu.cpython-311.pyc
--rw-r--r--   0        0        0     3266 2024-05-02 13:14:11.199127 lemon8-1.3.8/lemon8/components/__pycache__/display.cpython-310.pyc
--rw-r--r--   0        0        0     5014 2024-05-02 17:32:51.070218 lemon8-1.3.8/lemon8/components/__pycache__/display.cpython-311.pyc
--rw-r--r--   0        0        0     3159 2024-05-02 17:00:27.330486 lemon8-1.3.8/lemon8/components/__pycache__/keypad.cpython-311.pyc
--rw-r--r--   0        0        0     1714 2024-05-02 17:00:27.330486 lemon8-1.3.8/lemon8/components/__pycache__/memory.cpython-311.pyc
--rw-r--r--   0        0        0     3383 2024-05-02 17:00:27.330486 lemon8-1.3.8/lemon8/components/__pycache__/opcode.cpython-311.pyc
--rw-r--r--   0        0        0      193 2024-05-02 14:07:41.658947 lemon8-1.3.8/lemon8/components/constants.py
--rw-r--r--   0        0        0    12155 2024-05-02 17:32:47.890218 lemon8-1.3.8/lemon8/components/cpu.py
--rw-r--r--   0        0        0     2871 2024-05-02 17:32:05.700224 lemon8-1.3.8/lemon8/components/display.py
--rw-r--r--   0        0        0     1644 2024-05-02 14:07:41.658947 lemon8-1.3.8/lemon8/components/keypad.py
--rw-r--r--   0        0        0      804 2024-05-02 17:45:12.530119 lemon8-1.3.8/lemon8/components/memory.py
--rw-r--r--   0        0        0     1763 2024-05-02 14:07:41.658947 lemon8-1.3.8/lemon8/components/opcode.py
--rw-r--r--   0        0        0    40076 2024-05-02 17:08:24.900421 lemon8-1.3.8/lemon8/lemon.png
--rw-r--r--   0        0        0      536 2024-05-02 17:45:28.750117 lemon8-1.3.8/pyproject.toml
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 lemon8-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-02 14:07:41.628947 lemon8-1.3.9/LICENSE
+-rw-r--r--   0        0        0     3706 2024-05-02 17:50:19.830079 lemon8-1.3.9/lemon8/__main__.py
+-rw-r--r--   0        0        0    22170 2024-05-02 14:07:41.638947 lemon8-1.3.9/lemon8/beep.mp3
+-rw-r--r--   0        0        0       80 2024-05-02 14:07:41.638947 lemon8-1.3.9/lemon8/bin/FONT
+-rw-r--r--   0        0        0      132 2024-05-02 14:07:41.638947 lemon8-1.3.9/lemon8/bin/ibm.ch8
+-rw-r--r--   0        0        0      133 2024-05-02 14:07:41.658947 lemon8-1.3.9/lemon8/components/__init__.py
+-rw-r--r--   0        0        0      260 2024-05-02 13:14:11.199127 lemon8-1.3.9/lemon8/components/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      337 2024-05-02 17:00:27.180486 lemon8-1.3.9/lemon8/components/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      346 2024-05-02 13:14:11.199127 lemon8-1.3.9/lemon8/components/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0      391 2024-05-02 17:00:27.190486 lemon8-1.3.9/lemon8/components/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0        0        0    13300 2024-05-02 13:14:11.199127 lemon8-1.3.9/lemon8/components/__pycache__/cpu.cpython-310.pyc
+-rw-r--r--   0        0        0    21353 2024-05-02 17:32:51.070218 lemon8-1.3.9/lemon8/components/__pycache__/cpu.cpython-311.pyc
+-rw-r--r--   0        0        0     3266 2024-05-02 13:14:11.199127 lemon8-1.3.9/lemon8/components/__pycache__/display.cpython-310.pyc
+-rw-r--r--   0        0        0     5014 2024-05-02 17:32:51.070218 lemon8-1.3.9/lemon8/components/__pycache__/display.cpython-311.pyc
+-rw-r--r--   0        0        0     3159 2024-05-02 17:00:27.330486 lemon8-1.3.9/lemon8/components/__pycache__/keypad.cpython-311.pyc
+-rw-r--r--   0        0        0     1714 2024-05-02 17:00:27.330486 lemon8-1.3.9/lemon8/components/__pycache__/memory.cpython-311.pyc
+-rw-r--r--   0        0        0     3383 2024-05-02 17:00:27.330486 lemon8-1.3.9/lemon8/components/__pycache__/opcode.cpython-311.pyc
+-rw-r--r--   0        0        0      193 2024-05-02 14:07:41.658947 lemon8-1.3.9/lemon8/components/constants.py
+-rw-r--r--   0        0        0    12155 2024-05-02 17:32:47.890218 lemon8-1.3.9/lemon8/components/cpu.py
+-rw-r--r--   0        0        0     2871 2024-05-02 17:32:05.700224 lemon8-1.3.9/lemon8/components/display.py
+-rw-r--r--   0        0        0     1644 2024-05-02 14:07:41.658947 lemon8-1.3.9/lemon8/components/keypad.py
+-rw-r--r--   0        0        0      801 2024-05-02 17:49:19.210087 lemon8-1.3.9/lemon8/components/memory.py
+-rw-r--r--   0        0        0     1763 2024-05-02 14:07:41.658947 lemon8-1.3.9/lemon8/components/opcode.py
+-rw-r--r--   0        0        0    40076 2024-05-02 17:08:24.900421 lemon8-1.3.9/lemon8/lemon.png
+-rw-r--r--   0        0        0      536 2024-05-02 17:50:35.410077 lemon8-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 lemon8-1.3.9/PKG-INFO
```

### Comparing `lemon8-1.3.8/LICENSE` & `lemon8-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.8/lemon8/__main__.py` & `lemon8-1.3.9/lemon8/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,25 +48,25 @@
             display=self.display, memory=self.memory, keypad=self.keypad
         )
 
     def load_font(self) -> None:
         """
         Load Font from the `/bin/FONT` file in memory from location `0x0`
         """
-        self.memory.load_binary("./bin/FONT")
+        self.memory.load_binary("lemon8.bin", "FONT")
         logging.info(f"{TICK} Successfully loaded Fontset at location 0x0")
 
     def load_rom(self, rom: str) -> None:
         """
         Load ROM in memory from location `0x200` (512)
 
         Args:
             rom: Path to the ROM file.
         """
-        self.memory.load_binary(rom, offset=INIT_LOC_CONSTANT)
+        self.memory.load_binary("lemon8", rom, offset=INIT_LOC_CONSTANT)
         logging.info(
             f"{TICK} Successfully loaded ROM at location {hex(INIT_LOC_CONSTANT)}"
         )
 
     def tick(self) -> None:
         """
         Method representing a single tick from the emulator.
```

### Comparing `lemon8-1.3.8/lemon8/beep.mp3` & `lemon8-1.3.9/lemon8/beep.mp3`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.8/lemon8/components/__pycache__/cpu.cpython-310.pyc` & `lemon8-1.3.9/lemon8/components/__pycache__/cpu.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.8/lemon8/components/__pycache__/cpu.cpython-311.pyc` & `lemon8-1.3.9/lemon8/components/__pycache__/cpu.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.8/lemon8/components/__pycache__/display.cpython-310.pyc` & `lemon8-1.3.9/lemon8/components/__pycache__/display.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.8/lemon8/components/__pycache__/display.cpython-311.pyc` & `lemon8-1.3.9/lemon8/components/__pycache__/display.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.8/lemon8/components/__pycache__/keypad.cpython-311.pyc` & `lemon8-1.3.9/lemon8/components/__pycache__/keypad.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.8/lemon8/components/__pycache__/memory.cpython-311.pyc` & `lemon8-1.3.9/lemon8/components/__pycache__/memory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.8/lemon8/components/__pycache__/opcode.cpython-311.pyc` & `lemon8-1.3.9/lemon8/components/__pycache__/opcode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.8/lemon8/components/cpu.py` & `lemon8-1.3.9/lemon8/components/cpu.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.8/lemon8/components/display.py` & `lemon8-1.3.9/lemon8/components/display.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.8/lemon8/components/keypad.py` & `lemon8-1.3.9/lemon8/components/keypad.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.8/lemon8/components/memory.py` & `lemon8-1.3.9/lemon8/components/memory.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,18 +15,18 @@
         Memory Constructor.
 
         Attributes:
             space (bytearray): A bytearray of size 4096 virtually representing CHP-8 memory.
         """
         self.space: bytearray = bytearray(4096)
 
-    def load_binary(self, binary: str, offset: int = 0) -> None:
+    def load_binary(self, dir: str, path: str, offset: int = 0) -> None:
         """
         Load file onto the RAM.
 
         Arguments:
             binary: Path to the binary.
             offset: From where to start loading the elements of the binary.
         """
-        with ilr.open_binary("lemon8.bin", "FONT") as f:
+        with ilr.open_binary(dir, path) as f:
             for i, data in enumerate(f.read()):
                 self.space[i + offset] = data
```

### Comparing `lemon8-1.3.8/lemon8/components/opcode.py` & `lemon8-1.3.9/lemon8/components/opcode.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.8/lemon8/lemon.png` & `lemon8-1.3.9/lemon8/lemon.png`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.8/pyproject.toml` & `lemon8-1.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lemon8"
-version = "1.3.8"
+version = "1.3.9"
 description = "A CHIP-8 emulator written in Python."
 authors = ["mooncell07 <80042274+mooncell07@users.noreply.github.com>"]
 license = "MIT"
 documentation = "https://mooncell07.github.io/lemon.pie/"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

