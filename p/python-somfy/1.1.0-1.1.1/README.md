# Comparing `tmp/python_somfy-1.1.0.tar.gz` & `tmp/python_somfy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_somfy-1.1.0.tar", last modified: Fri Apr 26 04:05:13 2024, max compression
+gzip compressed data, was "python_somfy-1.1.1.tar", last modified: Wed May  1 04:56:42 2024, max compression
```

## Comparing `python_somfy-1.1.0.tar` & `python_somfy-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:05:13.252845 python_somfy-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 04:05:08.000000 python_somfy-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-26 04:05:13.252845 python_somfy-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-26 04:05:08.000000 python_somfy-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 04:05:08.000000 python_somfy-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:05:13.252845 python_somfy-1.1.0/python_somfy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-26 04:05:13.000000 python_somfy-1.1.0/python_somfy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-26 04:05:13.000000 python_somfy-1.1.0/python_somfy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 04:05:13.000000 python_somfy-1.1.0/python_somfy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 04:05:13.000000 python_somfy-1.1.0/python_somfy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-26 04:05:13.000000 python_somfy-1.1.0/python_somfy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 04:05:13.000000 python_somfy-1.1.0/python_somfy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-26 04:05:13.252845 python_somfy-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:05:13.248845 python_somfy-1.1.0/somfy/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16043 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/enumutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    22061 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/payloads.py
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/recognizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-26 04:05:08.000000 python_somfy-1.1.0/somfy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:05:13.252845 python_somfy-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-04-26 04:05:08.000000 python_somfy-1.1.0/tests/test_decoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:56:42.698436 python_somfy-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 04:56:38.000000 python_somfy-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-05-01 04:56:42.698436 python_somfy-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-05-01 04:56:38.000000 python_somfy-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-01 04:56:38.000000 python_somfy-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:56:42.694436 python_somfy-1.1.1/python_somfy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-05-01 04:56:42.000000 python_somfy-1.1.1/python_somfy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-01 04:56:42.000000 python_somfy-1.1.1/python_somfy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 04:56:42.000000 python_somfy-1.1.1/python_somfy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 04:56:42.000000 python_somfy-1.1.1/python_somfy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 04:56:42.000000 python_somfy-1.1.1/python_somfy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 04:56:42.000000 python_somfy-1.1.1/python_somfy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-01 04:56:42.698436 python_somfy-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:56:42.694436 python_somfy-1.1.1/somfy/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-01 04:56:38.000000 python_somfy-1.1.1/somfy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-05-01 04:56:38.000000 python_somfy-1.1.1/somfy/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-01 04:56:38.000000 python_somfy-1.1.1/somfy/enumutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-05-01 04:56:38.000000 python_somfy-1.1.1/somfy/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22061 2024-05-01 04:56:38.000000 python_somfy-1.1.1/somfy/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-01 04:56:38.000000 python_somfy-1.1.1/somfy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-01 04:56:38.000000 python_somfy-1.1.1/somfy/recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-01 04:56:38.000000 python_somfy-1.1.1/somfy/serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-01 04:56:38.000000 python_somfy-1.1.1/somfy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:56:42.694436 python_somfy-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-05-01 04:56:38.000000 python_somfy-1.1.1/tests/test_decoding.py
```

### Comparing `python_somfy-1.1.0/LICENSE` & `python_somfy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_somfy-1.1.0/PKG-INFO` & `python_somfy-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-somfy
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python library for local control of Somfy SDN shades
 Home-page: https://github.com/Cyberax/py-somfy-sdn
 Author: Aleksei Besogonov
 Author-email: b@alex.net
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Cyberax/py-somfy-sdn
 Platform: any
```

### Comparing `python_somfy-1.1.0/README.md` & `python_somfy-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `python_somfy-1.1.0/python_somfy.egg-info/PKG-INFO` & `python_somfy-1.1.1/python_somfy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-somfy
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python library for local control of Somfy SDN shades
 Home-page: https://github.com/Cyberax/py-somfy-sdn
 Author: Aleksei Besogonov
 Author-email: b@alex.net
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Cyberax/py-somfy-sdn
 Platform: any
```

### Comparing `python_somfy-1.1.0/setup.cfg` & `python_somfy-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-somfy
-version = 1.1.0
+version = 1.1.1
 author = Aleksei Besogonov
 author_email = b@alex.net
 description = Python library for local control of Somfy SDN shades
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache-2.0
 platforms = any
```

### Comparing `python_somfy-1.1.0/somfy/connector.py` & `python_somfy-1.1.1/somfy/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,17 +362,20 @@
                         break
                     except OSError:
                         pass
 
     @override
     async def exchange(self, to_send: Optional[SomfyMessage],
                        msg_consumer: Optional[Callable[[SomfyMessage], bool]]) -> bool:
-        async with asyncio.timeout(self.timeout):
-            async with self.lock:
-                return await self.connector.exchange(to_send, msg_consumer)
+        try:
+            async with asyncio.timeout(self.timeout):
+                async with self.lock:
+                    return await self.connector.exchange(to_send, msg_consumer)
+        except asyncio.TimeoutError:
+            return False
 
 
 async def fire_and_forget(conn: SomfyExchanger, to_send: SomfyMessage):
     await conn.exchange(to_send, None)
 
 
 # Attempt to detect Somfy devices on the SDN bus. Always waits for the communication timeout
```

### Comparing `python_somfy-1.1.0/somfy/messages.py` & `python_somfy-1.1.1/somfy/messages.py`

 * *Files identical despite different names*

### Comparing `python_somfy-1.1.0/somfy/payloads.py` & `python_somfy-1.1.1/somfy/payloads.py`

 * *Files identical despite different names*

### Comparing `python_somfy-1.1.0/somfy/recognizer.py` & `python_somfy-1.1.1/somfy/recognizer.py`

 * *Files identical despite different names*

### Comparing `python_somfy-1.1.0/somfy/serial.py` & `python_somfy-1.1.1/somfy/serial.py`

 * *Files identical despite different names*

### Comparing `python_somfy-1.1.0/somfy/utils.py` & `python_somfy-1.1.1/somfy/utils.py`

 * *Files identical despite different names*

### Comparing `python_somfy-1.1.0/tests/test_decoding.py` & `python_somfy-1.1.1/tests/test_decoding.py`

 * *Files identical despite different names*

