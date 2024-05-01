# Comparing `tmp/pthugefileviewer-0.4.0.tar.gz` & `tmp/pthugefileviewer-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pthugefileviewer-0.4.0.tar", last modified: Sun Apr  7 21:32:45 2024, max compression
+gzip compressed data, was "pthugefileviewer-0.4.1.tar", last modified: Wed May  1 22:08:28 2024, max compression
```

## Comparing `pthugefileviewer-0.4.0.tar` & `pthugefileviewer-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:32:45.837603 pthugefileviewer-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-07 21:32:45.837603 pthugefileviewer-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:32:45.837603 pthugefileviewer-0.4.0/pthugefileviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-07 21:32:45.000000 pthugefileviewer-0.4.0/pthugefileviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-07 21:32:45.000000 pthugefileviewer-0.4.0/pthugefileviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:32:45.000000 pthugefileviewer-0.4.0/pthugefileviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 21:32:45.000000 pthugefileviewer-0.4.0/pthugefileviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-07 21:32:45.000000 pthugefileviewer-0.4.0/pthugefileviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-07 21:32:45.837603 pthugefileviewer-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:32:45.833603 pthugefileviewer-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:32:45.833603 pthugefileviewer-0.4.0/src/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9968 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/src/bin/hfv-regexbuild
--rwxr-xr-x   0 runner    (1001) docker     (127)     1895 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/src/bin/hfv-view
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:32:45.837603 pthugefileviewer-0.4.0/src/pthugefileviewer/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/src/pthugefileviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/src/pthugefileviewer/hugefilevieweruicontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/src/pthugefileviewer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:32:45.837603 pthugefileviewer-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/tests/test_hfv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:08:28.575317 pthugefileviewer-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-01 22:08:28.575317 pthugefileviewer-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:08:28.575317 pthugefileviewer-0.4.1/pthugefileviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-01 22:08:28.000000 pthugefileviewer-0.4.1/pthugefileviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-01 22:08:28.000000 pthugefileviewer-0.4.1/pthugefileviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:08:28.000000 pthugefileviewer-0.4.1/pthugefileviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 22:08:28.000000 pthugefileviewer-0.4.1/pthugefileviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 22:08:28.000000 pthugefileviewer-0.4.1/pthugefileviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-01 22:08:28.575317 pthugefileviewer-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:08:28.571317 pthugefileviewer-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:08:28.575317 pthugefileviewer-0.4.1/src/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7986 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/src/bin/hfv-regexbuild
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1895 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/src/bin/hfv-view
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:08:28.575317 pthugefileviewer-0.4.1/src/pthugefileviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/src/pthugefileviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/src/pthugefileviewer/hugefilevieweruicontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/src/pthugefileviewer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:08:28.575317 pthugefileviewer-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-01 22:08:21.000000 pthugefileviewer-0.4.1/tests/test_hfv.py
```

### Comparing `pthugefileviewer-0.4.0/LICENSE` & `pthugefileviewer-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.4.0/PKG-INFO` & `pthugefileviewer-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pthugefileviewer
-Version: 0.4.0
+Version: 0.4.1
 Summary: Huge file viewer control for prompt-toolkit
 Home-page: http://github.com/lpenz/pthugefileviewer
 Author: "Leandro Lisboa Penz"
 Author-email: "lpenz@lpenz.org"
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

### Comparing `pthugefileviewer-0.4.0/README.md` & `pthugefileviewer-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.4.0/pthugefileviewer.egg-info/PKG-INFO` & `pthugefileviewer-0.4.1/pthugefileviewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pthugefileviewer
-Version: 0.4.0
+Version: 0.4.1
 Summary: Huge file viewer control for prompt-toolkit
 Home-page: http://github.com/lpenz/pthugefileviewer
 Author: "Leandro Lisboa Penz"
 Author-email: "lpenz@lpenz.org"
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

### Comparing `pthugefileviewer-0.4.0/setup.cfg` & `pthugefileviewer-0.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pthugefileviewer
-version = 0.4.0
+version = 0.4.1
 description = Huge file viewer control for prompt-toolkit
 license = MIT
 license_files = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = "Leandro Lisboa Penz"
 author_email = "lpenz@lpenz.org"
```

### Comparing `pthugefileviewer-0.4.0/src/bin/hfv-regexbuild` & `pthugefileviewer-0.4.1/src/bin/hfv-regexbuild`

 * *Files 18% similar despite different names*

```diff
@@ -29,74 +29,18 @@
 from prompt_toolkit.layout.utils import explode_text_fragments
 from prompt_toolkit.styles import Style
 from prompt_toolkit.widgets import Frame
 
 E = KeyPressEvent
 
 
-class FileviewControl(pthugefileviewer.HugeFileViewerUIControl):
+class FileviewControl(pthugefileviewer.HugeFileViewerRegexUIControl):
     def __init__(self, filename: os.PathLike[str]) -> None:
-        self.regex: Optional[re.Pattern[bytes]] = None
-        self.regex_ok: Optional[re.Pattern[bytes]] = None
         with open(filename, "rb") as fd:
-            pthugefileviewer.HugeFileViewerUIControl.__init__(self, fd=fd)
-
-    def use_regex(self, regex: Optional[re.Pattern[bytes]]) -> None:
-        self.regex = regex
-        self.update_lines()
-
-    def search_down(self) -> None:
-        if self.regex is None:
-            return
-        with self.tmp_offset():
-            self.go_pagedown()
-            offset = self.offset
-        m = self.re_search(self.regex, offset)
-        if m:
-            self.go_line_offset(m.end())
-            self.go_up(self.height - 2)
-        else:
-            self.update_lines()
-
-    def update_lines(self) -> None:
-        contents = b"\n".join(self.get_lines())
-        m = None
-        if self.regex is not None:
-            m = self.regex.search(contents)
-        if m:
-            self.regex_ok = self.regex
-            style = "class:match"
-        elif not m and self.regex_ok is not None:
-            m = self.regex_ok.search(contents)
-            style = "class:oldmatch"
-        if not m:
-            pthugefileviewer.HugeFileViewerUIControl.update_lines(self)
-            return
-        start = m.start()
-        end = m.end()
-        pre, matched, pos = contents[:start], contents[start:end], contents[end:]
-        self._lines = []
-        current: StyleAndTextTuples = []
-        lines = pre.split(b"\n")
-        for i, line in enumerate(lines):
-            current += [("", line.decode("utf-8"))]
-            if i != len(lines) - 1:
-                self._lines.append(current)
-                current = []
-        lines = matched.split(b"\n")
-        for i, line in enumerate(lines):
-            current += [(style, line.decode("utf-8"))]
-            if i != len(lines) - 1:
-                self._lines.append(current)
-                current = []
-        lines = pos.split(b"\n")
-        for i, line in enumerate(lines):
-            current += [("", line.decode("utf-8"))]
-            self._lines.append(current)
-            current = []
+            pthugefileviewer.HugeFileViewerRegexUIControl.__init__(self, fd=fd)
 
 
 class FileviewWidget:
     def __init__(self, filename: os.PathLike[str]):
         self.filename = filename
         self.control = FileviewControl(filename)
         self.window = Window(self.control, style=self.get_style)
@@ -287,15 +231,15 @@
     def c_home(event: E) -> None:
         fileview.control.go_top()
 
     @kb.add("c-end")
     def c_end(event: E) -> None:
         fileview.control.go_bottom()
 
-    @kb.add("escape", "j")
+    @kb.add("f3")
     def search_down(event: E) -> None:
         fileview.control.search_down()
 
     @kb.add("c-c")
     @kb.add("c-d")
     @kb.add("escape", "q")
     def close(event: E) -> None:
```

### Comparing `pthugefileviewer-0.4.0/src/bin/hfv-view` & `pthugefileviewer-0.4.1/src/bin/hfv-view`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.4.0/src/pthugefileviewer/hugefilevieweruicontrol.py` & `pthugefileviewer-0.4.1/src/pthugefileviewer/hugefilevieweruicontrol.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Control for the huge file widget"""
 
 import io
 import mmap
 import re
 from contextlib import contextmanager
-from typing import TYPE_CHECKING, Generator, List, Optional  # noqa: I101
+from typing import TYPE_CHECKING, Generator, Iterator, List, Optional  # noqa: I101
 
 from prompt_toolkit.formatted_text import StyleAndTextTuples
 from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.key_binding.key_bindings import KeyBindingsBase
 from prompt_toolkit.key_binding.key_processor import KeyPressEvent
 from prompt_toolkit.layout.controls import UIContent, UIControl
 from prompt_toolkit.mouse_events import MouseEvent, MouseEventType
@@ -42,14 +42,17 @@
 
     @offset.setter
     def offset(self, offset: int) -> None:
         if offset < 0:
             offset = 0
         if offset >= self._offset_max:
             self._offset = self._offset_max
+        assert (
+            offset == 0 or self.get_char(offset - 1) == b"\n"
+        ), f"offset {offset} char {self.get_char(offset - 1)!r}"
         self._mm.seek(offset)
         self.update_lines()
 
     @property
     def height(self) -> int:
         return self._height
 
@@ -78,36 +81,33 @@
         finally:
             self._mm.seek(offset)
 
     def find_prev_newline(self, offset: int) -> int:
         start_offset = (self._size % mmap.PAGESIZE) - 2 * mmap.PAGESIZE
         return self._mm.rfind(b"\n", max(0, start_offset), offset)
 
-    def get_lines(self) -> List[bytes]:
+    def get_lines(self) -> Iterator[bytes]:
         with self.tmp_offset():
-            lines = []
             for _ in range(self._height):
                 line = self._mm.readline()
                 if not line:
                     break
-                line = line.rstrip()
-                lines.append(line)
-            return lines
+                yield line.rstrip()
 
     def update_lines(self) -> None:
         self._lines = [
             [("", line.decode("utf-8", errors="replace"))] for line in self.get_lines()
         ]
         if self.height > len(self._lines) and self.offset < self._offset_max:
             self.go_up(self._height - len(self._lines))
 
     def get_char(self, offset: Optional[int] = None) -> bytes:
         with self.tmp_offset():
             if offset is not None:
-                self.offset = offset
+                self._mm.seek(offset)
             return self._mm.read(1)
 
     # Implement UIControl methods:
 
     def _get_line(self, lineno: int) -> StyleAndTextTuples:
         if lineno >= len(self._lines):
             return [("", "")]
@@ -145,24 +145,17 @@
             self.go_down()
         else:
             return NotImplemented
         return None
 
     # Exported utility functions:
 
-    def re_search(
-        self, regex: re.Pattern[bytes], offset: Optional[int] = None
-    ) -> Optional[re.Match[bytes]]:
-        offset = offset or 0
-        with self.tmp_offset():
-            return regex.search(bytes(self._mm), offset)
-
     def go_line_offset(self, offset: int) -> None:
-        self.offset = offset
-        if self.get_char(offset - 1) == b"\n":
+        if offset == 0 or self.get_char(offset - 1) == b"\n":
+            self.offset = offset
             return
         offset = self.find_prev_newline(offset)
         if offset != -1:
             self.offset = offset + 1
 
     def go_top(self) -> None:
         self.offset = 0
@@ -197,7 +190,75 @@
         self.update_lines()
 
     def go_pageup(self) -> None:
         self.go_up(self.height)
 
     def go_pagedown(self) -> None:
         self.go_down(self.height)
+
+
+class HugeFileViewerRegexUIControl(HugeFileViewerUIControl):
+    def __init__(self, fd: io.BufferedReader):
+        self.regex: Optional[re.Pattern[bytes]] = None
+        self.regex_ok: Optional[re.Pattern[bytes]] = None
+        HugeFileViewerUIControl.__init__(self, fd)
+
+    def re_search(
+        self, regex: re.Pattern[bytes], offset: Optional[int] = None
+    ) -> Optional[re.Match[bytes]]:
+        offset = offset or 0
+        with self.tmp_offset():
+            return regex.search(bytes(self._mm), offset)
+
+    def use_regex(self, regex: Optional[re.Pattern[bytes]]) -> None:
+        self.regex = regex
+        self.update_lines()
+
+    def search_down(self) -> None:
+        if self.regex is None:
+            return
+        with self.tmp_offset():
+            self.go_pagedown()
+            offset = self.offset
+        m = self.re_search(self.regex, offset)
+        if m:
+            self.go_line_offset(m.end())
+            self.go_down(1)
+        else:
+            self.update_lines()
+
+    def update_lines(self) -> None:
+        contents = b"\n".join(self.get_lines())
+        m = None
+        if self.regex is not None:
+            m = self.regex.search(contents)
+        if m:
+            self.regex_ok = self.regex
+            style = "class:match"
+        elif not m and self.regex_ok is not None:
+            m = self.regex_ok.search(contents)
+            style = "class:oldmatch"
+        if not m:
+            HugeFileViewerUIControl.update_lines(self)
+            return
+        start = m.start()
+        end = m.end()
+        pre, matched, pos = contents[:start], contents[start:end], contents[end:]
+        self._lines = []
+        current: StyleAndTextTuples = []
+        lines = pre.split(b"\n")
+        for i, line in enumerate(lines):
+            current += [("", line.decode("utf-8"))]
+            if i != len(lines) - 1:
+                self._lines.append(current)
+                current = []
+        lines = matched.split(b"\n")
+        for i, line in enumerate(lines):
+            current += [(style, line.decode("utf-8"))]
+            if i != len(lines) - 1:
+                self._lines.append(current)
+                current = []
+        lines = pos.split(b"\n")
+        for i, line in enumerate(lines):
+            current += [("", line.decode("utf-8"))]
+            self._lines.append(current)
+            current = []
```

