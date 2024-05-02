# Comparing `tmp/dimentyy_tl_parse-0.0.1.dev2.tar.gz` & `tmp/dimentyy_tl_parse-0.0.1.dev3.tar.gz`

## Comparing `dimentyy_tl_parse-0.0.1.dev2.tar` & `dimentyy_tl_parse-0.0.1.dev3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/fake-src/dimentyy/tl/parse/__init__.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/fake-src/dimentyy/tl/parse/container.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/fake-src/dimentyy/tl/parse/new_html.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/fake-src/dimentyy/tl/parse/types.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/LICENSE.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/pyproject.toml
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/.fake-src/dimentyy/tl/parse/__init__.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/.fake-src/dimentyy/tl/parse/container.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/.fake-src/dimentyy/tl/parse/new_html.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/LICENSE.md
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/README.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/PKG-INFO
```

### Comparing `dimentyy_tl_parse-0.0.1.dev2/fake-src/dimentyy/tl/parse/__init__.py` & `dimentyy_tl_parse-0.0.1.dev3/.fake-src/dimentyy/tl/parse/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 """Better parsing modes for telethon.TelegramClient"""
+
+from telethon import TelegramClient
 from telethon.tl.types import TypeMessageEntity
 
 from .new_html import HTMLParser, OnUnknownTag
 
 
 class HTML:
     """
-    **Don't forget to initialize this class!**
-
     This class should primarily be used
     only by telethon.TelegramClient as it
     automatically parses and unparses messages
     making it easier to work with messages.
 
     **Setup**:
 
     >>> client = TelegramClient(...)
     >>> client.parse_mode = HTML()
     """
 
-    def __init__(self, on_unknown_tag: OnUnknownTag = "ignore"):
+    def __init__(self, client: TelegramClient, on_unknown_tag: OnUnknownTag = "ignore"):
+        self.client = client
         self.on_unknown_tag = on_unknown_tag
 
+    @classmethod
+    def applied_to(cls, client: TelegramClient, on_unknown_tag: OnUnknownTag = "ignore"):
+        self = cls(
+            client=client,
+            on_unknown_tag=on_unknown_tag
+        )
+        client.parse_mode = self
+        return self
+
     def parse(self, text: str) -> tuple[str, list[TypeMessageEntity]]:
         """
         **This method is called by** ``telethon.TelegramClient``.
         """
 
         return HTMLParser.immediate(text, self.on_unknown_tag)
```

### Comparing `dimentyy_tl_parse-0.0.1.dev2/LICENSE.md` & `dimentyy_tl_parse-0.0.1.dev3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dimentyy_tl_parse-0.0.1.dev2/pyproject.toml` & `dimentyy_tl_parse-0.0.1.dev3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
-packages = ["fake-src/dimentyy"]
+packages = [".fake-src/dimentyy"]
 
 [tool.hatch.build.targets.sdist]
-only-include = ["fake-src/dimentyy"]
+only-include = [".fake-src/dimentyy"]
 
 [project]
 name = "dimentyy.tl-parse"
 description = "Better parsing modes for telethon.TelegramClient"
-version = "0.0.1dev2"
+version = "0.0.1dev3"
 readme = "README.md"
-requires-python = ">=3.10"
+#requires-python = ">=3.10" #currently unknown
 license = "MIT"
 authors = [
   { name = "dimentyy" },
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

