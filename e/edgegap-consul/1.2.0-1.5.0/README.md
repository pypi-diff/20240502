# Comparing `tmp/edgegap_consul-1.2.0.tar.gz` & `tmp/edgegap_consul-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_consul-1.2.0.tar", max compression
+gzip compressed data, was "edgegap_consul-1.5.0.tar", max compression
```

## Comparing `edgegap_consul-1.2.0.tar` & `edgegap_consul-1.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1993 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/LICENSE
--rw-r--r--   0        0        0     2152 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/README.md
--rw-r--r--   0        0        0       17 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/edgegap_consul/BUILD
--rw-r--r--   0        0        0      341 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/edgegap_consul/__init__.py
--rw-r--r--   0        0        0     2257 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/edgegap_consul/_client.py
--rw-r--r--   0        0        0      399 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/edgegap_consul/_configuration.py
--rw-r--r--   0        0        0     1298 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/edgegap_consul/_factory.py
--rw-r--r--   0        0        0     1623 2024-05-01 17:52:18.959014 edgegap_consul-1.2.0/edgegap_consul/_reader.py
--rw-r--r--   0        0        0      720 2024-05-01 17:52:31.791329 edgegap_consul-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 edgegap_consul-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-02 18:20:19.987672 edgegap_consul-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2152 2024-05-02 18:20:19.987672 edgegap_consul-1.5.0/README.md
+-rw-r--r--   0        0        0       17 2024-05-02 18:20:19.987672 edgegap_consul-1.5.0/edgegap_consul/BUILD
+-rw-r--r--   0        0        0      341 2024-05-02 18:20:19.987672 edgegap_consul-1.5.0/edgegap_consul/__init__.py
+-rw-r--r--   0        0        0     2257 2024-05-02 18:20:19.987672 edgegap_consul-1.5.0/edgegap_consul/_client.py
+-rw-r--r--   0        0        0      399 2024-05-02 18:20:19.987672 edgegap_consul-1.5.0/edgegap_consul/_configuration.py
+-rw-r--r--   0        0        0     1325 2024-05-02 18:20:19.987672 edgegap_consul-1.5.0/edgegap_consul/_factory.py
+-rw-r--r--   0        0        0     1623 2024-05-02 18:20:19.987672 edgegap_consul-1.5.0/edgegap_consul/_reader.py
+-rw-r--r--   0        0        0      720 2024-05-02 18:20:44.464294 edgegap_consul-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 edgegap_consul-1.5.0/PKG-INFO
```

### Comparing `edgegap_consul-1.2.0/LICENSE` & `edgegap_consul-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.2.0/README.md` & `edgegap_consul-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.2.0/edgegap_consul/_client.py` & `edgegap_consul-1.5.0/edgegap_consul/_client.py`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.2.0/edgegap_consul/_factory.py` & `edgegap_consul-1.5.0/edgegap_consul/_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class ConsulReaderFactory:
     __consul_pattern__ = r'\[h=(?P<host>[^\]]*),t=(?P<token>[^\]]*)\]'
 
     def __parse_old_syntax(self) -> ConsulConfiguration | None:
         consul_values = os.environ.get('CONSUL', '[h=localhost,t=None]')
 
-        if isinstance(consul_values, str):
+        if isinstance(consul_values, str) and len(consul_values) > 0:
             match = re.match(self.__consul_pattern__, consul_values)
 
             if match:
                 host = match.group('host')
                 token = match.group('token')
 
                 return ConsulConfiguration(host=host, token=token)
```

### Comparing `edgegap_consul-1.2.0/edgegap_consul/_reader.py` & `edgegap_consul-1.5.0/edgegap_consul/_reader.py`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.2.0/pyproject.toml` & `edgegap_consul-1.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-consul"
-version = "1.2.0"
+version = "1.5.0"
 description = "The Edgegap Consul library includes various tools and helpers for interacting with Consul. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = { version = "^3.9.5", extras = ["speedups"] }
```

### Comparing `edgegap_consul-1.2.0/PKG-INFO` & `edgegap_consul-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-consul
-Version: 1.2.0
+Version: 1.5.0
 Summary: The Edgegap Consul library includes various tools and helpers for interacting with Consul. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

