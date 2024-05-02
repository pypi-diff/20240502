# Comparing `tmp/gaplint-1.1.5.tar.gz` & `tmp/gaplint-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaplint-1.1.5.tar", last modified: Fri Jan 13 10:27:31 2023, max compression
+gzip compressed data, was "gaplint-1.2.0.tar", last modified: Thu May  2 10:18:46 2024, max compression
```

## Comparing `gaplint-1.1.5.tar` & `gaplint-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 10:27:31.881681 gaplint-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-01-13 10:27:22.000000 gaplint-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15721 2023-01-13 10:27:31.881681 gaplint-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-01-13 10:27:22.000000 gaplint-1.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 10:27:31.881681 gaplint-1.1.5/gaplint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15721 2023-01-13 10:27:31.000000 gaplint-1.1.5/gaplint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-13 10:27:31.000000 gaplint-1.1.5/gaplint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 10:27:31.000000 gaplint-1.1.5/gaplint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-13 10:27:31.000000 gaplint-1.1.5/gaplint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 10:27:31.000000 gaplint-1.1.5/gaplint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-13 10:27:31.000000 gaplint-1.1.5/gaplint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-13 10:27:31.000000 gaplint-1.1.5/gaplint.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    54360 2023-01-13 10:27:22.000000 gaplint-1.1.5/gaplint.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-13 10:27:22.000000 gaplint-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-13 10:27:31.881681 gaplint-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-01-13 10:27:22.000000 gaplint-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:18:46.066417 gaplint-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-02 10:18:40.000000 gaplint-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-02 10:18:46.066417 gaplint-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-05-02 10:18:40.000000 gaplint-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:18:46.066417 gaplint-1.2.0/gaplint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-02 10:18:46.000000 gaplint-1.2.0/gaplint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-02 10:18:46.000000 gaplint-1.2.0/gaplint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:18:46.000000 gaplint-1.2.0/gaplint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 10:18:46.000000 gaplint-1.2.0/gaplint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:18:45.000000 gaplint-1.2.0/gaplint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 10:18:46.000000 gaplint-1.2.0/gaplint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 10:18:46.000000 gaplint-1.2.0/gaplint.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    59984 2024-05-02 10:18:40.000000 gaplint-1.2.0/gaplint.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 10:18:40.000000 gaplint-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-02 10:18:46.066417 gaplint-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-02 10:18:40.000000 gaplint-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:18:46.066417 gaplint-1.2.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8520 2024-05-02 10:18:40.000000 gaplint-1.2.0/tests/test_gaplint.py
```

### Comparing `gaplint-1.1.5/LICENSE` & `gaplint-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaplint-1.1.5/gaplint.py` & `gaplint-1.2.0/gaplint.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 """
 This module provides functions for automatically checking the format of a GAP
 file according to some conventions.
 """
-# pylint: disable=fixme, too-many-lines, invalid-name,
-# pylint: disable=bad-option-value, consider-using-f-string
+# pylint: disable=fixme, too-many-lines
 
 import argparse
 import os
 import re
 import sys
+from typing import Callable, Tuple, List, Dict, Union, Optional
 
 from os import listdir
 from os.path import isdir, exists, isfile, abspath, join
+from importlib.metadata import version
 
-import pkg_resources
 import yaml
 
 ###############################################################################
 # Globals
 ###############################################################################
 
 _VERBOSE = False
@@ -58,133 +58,143 @@
     "IsBound",
     "Unbind",
     "TryNextMethod",
     "Info",
     "Assert",
 }
 
-_DEFAULT_CONFIG = {"max_warnings": 1000, "columns": 80, "indentation": 2}
+_DEFAULT_CONFIG = {
+    "max_warnings": 1000,
+    "columns": 80,
+    "indentation": 2,
+    "duplicate-function-min-length": 4,
+}
 
 _GLOB_CONFIG = {}
 _GLOB_SUPPRESSIONS = {}
 _FILE_SUPPRESSIONS = {}
 _LINE_SUPPRESSIONS = {}
 
-_CONFIGURED = False
 _LINE_RULES = []
 _FILE_RULES = []
 _EXPERIMENTAL_FILE_RULES = []
 
 _ESCAPE_PATTERN = re.compile(r"(^\\(\\\\)*[^\\]+.*$|^\\(\\\\)*$)")
 
 
 ###############################################################################
 # Strings helpers
 ###############################################################################
 
 
-def _is_tst_or_xml_file(fname):
+def _is_tst_or_xml_file(fname: str) -> bool:
     """Returns True if the extension of fname is '.xml' or '.tst'."""
     assert isinstance(fname, str)
     ext = fname.split(".")[-1]
     return ext in ("tst", "xml")
 
 
-def _is_escaped(lines, pos):
+def _is_escaped(lines: str, pos: int) -> Union[bool, re.Match, None]:
     assert isinstance(lines, str)
     assert isinstance(pos, int)
     assert 0 <= pos < len(lines)
     if lines[pos - 1] != "\\":
         return False
     start = lines.rfind("\n", 0, pos)
     # Search for an odd number of backslashes immediately before line[pos]
     return _ESCAPE_PATTERN.search(lines[start + 1 : pos][::-1])
 
 
-def _is_double_quote_in_char(line, pos):
+def _is_double_quote_in_char(line: str, pos: int) -> bool:
     assert isinstance(line, str)
     assert isinstance(pos, int)
     assert 0 <= pos < len(line)
     return (
         pos > 0
         and pos + 1 < len(line)
         and line[pos - 1 : pos + 2] == "'\"'"
         and not _is_escaped(line, pos - 1)
     )
 
 
-def _is_in_string(lines, pos):
+def _is_in_string(lines: str, pos: int) -> bool:
+    assert isinstance(lines, str)
+    assert isinstance(pos, int)
     start = lines.rfind("\n", 0, pos)
     line = re.sub(r"\\.", "", lines[start:pos])
     return line.count('"') % 2 == 1 or line.count("'") % 2 == 1
 
 
 ###############################################################################
 # Info messages
 ###############################################################################
 
 
-def _warn_or_error(fname, linenum, msg, threshold):
+# TODO report rule code and/or name here too
+def _warn_or_error(fname: str, linenum: int, msg: str, threshold: int) -> None:
     if not _SILENT:
         assert isinstance(fname, str)
         assert isinstance(linenum, int)
         assert isinstance(msg, str)
         assert isinstance(threshold, int)
-        sys.stderr.write(
-            "%s:%d: %s [%d]\n" % (fname, linenum + 1, msg, threshold)
-        )
+        sys.stderr.write(f"{fname}:{linenum + 1}: {msg} [{threshold}]\n")
 
 
-def _warn(fname, linenum, msg):
+def _warn(fname: str, linenum: int, msg: str) -> None:
     _warn_or_error(fname, linenum, msg, 0)
 
 
-def _error(fname, linenum, msg):
+def _error(fname: str, linenum: int, msg: str) -> None:
     _warn_or_error(fname, linenum, msg, 1)
     sys.exit("Aborting!")
 
 
-def _info_statement(msg):
+def _info_action(msg: str) -> None:
     if not _SILENT:
         assert isinstance(msg, str)
-        sys.stdout.write("\033[40;38;5;82m%s\033[0m\n" % msg)
+        sys.stdout.write(f"\033[33m{msg}\033[0m\n")
 
 
-def _info_action(msg):
-    if not _SILENT:
-        assert isinstance(msg, str)
-        sys.stdout.write("\033[33m%s\033[0m\n" % msg)
-
-
-def _info_verbose(msg):
+def _info_verbose(msg: str) -> None:
     if not _SILENT and _VERBOSE:
         assert isinstance(msg, str)
-        sys.stdout.write("\033[40;38;5;208m%s\033[0m\n" % msg)
+        sys.stdout.write(f"\033[2m{msg}\033[0m\n")
 
 
 ###############################################################################
-# Rules: a rule is just a function or callable class.
+# Rules: a rule must have Rule as a base class.
 ###############################################################################
 
 
 class Rule:  # pylint: disable=too-few-public-methods
     """
     Base class for rules.
 
     A rule is a subclass of this class which has a __call__ method that returns
-    TODO
+    Tuple[int, str] where the \"int\" is the number of warnings issued, and where
+    the \"str\" is the lines of the file on which the rules are being applied.
     """
 
-    def __init__(self, name=None, code=None):
+    _all_codes = set()
+    _all_names = set()
+
+    def __init__(self, name: Optional[str] = None, code: Optional[str] = None):
         assert isinstance(name, str) or (name is None and code is None)
         assert isinstance(code, str) or (name is None and code is None)
+        if __debug__:
+            if code is not None and code in Rule._all_codes:
+                raise ValueError(f"Duplicate rule code {code}")
+            Rule._all_codes.add(code)
+            if name is not None and code in Rule._all_names:
+                raise ValueError(f"Duplicate rule name {name}")
+            Rule._all_names.add(name)
         self.name = name
         self.code = code
 
-    def reset(self):
+    def reset(self) -> None:
         """
         Reset the rule.
 
         This is only used by rules like those for checking the indentation of
         lines. This method is called once per file on which gaplint it run, so
         that issues with indentation, for example, in one file do not spill
         over into the next file.
@@ -196,36 +206,36 @@
     Instances of this class produce a warning whenever a line matches the
     pattern used to construct the instance except if one of a list of
     exceptions is also matched.
     """
 
     def __init__(  # pylint: disable=too-many-arguments, dangerous-default-value
         self,
-        name,
-        code,
-        pattern,
-        warning_msg,
-        exceptions=[],
-        skip=lambda fname: False,
-    ):
+        name: str,
+        code: str,
+        pattern: str,
+        warning_msg: str,
+        exceptions: List[str] = [],
+        skip: Callable[[str], bool] = lambda _: False,
+    ) -> None:
         Rule.__init__(self, name, code)
         assert isinstance(pattern, str)
         assert isinstance(warning_msg, str)
         assert isinstance(exceptions, list)
         assert all(isinstance(e, str) for e in exceptions)
         self._pattern = re.compile(pattern)
         self._warning_msg = warning_msg
         self._exception_patterns = exceptions
         self._exception_group = None
         self._exceptions = [re.compile(e) for e in exceptions]
         self._skip = skip
 
-    def _match(self, line):
+    def _match(self, line: str, start: int = 0) -> Union[int, None]:
         exception_group = self._exception_group
-        it = self._pattern.finditer(line)
+        it = self._pattern.finditer(line, start)
         for x in it:
             exception = False
             if len(self._exceptions) > 0:
                 x_group = x.groups().index(exception_group) + 1
                 for e in self._exceptions:
                     ite = e.finditer(line)
                     for m in ite:
@@ -235,104 +245,71 @@
                             break
                     if exception:
                         break
             if not exception:
                 return x.start()
         return None
 
-    def skip(self, fname):
+    def skip(self, fname: str) -> bool:
         """
         Returns True if this rule should not be applied to fname.
         """
         return self._skip(fname)
 
 
 ###############################################################################
-# File rules
+# Global rules
 ###############################################################################
 
 
-class ReplaceAnnoyUTF8Chars(Rule):
+class GlobalRules:
     """
-    This rule replaces occurrences of annoying UTF characters from an entire
-    file by their ascii equivalent.
-
-    This could issue a warning rather than doing this replacement, but
-    currently does not.
+    A class for containing rules that should be applied to all the input
+    files, such as AnalyseDecls. This is an experimental feature.
     """
 
-    def __init__(self, name=None, code=None):
-        Rule.__init__(self, name, code)
-        self._chars = {
-            "\xc2\x82": ",",  # High code comma
-            "\xc2\x84": ",,",  # High code double comma
-            "\xc2\x85": "...",  # Triple dot
-            "\xc2\x88": "^",  # High carat
-            "\xc2\x91": "\x27",  # Forward single quote
-            "\xc2\x92": "\x27",  # Reverse single quote
-            "\xc2\x93": "\x22",  # Forward double quote
-            "\xc2\x94": "\x22",  # Reverse double quote
-            "\xc2\x95": " ",
-            "\xc2\x96": "-",  # High hyphen
-            "\xc2\x97": "--",  # Double hyphen
-            "\xc2\x99": " ",
-            "\xc2\xa0": " ",
-            "\xc2\xa6": "|",  # Split vertical bar
-            "\xc2\xab": "<<",  # Double less than
-            "\xc2\xbb": ">>",  # Double greater than
-            "\xc2\xbc": "1/4",  # one quarter
-            "\xc2\xbd": "1/2",  # one half
-            "\xc2\xbe": "3/4",  # three quarters
-            "\xca\xbf": "\x27",  # c-single quote
-            "\xcc\xa8": "",  # modifier - under curve
-            "\xcc\xb1": "",
-        }  # modifier - under line
-
-    def __call__(self, fname, lines, nr_warnings=0):
-        assert isinstance(fname, str)
-        assert isinstance(lines, str)
-        assert isinstance(nr_warnings, int)
-
-        # Remove annoying characters
-        def replace_chars(match):  # pylint: disable=missing-docstring
-            char = match.group(0)
-            return self._chars[char]
-
-        return (
-            nr_warnings,
-            re.sub(
-                "(" + "|".join(self._chars.keys()) + ")", replace_chars, lines
-            ),
-        )
-
+    def __init__(self):
+        self.gd_files = {}
+        self.gi_files = ""
+        self.xml_files = ""
+        self._rules = []
+        self._global_rules = []
 
-class WarnRegexFile(WarnRegexBase):
-    """
-    A rule that issues a warning if everytime a regex is matched in a file.
-    """
+    def add_rule(self, global_rule: Rule) -> None:
+        """Adds a rule to the global rules to be applied."""
+        self._global_rules.append(global_rule)
 
-    def __call__(self, fname, lines, nr_warnings=0):
+    def __call__(
+        self, fname: str, lines: str, nr_warnings: int = 0
+    ) -> Tuple[int, str]:
         assert isinstance(fname, str)
         assert isinstance(lines, str)
         assert isinstance(nr_warnings, int)
-        if not _is_tst_or_xml_file(fname):
-            match = self._match(lines)
-            if match:
-                _warn(fname, lines.count("\n", 0, match), self._warning_msg)
-                return nr_warnings + 1, lines
+        if fname.split(".")[-1] == "gd":
+            self.gd_files[fname] = lines
+        elif fname.split(".")[-1] == "gi":
+            self.gi_files += lines
+        elif fname.split(".")[-1] == "xml":
+            self.xml_files += lines
         return nr_warnings, lines
 
+    def apply_rules(self, nr_warnings: int):
+        """Applies all the currently added global rules."""
+        for global_rule in self._global_rules:
+            nr_warnings = global_rule(self, nr_warnings)
+        return nr_warnings
+
 
 class AnalyseDecls(Rule):
     """
     A global rule that detects operations/attributes/properties that are
     declared but not documented or not implemented.
     """
 
-    def __init__(self, name, code):
+    def __init__(self, name: str, code: str) -> None:
         Rule.__init__(self, name, code)
         self._patterns = [
             (
                 re.compile(r"DeclareOperation\(\"(\w+)"),
                 "operation",
             ),
             (
@@ -349,99 +326,152 @@
             ),
             (
                 re.compile(r"BindGlobal\(\"(\w+)"),
                 "global value",
             ),
         ]
 
-    def __call__(self, global_rules, nr_warnings):
+    def __call__(self, global_rules: GlobalRules, nr_warnings: int) -> int:
         for gd_fname, gd_file in global_rules.gd_files.items():
             for decl, name in self._patterns:
                 for decl_match in decl.finditer(gd_file):
                     decl_name = re.compile(decl_match.group(1))
                     if not decl_name.search(
                         global_rules.gi_files
                     ) and not decl_name.search(
                         gd_file,
                         decl_match.start() + len(decl.pattern) + 1,
                     ):
                         nr_warnings += 1
-                        msg = "%s %s declared, but not used" % (
-                            name,
-                            decl_name.pattern,
+                        msg = (
+                            f"{name} {decl_name.pattern} declared, but not used"
                         )
                         _warn(
                             gd_fname,
                             gd_file.count("\n", 0, decl_match.start()),
                             msg,
                         )
                     doc_pattern = re.compile(
-                        r'Name\s*=\s*"%s"' % decl_name.pattern
+                        rf'Name\s*=\s*"{decl_name.pattern}"'
                     )
                     if not decl_name.pattern.endswith(
                         "NC"
                     ) and not doc_pattern.search(global_rules.xml_files):
                         nr_warnings += 1
-                        msg = "%s %s declared, but not documented" % (
-                            name,
-                            decl_name.pattern,
-                        )
+                        msg = f"{name} {decl_name.pattern} declared, but not documented"
                         _warn(
                             gd_fname,
                             gd_file.count("\n", 0, decl_match.start()),
                             msg,
                         )
 
         return nr_warnings
 
 
-class GlobalRules:
-    """A class for containing rules that should be applied to all the input
-    files, such as AnalyseDecls. This is an experimental feature."""
+###############################################################################
+# File rules
+###############################################################################
 
-    def __init__(self):
-        self.gd_files = {}
-        self.gi_files = ""
-        self.xml_files = ""
-        self._rules = []
-        self._global_rules = []
 
-    def add_rule(self, global_rule):
-        """Adds a rule to the global rules to be applied."""
-        self._global_rules.append(global_rule)
+class ReplaceAnnoyUTF8Chars(Rule):
+    """
+    This rule replaces occurrences of annoying UTF characters from an entire
+    file by their ascii equivalent.
+
+    This could issue a warning rather than doing this replacement, but
+    currently does not.
+    """
+
+    def __init__(
+        self, name: Optional[str] = None, code: Optional[str] = None
+    ) -> None:
+        Rule.__init__(self, name, code)
+        self._chars = {
+            "\xc2\x82": ",",  # High code comma
+            "\xc2\x84": ",,",  # High code double comma
+            "\xc2\x85": "...",  # Triple dot
+            "\xc2\x88": "^",  # High carat
+            "\xc2\x91": "\x27",  # Forward single quote
+            "\xc2\x92": "\x27",  # Reverse single quote
+            "\xc2\x93": "\x22",  # Forward double quote
+            "\xc2\x94": "\x22",  # Reverse double quote
+            "\xc2\x95": " ",
+            "\xc2\x96": "-",  # High hyphen
+            "\xc2\x97": "--",  # Double hyphen
+            "\xc2\x99": " ",
+            "\xc2\xa0": " ",
+            "\xc2\xa6": "|",  # Split vertical bar
+            "\xc2\xab": "<<",  # Double less than
+            "\xc2\xbb": ">>",  # Double greater than
+            "\xc2\xbc": "1/4",  # one quarter
+            "\xc2\xbd": "1/2",  # one half
+            "\xc2\xbe": "3/4",  # three quarters
+            "\xca\xbf": "\x27",  # c-single quote
+            "\xcc\xa8": "",  # modifier - under curve
+            "\xcc\xb1": "",  # modifier - under line
+        }
 
-    def __call__(self, fname, lines, nr_warnings=0):
+    def __call__(
+        self, fname: str, lines: str, nr_warnings: int = 0
+    ) -> Tuple[int, str]:
         assert isinstance(fname, str)
         assert isinstance(lines, str)
         assert isinstance(nr_warnings, int)
-        if fname.split(".")[-1] == "gd":
-            self.gd_files[fname] = lines
-        elif fname.split(".")[-1] == "gi":
-            self.gi_files += lines
-        elif fname.split(".")[-1] == "xml":
-            self.xml_files += lines
-        return nr_warnings, lines
 
-    def apply_rules(self, nr_warnings):
-        """Applies all the currently added global rules."""
-        for global_rule in self._global_rules:
-            nr_warnings = global_rule(self, nr_warnings)
-        return nr_warnings
+        # Remove annoying characters
+        def replace_chars(
+            match: re.Match,
+        ) -> str:  # pylint: disable=missing-docstring
+            char = match.group(0)
+            return self._chars[char]
+
+        return (
+            nr_warnings,
+            re.sub(
+                "(" + "|".join(self._chars.keys()) + ")", replace_chars, lines
+            ),
+        )
+
+
+class WarnRegexFile(WarnRegexBase):
+    """
+    A rule that issues a warning if a regex is matched in a file.
+    """
+
+    def __call__(
+        self, fname: str, lines: str, nr_warnings: int = 0
+    ) -> Tuple[int, str]:
+        assert isinstance(fname, str)
+        assert isinstance(lines, str)
+        assert isinstance(nr_warnings, int)
+        if _is_tst_or_xml_file(fname):
+            return nr_warnings, lines
+
+        match = self._match(lines)
+        while match is not None:
+            line_num = lines.count("\n", 0, match)
+            if not _is_rule_suppressed(fname, line_num + 1, self):
+                _warn(fname, line_num, self._warning_msg)
+                nr_warnings += 1
+            match = self._match(lines, match + len(self._pattern.pattern))
+        return nr_warnings, lines
 
 
 class ReplaceComments(Rule):
     """
     Replace between '#+' and the end of a line by '#+' and as many '@' as there
     were other characters in the line, call before replacing strings, and
     chars, and so on.
 
     This rule does not return any warnings.
     """
 
-    def __call__(self, fname, lines, nr_warnings=0):
+    def __call__(
+        self, fname: str, lines: str, nr_warnings: int = 0
+    ) -> Tuple[int, str]:
         assert isinstance(fname, str)
         assert isinstance(lines, str)
         assert isinstance(nr_warnings, int)
         start = lines.find("#", 0)
         while start != -1 and _is_in_string(lines, start):
             start = lines.find("#", start + 1)
         while start != -1:
@@ -463,48 +493,50 @@
     """
     Replace all characters between delim1 and delim2 by #'s except possibly
     whitespace.
 
     This rule does not return any warnings.
     """
 
-    def __init__(self, name, code, delim1, delim2):
+    def __init__(self, name: str, code: str, delim1: str, delim2: str) -> None:
         Rule.__init__(self, name, code)
         assert isinstance(delim1, str)
         assert isinstance(delim2, str)
         self._delims = [re.compile(delim1), re.compile(delim2)]
 
-    def __find_next(self, which, lines, start):
+    def __find_next(self, which: int, lines: str, start: int) -> int:
         assert which in (0, 1)
         assert isinstance(lines, str)
         assert isinstance(start, int)
         if start >= len(lines):
             return -1
         delim = self._delims[which]
         match = delim.search(lines, start)
         while match is not None and (
             _is_escaped(lines, match.start())
             or _is_double_quote_in_char(lines, match.start())
         ):
             match = delim.search(lines, match.start() + len(delim.pattern))
         return -1 if match is None else match.start()
 
-    def __call__(self, fname, lines, nr_warnings=0):
+    def __call__(
+        self, fname: str, lines: str, nr_warnings: int = 0
+    ) -> Tuple[int, str]:
         assert isinstance(fname, str)
         assert isinstance(lines, str)
         assert isinstance(nr_warnings, int)
 
         start = self.__find_next(0, lines, 0)
         while start != -1:
             end = self.__find_next(1, lines, start + 1)
             if end == -1:
                 _error(
                     fname,
                     lines.count("\n", 0, start),
-                    "Unmatched %s" % self._delims[0].pattern,
+                    "Unmatched {self._delims[0].pattern}",
                 )
             end += len(self._delims[1].pattern)
             repl = re.sub("[^\n ]", "@", lines[start:end])
             assert len(repl) == end - start
 
             lines = lines[:start] + repl + lines[end:]
             start = self.__find_next(0, lines, end + 1)
@@ -515,22 +547,26 @@
     """
     This rule removes the prefix 'gap>' or '>' if called with a line from a
     file with extension 'tst' or 'xml', if the line does not start with a
     'gap>' or '>', then the entire line is replaced with an equal number of
     '@''s.
     """
 
-    def __init__(self, name=None, code=None):
+    def __init__(
+        self, name: Optional[str] = None, code: Optional[str] = None
+    ) -> None:
         Rule.__init__(self, name, code)
         self._consuming = False
         self._sol_p = re.compile(r"(^|\n)gap>\s*")
         self._eol_p = re.compile(r"($|\n)")
         self._rep_p = re.compile(r"[^\n]")
 
-    def __call__(self, fname, lines, nr_warnings=0):
+    def __call__(
+        self, fname: str, lines: str, nr_warnings: int = 0
+    ) -> Tuple[int, str]:
         assert isinstance(fname, str)
         assert isinstance(lines, str)
         assert isinstance(nr_warnings, int)
         if _is_tst_or_xml_file(fname):
             eol, out = 0, ""
             for sol in self._sol_p.finditer(lines):
                 # Replace everything except '\n' with '@'
@@ -546,37 +582,41 @@
 
 
 class AnalyseLVars(Rule):  # pylint: disable=too-many-instance-attributes
     """
     This rule checks if there are unused local variables in a function.
     """
 
-    def __init__(self, name=None, code=None):
+    def __init__(
+        self, name: Optional[str] = None, code: Optional[str] = None
+    ) -> None:
         Rule.__init__(self, name, code)
         self.reset()
 
         self._function_p = re.compile(r"\bfunction\b")
         self._end_p = re.compile(r"\bend\b")
         self._local_p = re.compile(r"\blocal\b")
         self._var_p = re.compile(r"\w+\s*\w*")
         self._ass_var_p = re.compile(r"([a-zA-Z0-9_\.]+)\s*:=")
         self._use_var_p = re.compile(r"(\b\w+\b)(?!\s*:=)\W*")
         self._ws1_p = re.compile(r"[ \t\r\f\v]+")
         self._ws2_p = re.compile(r"\n[ \t\r\f\v]+")
         self._rec_p = re.compile(r"\brec\(")
+        self._func_bodies = []
+        self._func_position = []
 
-    def reset(self):
+    def reset(self) -> None:
         self._depth = -1
         self._func_args = []
         self._declared_lvars = []
         self._assigned_lvars = []
         self._used_lvars = []
         self._func_start_pos = []
 
-    def _remove_recs_and_whitespace(self, lines):
+    def _remove_recs_and_whitespace(self, lines: str) -> str:
         # Remove almost all whitespace
         lines = re.sub(self._ws1_p, " ", lines)
         lines = re.sub(self._ws2_p, "\n", lines)
 
         stack = []
         pos = 0
         # Replace rec( -> ) so that we do not match assignments inside records
@@ -597,15 +637,17 @@
                     lines = lines[: start + 1] + replacement + lines[pos + 1 :]
                     pos -= pos - start
                     pos += len(replacement)
             pos += 1
         assert len(stack) == 0
         return lines
 
-    def _start_function(self, fname, lines, pos, nr_warnings):
+    def _start_function(
+        self, fname: str, lines: str, pos: int, nr_warnings: int
+    ) -> Tuple[int, int]:
         self._depth += 1
 
         assert self._depth == len(self._func_args)
         assert self._depth == len(self._declared_lvars)
         assert self._depth == len(self._assigned_lvars)
         assert self._depth == len(self._used_lvars)
         assert self._depth == len(self._func_start_pos)
@@ -625,75 +667,99 @@
             var = [x.strip() for x in var.split(" ") if len(x) != 0]
             if len(var) == 1:
                 var = var[0].strip()
             elif len(var) != 2 or var[0] not in ("readonly", "readwrite"):
                 _error(
                     fname,
                     lines.count("\n", 0, pos),
-                    'Invalid syntax: "%s"' % lines[start:end],
+                    f'Invalid syntax: "{lines[start:end]}"',
                 )
             else:
                 var = var[1].strip()
             if var in args:
                 _error(
                     fname,
                     lines.count("\n", 0, pos),
-                    "Duplicate function argument: %s" % var,
+                    f"Duplicate function argument: {var}",
                 )
             elif var in _GAP_KEYWORDS:
                 _error(
                     fname,
                     lines.count("\n", 0, pos),
-                    "Function argument is keyword: %s" % var,
+                    f"Function argument is keyword: {var}",
                 )
             else:
                 args.add(var)
         return end + 1, nr_warnings
 
-    def _end_function(self, fname, lines, pos, nr_warnings):
+    def _end_function(
+        self, fname: str, lines: str, pos: int, nr_warnings: int
+    ) -> Tuple[int, int]:
         if len(self._declared_lvars) == 0:
             _error(fname, lines.count("\n", 0, pos), "'end' outside function")
 
         self._depth -= 1
 
         ass_lvars = self._assigned_lvars.pop()
         decl_lvars = self._declared_lvars.pop()
         use_lvars = self._used_lvars.pop()
+        func_args = self._func_args.pop()
 
         if len(self._used_lvars) > 0:
             self._used_lvars[-1] |= use_lvars  # union
 
         ass_lvars -= use_lvars  # difference
         ass_lvars &= decl_lvars  # intersection
         decl_lvars -= ass_lvars  # difference
         decl_lvars -= use_lvars  # difference
+        func_args -= use_lvars  # difference
+
+        linenum = lines.count("\n", 0, self._func_start_pos[-1])
 
         if len(ass_lvars) != 0:
             ass_lvars = [key for key in ass_lvars if key.find(".") == -1]
-            msg = "Variables assigned but never used: " + ass_lvars[0]
-            for x in ass_lvars[1:]:
-                msg += ", " + x
-            linenum = lines.count("\n", 0, self._func_start_pos[-1])
+            msg = f"Variables assigned but never used: {', '.join(ass_lvars)}"
             _warn(fname, linenum, msg)
             nr_warnings += 1
 
         if len(decl_lvars) != 0:
             decl_lvars = list(decl_lvars)
-            msg = "Unused local variables: " + decl_lvars[0]
-            for x in decl_lvars[1:]:
-                msg += ", " + x
-            linenum = lines.count("\n", 0, self._func_start_pos[-1])
+            msg = f"Unused local variables: {', '.join(decl_lvars)}"
             _warn(fname, linenum, msg)
             nr_warnings += 1
 
-        self._func_args.pop()  # TODO do something with these
+        func_args = [arg for arg in func_args if arg != "_"]
+        if len(func_args) != 0:
+            msg = f"Unused function arguments: {', '.join(func_args)}"
+            if not _is_rule_suppressed(fname, linenum + 1, self):
+                _warn(fname, linenum, msg)
+                nr_warnings += 1
+        func_body = lines[self._func_start_pos[-1] : pos]
+        num_func_lines = func_body.count("\n")
+        limit = _GLOB_CONFIG["duplicate-function-min-length"]
+        if num_func_lines + 1 > limit:
+            func_body = re.sub(r"\n", "", func_body)
+            try:
+                index = self._func_bodies.index(func_body)
+                _warn(
+                    fname,
+                    linenum,
+                    f"Duplicate function with {num_func_lines + 1} > {limit}"
+                    + f" lines, previously defined at {self._func_position[index]}!",
+                )
+                nr_warnings += 1
+            except ValueError:
+                self._func_bodies.append(func_body)
+                self._func_position.append(f"{fname}:{linenum + 1}")
         self._func_start_pos.pop()
         return pos + len("end"), nr_warnings
 
-    def _add_declared_lvars(self, fname, lines, pos, nr_warnings):
+    def _add_declared_lvars(
+        self, fname: str, lines: str, pos: int, nr_warnings: int
+    ) -> Tuple[int, int]:
         end = lines.find(";", pos)
         lvars = self._declared_lvars[self._depth]
         args = self._func_args[self._depth]
 
         new_lvars = self._var_p.findall(lines, pos, end)
         for var in new_lvars:
             var = var.strip()
@@ -703,28 +769,29 @@
                     lines.count("\n", 0, pos),
                     "Name used for two local variables: " + var,
                 )
             elif var in args:
                 _error(
                     fname,
                     lines.count("\n", 0, pos),
-                    "Name used for function argument and local variable: %s"
-                    % var,
+                    f"Name used for function argument and local variable: {var}",
                 )
             elif var in _GAP_KEYWORDS:
                 _error(
                     fname,
                     lines.count("\n", 0, pos),
-                    "Local variable is keyword: " + var,
+                    f"Local variable is keyword: {var}",
                 )
             else:
                 lvars.add(var)
         return end, nr_warnings
 
-    def _find_lvars(self, fname, lines, pos, nr_warnings):
+    def _find_lvars(
+        self, fname: str, lines: str, pos: int, nr_warnings: int
+    ) -> Tuple[int, int]:
         end = self._end_p.search(lines, pos + 1)
         func = self._function_p.search(lines, pos + 1)
         if end is None and func is None:
             return len(lines), nr_warnings
         if end is None and func is not None:
             _error(fname, lines.count("\n", 0, pos), "'function' without 'end'")
 
@@ -736,15 +803,17 @@
         if self._depth >= 0:
             a_lvars = self._assigned_lvars[self._depth]
             a_lvars |= set(self._ass_var_p.findall(lines, pos, end))
             u_lvars = self._used_lvars[self._depth]
             u_lvars |= set(self._use_var_p.findall(lines, pos, end))
         return end, nr_warnings
 
-    def __call__(self, fname, lines, nr_warnings=0):
+    def __call__(
+        self, fname: str, lines: str, nr_warnings: int = 0
+    ) -> Tuple[int, str]:
         assert isinstance(fname, str)
         assert isinstance(lines, str)
         assert isinstance(nr_warnings, int)
         if _is_tst_or_xml_file(fname):
             return nr_warnings, lines
         orig_lines = lines[:]
         lines = self._remove_recs_and_whitespace(lines)
@@ -778,38 +847,43 @@
 class LineTooLong(Rule):
     """
     Warn if the length of a line exceeds 80 characters.
 
     This rule does not modify the line.
     """
 
-    def __init__(self, name=None, code=None):
+    def __init__(
+        self, name: Optional[str] = None, code: Optional[str] = None
+    ) -> None:
         Rule.__init__(self, name, code)
         self._cols = _GLOB_CONFIG["columns"]
 
-    def __call__(self, fname, lines, linenum, nr_warnings=0):
+    def __call__(
+        self, fname: str, lines: str, linenum: int, nr_warnings: int = 0
+    ) -> Tuple[int, str]:
         if _is_tst_or_xml_file(fname):
             return nr_warnings, lines
         if len(lines[linenum]) - 1 > self._cols:
             _warn(
                 fname,
                 linenum,
-                "Too long line (%d / %d)"
-                % (len(lines[linenum]) - 1, self._cols),
+                f"Too long line ({len(lines[linenum]) - 1} / {self._cols})",
             )
             nr_warnings += 1
         return nr_warnings, lines
 
 
 class WarnRegexLine(WarnRegexBase):
     """
     Warn if regex matches.
     """
 
-    def __call__(self, fname, lines, linenum, nr_warnings=0):
+    def __call__(
+        self, fname: str, lines: str, linenum: int, nr_warnings: int = 0
+    ) -> Tuple[int, str]:
         assert isinstance(fname, str)
         assert isinstance(lines, list)
         assert isinstance(linenum, int)
         assert linenum < len(lines)
         assert isinstance(nr_warnings, int)
         if not self.skip(fname):
             if self._match(lines[linenum]) is not None:
@@ -820,61 +894,54 @@
 
 class WhitespaceOperator(WarnRegexLine):
     """
     Instances of this class produce a warning whenever the whitespace around an
     operator is incorrect.
     """
 
-    def __init__(self, name, code, op, exceptions=[]):  # pylint: disable=W0102
+    def __init__(
+        self, name: str, code: str, op: str, exceptions: List[str] = []
+    ):  # pylint: disable=W0102
         WarnRegexLine.__init__(self, name, code, "", "")
         assert isinstance(op, str)
         assert op[0] != "(" and op[-1] != ")"
         assert exceptions is None or isinstance(exceptions, list)
         assert all(isinstance(e, str) for e in exceptions)
         gop = "(" + op + ")"
-        pattern = (
-            r"(\S"
-            + gop
-            + "|"
-            + gop
-            + r"\S|\s{2,}"
-            + gop
-            + "|"
-            + gop
-            + r"\s{2,})"
-        )
+        pattern = rf"(\S{gop}|{gop}\S|\s{{2,}}{gop}|{gop}\s{{2,}})"
         self._pattern = re.compile(pattern)
         self._warning_msg = "Wrong whitespace around operator " + op.replace(
             "\\", ""
         )
         exceptions = [e.replace(op, "(" + op + ")") for e in exceptions]
         self._exceptions = [re.compile(e) for e in exceptions]
-
         self._exception_group = op.replace("\\", "")
 
 
 class UnalignedPatterns(Rule):
     """
     This rule checks if pattern occurs in consecutive lines and that they are
     aligned.
     """
 
     def __init__(  # pylint: disable=too-many-arguments
-        self, name, code, pattern, group, msg
-    ):
+        self, name: str, code: str, pattern: str, group: int, msg: str
+    ) -> None:
         Rule.__init__(self, name, code)
         assert isinstance(pattern, str)
         assert isinstance(group, int)
         assert isinstance(msg, str)
         self._last_line_col = None
         self._pattern = re.compile(pattern)
         self._group = group
         self._msg = msg
 
-    def __call__(self, fname, lines, linenum, nr_warnings=0):
+    def __call__(
+        self, fname: str, lines: List[str], linenum: int, nr_warnings: int = 0
+    ) -> Tuple[int, List[str]]:
         assert isinstance(fname, str)
         assert isinstance(lines, list)
         assert isinstance(linenum, int)
         assert isinstance(nr_warnings, int)
         if (
             _is_rule_suppressed(fname, linenum, self)
             or _is_tst_or_xml_file(fname)
@@ -896,15 +963,15 @@
     This class checks that the indentation level is correct in a given line.
 
     Certain keywords increase the indentation level, while others decrease it,
     this rule checks that a given line has the minimum indentation level
     required.
     """
 
-    def __init__(self, name, code):
+    def __init__(self, name: str, code: str) -> None:
         Rule.__init__(self, name, code)
         ind = _GLOB_CONFIG["indentation"]
         self._expected = 0
         self._before = [
             (re.compile(r"(\W|^)(elif|else)(\W|$)"), -ind),
             (re.compile(r"(\W|^)end(\W|$)"), -ind),
             (re.compile(r"(\W|^)(od|fi)(\W|$)"), -ind),
@@ -916,15 +983,17 @@
             (re.compile(r"(\W|^)function(\W|$)"), ind),
             (re.compile(r"(\W|^)(if|for|while|elif|atomic)(\W|$)"), 2 * ind),
         ]
         self._indent = re.compile(r"^(\s*)\S")
         self._blank = re.compile(r"^\s*$")
         self._msg = "Bad indentation: found %d but expected at least %d"
 
-    def __call__(self, fname, lines, linenum, nr_warnings=0):
+    def __call__(
+        self, fname: str, lines: List[str], linenum: int, nr_warnings: int = 0
+    ) -> Tuple[int, List[str]]:
         assert isinstance(fname, str)
         assert isinstance(lines, list)
         assert isinstance(linenum, int)
         assert isinstance(nr_warnings, int)
         assert self._expected >= 0
 
         if (
@@ -944,29 +1013,29 @@
             nr_warnings += 1
 
         for pair in self._after:
             if pair[0].search(lines[linenum]):
                 self._expected += pair[1]
         return nr_warnings, lines
 
-    def _get_indent_level(self, line):
+    def _get_indent_level(self, line: str) -> int:
         indent = self._indent.search(line)
         assert indent
         return len(indent.group(1))
 
     def reset(self):
         self._expected = 0
 
 
 ###############################################################################
 # Functions for running this as a script instead of a module
 ###############################################################################
 
 
-def _parse_args(kwargs):
+def _parse_args(kwargs: Dict[str, bool]) -> argparse.Namespace:
     # pylint: disable=too-many-branches, too-many-statements, global-statement
     global _SILENT, _VERBOSE
     parser = argparse.ArgumentParser(prog="gaplint", usage="%(prog)s [options]")
     if "files" not in kwargs:
         parser.add_argument("files", nargs="+", help="the files to lint")
 
     parser.add_argument(
@@ -985,15 +1054,15 @@
     )
     parser.set_defaults(columns=None)
 
     parser.add_argument(
         "--disable",
         nargs="?",
         type=str,
-        help="gaplint rules " + "(name or code) to disable (default: None)",
+        help="gaplint rules (name or code) to disable (default: None)",
     )
     parser.set_defaults(disable="")
     # TODO an --enable option to enable only the specified rules
 
     parser.add_argument(
         "--indentation",
         nargs="?",
@@ -1013,31 +1082,36 @@
     parser.add_argument(
         "--verbose",
         dest="verbose",
         action="store_true",
         help=" (default: False)",
     )
     parser.set_defaults(verbose=False)
-
-    version = pkg_resources.require("gaplint")[0].version
+    vers_num = version("gaplint")
     parser.add_argument(
         "--version",
         action="version",
-        version="%(prog)s version {0}".format(version),
+        version=f"%(prog)s version {vers_num}",
     )
 
     parser.add_argument(
         "--enable-experimental",
         dest="enable_experimental",
         action="store_true",
         help=" (default: False)",
     )
     parser.set_defaults(enable_experimental=False)
 
-    args = parser.parse_args()
+    args, unknown = parser.parse_known_args()
+
+    if len(unknown) != 0:
+        sys.stderr.write(
+            f"Unknown command line option{'' if len(unknown) == 1 else 's'}: {unknown}\n"
+        )
+        sys.exit("Aborting!")
 
     if "silent" in kwargs:
         _SILENT = kwargs["silent"]
     else:
         _SILENT = args.silent
 
     if "verbose" in kwargs:
@@ -1071,57 +1145,60 @@
         if not isinstance(kwargs["files"], list):
             sys.exit("Keyword arg 'files' must be a list")
         args.files = kwargs["files"]
 
     files = []
     for fname in args.files:
         if not (exists(fname) and isfile(fname)):
-            _info_action("SKIPPING " + fname + ": cannot open for reading")
+            _info_action(f"SKIPPING {fname}: cannot open for reading")
         elif (
-            not fname.split(".")[-1] in _VALID_EXTENSIONS
-            and not ".".join(fname.split(".")[-2:]) in _VALID_EXTENSIONS
+            fname.split(".")[-1] not in _VALID_EXTENSIONS
+            and ".".join(fname.split(".")[-2:]) not in _VALID_EXTENSIONS
         ):
-            _info_action("IGNORING " + fname + ": not a valid file extension")
+            _info_action(f"IGNORING {fname}: not a valid file extension")
         else:
             files.append(fname)
     args.files = files
 
     return args
 
 
 ###############################################################################
 # Global configuration and suppressions - run before defining RULES
 ###############################################################################
 
 
-def __init_config_and_suppressions_command_line(args):
+def __init_config_and_suppressions_command_line(
+    args: argparse.Namespace,
+) -> None:
     assert isinstance(args, argparse.Namespace)
     assert hasattr(args, "files")
     assert hasattr(args, "config")
     assert "disable" in args.config
 
     for key in args.config:
         if key != "disable" and args.config[key] is not None:
             _GLOB_CONFIG[key] = args.config[key]
 
     names_or_codes = args.config["disable"].split(",")
     for name_or_code in names_or_codes:
         _GLOB_SUPPRESSIONS[name_or_code] = None
 
 
-def __config_yml_path(dir_path):
+def __config_yml_path(dir_path: str) -> Union[None, str]:
     """
     Recursive function that takes the path of a directory to search and
     searches for the gaplint.yml config script. If the script is not found the
     function is then called on the parent directory - recursive case. This
     continues until we encounter a directory .git in our search (script not
     found, returns None), locate the script (returns script path), or until the
     root directory has been searched (script not found, returns None) - base
     cases A, B, C.
     """
+    assert isinstance(dir_path, str)
     assert isdir(dir_path)
     entries = listdir(dir_path)
 
     if ".gaplint.yml" in entries:
         yml_path = abspath(join(dir_path, ".gaplint.yml"))
         return yml_path
     if ".git" in entries and isdir(abspath(join(dir_path, ".git"))):
@@ -1129,98 +1206,97 @@
 
     pardir_path = abspath(join(dir_path, os.pardir))
     if pardir_path == dir_path:
         return None
     return __config_yml_path(pardir_path)  # recursive call
 
 
-def __init_config_and_suppressions_yml():
-
+def __init_config_and_suppressions_yml() -> None:
     config_yml_fname = __config_yml_path(os.getcwd())
     if config_yml_fname is None:
         return
 
-    _info_action("Using configurations in %s" % config_yml_fname)
+    _info_action(f"Using configurations in {config_yml_fname}")
     try:
-        with open(config_yml_fname, "r", encoding="utf8") as config_yml_file:
+        with open(config_yml_fname, "r", encoding="utf-8") as config_yml_file:
             ymldic = yaml.load(config_yml_file, Loader=yaml.FullLoader)
-    except yaml.YAMLError:
-        _info_action("IGNORING %s: error parsing YAML" % config_yml_fname)
+    except (yaml.YAMLError, IOError):
+        _info_action("IGNORING {config_yml_fname}: error parsing YAML")
         return
 
     if ymldic is None:
         return
     for key in ymldic:
         if key not in _GLOB_CONFIG and key != "disable":
             _info_action(
-                "IGNORING unknown configuration value '%s' in %s"
-                % (key, config_yml_fname)
+                f"IGNORING unknown configuration value '{key}' in {config_yml_fname}"
             )
         elif key != "disable":
             _GLOB_CONFIG[key] = ymldic[key]
         else:
             if not isinstance(ymldic[key], list):
                 _info_action(
-                    "IGNORING %s: badly formed field 'disable'"
-                    % config_yml_fname
+                    f"IGNORING {config_yml_fname}: badly formed field 'disable'"
                 )
             else:
                 for name_or_code in ymldic[key]:
                     if isinstance(name_or_code, str):
                         _GLOB_SUPPRESSIONS[name_or_code] = None
                     else:
                         _info_action(
-                            "IGNORING bad value %s in field" % name_or_code
-                            + " 'disable' in %s" % config_yml_fname
+                            f"IGNORING bad value {name_or_code} in field"
+                            + f" 'disable' in {config_yml_fname}"
                         )
 
 
-def __verify_glob_suppressions():
+def __verify_glob_suppressions() -> None:
     global _GLOB_SUPPRESSIONS  # pylint: disable=global-variable-not-assigned, global-statement
     delete = []
     for name_or_code in _GLOB_SUPPRESSIONS:
         if name_or_code in ("all", ""):
             continue
         ok = False
         for rule in _LINE_RULES + _FILE_RULES:
             if isinstance(rule, GlobalRules):
                 ok = True
                 continue
             if name_or_code in (rule.name, rule.code):
                 if rule.code[0] == "M":
                     _info_action(
-                        "IGNORING cannot disable rule: %s" % name_or_code
+                        f"IGNORING cannot disable rule: {name_or_code}"
                     )
                 else:
                     ok = True
                 break
         if not ok:
             delete.append(name_or_code)
 
     for name_or_code in delete:
         del _GLOB_SUPPRESSIONS[name_or_code]
         config_yml_fname = __config_yml_path(os.getcwd())
         msg = "IGNORING in command line "
         if config_yml_fname is not None:
-            msg += "or %s " % config_yml_fname
-        msg += "invalid rule name or code: %s" % name_or_code
+            msg += f"or {config_yml_fname}"
+        msg += f"invalid rule name or code: {name_or_code}"
         _info_action(msg)
 
 
 ###############################################################################
 # The list of rules (the order is important!)
 ###############################################################################
 
 
-def __init_rules(args):
+def __init_rules(args: argparse.Namespace) -> None:
     global _EXPERIMENTAL_FILE_RULES, _FILE_RULES, _LINE_RULES  # pylint: disable=global-statement
+    if len(_FILE_RULES) != 0:
+        return
     _EXPERIMENTAL_FILE_RULES = [
         WarnRegexFile(
             "combine-ifs-with-elif",
-            "W034",
+            "W998",
             r"\n\s*if(.*\n\s*(ErrorNoReturn|Error|return|TryNextMethod)"
             + r"(.*\n\s*elif)?)+.*\n\s*fi;(\n)+\s*if",
             "Combine multiple ifs using elif",
         ),
     ]
     _FILE_RULES = [
         ReplaceAnnoyUTF8Chars("replace-weird-chars", "M000"),
@@ -1241,14 +1317,20 @@
         ),
         WarnRegexFile(
             "assign-then-return",
             "W033",
             r"(\w+)\s*:=[^;]*;\n\s*return\s+(\1);",
             "Pointless assignment immediately returned",
         ),
+        WarnRegexFile(
+            "1-line-function",
+            "W034",
+            r"\bfunction\b.*?\n.*?\breturn\b.*?\n.*?\bend\b",
+            "One line function could be a lambda",
+        ),
     ]
     if args.enable_experimental:
         _FILE_RULES += _EXPERIMENTAL_FILE_RULES
     _LINE_RULES = [
         LineTooLong("line-too-long", "W002"),
         Indentation("indentation", "W003"),
         UnalignedPatterns(
@@ -1333,28 +1415,58 @@
             r"(\S:=|:=(\S|\s{2,}))",
             "Wrong whitespace around operator :=",
         ),
         WarnRegexLine(
             "tabs",
             "W017",
             r"\t",
-            "There are tabs in this line, " + "replace with spaces",
+            "There are tabs in this line, replace with spaces",
         ),
         WarnRegexLine(
             "function-local-same-line",
             "W018",
             r"function\W.*\Wlocal\W",
-            "Keywords 'function' and 'local' in the" + " same line",
+            "Keywords 'function' and 'local' in the same line",
         ),
         WarnRegexLine(
             "whitespace-op-minus",
             "W019",
             r"(return|\^|\*|,|=|\.|>) - \d",
             "Wrong whitespace around operator -",
         ),
+        WarnRegexLine(
+            "pointless-lambda",
+            "W035",
+            r"\b(\w+)\b\s*->\s*\b\w+\(\1\)\s*\)",
+            "Replace x -> f(x) by f",
+        ),
+        WarnRegexLine(
+            "use-return-true",
+            "W036",
+            r"\b(\w+)\b\s*->\s*\btrue\b\s*\)",
+            "Replace x -> true by ReturnTrue",
+        ),
+        WarnRegexLine(
+            "use-return-false",
+            "W037",
+            r"\b(\w+)\b\s*->\s*\bfalse\b\s*\)",
+            "Replace x -> false by ReturnFalse",
+        ),
+        WarnRegexLine(
+            "use-return-fail",
+            "W038",
+            r"\b(\w+)\b\s*->\s*\bfail\b\s*\)",
+            "Replace x -> fail by ReturnFail",
+        ),
+        WarnRegexLine(
+            "use-remove-not-unbind",
+            "W039",
+            r"\bUnbind\((\w+)\[Length\(\1\)\]\)",
+            "Replace Unbind(foo[Length(foo)]) by Remove(foo)",
+        ),
         WhitespaceOperator("whitespace-op-plus", "W020", r"\+", [r"^\s*\+"]),
         WhitespaceOperator(
             "whitespace-op-multiply", "W021", r"\*", [r"^\s*\*", r"\\\*"]
         ),
         WhitespaceOperator(
             "whitespace-op-negative",
             "W022",
@@ -1399,63 +1511,75 @@
 
 
 ###############################################################################
 # File and line suppressions - run after defining RULES
 ###############################################################################
 
 
-def __is_valid_rule_name_or_code(name_or_code, fname, linenum):
-    # TODO assertions
+def __is_valid_rule_name_or_code(
+    name_or_code: str, fname: str, linenum: int
+) -> bool:
+    assert isinstance(name_or_code, str)
+    assert isinstance(fname, str)
+    assert isinstance(linenum, int)
+
     if name_or_code == "all":
         return True
     for rule in _LINE_RULES + _FILE_RULES:
         if isinstance(rule, GlobalRules):
             continue
 
         if name_or_code in (rule.name, rule.code):
             if rule.code[0] == "M":
-                _info_action("IGNORING cannot disable rule: %s" % name_or_code)
+                _info_action(f"IGNORING cannot disable rule: {name_or_code}")
                 return False
             return True
     _info_action(
-        "IGNORING in %s:%d invalid rule name or code: %s"
-        % (fname, linenum + 1, name_or_code)
+        f"IGNORING in {fname}:{linenum + 1} invalid rule name or code: {name_or_code}"
     )
     return False
 
 
-def __add_file_suppressions(names_or_codes, fname, linenum):
+def __add_file_suppressions(
+    names_or_codes: List[str], fname: str, linenum: int
+) -> None:
     assert isinstance(names_or_codes, list)
-    #  TODO add more assertions
+    assert all(isinstance(x, str) for x in names_or_codes)
+    assert isinstance(fname, str)
+    assert isinstance(linenum, int)
 
     for name_or_code in names_or_codes:
         assert isinstance(name_or_code, str)
         if __is_valid_rule_name_or_code(name_or_code, fname, linenum):
             if fname not in _FILE_SUPPRESSIONS:
                 _FILE_SUPPRESSIONS[fname] = {}
             _FILE_SUPPRESSIONS[fname][name_or_code] = None
 
 
-def __add_line_suppressions(names_or_codes, fname, linenum):
+def __add_line_suppressions(
+    names_or_codes: List[str], fname: str, linenum: int
+) -> None:
     assert isinstance(names_or_codes, list)
-    #  TODO add more assertions
+    assert all(isinstance(x, str) for x in names_or_codes)
+    assert isinstance(fname, str)
+    assert isinstance(linenum, int)
 
     for name_or_code in names_or_codes:
         assert isinstance(name_or_code, str)
         if __is_valid_rule_name_or_code(name_or_code, fname, linenum):
             if fname not in _LINE_SUPPRESSIONS:
                 _LINE_SUPPRESSIONS[fname] = {}
             if linenum + 1 not in _LINE_SUPPRESSIONS[fname]:
                 _LINE_SUPPRESSIONS[fname][linenum + 1] = {}
             _LINE_SUPPRESSIONS[fname][linenum + 1][name_or_code] = None
 
 
 # FIXME this should be a line rule called before any other line rule, to avoid
 # reading the files more than once
-def __init_file_and_line_suppressions(args):
+def __init_file_and_line_suppressions(args: argparse.Namespace) -> None:
     assert isinstance(args, argparse.Namespace)
     assert hasattr(args, "files")
 
     comment_line_p = re.compile(r"^\s*($|#)")
     gaplint_p = re.compile(r"\s*#\s*gaplint:\s*disable\s*=\s*")
     rules_p = re.compile(r"[a-zA-Z0-9_\-]+")
 
@@ -1463,15 +1587,15 @@
     next_line_p = re.compile(r"#\s* gaplint:\s*disable\(nextline\)=\s*")
 
     for fname in args.files:
         try:
             with open(fname, "r", encoding="utf8") as f:
                 lines = f.readlines()
         except IOError:
-            _info_action("cannot read file %s, this shouldn't happen" % fname)
+            _info_action(f"cannot read file {fname}, this shouldn't happen")
             continue
         linenum = 0
         # Find rules suppressed for the entire file at the start of the file
         while linenum < len(lines) and comment_line_p.search(lines[linenum]):
             match = gaplint_p.search(lines[linenum])
             if match:
                 names_or_codes = rules_p.findall(lines[linenum], match.end())
@@ -1490,40 +1614,44 @@
                     names_or_codes = rules_p.findall(
                         lines[linenum], match.end()
                     )
                     __add_line_suppressions(names_or_codes, fname, linenum)
             linenum += 1
 
 
-def _is_rule_suppressed(fname, linenum, rule):
+def _is_rule_suppressed(
+    fname: str, linenum: int, rule: Union[Rule, GlobalRules]
+) -> bool:
     """
-    Takes a filename, line number and rule code. Returns True if the rule is
+    Takes a filename, line number, and rule. Returns True if the rule is
     suppressed for that particular line, and False otherwise.
     """
     assert isinstance(fname, str)
     assert isinstance(linenum, int)
     assert isinstance(rule, (Rule, GlobalRules))
 
     if isinstance(rule, GlobalRules):
         return False
-
+    assert rule.code is not None
+    assert rule.name is not None
     if rule.code[0] == "M":
         return False
     if (
         "all" in _GLOB_SUPPRESSIONS
         or rule.code in _GLOB_SUPPRESSIONS
         or rule.name in _GLOB_SUPPRESSIONS
     ):
         return True
     if fname in _FILE_SUPPRESSIONS and (
         "all" in _FILE_SUPPRESSIONS[fname]
         or rule.code in _FILE_SUPPRESSIONS[fname]
         or rule.name in _FILE_SUPPRESSIONS[fname]
     ):
         return True
+
     if (
         fname in _LINE_SUPPRESSIONS
         and linenum in _LINE_SUPPRESSIONS[fname]
         and (
             rule.code in _LINE_SUPPRESSIONS[fname][linenum]
             or rule.name in _LINE_SUPPRESSIONS[fname][linenum]
         )
@@ -1533,16 +1661,27 @@
 
 
 ###############################################################################
 # The main event
 ###############################################################################
 
 
+def _verbose_msg_per_file(args: argparse.Namespace, fname: str, i: int) -> None:
+    num_files = len(args.files)
+    num_digits = len(str(num_files))
+    prefix_len = max(len(x) for x in args.files) + 2
+    index_str = str(i + 1).rjust(num_digits)
+
+    _info_verbose(
+        f"Linting {fname.ljust(prefix_len, '.')}.[{index_str}/{num_files}]"
+    )
+
+
 # pylint: disable=too-many-branches
-def main(**kwargs):
+def main(**kwargs) -> None:
     """
     This function applies all rules in this module to the files specified by
     the keywords argument files.
 
     Keyword Args:
         files (list):         a list of the filenames (str) of the files to
                               lint
@@ -1550,14 +1689,17 @@
                               (defaults to 1000)
         columns (int):        max characters per line (defaults to 80)
         indentation (int):    indentation of nested statements (defaults to 2)
         disable (list):       rules (names/codes) to suppress (defaults to [])
         silent (bool):        no output but all rules run
         verbose (bool):       so much output you will not know what to do
     """
+
+    if __name__ != "__main__":
+        sys.argv = []
     args = _parse_args(kwargs)
 
     if __debug__:
         _info_verbose("Debug on . . .")
     else:
         _info_verbose("Debug off . . .")
 
@@ -1568,58 +1710,60 @@
     __init_config_and_suppressions_command_line(args)
     __init_rules(args)
     __verify_glob_suppressions()
     __init_file_and_line_suppressions(args)
 
     total_nr_warnings = 0
     max_warnings = _GLOB_CONFIG["max_warnings"]
+    global_rules = _FILE_RULES[2]
+    if args.enable_experimental:
+        global_rules.add_rule(AnalyseDecls("analyse-decls", "W999"))
 
     def too_many_warnings(nr_warnings):
         if nr_warnings >= max_warnings:
             if not _SILENT:
-                sys.stderr.write("Total errors found: %d\n" % nr_warnings)
+                sys.stderr.write(f"Total errors found: {nr_warnings}\n")
             sys.exit("Too many warnings, giving up!")
 
-    for fname in args.files:
-        _info_verbose("Linting %s . . ." % fname)
+    for i, fname in enumerate(args.files):
+        _verbose_msg_per_file(args, fname, i)
         try:
-            with open(fname, "r", encoding="utf8") as ffile:
+            with open(fname, "r", encoding="utf-8") as ffile:
                 lines = ffile.read()
         except IOError:
-            _info_action("SKIPPING " + fname + ": cannot open for reading")
+            _info_action(f"SKIPPING {fname}: cannot open for reading")
+            continue
 
         nr_warnings = 0
         for rule in _FILE_RULES:
             if not _is_rule_suppressed(fname, 0, rule):
                 nr_warnings, lines = rule(fname, lines, nr_warnings)
                 too_many_warnings(nr_warnings + total_nr_warnings)
         lines = lines.split("\n")
         for linenum in range(len(lines)):
             for rule in _LINE_RULES:
-                if not _is_rule_suppressed(fname, linenum, rule):
+                if not _is_rule_suppressed(fname, linenum + 1, rule):
                     nr_warnings, lines = rule(
                         fname, lines, linenum, nr_warnings
                     )
-                    too_many_warnings(nr_warnings + total_nr_warnings)
+        too_many_warnings(nr_warnings + total_nr_warnings)
         for rule in _LINE_RULES:
             rule.reset()
         total_nr_warnings += nr_warnings
 
     if args.enable_experimental:
-        global_rules = _FILE_RULES[2]
-        global_rules.add_rule(AnalyseDecls("analyse-decls", "W034"))
         total_nr_warnings = global_rules.apply_rules(total_nr_warnings)
 
     if not _SILENT:
         if total_nr_warnings == 0:
             write_to = sys.stdout
         else:
             write_to = sys.stderr
+        # TODO output time taken too
         write_to.write(
-            "Analysed %d files, found %d errors!\n"
-            % (len(args.files), total_nr_warnings)
+            f"Analysed {len(args.files)} files, found {total_nr_warnings} errors!\n"
         )
     sys.exit(total_nr_warnings > 0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gaplint-1.1.5/setup.py` & `gaplint-1.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 A rudimentary linter for GAP (https://www.gap-system.org/) code.
 """
 from setuptools import find_packages, setup
 
 with open("README.rst", "r", encoding="utf8") as f:
     setup(
         name="gaplint",
-        version="1.1.5",
+        version="1.2.0",
+        python_requires=">3.8.0",
         py_modules=["gaplint"],
         url="https://github.com/james-d-mitchell/gaplint",
         license="GPL3",
         author="James D. Mitchell, Simon Tollman",
         author_email="jdm3@st-andrews.ac.uk, skt4@st-andrews.ac.uk",
         description=(
             "A rudimentary linter for GAP "
```

