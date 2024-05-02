# Comparing `tmp/pathlib_next-0.3.0.tar.gz` & `tmp/pathlib_next-0.3.5.tar.gz`

## Comparing `pathlib_next-0.3.0.tar` & `pathlib_next-0.3.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/example.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/__init__.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/fspath.py
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/mempath.py
--rw-r--r--   0        0        0    12834 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/path.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/protocols/__init__.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/protocols/fs.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/protocols/io.py
--rw-r--r--   0        0        0    15590 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/uri/__init__.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/uri/query.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/uri/source.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/uri/schemes/__init__.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/uri/schemes/file.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/uri/schemes/http.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/uri/schemes/sftp.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/utils/__init__.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/utils/glob.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/utils/stat.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/utils/sync.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/tests/test_local.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/tests/test_uri.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/LICENSE
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/example.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/__init__.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/fspath.py
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/mempath.py
+-rw-r--r--   0        0        0    12834 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/path.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/protocols/__init__.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/protocols/fs.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/protocols/io.py
+-rw-r--r--   0        0        0    15590 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/uri/__init__.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/uri/query.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/uri/source.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/uri/schemes/__init__.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/uri/schemes/file.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/uri/schemes/http.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/uri/schemes/sftp.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/utils/__init__.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/utils/glob.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/utils/stat.py
+-rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/src/pathlib_next/utils/sync.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/tests/test_local.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/tests/test_uri.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/LICENSE
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pathlib_next-0.3.5/PKG-INFO
```

### Comparing `pathlib_next-0.3.0/src/example.py` & `pathlib_next-0.3.5/src/example.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import os
 
 from pathlib_next import Path, glob
 from pathlib_next.mempath import MemPath
 from pathlib_next.uri import Query, Source, Uri, UriPath
-from pathlib_next.utils.sync import PathSyncer
+from pathlib_next.utils.sync import PathAndStat, PathSyncer
 
 rootless = Uri("sftp://root@sftpexample")
 rootless.source
 authkeys = rootless / "root/.ssh/authorized_keys"
 keys = authkeys.as_uri()
 
 local = Path("./_ssh")
 
 mempath = MemPath("test/test3") / "subpath"
 mempath.parent.mkdir(parents=True, exist_ok=True)
 mempath.write_text("test")
 check = mempath.read_text()
 mempath.parent.rm(recursive=True)
 
-test = list(os.scandir(local))
-print(list(local.iterdir()))
 query = Query({"test": "://$#!1", "test2&": [1, 2]})
 q2 = Query(str(query)).to_dict()
 for name, value in query:
     print(f"{name}: {value}")
 src = Source(scheme="scheme", userinfo="user", host="123.com", port=0)
 test = {**src}
 test2 = [*src]
@@ -49,21 +47,21 @@
 
 sftp_root = UriPath("sftp://root@sftpexample/")
 print(sftp_root.as_posix())
 authkeys = sftp_root / "root/.ssh/authorized_keys"
 print(authkeys.as_posix())
 
 
-def checksum(uri: UriPath):
-    stat = uri.stat()
+def checksum(uri: PathAndStat):
+    stat = uri.stat
     return hash(stat.st_size)
 
 
 syncer = PathSyncer(checksum, remove_missing=False)
-syncer.sync((sftp_root / "root/.ssh"), dest, dry_run=True)
+syncer.sync((sftp_root / "root/.ssh"), dest, dry_run=False)
 
 rocky_repo = UriPath("http://dl.rockylinux.org/pub")
 
 glob_test = UriPath("file:src/**/*.py")
 
 for path in glob.glob(glob_test, recursive=True):
     print(path)
```

### Comparing `pathlib_next-0.3.0/src/pathlib_next/fspath.py` & `pathlib_next-0.3.5/src/pathlib_next/fspath.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/src/pathlib_next/mempath.py` & `pathlib_next-0.3.5/src/pathlib_next/mempath.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/src/pathlib_next/path.py` & `pathlib_next-0.3.5/src/pathlib_next/path.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/src/pathlib_next/protocols/fs.py` & `pathlib_next-0.3.5/src/pathlib_next/protocols/fs.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/src/pathlib_next/protocols/io.py` & `pathlib_next-0.3.5/src/pathlib_next/protocols/io.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/src/pathlib_next/uri/__init__.py` & `pathlib_next-0.3.5/src/pathlib_next/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/src/pathlib_next/uri/query.py` & `pathlib_next-0.3.5/src/pathlib_next/uri/query.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/src/pathlib_next/uri/source.py` & `pathlib_next-0.3.5/src/pathlib_next/uri/source.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/src/pathlib_next/uri/schemes/file.py` & `pathlib_next-0.3.5/src/pathlib_next/uri/schemes/file.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/src/pathlib_next/uri/schemes/http.py` & `pathlib_next-0.3.5/src/pathlib_next/uri/schemes/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import time as _time
 import typing as _ty
 
 import bs4 as _bs4
 import requests as _req
 from htmllistparse import parse as _htmlparse
 
+if _ty.TYPE_CHECKING:
+    from urllib3.response import HTTPResponse
+
 from ... import utils as _utils
 from ...utils.stat import FileStat
 from .. import UriPath
 
 
 class _FileEntry(_ty.NamedTuple):
     name: str
@@ -115,18 +118,20 @@
         mode="r",
         buffering=-1,
     ):
         if mode != "r":
             raise NotImplementedError(mode)
         buffer_size = _io.DEFAULT_BUFFER_SIZE if buffering < 0 else buffering
         req = self.backend.request("GET", self.as_uri(), stream=True)
+        resp: "HTTPResponse" = req.raw
+        resp.auto_close = False
         return (
-            req.raw
+            resp
             if buffer_size == 0
-            else _io.BufferedReader(req.raw, buffer_size=buffer_size)
+            else _io.BufferedReader(resp, buffer_size=buffer_size)
         )
 
     def is_dir(self):
         if self._isdir is None:
             self.stat()
         return self._is_dir is not None and self._isdir
```

### Comparing `pathlib_next-0.3.0/src/pathlib_next/uri/schemes/sftp.py` & `pathlib_next-0.3.5/src/pathlib_next/uri/schemes/sftp.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/src/pathlib_next/utils/__init__.py` & `pathlib_next-0.3.5/src/pathlib_next/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/src/pathlib_next/utils/glob.py` & `pathlib_next-0.3.5/src/pathlib_next/utils/glob.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/src/pathlib_next/utils/stat.py` & `pathlib_next-0.3.5/src/pathlib_next/utils/stat.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/tests/test_local.py` & `pathlib_next-0.3.5/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/tests/test_uri.py` & `pathlib_next-0.3.5/tests/test_uri.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/LICENSE` & `pathlib_next-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.3.0/pyproject.toml` & `pathlib_next-0.3.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pathlib_next"
-version = "0.3.0"
+version = "0.3.5"
 authors = [{ name = "Jose A" }]
 description = "Generic Path Protocol based pathlib"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pathlib_next-0.3.0/PKG-INFO` & `pathlib_next-0.3.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pathlib_next
-Version: 0.3.0
+Version: 0.3.5
 Summary: Generic Path Protocol based pathlib
 Project-URL: Homepage, https://github.com/jose-pr/pathlib_next/
 Project-URL: Issues, https://github.com/jose-pr/pathlib_next/issues
 Author: Jose A
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

