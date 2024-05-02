# Comparing `tmp/snitun-0.8.tar.gz` & `tmp/snitun-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/snitun-0.8.tar", last modified: Fri Mar  1 21:22:08 2019, max compression
+gzip compressed data, was "dist/snitun-0.9.tar", last modified: Fri Mar  1 21:53:39 2019, max compression
```

## Comparing `snitun-0.8.tar` & `snitun-0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-01 21:22:08.000000 snitun-0.8/
--rw-r--r--   0 root         (0) root         (0)      880 2019-03-01 21:22:08.000000 snitun-0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2940 2019-02-06 09:26:00.000000 snitun-0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      396 2019-03-01 21:22:08.000000 snitun-0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1300 2019-03-01 21:22:04.000000 snitun-0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-01 21:22:08.000000 snitun-0.8/snitun/
--rw-r--r--   0 root         (0) root         (0)       44 2019-02-06 09:26:00.000000 snitun-0.8/snitun/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-01 21:22:08.000000 snitun-0.8/snitun/client/
--rw-r--r--   0 root         (0) root         (0)       29 2019-02-06 09:26:00.000000 snitun-0.8/snitun/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3198 2019-03-01 21:22:04.000000 snitun-0.8/snitun/client/client_peer.py
--rw-r--r--   0 root         (0) root         (0)     3706 2019-02-06 09:26:00.000000 snitun-0.8/snitun/client/connector.py
--rw-r--r--   0 root         (0) root         (0)      754 2019-02-06 09:26:00.000000 snitun-0.8/snitun/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-01 21:22:08.000000 snitun-0.8/snitun/multiplexer/
--rw-r--r--   0 root         (0) root         (0)       30 2019-02-06 09:26:00.000000 snitun-0.8/snitun/multiplexer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2676 2019-03-01 12:58:32.000000 snitun-0.8/snitun/multiplexer/channel.py
--rw-r--r--   0 root         (0) root         (0)     8234 2019-03-01 21:22:04.000000 snitun-0.8/snitun/multiplexer/core.py
--rw-r--r--   0 root         (0) root         (0)     1018 2019-02-06 09:26:00.000000 snitun-0.8/snitun/multiplexer/crypto.py
--rw-r--r--   0 root         (0) root         (0)      573 2019-02-06 09:26:00.000000 snitun-0.8/snitun/multiplexer/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-01 21:22:08.000000 snitun-0.8/snitun/server/
--rw-r--r--   0 root         (0) root         (0)       29 2019-02-06 09:26:00.000000 snitun-0.8/snitun/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2245 2019-02-22 09:17:57.000000 snitun-0.8/snitun/server/listener_peer.py
--rw-r--r--   0 root         (0) root         (0)     4946 2019-02-22 09:17:57.000000 snitun-0.8/snitun/server/listener_sni.py
--rw-r--r--   0 root         (0) root         (0)     2209 2019-03-01 21:22:04.000000 snitun-0.8/snitun/server/peer.py
--rw-r--r--   0 root         (0) root         (0)     1936 2019-02-06 09:26:00.000000 snitun-0.8/snitun/server/peer_manager.py
--rw-r--r--   0 root         (0) root         (0)     2937 2019-02-22 09:17:57.000000 snitun-0.8/snitun/server/run.py
--rw-r--r--   0 root         (0) root         (0)     3391 2019-02-06 09:26:00.000000 snitun-0.8/snitun/server/sni.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-01 21:22:08.000000 snitun-0.8/snitun/utils/
--rw-r--r--   0 root         (0) root         (0)       44 2019-02-06 09:26:00.000000 snitun-0.8/snitun/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      192 2019-02-06 09:26:00.000000 snitun-0.8/snitun/utils/aes.py
--rw-r--r--   0 root         (0) root         (0)     2694 2019-03-01 21:22:04.000000 snitun-0.8/snitun/utils/aiohttp_client.py
--rw-r--r--   0 root         (0) root         (0)      573 2019-02-06 09:26:00.000000 snitun-0.8/snitun/utils/ipaddress.py
--rw-r--r--   0 root         (0) root         (0)      666 2019-02-06 09:26:00.000000 snitun-0.8/snitun/utils/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-01 21:22:08.000000 snitun-0.8/snitun.egg-info/
--rw-r--r--   0 root         (0) root         (0)      880 2019-03-01 21:22:08.000000 snitun-0.8/snitun.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      781 2019-03-01 21:22:08.000000 snitun-0.8/snitun.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-03-01 21:22:08.000000 snitun-0.8/snitun.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-03-01 21:22:08.000000 snitun-0.8/snitun.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       53 2019-03-01 21:22:08.000000 snitun-0.8/snitun.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2019-03-01 21:22:08.000000 snitun-0.8/snitun.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-01 21:53:39.000000 snitun-0.9/
+-rw-r--r--   0 root         (0) root         (0)      880 2019-03-01 21:53:39.000000 snitun-0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2940 2019-02-06 09:26:00.000000 snitun-0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      396 2019-03-01 21:53:39.000000 snitun-0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1300 2019-03-01 21:53:33.000000 snitun-0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-01 21:53:39.000000 snitun-0.9/snitun/
+-rw-r--r--   0 root         (0) root         (0)       44 2019-02-06 09:26:00.000000 snitun-0.9/snitun/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-01 21:53:39.000000 snitun-0.9/snitun/client/
+-rw-r--r--   0 root         (0) root         (0)       29 2019-02-06 09:26:00.000000 snitun-0.9/snitun/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2019-03-01 21:22:04.000000 snitun-0.9/snitun/client/client_peer.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2019-02-06 09:26:00.000000 snitun-0.9/snitun/client/connector.py
+-rw-r--r--   0 root         (0) root         (0)      754 2019-02-06 09:26:00.000000 snitun-0.9/snitun/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-01 21:53:39.000000 snitun-0.9/snitun/multiplexer/
+-rw-r--r--   0 root         (0) root         (0)       30 2019-02-06 09:26:00.000000 snitun-0.9/snitun/multiplexer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2676 2019-03-01 12:58:32.000000 snitun-0.9/snitun/multiplexer/channel.py
+-rw-r--r--   0 root         (0) root         (0)     8250 2019-03-01 21:53:33.000000 snitun-0.9/snitun/multiplexer/core.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2019-02-06 09:26:00.000000 snitun-0.9/snitun/multiplexer/crypto.py
+-rw-r--r--   0 root         (0) root         (0)      573 2019-02-06 09:26:00.000000 snitun-0.9/snitun/multiplexer/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-01 21:53:39.000000 snitun-0.9/snitun/server/
+-rw-r--r--   0 root         (0) root         (0)       29 2019-02-06 09:26:00.000000 snitun-0.9/snitun/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2019-02-22 09:17:57.000000 snitun-0.9/snitun/server/listener_peer.py
+-rw-r--r--   0 root         (0) root         (0)     4946 2019-02-22 09:17:57.000000 snitun-0.9/snitun/server/listener_sni.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2019-03-01 21:22:04.000000 snitun-0.9/snitun/server/peer.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2019-02-06 09:26:00.000000 snitun-0.9/snitun/server/peer_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2937 2019-02-22 09:17:57.000000 snitun-0.9/snitun/server/run.py
+-rw-r--r--   0 root         (0) root         (0)     3391 2019-02-06 09:26:00.000000 snitun-0.9/snitun/server/sni.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-01 21:53:39.000000 snitun-0.9/snitun/utils/
+-rw-r--r--   0 root         (0) root         (0)       44 2019-02-06 09:26:00.000000 snitun-0.9/snitun/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      192 2019-02-06 09:26:00.000000 snitun-0.9/snitun/utils/aes.py
+-rw-r--r--   0 root         (0) root         (0)     2694 2019-03-01 21:22:04.000000 snitun-0.9/snitun/utils/aiohttp_client.py
+-rw-r--r--   0 root         (0) root         (0)      573 2019-02-06 09:26:00.000000 snitun-0.9/snitun/utils/ipaddress.py
+-rw-r--r--   0 root         (0) root         (0)      666 2019-02-06 09:26:00.000000 snitun-0.9/snitun/utils/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-01 21:53:39.000000 snitun-0.9/snitun.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      880 2019-03-01 21:53:39.000000 snitun-0.9/snitun.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      781 2019-03-01 21:53:39.000000 snitun-0.9/snitun.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-03-01 21:53:39.000000 snitun-0.9/snitun.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-03-01 21:53:39.000000 snitun-0.9/snitun.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       53 2019-03-01 21:53:39.000000 snitun-0.9/snitun.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2019-03-01 21:53:39.000000 snitun-0.9/snitun.egg-info/top_level.txt
```

### Comparing `snitun-0.8/PKG-INFO` & `snitun-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: snitun
-Version: 0.8
+Version: 0.9
 Summary: SNI proxy with TCP multiplexer
 Home-page: https://www.nabucasa.com/
 Author: Nabu Casa, Inc.
 Author-email: opensource@nabucasa.com
 License: GPL v3
-Download-URL: https://github.com/NabuCasa/snitun/tarball/0.8
+Download-URL: https://github.com/NabuCasa/snitun/tarball/0.9
 Description: UNKNOWN
 Keywords: sni,proxy,multiplexer,tls
 Platform: any
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `snitun-0.8/README.md` & `snitun-0.9/README.md`

 * *Files identical despite different names*

### Comparing `snitun-0.8/setup.py` & `snitun-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.8"
+VERSION = "0.9"
 
 setup(
     name="snitun",
     version=VERSION,
     license="GPL v3",
     author="Nabu Casa, Inc.",
     author_email="opensource@nabucasa.com",
```

### Comparing `snitun-0.8/snitun/client/client_peer.py` & `snitun-0.9/snitun/client/client_peer.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun/client/connector.py` & `snitun-0.9/snitun/client/connector.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun/exceptions.py` & `snitun-0.9/snitun/exceptions.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun/multiplexer/channel.py` & `snitun-0.9/snitun/multiplexer/channel.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun/multiplexer/core.py` & `snitun-0.9/snitun/multiplexer/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         return not self._processing_task.done()
 
     def wait(self) -> asyncio.Task:
         """Block until the connection is closed.
 
         Return a awaitable object.
         """
-        return self._processing_task
+        return asyncio.shield(self._processing_task)
 
     async def shutdown(self):
         """Shutdown connection."""
         if self._processing_task.done():
             return
 
         _LOGGER.debug("Cancel connection")
```

### Comparing `snitun-0.8/snitun/multiplexer/crypto.py` & `snitun-0.9/snitun/multiplexer/crypto.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun/multiplexer/message.py` & `snitun-0.9/snitun/multiplexer/message.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun/server/listener_peer.py` & `snitun-0.9/snitun/server/listener_peer.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun/server/listener_sni.py` & `snitun-0.9/snitun/server/listener_sni.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun/server/peer.py` & `snitun-0.9/snitun/server/peer.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun/server/peer_manager.py` & `snitun-0.9/snitun/server/peer_manager.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun/server/run.py` & `snitun-0.9/snitun/server/run.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun/server/sni.py` & `snitun-0.9/snitun/server/sni.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun/utils/aiohttp_client.py` & `snitun-0.9/snitun/utils/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun/utils/ipaddress.py` & `snitun-0.9/snitun/utils/ipaddress.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun/utils/server.py` & `snitun-0.9/snitun/utils/server.py`

 * *Files identical despite different names*

### Comparing `snitun-0.8/snitun.egg-info/PKG-INFO` & `snitun-0.9/snitun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: snitun
-Version: 0.8
+Version: 0.9
 Summary: SNI proxy with TCP multiplexer
 Home-page: https://www.nabucasa.com/
 Author: Nabu Casa, Inc.
 Author-email: opensource@nabucasa.com
 License: GPL v3
-Download-URL: https://github.com/NabuCasa/snitun/tarball/0.8
+Download-URL: https://github.com/NabuCasa/snitun/tarball/0.9
 Description: UNKNOWN
 Keywords: sni,proxy,multiplexer,tls
 Platform: any
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `snitun-0.8/snitun.egg-info/SOURCES.txt` & `snitun-0.9/snitun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

