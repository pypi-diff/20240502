# Comparing `tmp/aiounifi-8.tar.gz` & `tmp/aiounifi-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiounifi-8.tar", last modified: Mon Jul 29 22:20:04 2019, max compression
+gzip compressed data, was "dist/aiounifi-9.tar", last modified: Thu Aug  1 10:04:50 2019, max compression
```

## Comparing `aiounifi-8.tar` & `aiounifi-9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 r          (501) staff       (20)        0 2019-07-29 22:20:04.000000 aiounifi-8/
--rw-r--r--   0 r          (501) staff       (20)      488 2019-07-29 22:20:04.000000 aiounifi-8/PKG-INFO
--rw-r--r--   0 r          (501) staff       (20)      189 2018-09-30 20:48:03.000000 aiounifi-8/README.md
-drwxr-xr-x   0 r          (501) staff       (20)        0 2019-07-29 22:20:04.000000 aiounifi-8/aiounifi/
--rw-r--r--   0 r          (501) staff       (20)       57 2018-09-30 20:47:50.000000 aiounifi-8/aiounifi/__init__.py
--rw-r--r--   0 r          (501) staff       (20)     1086 2019-06-01 21:45:47.000000 aiounifi-8/aiounifi/api.py
--rw-r--r--   0 r          (501) staff       (20)     2905 2019-07-29 22:18:51.000000 aiounifi-8/aiounifi/clients.py
--rw-r--r--   0 r          (501) staff       (20)     2567 2019-07-25 15:14:17.000000 aiounifi-8/aiounifi/controller.py
--rw-r--r--   0 r          (501) staff       (20)     5151 2019-07-29 22:18:51.000000 aiounifi-8/aiounifi/devices.py
--rw-r--r--   0 r          (501) staff       (20)      790 2018-09-30 20:47:50.000000 aiounifi-8/aiounifi/errors.py
-drwxr-xr-x   0 r          (501) staff       (20)        0 2019-07-29 22:20:04.000000 aiounifi-8/aiounifi.egg-info/
--rw-r--r--   0 r          (501) staff       (20)      488 2019-07-29 22:20:03.000000 aiounifi-8/aiounifi.egg-info/PKG-INFO
--rw-r--r--   0 r          (501) staff       (20)      296 2019-07-29 22:20:03.000000 aiounifi-8/aiounifi.egg-info/SOURCES.txt
--rw-r--r--   0 r          (501) staff       (20)        1 2019-07-29 22:20:03.000000 aiounifi-8/aiounifi.egg-info/dependency_links.txt
--rw-r--r--   0 r          (501) staff       (20)        8 2019-07-29 22:20:03.000000 aiounifi-8/aiounifi.egg-info/requires.txt
--rw-r--r--   0 r          (501) staff       (20)        9 2019-07-29 22:20:03.000000 aiounifi-8/aiounifi.egg-info/top_level.txt
--rw-r--r--   0 r          (501) staff       (20)       38 2019-07-29 22:20:04.000000 aiounifi-8/setup.cfg
--rw-r--r--   0 r          (501) staff       (20)      962 2019-07-29 22:19:09.000000 aiounifi-8/setup.py
+drwxr-xr-x   0 r          (501) staff       (20)        0 2019-08-01 10:04:50.000000 aiounifi-9/
+-rw-r--r--   0 r          (501) staff       (20)      488 2019-08-01 10:04:50.000000 aiounifi-9/PKG-INFO
+-rw-r--r--   0 r          (501) staff       (20)      189 2018-09-30 20:48:03.000000 aiounifi-9/README.md
+drwxr-xr-x   0 r          (501) staff       (20)        0 2019-08-01 10:04:50.000000 aiounifi-9/aiounifi/
+-rw-r--r--   0 r          (501) staff       (20)       57 2018-09-30 20:47:50.000000 aiounifi-9/aiounifi/__init__.py
+-rw-r--r--   0 r          (501) staff       (20)     1086 2019-06-01 21:45:47.000000 aiounifi-9/aiounifi/api.py
+-rw-r--r--   0 r          (501) staff       (20)     2905 2019-07-29 22:18:51.000000 aiounifi-9/aiounifi/clients.py
+-rw-r--r--   0 r          (501) staff       (20)     2686 2019-08-01 10:02:48.000000 aiounifi-9/aiounifi/controller.py
+-rw-r--r--   0 r          (501) staff       (20)     5248 2019-08-01 10:02:48.000000 aiounifi-9/aiounifi/devices.py
+-rw-r--r--   0 r          (501) staff       (20)      790 2018-09-30 20:47:50.000000 aiounifi-9/aiounifi/errors.py
+-rw-r--r--   0 r          (501) staff       (20)     3865 2019-07-30 21:43:56.000000 aiounifi-9/aiounifi/wlan.py
+drwxr-xr-x   0 r          (501) staff       (20)        0 2019-08-01 10:04:50.000000 aiounifi-9/aiounifi.egg-info/
+-rw-r--r--   0 r          (501) staff       (20)      488 2019-08-01 10:04:49.000000 aiounifi-9/aiounifi.egg-info/PKG-INFO
+-rw-r--r--   0 r          (501) staff       (20)      313 2019-08-01 10:04:49.000000 aiounifi-9/aiounifi.egg-info/SOURCES.txt
+-rw-r--r--   0 r          (501) staff       (20)        1 2019-08-01 10:04:49.000000 aiounifi-9/aiounifi.egg-info/dependency_links.txt
+-rw-r--r--   0 r          (501) staff       (20)        8 2019-08-01 10:04:49.000000 aiounifi-9/aiounifi.egg-info/requires.txt
+-rw-r--r--   0 r          (501) staff       (20)        9 2019-08-01 10:04:49.000000 aiounifi-9/aiounifi.egg-info/top_level.txt
+-rw-r--r--   0 r          (501) staff       (20)       38 2019-08-01 10:04:50.000000 aiounifi-9/setup.cfg
+-rw-r--r--   0 r          (501) staff       (20)      962 2019-08-01 10:04:03.000000 aiounifi-9/setup.py
```

### Comparing `aiounifi-8/aiounifi/api.py` & `aiounifi-9/aiounifi/api.py`

 * *Files identical despite different names*

### Comparing `aiounifi-8/aiounifi/clients.py` & `aiounifi-9/aiounifi/clients.py`

 * *Files identical despite different names*

### Comparing `aiounifi-8/aiounifi/controller.py` & `aiounifi-9/aiounifi/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 """Unifi implementation."""
 
+import logging
+
+from pprint import pformat
+
 from aiohttp import client_exceptions
 
 from .clients import (Clients, URL as client_url,
                       ClientsAll, URL_ALL as all_client_url)
 from .devices import Devices, URL as device_url
 from .errors import raise_error, ResponseError, RequestError
 
+LOGGER = logging.getLogger(__name__)
+
 
 class Controller:
     """Control a UniFi controller."""
 
     def __init__(self, host, websession, *,
                  username, password, port=8443, site='default',
                  sslcontext=None):
@@ -34,14 +40,15 @@
             'remember': True,
         }
         await self.request('post', url, json=auth)
 
     async def sites(self):
         url = 'self/sites'
         sites = await self.request('get', url)
+        LOGGER.debug(pformat(sites))
         return {site['desc']: site for site in sites}
 
     async def initialize(self):
         clients = await self.request('get', client_url)
         self.clients = Clients(clients, self.request)
         devices = await self.request('get', device_url)
         self.devices = Devices(devices, self.request)
```

### Comparing `aiounifi-8/aiounifi/devices.py` & `aiounifi-9/aiounifi/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,73 +33,77 @@
 
     @raw.setter
     def raw(self, raw):
         self._raw = raw
         self.ports.update(raw.get('port_table', []))
 
     @property
+    def board_rev(self):
+        return self.raw['board_rev']
+
+    @property
+    def disabled(self):
+        return self.raw.get('disabled', False)
+
+    @property
     def id(self):
         return self.raw['device_id']
 
     @property
     def ip(self):
         return self.raw['ip']
 
     @property
-    def mac(self):
-        return self.raw['mac']
+    def fan_level(self):
+        return self.raw.get('fan_level')
 
     @property
-    def type(self):
-        return self.raw['type']
+    def has_fan(self):
+        return self.raw.get('has_fan', False)
 
     @property
     def last_seen(self):
-        return self.raw['last_seen']
-
-    @property
-    def board_rev(self):
-        return self.raw['board_rev']
+        return self.raw.get('last_seen')
 
     @property
-    def has_fan(self):
-        return self.raw.get('has_fan')
-
-    @property
-    def fan_level(self):
-        return self.raw.get('fan_level')
+    def mac(self):
+        return self.raw['mac']
 
     @property
     def model(self):
         return self.raw['model']
 
     @property
     def name(self):
         return self.raw['name']
 
     @property
-    def version(self):
-        return self.raw['version']
-
-    @property
     def overheating(self):
         return self.raw.get('overheating')
 
     @property
-    def upgradable(self):
-        return self.raw['upgradable']
-
-    @property
     def port_overrides(self):
         return self.raw['port_overrides']
 
     @property
     def port_table(self):
         return self.raw.get('port_table', [])
 
+    @property
+    def type(self):
+        return self.raw['type']
+
+    @property
+    def version(self):
+        return self.raw['version']
+
+    @property
+    def upgradable(self):
+        return self.raw['upgradable']
+
     async def async_set_port_poe_mode(self, port_idx, mode):
         """Set port poe mode.
 
         Auto, 24v, passthrough, off.
         Make sure to not overwrite any existing configs.
         """
         LOGGER.debug("Override port %d with mode %s", port_idx, mode)
```

### Comparing `aiounifi-8/aiounifi/errors.py` & `aiounifi-9/aiounifi/errors.py`

 * *Files identical despite different names*

### Comparing `aiounifi-8/setup.py` & `aiounifi-9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 # twine upload dist/aiounifi-* --skip-existing
 
 from setuptools import setup
 
 setup(
     name='aiounifi',
     packages=['aiounifi'],
-    version='8',
+    version='9',
     description='An asynchronous Python library for communicating with Unifi Controller API',
     author='Robert Svensson',
     author_email='Kane610@users.noreply.github.com',
     license='MIT',
     url='https://github.com/Kane610/aiounifi',
-    download_url='https://github.com/Kane610/aiounifi/archive/v8.tar.gz',
+    download_url='https://github.com/Kane610/aiounifi/archive/v9.tar.gz',
     install_requires=['aiohttp'],
     keywords=['unifi', 'homeassistant'],
     classifiers=[
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
     ],
 )
```

