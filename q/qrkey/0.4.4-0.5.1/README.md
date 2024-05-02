# Comparing `tmp/qrkey-0.4.4.tar.gz` & `tmp/qrkey-0.5.1.tar.gz`

## Comparing `qrkey-0.4.4.tar` & `qrkey-0.5.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/__about__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/__init__.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/api.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/crypto.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/models.py
--rw-r--r--   0        0        0    10632 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/mqtt.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/settings.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/tests/__init__.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/tests/test_api.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/tests/test_crypto.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/.env
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/.env.test
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/.gitignore
--rw-r--r--   0        0        0  1392895 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/package-lock.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/package.json
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/build/asset-manifest.json
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/build/index.html
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/build/manifest.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/build/robots.txt
--rw-r--r--   0        0        0    84530 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/build/static/css/main.3135d883.css
--rw-r--r--   0        0        0   147020 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/build/static/css/main.3135d883.css.map
--rw-r--r--   0        0        0   192900 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/build/static/js/main.521f7acd.js
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/build/static/js/main.521f7acd.js.LICENSE.txt
--rw-r--r--   0        0        0   553770 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/build/static/js/main.521f7acd.js.map
--rw-r--r--   0        0        0   176032 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/build/static/media/bootstrap-icons.39795c0b4513de014cf8.woff
--rw-r--r--   0        0        0   130396 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/build/static/media/bootstrap-icons.b7bcc075b395c14ce8c2.woff2
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/public/index.html
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/public/manifest.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/public/robots.txt
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/src/PinCode.css
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/src/PinCode.js
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/src/PinCode.test.js
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/src/index.css
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/src/index.js
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 qrkey-0.4.4/qrkey/ui/src/setupTests.js
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 qrkey-0.4.4/utils/hooks/sdist.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 qrkey-0.4.4/utils/hooks/wheel.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 qrkey-0.4.4/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 qrkey-0.4.4/LICENSE.txt
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 qrkey-0.4.4/README.md
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 qrkey-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 qrkey-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/__about__.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/__init__.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/api.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/crypto.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/models.py
+-rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/mqtt.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/settings.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/tests/__init__.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/tests/test_api.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/tests/test_crypto.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/.env
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/.env.test
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/.gitignore
+-rw-r--r--   0        0        0  1392895 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/package-lock.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/package.json
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/build/asset-manifest.json
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/build/index.html
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/build/manifest.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/build/robots.txt
+-rw-r--r--   0        0        0    84530 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/build/static/css/main.3135d883.css
+-rw-r--r--   0        0        0   147020 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/build/static/css/main.3135d883.css.map
+-rw-r--r--   0        0        0   192900 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/build/static/js/main.521f7acd.js
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/build/static/js/main.521f7acd.js.LICENSE.txt
+-rw-r--r--   0        0        0   553770 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/build/static/js/main.521f7acd.js.map
+-rw-r--r--   0        0        0   176032 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/build/static/media/bootstrap-icons.39795c0b4513de014cf8.woff
+-rw-r--r--   0        0        0   130396 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/build/static/media/bootstrap-icons.b7bcc075b395c14ce8c2.woff2
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/public/index.html
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/public/manifest.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/public/robots.txt
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/src/PinCode.css
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/src/PinCode.js
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/src/PinCode.test.js
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/src/index.css
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/src/index.js
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 qrkey-0.5.1/qrkey/ui/src/setupTests.js
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 qrkey-0.5.1/utils/hooks/sdist.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 qrkey-0.5.1/utils/hooks/wheel.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 qrkey-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 qrkey-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 qrkey-0.5.1/README.md
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 qrkey-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 qrkey-0.5.1/PKG-INFO
```

### Comparing `qrkey-0.4.4/qrkey/api.py` & `qrkey-0.5.1/qrkey/api.py`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/crypto.py` & `qrkey-0.5.1/qrkey/crypto.py`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/models.py` & `qrkey-0.5.1/qrkey/models.py`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/mqtt.py` & `qrkey-0.5.1/qrkey/mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,18 @@
             logger.warning('Cannot parse payload as JSON')
             return
         try:
             payload = PayloadModel(**payload)
         except ValidationError as exc:
             logger.warning(f'Invalid payload received: {exc.errors()}')
             return
-        if payload.timestamp < time.time() - 1 or payload.timestamp > time.time() + 1:
+        if (
+            payload.timestamp < time.time() - qrkey_settings.timestamp_tolerance
+            or payload.timestamp > time.time() + qrkey_settings.timestamp_tolerance
+        ):
             logger.warning(
                 f'Invalid payload timestamp {payload.timestamp}, {time.time()}'
             )
             return
         payload = payload.payload
         if sub_topic == '/request':
             self.request_callback(payload)
```

### Comparing `qrkey-0.4.4/qrkey/settings.py` & `qrkey-0.5.1/qrkey/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,9 +29,11 @@
     mqtt_reconnect_retries: Optional[int] = Field(default=3)
     mqtt_reconnect_delay: Optional[int] = Field(default=5)
 
     pin_code_length: int = Field(default=12)
     pin_code_refresh_interval: int = Field(default=15 * 60)  # in seconds
     pin_code_revoke_delay: int = Field(default=2 * 60)  # in seconds
 
+    timestamp_tolerance: int = Field(default=2)  # [-2:2] range in seconds
+
 
 qrkey_settings = QrkeySettings()
```

### Comparing `qrkey-0.4.4/qrkey/tests/test_api.py` & `qrkey-0.5.1/qrkey/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/tests/test_crypto.py` & `qrkey-0.5.1/qrkey/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/ui/package-lock.json` & `qrkey-0.5.1/qrkey/ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/ui/package.json` & `qrkey-0.5.1/qrkey/ui/package.json`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/ui/build/asset-manifest.json` & `qrkey-0.5.1/qrkey/ui/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/ui/build/static/css/main.3135d883.css` & `qrkey-0.5.1/qrkey/ui/build/static/css/main.3135d883.css`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/ui/build/static/css/main.3135d883.css.map` & `qrkey-0.5.1/qrkey/ui/build/static/css/main.3135d883.css.map`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/ui/build/static/js/main.521f7acd.js` & `qrkey-0.5.1/qrkey/ui/build/static/js/main.521f7acd.js`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/ui/build/static/js/main.521f7acd.js.LICENSE.txt` & `qrkey-0.5.1/qrkey/ui/build/static/js/main.521f7acd.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/ui/build/static/js/main.521f7acd.js.map` & `qrkey-0.5.1/qrkey/ui/build/static/js/main.521f7acd.js.map`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/ui/build/static/media/bootstrap-icons.39795c0b4513de014cf8.woff` & `qrkey-0.5.1/qrkey/ui/build/static/media/bootstrap-icons.39795c0b4513de014cf8.woff`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/ui/build/static/media/bootstrap-icons.b7bcc075b395c14ce8c2.woff2` & `qrkey-0.5.1/qrkey/ui/build/static/media/bootstrap-icons.b7bcc075b395c14ce8c2.woff2`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/ui/src/PinCode.css` & `qrkey-0.5.1/qrkey/ui/src/PinCode.css`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/ui/src/PinCode.js` & `qrkey-0.5.1/qrkey/ui/src/PinCode.js`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/ui/src/PinCode.test.js` & `qrkey-0.5.1/qrkey/ui/src/PinCode.test.js`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/qrkey/ui/src/setupTests.js` & `qrkey-0.5.1/qrkey/ui/src/setupTests.js`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/utils/hooks/sdist.py` & `qrkey-0.5.1/utils/hooks/sdist.py`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/utils/hooks/wheel.py` & `qrkey-0.5.1/utils/hooks/wheel.py`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/.gitignore` & `qrkey-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/LICENSE.txt` & `qrkey-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/README.md` & `qrkey-0.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Qrkey
 
 [![PyPI - Version](https://img.shields.io/pypi/v/qrkey.svg)](https://pypi.org/project/qrkey)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qrkey.svg)](https://pypi.org/project/qrkey)
 [![NPM - Version](https://img.shields.io/npm/v/qrkey.svg)](https://npmjs.org/package/qrkey)
 
+<p align="center">
+  <img src="qrkey.png" width="328"/>
+</p>
+
 ## Summary
 
 Qrkey is a library implementing a protocol designed to facilitate the
 deployment of robots swarm.
 The protocol relies on [MQTT](https://en.wikipedia.org/wiki/MQTT) so that a
 Qrkey server is reachable even with a private IP address.
 Access to the swarm is managed by a QR code based authentication scheme.
```

### Comparing `qrkey-0.4.4/pyproject.toml` & `qrkey-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qrkey-0.4.4/PKG-INFO` & `qrkey-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: qrkey
-Version: 0.4.4
+Version: 0.5.1
 Summary: Swarm robotics deployments made easy.
 Project-URL: Documentation, https://github.com/DotBots/qrkey#readme
 Project-URL: Issues, https://github.com/DotBots/qrkey/issues
 Project-URL: Source, https://github.com/DotBots/qrkey
 Author-email: Alexandre Abadie <alexandre.abadie@inria.fr>
 License-Expression: BSD-3-Clause
 License-File: LICENSE.txt
@@ -31,14 +31,18 @@
 
 # Qrkey
 
 [![PyPI - Version](https://img.shields.io/pypi/v/qrkey.svg)](https://pypi.org/project/qrkey)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qrkey.svg)](https://pypi.org/project/qrkey)
 [![NPM - Version](https://img.shields.io/npm/v/qrkey.svg)](https://npmjs.org/package/qrkey)
 
+<p align="center">
+  <img src="qrkey.png" width="328"/>
+</p>
+
 ## Summary
 
 Qrkey is a library implementing a protocol designed to facilitate the
 deployment of robots swarm.
 The protocol relies on [MQTT](https://en.wikipedia.org/wiki/MQTT) so that a
 Qrkey server is reachable even with a private IP address.
 Access to the swarm is managed by a QR code based authentication scheme.
```

