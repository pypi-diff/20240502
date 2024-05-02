# Comparing `tmp/lemon8-1.3.4.tar.gz` & `tmp/lemon8-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemon8-1.3.4.tar", max compression
+gzip compressed data, was "lemon8-1.3.5.tar", max compression
```

## Comparing `lemon8-1.3.4.tar` & `lemon8-1.3.5.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0     1061 2024-05-02 14:07:41.628947 lemon8-1.3.4/LICENSE
--rw-r--r--   0        0        0     1315 2024-05-02 14:07:41.628947 lemon8-1.3.4/README.md
--rw-r--r--   0        0        0     3688 2024-05-02 17:33:07.960216 lemon8-1.3.4/lemon8/__main__.py
--rw-r--r--   0        0        0    22170 2024-05-02 14:07:41.638947 lemon8-1.3.4/lemon8/beep.mp3
--rw-r--r--   0        0        0       80 2024-05-02 14:07:41.638947 lemon8-1.3.4/lemon8/bin/FONT
--rw-r--r--   0        0        0      132 2024-05-02 14:07:41.638947 lemon8-1.3.4/lemon8/bin/ibm.ch8
--rw-r--r--   0        0        0      133 2024-05-02 14:07:41.658947 lemon8-1.3.4/lemon8/components/__init__.py
--rw-r--r--   0        0        0      260 2024-05-02 13:14:11.199127 lemon8-1.3.4/lemon8/components/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      337 2024-05-02 17:00:27.180486 lemon8-1.3.4/lemon8/components/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      346 2024-05-02 13:14:11.199127 lemon8-1.3.4/lemon8/components/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0      391 2024-05-02 17:00:27.190486 lemon8-1.3.4/lemon8/components/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0        0        0    13300 2024-05-02 13:14:11.199127 lemon8-1.3.4/lemon8/components/__pycache__/cpu.cpython-310.pyc
--rw-r--r--   0        0        0    21353 2024-05-02 17:32:51.070218 lemon8-1.3.4/lemon8/components/__pycache__/cpu.cpython-311.pyc
--rw-r--r--   0        0        0     3266 2024-05-02 13:14:11.199127 lemon8-1.3.4/lemon8/components/__pycache__/display.cpython-310.pyc
--rw-r--r--   0        0        0     5014 2024-05-02 17:32:51.070218 lemon8-1.3.4/lemon8/components/__pycache__/display.cpython-311.pyc
--rw-r--r--   0        0        0     3159 2024-05-02 17:00:27.330486 lemon8-1.3.4/lemon8/components/__pycache__/keypad.cpython-311.pyc
--rw-r--r--   0        0        0     1714 2024-05-02 17:00:27.330486 lemon8-1.3.4/lemon8/components/__pycache__/memory.cpython-311.pyc
--rw-r--r--   0        0        0     3383 2024-05-02 17:00:27.330486 lemon8-1.3.4/lemon8/components/__pycache__/opcode.cpython-311.pyc
--rw-r--r--   0        0        0      193 2024-05-02 14:07:41.658947 lemon8-1.3.4/lemon8/components/constants.py
--rw-r--r--   0        0        0    12155 2024-05-02 17:32:47.890218 lemon8-1.3.4/lemon8/components/cpu.py
--rw-r--r--   0        0        0     2871 2024-05-02 17:32:05.700224 lemon8-1.3.4/lemon8/components/display.py
--rw-r--r--   0        0        0     1644 2024-05-02 14:07:41.658947 lemon8-1.3.4/lemon8/components/keypad.py
--rw-r--r--   0        0        0      750 2024-05-02 14:07:41.658947 lemon8-1.3.4/lemon8/components/memory.py
--rw-r--r--   0        0        0     1763 2024-05-02 14:07:41.658947 lemon8-1.3.4/lemon8/components/opcode.py
--rw-r--r--   0        0        0    40076 2024-05-02 17:08:24.900421 lemon8-1.3.4/lemon8/lemon.png
--rw-r--r--   0        0        0      557 2024-05-02 17:33:13.230215 lemon8-1.3.4/pyproject.toml
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 lemon8-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-02 14:07:41.628947 lemon8-1.3.5/LICENSE
+-rw-r--r--   0        0        0     3688 2024-05-02 17:33:07.960216 lemon8-1.3.5/lemon8/__main__.py
+-rw-r--r--   0        0        0    22170 2024-05-02 14:07:41.638947 lemon8-1.3.5/lemon8/beep.mp3
+-rw-r--r--   0        0        0       80 2024-05-02 14:07:41.638947 lemon8-1.3.5/lemon8/bin/FONT
+-rw-r--r--   0        0        0      132 2024-05-02 14:07:41.638947 lemon8-1.3.5/lemon8/bin/ibm.ch8
+-rw-r--r--   0        0        0      133 2024-05-02 14:07:41.658947 lemon8-1.3.5/lemon8/components/__init__.py
+-rw-r--r--   0        0        0      260 2024-05-02 13:14:11.199127 lemon8-1.3.5/lemon8/components/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      337 2024-05-02 17:00:27.180486 lemon8-1.3.5/lemon8/components/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      346 2024-05-02 13:14:11.199127 lemon8-1.3.5/lemon8/components/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0      391 2024-05-02 17:00:27.190486 lemon8-1.3.5/lemon8/components/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0        0        0    13300 2024-05-02 13:14:11.199127 lemon8-1.3.5/lemon8/components/__pycache__/cpu.cpython-310.pyc
+-rw-r--r--   0        0        0    21353 2024-05-02 17:32:51.070218 lemon8-1.3.5/lemon8/components/__pycache__/cpu.cpython-311.pyc
+-rw-r--r--   0        0        0     3266 2024-05-02 13:14:11.199127 lemon8-1.3.5/lemon8/components/__pycache__/display.cpython-310.pyc
+-rw-r--r--   0        0        0     5014 2024-05-02 17:32:51.070218 lemon8-1.3.5/lemon8/components/__pycache__/display.cpython-311.pyc
+-rw-r--r--   0        0        0     3159 2024-05-02 17:00:27.330486 lemon8-1.3.5/lemon8/components/__pycache__/keypad.cpython-311.pyc
+-rw-r--r--   0        0        0     1714 2024-05-02 17:00:27.330486 lemon8-1.3.5/lemon8/components/__pycache__/memory.cpython-311.pyc
+-rw-r--r--   0        0        0     3383 2024-05-02 17:00:27.330486 lemon8-1.3.5/lemon8/components/__pycache__/opcode.cpython-311.pyc
+-rw-r--r--   0        0        0      193 2024-05-02 14:07:41.658947 lemon8-1.3.5/lemon8/components/constants.py
+-rw-r--r--   0        0        0    12155 2024-05-02 17:32:47.890218 lemon8-1.3.5/lemon8/components/cpu.py
+-rw-r--r--   0        0        0     2871 2024-05-02 17:32:05.700224 lemon8-1.3.5/lemon8/components/display.py
+-rw-r--r--   0        0        0     1644 2024-05-02 14:07:41.658947 lemon8-1.3.5/lemon8/components/keypad.py
+-rw-r--r--   0        0        0      775 2024-05-02 17:39:06.570170 lemon8-1.3.5/lemon8/components/memory.py
+-rw-r--r--   0        0        0     1763 2024-05-02 14:07:41.658947 lemon8-1.3.5/lemon8/components/opcode.py
+-rw-r--r--   0        0        0    40076 2024-05-02 17:08:24.900421 lemon8-1.3.5/lemon8/lemon.png
+-rw-r--r--   0        0        0      536 2024-05-02 17:39:22.910168 lemon8-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 lemon8-1.3.5/PKG-INFO
```

### Comparing `lemon8-1.3.4/LICENSE` & `lemon8-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/lemon8/__main__.py` & `lemon8-1.3.5/lemon8/__main__.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/lemon8/beep.mp3` & `lemon8-1.3.5/lemon8/beep.mp3`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/lemon8/components/__pycache__/cpu.cpython-310.pyc` & `lemon8-1.3.5/lemon8/components/__pycache__/cpu.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/lemon8/components/__pycache__/cpu.cpython-311.pyc` & `lemon8-1.3.5/lemon8/components/__pycache__/cpu.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/lemon8/components/__pycache__/display.cpython-310.pyc` & `lemon8-1.3.5/lemon8/components/__pycache__/display.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/lemon8/components/__pycache__/display.cpython-311.pyc` & `lemon8-1.3.5/lemon8/components/__pycache__/display.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/lemon8/components/__pycache__/keypad.cpython-311.pyc` & `lemon8-1.3.5/lemon8/components/__pycache__/keypad.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/lemon8/components/__pycache__/memory.cpython-311.pyc` & `lemon8-1.3.5/lemon8/components/__pycache__/memory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/lemon8/components/__pycache__/opcode.cpython-311.pyc` & `lemon8-1.3.5/lemon8/components/__pycache__/opcode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/lemon8/components/cpu.py` & `lemon8-1.3.5/lemon8/components/cpu.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/lemon8/components/display.py` & `lemon8-1.3.5/lemon8/components/display.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/lemon8/components/keypad.py` & `lemon8-1.3.5/lemon8/components/keypad.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/lemon8/components/opcode.py` & `lemon8-1.3.5/lemon8/components/opcode.py`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/lemon8/lemon.png` & `lemon8-1.3.5/lemon8/lemon.png`

 * *Files identical despite different names*

### Comparing `lemon8-1.3.4/pyproject.toml` & `lemon8-1.3.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [tool.poetry]
 name = "lemon8"
-version = "1.3.4"
+version = "1.3.5"
 description = "A CHIP-8 emulator written in Python."
 authors = ["mooncell07 <80042274+mooncell07@users.noreply.github.com>"]
 license = "MIT"
-readme = "README.md"
 documentation = "https://mooncell07.github.io/lemon.pie/"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pygame = "^2.2.0"
 
 [tool.poetry.group.dev.dependencies]
```

