# Comparing `tmp/netlink-keepass-0.6.1.tar.gz` & `tmp/netlink-keepass-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netlink-keepass-0.6.1.tar", max compression
+gzip compressed data, was "netlink-keepass-0.6.2.tar", max compression
```

## Comparing `netlink-keepass-0.6.1.tar` & `netlink-keepass-0.6.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      112 2024-02-08 14:32:57.009088 netlink-keepass-0.6.1/netlink/keepass/__init__.py
--rw-r--r--   0        0        0     2719 2024-02-12 15:57:54.991537 netlink-keepass-0.6.1/netlink/keepass/cli.py
--rw-r--r--   0        0        0     1927 2024-05-02 13:59:44.325484 netlink-keepass-0.6.1/netlink/keepass/keepass.py
--rw-r--r--   0        0        0     1384 2024-04-03 08:47:59.396914 netlink-keepass-0.6.1/netlink/keepass/reader.py
--rw-r--r--   0        0        0     1019 2024-02-12 15:32:48.939329 netlink-keepass-0.6.1/netlink/keepass/util.py
--rw-r--r--   0        0        0      971 2024-05-02 13:55:41.077317 netlink-keepass-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1290 2024-05-02 14:04:05.942252 netlink-keepass-0.6.1/setup.py
--rw-r--r--   0        0        0      684 2024-05-02 14:04:05.942252 netlink-keepass-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      112 2024-02-08 14:32:57.009088 netlink-keepass-0.6.2/netlink/keepass/__init__.py
+-rw-r--r--   0        0        0     2719 2024-02-12 15:57:54.991537 netlink-keepass-0.6.2/netlink/keepass/cli.py
+-rw-r--r--   0        0        0     1867 2024-05-02 14:29:00.328439 netlink-keepass-0.6.2/netlink/keepass/keepass.py
+-rw-r--r--   0        0        0     1415 2024-05-02 14:26:46.739110 netlink-keepass-0.6.2/netlink/keepass/reader.py
+-rw-r--r--   0        0        0     1019 2024-02-12 15:32:48.939329 netlink-keepass-0.6.2/netlink/keepass/util.py
+-rw-r--r--   0        0        0      971 2024-05-02 14:29:06.929473 netlink-keepass-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1290 2024-05-02 14:29:14.665671 netlink-keepass-0.6.2/setup.py
+-rw-r--r--   0        0        0      684 2024-05-02 14:29:14.665671 netlink-keepass-0.6.2/PKG-INFO
```

### Comparing `netlink-keepass-0.6.1/netlink/keepass/cli.py` & `netlink-keepass-0.6.2/netlink/keepass/cli.py`

 * *Files identical despite different names*

### Comparing `netlink-keepass-0.6.1/netlink/keepass/keepass.py` & `netlink-keepass-0.6.2/netlink/keepass/keepass.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pykeepass import PyKeePass
 from pykeepass.entry import reserved_keys
 
 reserved_keys = set(
     [i.lower() for i in reserved_keys if i not in ("History", "IconID", "Times", "otp")]
 )
 
-URL_RE = re.compile(r"\{.+?\}")
+URL_RE = re.compile(r"\{.+?}")
 
 
 class KeePass(PyKeePass):
     def __init__(
             self,
             filename: pathlib.Path,
             secret: str,
@@ -25,30 +25,27 @@
             with token.open("rb") as f:
                 token_data = f.read()
             password = Fernet(secret.encode()).decrypt(token_data).decode()
         else:
             password = secret
         super().__init__(filename=filename, password=password, keyfile=keyfile)
 
-    def get(self, path: Union[str, List[str]]) -> Dict[str, str]:
+    def get(self, path: Union[str, List[str]], property: Union[str, None] = None) -> Union[str, Dict[str, str]]:
         """Get Entry as Dict"""
         if isinstance(path, str):
             path = path.strip("/").split("/")
-        query = ''
-        if '?' in path[-1]:
-            path[-1], query = path[-1].split('?', maxsplit=1)
         entry = self.find_entries(path=path)
         if not entry:
             raise KeyError("/".join(path))
         result = {k: getattr(entry, k) for k in reserved_keys}
         result.update(entry.custom_properties)
         for k in result:    # resolve internal refs
             if result[k] and result[k].startswith('{REF:'):
                 result[k] = entry.deref(k)
         if result['url']:
             for m in URL_RE.finditer(result['url']):
                 var = m.group()[3:-1] if m.group().startswith('{S:') else m.group()[1:-1].lower()
                 if var in result:
                     result['url'] = result['url'].replace(m.group(), result[var])
-        if query:
-            return result[query]
+        if property:
+            return result[property]
         return result
```

### Comparing `netlink-keepass-0.6.1/netlink/keepass/reader.py` & `netlink-keepass-0.6.2/netlink/keepass/reader.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 from netlink.keepass.keepass import KeePass
 
 app = fastapi.FastAPI()
 
 
 # noinspection PyUnresolvedReferences
 @app.get("/{full_path:path}")
-async def get_value(full_path: str):
+async def get_value(full_path: str, p: Union[str, None] = None):
     if full_path.startswith(app.state.shutdown):
         os.kill(os.getpid(), signal.SIGTERM)
         return fastapi.Response(status_code=200, content="Server shutting down...")
     try:
-        return app.state.kp.get(full_path)
+        return app.state.kp.get(full_path, p)
     except KeyError:
         raise fastapi.HTTPException(status_code=404, detail=f"{full_path} not found")
 
 
 # noinspection PyUnresolvedReferences
 def reader(
         filename: pathlib.Path,
```

### Comparing `netlink-keepass-0.6.1/netlink/keepass/util.py` & `netlink-keepass-0.6.2/netlink/keepass/util.py`

 * *Files identical despite different names*

### Comparing `netlink-keepass-0.6.1/pyproject.toml` & `netlink-keepass-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netlink-keepass"
-version = "0.6.1"
+version = "0.6.2"
 description = "Tools to work with (Py)KeePass"
 authors = ["Bernhard Radermacher <bernhard.radermacher@netlink-consulting.com>"]
 repository = "https://gitlab.com/netlink_python/netlink-keepass.git"
 packages = [ { include = "netlink/keepass" } ]
 
 [tool.poetry.scripts]
 netlink-keepass-rest-reader = 'netlink.keepass.cli:reader_cli'
```

### Comparing `netlink-keepass-0.6.1/setup.py` & `netlink-keepass-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                      'netlink-keepass-rest-reader = '
                      'netlink.keepass.cli:reader_cli',
                      'netlink-keepass-rest-shutdown = '
                      'netlink.keepass.cli:rest_shutdown_cli']}
 
 setup_kwargs = {
     'name': 'netlink-keepass',
-    'version': '0.6.1',
+    'version': '0.6.2',
     'description': 'Tools to work with (Py)KeePass',
     'long_description': None,
     'author': 'Bernhard Radermacher',
     'author_email': 'bernhard.radermacher@netlink-consulting.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/netlink_python/netlink-keepass.git',
```

### Comparing `netlink-keepass-0.6.1/PKG-INFO` & `netlink-keepass-0.6.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netlink-keepass
-Version: 0.6.1
+Version: 0.6.2
 Summary: Tools to work with (Py)KeePass
 Home-page: https://gitlab.com/netlink_python/netlink-keepass.git
 Author: Bernhard Radermacher
 Author-email: bernhard.radermacher@netlink-consulting.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

