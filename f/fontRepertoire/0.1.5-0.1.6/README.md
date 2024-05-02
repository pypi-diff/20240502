# Comparing `tmp/fontRepertoire-0.1.5.tar.gz` & `tmp/fontrepertoire-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fontRepertoire-0.1.5.tar", last modified: Tue Mar 26 13:44:51 2024, max compression
+gzip compressed data, was "fontrepertoire-0.1.6.tar", last modified: Thu May  2 19:20:52 2024, max compression
```

## Comparing `fontRepertoire-0.1.5.tar` & `fontrepertoire-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 13:44:51.417126 fontRepertoire-0.1.5/
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-03-26 13:44:50.000000 fontRepertoire-0.1.5/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 13:44:51.413126 fontRepertoire-0.1.5/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 13:44:51.415126 fontRepertoire-0.1.5/Lib/fontRepertoire/
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-03-26 13:44:50.000000 fontRepertoire-0.1.5/Lib/fontRepertoire/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2335 2024-03-26 13:44:50.000000 fontRepertoire-0.1.5/Lib/fontRepertoire/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6855 2024-03-26 13:44:50.000000 fontRepertoire-0.1.5/Lib/fontRepertoire/characterSet.py
--rw-rw-rw-   0 root         (0) root         (0)    10705 2024-03-26 13:44:50.000000 fontRepertoire-0.1.5/Lib/fontRepertoire/codepointToGlyphMap.py
--rw-rw-rw-   0 root         (0) root         (0)     7383 2024-03-26 13:44:50.000000 fontRepertoire-0.1.5/Lib/fontRepertoire/glyphRepertoire.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 13:44:51.417126 fontRepertoire-0.1.5/Lib/fontRepertoire.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1669 2024-03-26 13:44:51.000000 fontRepertoire-0.1.5/Lib/fontRepertoire.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      470 2024-03-26 13:44:51.000000 fontRepertoire-0.1.5/Lib/fontRepertoire.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 13:44:51.000000 fontRepertoire-0.1.5/Lib/fontRepertoire.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      123 2024-03-26 13:44:51.000000 fontRepertoire-0.1.5/Lib/fontRepertoire.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-26 13:44:51.000000 fontRepertoire-0.1.5/Lib/fontRepertoire.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2024-03-26 13:44:51.417126 fontRepertoire-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      353 2024-03-26 13:44:50.000000 fontRepertoire-0.1.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1909 2024-03-26 13:44:51.418126 fontRepertoire-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-03-26 13:44:50.000000 fontRepertoire-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 13:44:51.417126 fontRepertoire-0.1.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2579 2024-03-26 13:44:50.000000 fontRepertoire-0.1.5/tests/test_charset.py
--rw-rw-rw-   0 root         (0) root         (0)      964 2024-03-26 13:44:50.000000 fontRepertoire-0.1.5/tests/test_glyphrepertoire.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 19:20:52.771502 fontrepertoire-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-02 19:20:51.000000 fontrepertoire-0.1.6/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 19:20:52.767502 fontrepertoire-0.1.6/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 19:20:52.769502 fontrepertoire-0.1.6/Lib/fontRepertoire/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-02 19:20:51.000000 fontrepertoire-0.1.6/Lib/fontRepertoire/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2024-05-02 19:20:51.000000 fontrepertoire-0.1.6/Lib/fontRepertoire/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7322 2024-05-02 19:20:51.000000 fontrepertoire-0.1.6/Lib/fontRepertoire/characterSet.py
+-rw-rw-rw-   0 root         (0) root         (0)    11457 2024-05-02 19:20:51.000000 fontrepertoire-0.1.6/Lib/fontRepertoire/codepointToGlyphMap.py
+-rw-rw-rw-   0 root         (0) root         (0)     7657 2024-05-02 19:20:51.000000 fontrepertoire-0.1.6/Lib/fontRepertoire/glyphRepertoire.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 19:20:52.770502 fontrepertoire-0.1.6/Lib/fontRepertoire.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1669 2024-05-02 19:20:52.000000 fontrepertoire-0.1.6/Lib/fontRepertoire.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      470 2024-05-02 19:20:52.000000 fontrepertoire-0.1.6/Lib/fontRepertoire.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 19:20:52.000000 fontrepertoire-0.1.6/Lib/fontRepertoire.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      123 2024-05-02 19:20:52.000000 fontrepertoire-0.1.6/Lib/fontRepertoire.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-02 19:20:52.000000 fontrepertoire-0.1.6/Lib/fontRepertoire.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2024-05-02 19:20:52.771502 fontrepertoire-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      353 2024-05-02 19:20:51.000000 fontrepertoire-0.1.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1909 2024-05-02 19:20:52.771502 fontrepertoire-0.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-02 19:20:51.000000 fontrepertoire-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 19:20:52.770502 fontrepertoire-0.1.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2579 2024-05-02 19:20:51.000000 fontrepertoire-0.1.6/tests/test_charset.py
+-rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-02 19:20:51.000000 fontrepertoire-0.1.6/tests/test_glyphrepertoire.py
```

### Comparing `fontRepertoire-0.1.5/LICENSE` & `fontrepertoire-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fontRepertoire-0.1.5/Lib/fontRepertoire/base.py` & `fontrepertoire-0.1.6/Lib/fontRepertoire/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 base
 ===============================================================================
 """
 from __future__ import annotations
 
 from collections.abc import Set as AbstractSet
-from typing import Any
+from typing import Any, TYPE_CHECKING, Union
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 class BaseReperoire(set):
     itemtype = Any
 
     def __and__(self, other: AbstractSet) -> Self:
         return self.__class__(set(self) & other)
 
@@ -63,19 +66,19 @@
         return result
 
     def update(self, values):
         _values = set(values)
         self._check_type_squence(_values)
         super().update(_values)
 
-    def open(self, path: str) -> None:
+    def open(self, path: Union[str, Path]) -> None:
         raise NotImplementedError
 
     @property
     def as_set(self) -> set:
         return set(self)
 
     @classmethod
-    def fromFile(cls, path: str) -> Self:
+    def fromFile(cls, path: Union[str, Path]) -> Self:
         result = cls()
         result.open(path)
         return result
```

### Comparing `fontRepertoire-0.1.5/Lib/fontRepertoire/characterSet.py` & `fontrepertoire-0.1.6/Lib/fontRepertoire/characterSet.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """
 characterSet
 ===============================================================================
 """
+
 from __future__ import annotations
 
 import logging
 import os
 from datetime import date
-from typing import List
+from typing import List, TYPE_CHECKING, Union
 import unicodedata2
 from fontTools.agl import UV2AGL
 from fontTools.ttLib import TTFont
 from fontTools.unicodedata import block
 
 from .base import BaseReperoire
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 log = logging.getLogger(__name__)
 
 
 def unicodename(codepoint: int) -> str:
     try:
         value = int(codepoint)
     except ValueError:
@@ -40,14 +44,15 @@
     return f"uni{codepoint:04X}"
 
 
 class CharSet(BaseReperoire):
     """
     Class to represent a Character Set as a set of codepoints (integers)
     """
+
     itemtype = int
 
     def __init__(self, iterable=None, name=""):
         if iterable:
             super().__init__(iterable)
         else:
             super().__init__()
@@ -63,15 +68,15 @@
 
     def hasCodepoint(self, codepoint: int) -> bool:
         return codepoint in self
 
     def hasCharacter(self, character: str) -> bool:
         return ord(character) in self
     
-    def open(self, path: str) -> None:
+    def open(self, path: Union[str, Path]) -> None:
         """
         Open a Character Set from a plain text file.
         """
         codepoints = set()
         if os.path.isfile(path):
             with open(path, "r", encoding="utf-8") as charsetFile:
                 for line in charsetFile:
@@ -100,37 +105,43 @@
                             if parts:
                                 try:
                                     codepoints.add(int(parts[0], 16))
                                 except ValueError:
                                     pass
         self.codepoints = codepoints
         if not self.name:
-            self.name = os.path.splitext(os.path.basename(inPath))[0]
+            self.name = os.path.splitext(os.path.basename(path))[0]
 
-    def save(self, outPath: str, newLine: str = "\n") -> None:
+    def toString(self, newLine: str = "\n") -> str:
+        result = ""
         header = """
 # Character Set Definition
 #
 # Name: {c.name}
 # Version: {c.version}
 # Copyright: {c.copyright}
 # Description: {c.description}
 
 """
+        result += header.format(c=self)
+        currentBlock: str = ""
+        for codepoint in sorted(self):
+            _block = block(chr(codepoint))
+            if _block != currentBlock:
+                result += f"{newLine}# {_block}{newLine}"
+                currentBlock = _block
+            result += f"0x{codepoint:04X}\t# {unicodename(codepoint)}{newLine}"
+        return result
+
+    def save(self, outPath: str, newLine: str = "\n") -> None:
+        """
+        Save the Character Set as plain text file.
+        """
         with open(outPath, "w", encoding="utf-8") as charsetFile:
-            currentBlock:str = ""
-            charsetFile.write(header.format(c=self))
-            for codepoint in sorted(self):
-                _block = block(chr(codepoint))
-                if _block != currentBlock:
-                    charsetFile.write(f"{newLine}# {_block}{newLine}")
-                    currentBlock = _block
-                charsetFile.write(
-                    "0x%04X\t# %s%s" % (codepoint, unicodename(codepoint), newLine)
-                )
+            charsetFile.write(self.toString(newLine))
 
     @property
     def codepoints(self) -> List[int]:
         """
         Ordered list of codepoints (int)
         """
         return list(sorted(self))
@@ -141,23 +152,21 @@
         self.clear()
         self.update(_values)
 
     @property
     def as_set(self) -> set:
         return set(self)
 
-        
     @classmethod
     def fromString(cls, string: str) -> CharSet:
         """
         Instantiate a Character Set from a string.
         """
         return cls(ord(c) for c in string)
 
-        
     @classmethod
     def fromTTFont(cls, font: TTFont) -> CharSet:
         """
         Instantiate a Character Set from a fontTools TTFont font object.
         """
         cmap = font.getBestCmap()
         return cls(cmap.keys())
@@ -178,14 +187,23 @@
                 unicodedata = naked_ufo.unicodeData
         if unicodedata:
             return cls(unicodedata.keys())
         else:
             log.warning("Can't get Unicode data from UFO: %r", ufo)
         return cls()
 
+    @classmethod
+    def fromGSFont(cls, gsFont) -> CharSet:
+        """
+        Instantiate a Character Set from a GSFont font object (Glyphs App file).
+        """
+        return cls(
+            set(int(g.unicode, 16) for g in gsFont.glyphs if g.unicode is not None)
+        )
+
 
 class __CharSet:
     """
     Class to represent a Character Set
     """
 
     def __init__(self, name=""):
@@ -204,15 +222,14 @@
             for codepoint in sorted(self.codepoints):
                 charsetFile.write(
                     "%s \t# 0x%04X %s%s"
                     % (glyphname(codepoint), codepoint, unicodename(codepoint), newLine)
                 )
 
 
-
 def __test001():
     charset = CharSet()
     print(charset)
     print((ord(c) for c in "abc"))
     print(list(ord(c) for c in "abc"))
     charset.codepoints = (ord(c) for c in "abc")
     print(charset)
```

### Comparing `fontRepertoire-0.1.5/Lib/fontRepertoire/codepointToGlyphMap.py` & `fontrepertoire-0.1.6/Lib/fontRepertoire/codepointToGlyphMap.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 if TYPE_CHECKING:
     from defcon import Font as defconUFO
     from fontParts.base import BaseFont as fontPartsUFO
     from fontTools.ttLib import TTFont
     from fontTools.ttLib.tables._c_m_a_p import CmapSubtable, table__c_m_a_p
     from ufoLib2 import Font as ufoLib2UFO
+    from glyphsLib import GSFont, GSGlyph
 
 log = logging.getLogger(__name__)
 
 
 class CodepointToGlyphMap(dict):
     """
     Class to represent a codepoint (integer) to glyph name (string) mapping.
@@ -81,22 +82,42 @@
         """
         unicodedata = None
         if hasattr(ufo, "unicodeData"):
             # it's a defcon like UFO
             unicodedata = ufo.unicodeData
         elif hasattr(ufo, "naked"):
             # it's a fontParts like UFO
-            naked_ufo = ufo.naked()
+            naked_ufo:defconUFO = ufo.naked()
             if hasattr(naked_ufo, "unicodeData"):
                 unicodedata = naked_ufo.unicodeData
         if unicodedata:
             return cls(unicodedata)
         log.warning("Can't get Unicode data from UFO: %r", ufo)
         return cls()
 
+    @classmethod
+    def fromGSFont(cls, gsFont:GSFont) -> CodepointToGlyphMap:
+        """
+        Instantiate a CodepointToGlyphMap from a GSFont font object (Glyphs App file).
+        """
+        unicodedata = {}
+        glyph:GSGlyph
+        for glyph in gsFont.glyphs:
+            if not glyph.unicodes:
+                continue
+            for unicode in glyph.unicodes:
+                codepoint = int(unicode, 16)
+                if codepoint in unicodedata:
+                    continue
+                unicodedata[codepoint] = glyph.name
+        if unicodedata:
+            return cls(unicodedata)
+        log.warning("Can't get Unicode data from GSFont: %r", gsFont)
+        return cls()
+
     @property
     def codepoints(self) -> List[int]:
         """
         Ordered list of codepoints (int)
         """
         return list(sorted(self.keys()))
```

### Comparing `fontRepertoire-0.1.5/Lib/fontRepertoire/glyphRepertoire.py` & `fontrepertoire-0.1.6/Lib/fontRepertoire/glyphRepertoire.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from glyphsLib.glyphdata import get_glyph
 
 from .base import BaseReperoire
 
 if TYPE_CHECKING:
     from fontParts.base.font import BaseFont
     from fontTools.ttLib import TTFont
+    from glyphsLib import GSFont
 
 uni4name = re.compile(r"^uni[0-9A-F]{4}$")
 uni5name = re.compile(r"^u[0-9A-F]{5}$")
 
 
 def getCodepoint(glyphname: str, default: Any = None) -> Optional[int]:
     if uni4name.match(glyphname):
@@ -97,18 +98,26 @@
             return cls(font.glyphOrder)
         except AttributeError:
             return cls(font.getGlyphOrder())
 
     @classmethod
     def fromUFO(cls, ufo: BaseFont) -> GlyphRepertoire:
         """
-        Instantiate a Glyph Repertoire from a UFO font object
+        Instantiate a Glyph Repertoire from a UFO font object.
         """
         return cls(g.name for g in ufo)
 
+    @classmethod
+    def fromGSFont(cls, gsFont:GSFont) -> GlyphRepertoire:
+        """
+        Instantiate a Glyph Repertoire from a GSFont font object (Glyphs App file).
+        """
+        return cls(g.name for g in gsFont.glyphs)
+    
+
     def save(self, outPath: str, newLine: str = "\n", auto_comment: bool = True):
         """
         Save the Glyph Repertoire as plain text file.
         """
         header = """
 # Glyph Repertoire Definition
 #
```

### Comparing `fontRepertoire-0.1.5/Lib/fontRepertoire.egg-info/PKG-INFO` & `fontrepertoire-0.1.6/Lib/fontRepertoire.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fontRepertoire
-Version: 0.1.5
+Version: 0.1.6
 Summary: Basic classes to represent character set and glyph repertoire.
 Home-page: https://gitlab.com/fontstuff/fontRepertoire
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/fontstuff/fontRepertoire
 Project-URL: Documentation, https://fontstuff.gitlab.io/fontRepertoire
 Project-URL: Tracker, https://gitlab.com/fontstuff/fontRepertoire/-/issues
```

### Comparing `fontRepertoire-0.1.5/PKG-INFO` & `fontrepertoire-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fontRepertoire
-Version: 0.1.5
+Version: 0.1.6
 Summary: Basic classes to represent character set and glyph repertoire.
 Home-page: https://gitlab.com/fontstuff/fontRepertoire
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/fontstuff/fontRepertoire
 Project-URL: Documentation, https://fontstuff.gitlab.io/fontRepertoire
 Project-URL: Tracker, https://gitlab.com/fontstuff/fontRepertoire/-/issues
```

### Comparing `fontRepertoire-0.1.5/setup.cfg` & `fontrepertoire-0.1.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.5
+current_version = 0.1.6
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
```

### Comparing `fontRepertoire-0.1.5/tests/test_charset.py` & `fontrepertoire-0.1.6/tests/test_charset.py`

 * *Files identical despite different names*

### Comparing `fontRepertoire-0.1.5/tests/test_glyphrepertoire.py` & `fontrepertoire-0.1.6/tests/test_glyphrepertoire.py`

 * *Files identical despite different names*

