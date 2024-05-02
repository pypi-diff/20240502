# Comparing `tmp/htagui-0.5.6.tar.gz` & `tmp/htagui-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagui-0.5.6.tar", max compression
+gzip compressed data, was "htagui-0.5.7.tar", max compression
```

## Comparing `htagui-0.5.6.tar` & `htagui-0.5.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1065 2024-05-01 11:41:38.108568 htagui-0.5.6/LICENSE
--rw-r--r--   0        0        0     8505 2024-05-01 11:41:38.108568 htagui-0.5.6/README.md
--rw-r--r--   0        0        0      330 2024-05-01 11:41:38.360570 htagui-0.5.6/htagui/__init__.py
--rw-r--r--   0        0        0      892 2024-05-01 11:41:38.108568 htagui-0.5.6/htagui/all.py
--rw-r--r--   0        0        0      750 2024-05-01 11:41:38.108568 htagui-0.5.6/htagui/basics/__init__.py
--rw-r--r--   0        0        0    11404 2024-05-01 11:41:38.108568 htagui-0.5.6/htagui/basics/bases.py
--rw-r--r--   0        0        0      771 2024-05-01 11:41:38.108568 htagui-0.5.6/htagui/bulma/__init__.py
--rw-r--r--   0        0        0   656501 2024-05-01 11:41:38.108568 htagui-0.5.6/htagui/bulma/bases.py
--rw-r--r--   0        0        0     4268 2024-05-01 11:41:38.108568 htagui-0.5.6/htagui/common.py
--rw-r--r--   0        0        0     3401 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/dialog.py
--rw-r--r--   0        0        0      648 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/fileupload.py
--rw-r--r--   0        0        0     1856 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/flex.py
--rw-r--r--   0        0        0      785 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/fluent/__init__.py
--rw-r--r--   0        0        0     8538 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/fluent/bases.py
--rw-r--r--   0        0        0      771 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/form.py
--rw-r--r--   0        0        0     3795 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/ifields.py
--rw-r--r--   0        0        0      922 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/md/__init__.py
--rw-r--r--   0        0        0    10945 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/md/bases.py
--rw-r--r--   0        0        0      774 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/shoelace/__init__.py
--rw-r--r--   0        0        0     8489 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/shoelace/bases.py
--rw-r--r--   0        0        0     9619 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/splitters.py
--rw-r--r--   0        0        0     1441 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/tabs.py
--rw-r--r--   0        0        0     1069 2024-05-01 11:41:38.360570 htagui-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     9738 1970-01-01 00:00:00.000000 htagui-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-01 15:30:00.152963 htagui-0.5.7/LICENSE
+-rw-r--r--   0        0        0     8505 2024-05-01 15:30:00.152963 htagui-0.5.7/README.md
+-rw-r--r--   0        0        0      330 2024-05-01 15:30:00.416965 htagui-0.5.7/htagui/__init__.py
+-rw-r--r--   0        0        0      892 2024-05-01 15:30:00.152963 htagui-0.5.7/htagui/all.py
+-rw-r--r--   0        0        0      750 2024-05-01 15:30:00.152963 htagui-0.5.7/htagui/basics/__init__.py
+-rw-r--r--   0        0        0    11404 2024-05-01 15:30:00.152963 htagui-0.5.7/htagui/basics/bases.py
+-rw-r--r--   0        0        0      771 2024-05-01 15:30:00.152963 htagui-0.5.7/htagui/bulma/__init__.py
+-rw-r--r--   0        0        0   656501 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/bulma/bases.py
+-rw-r--r--   0        0        0     4268 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/common.py
+-rw-r--r--   0        0        0     3287 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/dialog.py
+-rw-r--r--   0        0        0      648 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/fileupload.py
+-rw-r--r--   0        0        0     1856 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/flex.py
+-rw-r--r--   0        0        0      785 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/fluent/__init__.py
+-rw-r--r--   0        0        0     8538 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/fluent/bases.py
+-rw-r--r--   0        0        0      771 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/form.py
+-rw-r--r--   0        0        0     3795 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/ifields.py
+-rw-r--r--   0        0        0      922 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/md/__init__.py
+-rw-r--r--   0        0        0    10945 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/md/bases.py
+-rw-r--r--   0        0        0      774 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/shoelace/__init__.py
+-rw-r--r--   0        0        0     8489 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/shoelace/bases.py
+-rw-r--r--   0        0        0     9619 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/splitters.py
+-rw-r--r--   0        0        0     1441 2024-05-01 15:30:00.156963 htagui-0.5.7/htagui/tabs.py
+-rw-r--r--   0        0        0     1069 2024-05-01 15:30:00.416965 htagui-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     9738 1970-01-01 00:00:00.000000 htagui-0.5.7/PKG-INFO
```

### Comparing `htagui-0.5.6/LICENSE` & `htagui-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/README.md` & `htagui-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/all.py` & `htagui-0.5.7/htagui/all.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/basics/__init__.py` & `htagui-0.5.7/htagui/basics/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/basics/bases.py` & `htagui-0.5.7/htagui/basics/bases.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/bulma/__init__.py` & `htagui-0.5.7/htagui/bulma/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/bulma/bases.py` & `htagui-0.5.7/htagui/bulma/bases.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/common.py` & `htagui-0.5.7/htagui/common.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/dialog.py` & `htagui-0.5.7/htagui/dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,22 +24,15 @@
         parent += self  # auto add
         parent += self._toasts  # add a personnal place for toasts
         parent += self._page  # add a personnal place for page
         parent += self._pop  
         MetaTag.init(self)
 
     def clipboard_copy(self,txt:str):
-        self.call(f"""
-let ta = document.createElement('textarea');
-ta.value = `{txt}`;
-self.appendChild(ta);
-ta.select();
-document.execCommand('copy');
-self.removeChild(ta);
-""")
+        self.call(f"""navigator.clipboard.writeText(`{txt}`);""")
 
     def alert(self,obj,size:float=None):
         """if no size is provided : use the default width size of the dialog (depending of ui used)"""
         self.step( alert = obj, size=size )
 
     def confirm(self,obj,cbresponse=lambda bool:bool):
         self.step( confirm = obj, cb=cbresponse )
```

### Comparing `htagui-0.5.6/htagui/fileupload.py` & `htagui-0.5.7/htagui/fileupload.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/flex.py` & `htagui-0.5.7/htagui/flex.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/fluent/__init__.py` & `htagui-0.5.7/htagui/fluent/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/fluent/bases.py` & `htagui-0.5.7/htagui/fluent/bases.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/form.py` & `htagui-0.5.7/htagui/form.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/ifields.py` & `htagui-0.5.7/htagui/ifields.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/md/__init__.py` & `htagui-0.5.7/htagui/md/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/md/bases.py` & `htagui-0.5.7/htagui/md/bases.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/shoelace/__init__.py` & `htagui-0.5.7/htagui/shoelace/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/shoelace/bases.py` & `htagui-0.5.7/htagui/shoelace/bases.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/splitters.py` & `htagui-0.5.7/htagui/splitters.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/htagui/tabs.py` & `htagui-0.5.7/htagui/tabs.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.6/pyproject.toml` & `htagui-0.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagui"
-version = "0.5.6" # auto-updated
+version = "0.5.7" # auto-updated
 description = "GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','gui', 'electron', "cef", "asyncio", "guy", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript"]
 homepage = "https://github.com/manatlan/htagui"
 repository = "https://github.com/manatlan/htagui"
```

### Comparing `htagui-0.5.6/PKG-INFO` & `htagui-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagui
-Version: 0.5.6
+Version: 0.5.7
 Summary: GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase
 Home-page: https://github.com/manatlan/htagui
 License: MIT
 Keywords: htag,gui,electron,cef,asyncio,guy,desktop,web,mobile,http,websocket,html,pyscript
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
```

