# Comparing `tmp/formol-0.5.0.tar.gz` & `tmp/formol-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formol-0.5.0.tar", max compression
+gzip compressed data, was "formol-0.6.0.tar", max compression
```

## Comparing `formol-0.5.0.tar` & `formol-0.6.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0    37464 2024-05-01 19:13:11.028779 formol-0.5.0/formol.py
--rw-r--r--   0        0        0     1802 2024-05-01 19:14:28.475326 formol-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 formol-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    38279 2024-05-02 15:05:27.388923 formol-0.6.0/formol.py
+-rw-r--r--   0        0        0     1786 2024-05-02 15:05:30.882261 formol-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 formol-0.6.0/PKG-INFO
```

### Comparing `formol-0.5.0/formol.py` & `formol-0.6.0/formol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2024 Philippe Proulx <eeppeliteloop@gmail.com>
+# Copyright (c) 2024 Philippe Proulx <eepp.ca>
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -17,14 +17,23 @@
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 # CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 # TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 # pyright: strict
 
+__all__ = [
+    'format',
+    'format_c_block_comment',
+    'format_prefixed_block_comment',
+]
+__version__ = '0.6.0'
+__author__ = 'Philippe Proulx <eepp.ca>'
+
+
 from typing import Dict, Any, Type, TypeVar, Callable, List, Sequence, Union, Pattern, Match, Optional
 from dataclasses import dataclass
 import re
 
 
 # Element base.
 class _Elem:
@@ -879,38 +888,52 @@
 
         for i, line in enumerate(lines):
             if len(line) >= 1:
                 lines[i] = f'{" " * indent_len}{line}'
 
         return lines
 
+    @staticmethod
+    def _p_line_list_len(lst: List[str]):
+        return sum([len(t) for t in lst])
+
     # Returns the lines of the paragraph `p`.
     def _p_lines(self, p: _P):
-        lines: List[str] = ['']
+        lines: List[List[str]] = [[]]
 
         # append each word, wrapping when necessary
         for word in p.words:
             to_append = f'{word} '
 
             if len(lines[-1]) == 0:
                 # first word of the line, in case it doesn't fit
-                lines[-1] += to_append
-            elif len(lines[-1]) + len(word) > self._max_line_len:
+                lines[-1].append(to_append)
+            elif self._p_line_list_len(lines[-1]) + len(word) > self._max_line_len:
                 # new line
-                lines.append(to_append)
+                lines.append([to_append])
             else:
                 # append to current line
-                lines[-1] += to_append
+                lines[-1].append(to_append)
+
+        # avoid runt: if there are at least two lines and the last line
+        # contains a single word when two would fit, then just do it:
+        # this is more readable than a single word on the last line
+        if len(lines) >= 2 and len(lines[-1]) == 1 and len(lines[-2][-1]) + len(lines[-1][0]) - 1 <= self._max_line_len:
+            lines[-1] = [lines[-2][-1], lines[-1][0]]
+            del lines[-2][-1]
+
+        # convert to real lines
+        new_lines = list(map(lambda words: ''.join(words), lines))
 
         # remove trailing empty lines
-        lines = _remove_trailing_empty_lines(lines)
+        new_lines = _remove_trailing_empty_lines(new_lines)
 
         # append final empty line and return lines
-        lines.append('')
-        return lines
+        new_lines.append('')
+        return new_lines
 
     # Returns the lines of the unordered list item `item`.
     def _ul_item_lines(self, item: _SimpleListItem):
         # get indented element lines
         lines = self._format_elems_indented(item.elems, 2)
 
         # insert bullet point
```

### Comparing `formol-0.5.0/pyproject.toml` & `formol-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2024 Philippe Proulx <eeppeliteloop@gmail.com>
+# Copyright (c) 2024 Philippe Proulx <eepp.ca>
 #
 # Permission is hereby granted, free of charge, to any person obtaining
 # a copy of this software and associated documentation files (the
 # "Software"), to deal in the Software without restriction, including
 # without limitation the rights to use, copy, modify, merge, publish,
 # distribute, sublicense, and/or sell copies of the Software, and to
 # permit persons to whom the Software is furnished to do so, subject to
@@ -21,15 +21,15 @@
 
 [build-system]
 requires = ['poetry-core']
 build-backend = 'poetry.core.masonry.api'
 
 [tool.poetry]
 name = 'formol'
-version = '0.5.0'
+version = '0.6.0'
 description = 'Plain text beautifier'
 license = 'MIT'
 authors = ['Philippe Proulx <eeppeliteloop@gmail.com>']
 repository = 'https://github.com/eepp/formol/'
 classifiers = [
 	'Development Status :: 4 - Beta',
 	'License :: OSI Approved :: MIT License',
```

### Comparing `formol-0.5.0/PKG-INFO` & `formol-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formol
-Version: 0.5.0
+Version: 0.6.0
 Summary: Plain text beautifier
 Home-page: https://github.com/eepp/formol/
 License: MIT
 Author: Philippe Proulx
 Author-email: eeppeliteloop@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

