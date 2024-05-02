# Comparing `tmp/grbl_streamer-2.0.0.tar.gz` & `tmp/grbl_streamer-2.0.2.tar.gz`

## Comparing `grbl_streamer-2.0.0.tar` & `grbl_streamer-2.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 grbl_streamer-2.0.0/Pipfile
--rw-r--r--   0        0        0    26606 2020-02-02 00:00:00.000000 grbl_streamer-2.0.0/Pipfile.lock
--rw-r--r--   0        0        0    41880 2020-02-02 00:00:00.000000 grbl_streamer-2.0.0/src/grbl_streamer/__init__.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 grbl_streamer-2.0.0/src/grbl_streamer/callbackloghandler.py
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 grbl_streamer-2.0.0/src/grbl_streamer/interface.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 grbl_streamer-2.0.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 grbl_streamer-2.0.0/COPYING
--rw-r--r--   0        0        0    12910 2020-02-02 00:00:00.000000 grbl_streamer-2.0.0/README.md
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 grbl_streamer-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    53951 2020-02-02 00:00:00.000000 grbl_streamer-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 grbl_streamer-2.0.2/Pipfile
+-rw-r--r--   0        0        0    26606 2020-02-02 00:00:00.000000 grbl_streamer-2.0.2/Pipfile.lock
+-rw-r--r--   0        0        0    41961 2020-02-02 00:00:00.000000 grbl_streamer-2.0.2/src/grbl_streamer/__init__.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 grbl_streamer-2.0.2/src/grbl_streamer/callbackloghandler.py
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 grbl_streamer-2.0.2/src/grbl_streamer/interface.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 grbl_streamer-2.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 grbl_streamer-2.0.2/COPYING
+-rw-r--r--   0        0        0    12910 2020-02-02 00:00:00.000000 grbl_streamer-2.0.2/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 grbl_streamer-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    53944 2020-02-02 00:00:00.000000 grbl_streamer-2.0.2/PKG-INFO
```

### Comparing `grbl_streamer-2.0.0/Pipfile.lock` & `grbl_streamer-2.0.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `grbl_streamer-2.0.0/src/grbl_streamer/__init__.py` & `grbl_streamer-2.0.2/src/grbl_streamer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,18 @@
     After assigning your own callback function (callback = ...)
     you will receive the following signals:
 
     on_boot
     : Emitted whenever Grbl boots (e.g. after a soft reset).
     : No arguments.
 
+    on_read
+    : Emitted whenever a line is read by GrblStreamer
+    : 1 argument: line
+
     on_disconnected
     : Emitted whenever the serial port has been closed.
     : No arguments
 
     on_log
     : Emitted for informal logging or debugging messages.
     : 1 argument: LogRecord instance
@@ -869,21 +873,21 @@
                 elif line == 'ok':
                     self._handle_ok()
 
                 elif re.match(r'^\[G[0123] .*', line):
                     self._update_gcode_parser_state(line)
                     self._callback("on_read", line)
 
-                elif line == '[MSG:Caution: Unlocked]':
+                elif line.startswith('[MSG:'):
                     # nothing to do here
                     pass
 
                 elif re.match(r'^\[...:.*', line):
-                    self._update_hash_state(line)
                     self._callback('on_read', line)
+                    self._update_hash_state(line)
 
                     if 'PRB' in line:
                         # last line
                         self._callback('on_hash_stateupdate', self.settings_hash)
                         self.preprocessor.cs_offsets = self.settings_hash
                         self._callback('on_probe', self.settings_hash['PRB'])
```

### Comparing `grbl_streamer-2.0.0/src/grbl_streamer/callbackloghandler.py` & `grbl_streamer-2.0.2/src/grbl_streamer/callbackloghandler.py`

 * *Files identical despite different names*

### Comparing `grbl_streamer-2.0.0/src/grbl_streamer/interface.py` & `grbl_streamer-2.0.2/src/grbl_streamer/interface.py`

 * *Files identical despite different names*

### Comparing `grbl_streamer-2.0.0/COPYING` & `grbl_streamer-2.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `grbl_streamer-2.0.0/README.md` & `grbl_streamer-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `grbl_streamer-2.0.0/pyproject.toml` & `grbl_streamer-2.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "grbl-streamer"
 authors = [
-  {name = "Michael Franzl", email = "public.michael@franzl.name"},
+  {name = "Michael Franzl", email = "michael@franzl.name"},
 ]
-version = "2.0.0"
+version = "2.0.2"
 description = "Universal interface module written in Python 3 for the grbl CNC firmware"
 readme = "README.md"
 requires-python = ">=3.5"
 dependencies = [
   "gcode-machine ~= 1.0",
   "pyserial ~= 3.5",
 ]
```

### Comparing `grbl_streamer-2.0.0/PKG-INFO` & `grbl_streamer-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: grbl-streamer
-Version: 2.0.0
+Version: 2.0.2
 Summary: Universal interface module written in Python 3 for the grbl CNC firmware
 Project-URL: repository, https://github.com/michaelfranzl/grbl-streamer
-Author-email: Michael Franzl <public.michael@franzl.name>
+Author-email: Michael Franzl <michael@franzl.name>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

