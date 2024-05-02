# Comparing `tmp/gr1336_toolbox-0.0.1.tar.gz` & `tmp/gr1336_toolbox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gr1336_toolbox-0.0.1.tar", last modified: Thu May  2 15:49:42 2024, max compression
+gzip compressed data, was "gr1336_toolbox-0.0.2.tar", last modified: Thu May  2 16:00:12 2024, max compression
```

## Comparing `gr1336_toolbox-0.0.1.tar` & `gr1336_toolbox-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:49:42.449966 gr1336_toolbox-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 15:49:34.000000 gr1336_toolbox-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-02 15:49:42.449966 gr1336_toolbox-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-02 15:49:34.000000 gr1336_toolbox-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:49:42.445966 gr1336_toolbox-0.0.1/gr1336_toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-02 15:49:34.000000 gr1336_toolbox-0.0.1/gr1336_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-02 15:49:34.000000 gr1336_toolbox-0.0.1/gr1336_toolbox/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-02 15:49:34.000000 gr1336_toolbox-0.0.1/gr1336_toolbox/misc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-02 15:49:34.000000 gr1336_toolbox-0.0.1/gr1336_toolbox/test_even_odd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-02 15:49:34.000000 gr1336_toolbox-0.0.1/gr1336_toolbox/text_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-02 15:49:34.000000 gr1336_toolbox-0.0.1/gr1336_toolbox/types_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:49:42.449966 gr1336_toolbox-0.0.1/gr1336_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-02 15:49:42.000000 gr1336_toolbox-0.0.1/gr1336_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 15:49:42.000000 gr1336_toolbox-0.0.1/gr1336_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:49:42.000000 gr1336_toolbox-0.0.1/gr1336_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 15:49:42.000000 gr1336_toolbox-0.0.1/gr1336_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 15:49:42.000000 gr1336_toolbox-0.0.1/gr1336_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:49:42.449966 gr1336_toolbox-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-02 15:49:34.000000 gr1336_toolbox-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:00:12.856040 gr1336_toolbox-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-02 16:00:12.856040 gr1336_toolbox-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:00:12.856040 gr1336_toolbox-0.0.2/gr1336_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/gr1336_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/gr1336_toolbox/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/gr1336_toolbox/misc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/gr1336_toolbox/test_even_odd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/gr1336_toolbox/text_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/gr1336_toolbox/types_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:00:12.856040 gr1336_toolbox-0.0.2/gr1336_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-02 16:00:12.000000 gr1336_toolbox-0.0.2/gr1336_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 16:00:12.000000 gr1336_toolbox-0.0.2/gr1336_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:00:12.000000 gr1336_toolbox-0.0.2/gr1336_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 16:00:12.000000 gr1336_toolbox-0.0.2/gr1336_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 16:00:12.000000 gr1336_toolbox-0.0.2/gr1336_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:00:12.856040 gr1336_toolbox-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-02 16:00:08.000000 gr1336_toolbox-0.0.2/setup.py
```

### Comparing `gr1336_toolbox-0.0.1/LICENSE` & `gr1336_toolbox-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.1/PKG-INFO` & `gr1336_toolbox-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gr1336_toolbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Personal collection of reusable tools in python.
 Home-page: https://github.com/gr1336/gr1336_toolbox/
 Author: gr1336
 License:  Apache Software License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `gr1336_toolbox-0.0.1/gr1336_toolbox/__init__.py` & `gr1336_toolbox-0.0.2/gr1336_toolbox/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-# requires: pyperclip, textblob, pyyaml, pyarrow,
-
 from .misc_tools import (
     np_list,
     current_time,
     clipboard,
     flatten_list,
     filter_list,
     dict_to_list,
     try_call,
-    atoi,
-    natural_keys,
     recursive_replacer,
 )
 from .file_manager import (
     load_parquet,
     load_text,
     load_yaml,
     save_parquet,
@@ -32,24 +28,22 @@
     _str,
     _compare,
     _int
 )
 from .text_tools import (
     unescape,
     trimincompletesentence,
-    simple_quotes,
+    simplify_quotes,
     blob_split,
 )
 
 __all__ = [
     "try_call",
     "np_list",
-    "natural_keys",
-    "simple_quotes",
-    "atoi",
+    "simplify_quotes",
     "blob_split",
     "load_text",
     "current_time",
     "recursive_replacer",
     "clipboard",
     "flatten_list",
     "get_files",
```

### Comparing `gr1336_toolbox-0.0.1/gr1336_toolbox/file_manager.py` & `gr1336_toolbox-0.0.2/gr1336_toolbox/file_manager.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from pathlib import Path
 import yaml
-from typing import Any
-from .types_check import _path
 import pandas as pd
 import pyarrow as pa
+from typing import Any
+from pathlib import Path
 import pyarrow.parquet as pq
+from .types_check import _path
 
 
 def get_dirs(path: str | Path) -> list[str]:
     if not _path(path):
         return []
     return [str(x) for x in Path(path).glob("*") if x.is_dir()]
```

### Comparing `gr1336_toolbox-0.0.1/gr1336_toolbox/misc_tools.py` & `gr1336_toolbox-0.0.2/gr1336_toolbox/misc_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from .types_check import _array, _dict, _numpy
-from typing import Any, TypeAlias, Literal, Callable
 import re
-from datetime import datetime
 import pyperclip
+from datetime import datetime
+from .types_check import _array, _dict, _numpy
+from typing import Any, TypeAlias, Literal, Callable
+
+
 
 
 def np_list(content):
     if _numpy(content):
         return content.flatten().tolist()
 
 
@@ -63,15 +65,15 @@
 def recursive_replacer(text: str, dic: dict) -> str:
     for i, j in dic.items():
         text = text.replace(i, j)
     return text
 
 
 def atoi(text: str):
-    # From oobabooga
+    """Credits"""
     text = text.strip()
     return int(text) if text.isdigit() else text.lower()
 
 
 def natural_keys(text):
     # From oobabooga
     return [atoi(c) for c in re.split(r"(\d+)", text)]
```

### Comparing `gr1336_toolbox-0.0.1/gr1336_toolbox/test_even_odd.py` & `gr1336_toolbox-0.0.2/gr1336_toolbox/test_even_odd.py`

 * *Files identical despite different names*

### Comparing `gr1336_toolbox-0.0.1/gr1336_toolbox/text_tools.py` & `gr1336_toolbox-0.0.2/gr1336_toolbox/text_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-import re
 from .types_check import _str
 from textblob import TextBlob
 
-
 def unescape(elem: str) -> str:
     assert _str(elem, True), "The input should be a valid string."
     return elem.encode().decode("unicode-escape", "ignore")
 
-
-def simple_quotes(txt):
-    """Idea from kobold"""
-    replacements = {
-        "“": '"',
-        "”": '"',
-        "’": "'",
-        "‘": "'",
-        "`": "'",
-    }
-    for key, value in replacements.items():
-        txt = txt.replace(key, value)
-    return txt
-
-
 def blob_split(text: str) -> list[str]:
     return [x for x in TextBlob(text).raw_sentences]
 
-
 def trimincompletesentence(txt: str) -> str:
     """Idea from KoboldAI"""
     # Cache length of text
     ln = len(txt)
     # Find last instance of punctuation (Borrowed from Clover-Edition by cloveranon)
-    lastpunc = max(txt.rfind("."), txt.rfind("!"), txt.rfind("?"))
+    lastpunc = max(txt.rfind(". "), txt.rfind("!"), txt.rfind("?"))
     # Is this the end of a quote?
     if lastpunc < ln - 1:
         if txt[lastpunc + 1] == '"':
             lastpunc = lastpunc + 1
     if lastpunc >= 0:
         txt = txt[: lastpunc + 1]
     return txt
+
+def simplify_quotes(txt:str) -> str:
+    """Idea from kobold"""
+    assert _str(txt, True), f"The input '{txt}' is not a valid string"
+    replacements = {
+        "“": '"',
+        "”": '"',
+        "’": "'",
+        "‘": "'",
+        "`": "'",
+    }
+    for key, value in replacements.items():
+        txt = txt.replace(key, value)
+    return txt
```

### Comparing `gr1336_toolbox-0.0.1/gr1336_toolbox/types_check.py` & `gr1336_toolbox-0.0.2/gr1336_toolbox/types_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Any, Callable
 from pathlib import Path
 from numpy import ndarray
+from typing import Any, Callable
+
 
 
 def _int(entry: Any, check_string: bool = False):
     if check_string and _str(entry):
         try:
             int(entry)
             return True
```

### Comparing `gr1336_toolbox-0.0.1/gr1336_toolbox.egg-info/PKG-INFO` & `gr1336_toolbox-0.0.2/gr1336_toolbox.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gr1336_toolbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Personal collection of reusable tools in python.
 Home-page: https://github.com/gr1336/gr1336_toolbox/
 Author: gr1336
 License:  Apache Software License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `gr1336_toolbox-0.0.1/setup.py` & `gr1336_toolbox-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    version="0.0.1",
+    version="0.0.2",
     name="gr1336_toolbox",
     description="Personal collection of reusable tools in python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gr1336/gr1336_toolbox/",
     install_requires=["numpy", "pyperclip", "textblob", "pyyaml", "pyarrow"],
     author="gr1336",
```

