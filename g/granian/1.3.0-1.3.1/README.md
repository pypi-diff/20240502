# Comparing `tmp/granian-1.3.0.tar.gz` & `tmp/granian-1.3.1.tar.gz`

## Comparing `granian-1.3.0.tar` & `granian-1.3.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 granian-1.3.0/Cargo.toml
--rw-r--r--   0     1001      127     1486 2024-04-27 00:05:55.000000 granian-1.3.0/LICENSE
--rw-r--r--   0     1001      127    10387 2024-04-27 00:05:55.000000 granian-1.3.0/README.md
--rw-r--r--   0     1001      127       87 2024-04-27 00:05:55.000000 granian-1.3.0/granian/__init__.py
--rw-r--r--   0     1001      127       50 2024-04-27 00:05:55.000000 granian-1.3.0/granian/__main__.py
--rw-r--r--   0     1001      127      276 2024-04-27 00:05:55.000000 granian-1.3.0/granian/_futures.py
--rw-r--r--   0     1001      127     3043 2024-04-27 00:05:55.000000 granian-1.3.0/granian/_granian.pyi
--rw-r--r--   0     1001      127      143 2024-04-27 00:05:55.000000 granian-1.3.0/granian/_imports.py
--rw-r--r--   0     1001      127     1677 2024-04-27 00:05:55.000000 granian-1.3.0/granian/_internal.py
--rw-r--r--   0     1001      127     2935 2024-04-27 00:05:55.000000 granian-1.3.0/granian/_loops.py
--rw-r--r--   0     1001      127       93 2024-04-27 00:05:55.000000 granian-1.3.0/granian/_types.py
--rw-r--r--   0     1001      127     3895 2024-04-27 00:05:55.000000 granian-1.3.0/granian/asgi.py
--rw-r--r--   0     1001      127     9221 2024-04-27 00:05:55.000000 granian-1.3.0/granian/cli.py
--rw-r--r--   0     1001      127      379 2024-04-27 00:05:55.000000 granian-1.3.0/granian/constants.py
--rw-r--r--   0     1001      127      615 2024-04-27 00:05:55.000000 granian-1.3.0/granian/http.py
--rw-r--r--   0     1001      127     1480 2024-04-27 00:05:55.000000 granian-1.3.0/granian/log.py
--rw-r--r--   0     1001      127      144 2024-04-27 00:05:55.000000 granian-1.3.0/granian/net.py
--rw-r--r--   0     1001      127        0 2024-04-27 00:05:55.000000 granian-1.3.0/granian/py.typed
--rw-r--r--   0     1001      127      769 2024-04-27 00:05:55.000000 granian-1.3.0/granian/rsgi.py
--rw-r--r--   0     1001      127    19087 2024-04-27 00:05:55.000000 granian-1.3.0/granian/server.py
--rw-r--r--   0     1001      127     1354 2024-04-27 00:05:55.000000 granian-1.3.0/granian/wsgi.py
--rw-r--r--   0     1001      127    12724 2024-04-27 00:05:55.000000 granian-1.3.0/src/asgi/callbacks.rs
--rw-r--r--   0     1001      127     2031 2024-04-27 00:05:55.000000 granian-1.3.0/src/asgi/errors.rs
--rw-r--r--   0     1001      127     6352 2024-04-27 00:05:55.000000 granian-1.3.0/src/asgi/http.rs
--rw-r--r--   0     1001      127    22323 2024-04-27 00:05:55.000000 granian-1.3.0/src/asgi/io.rs
--rw-r--r--   0     1001      127      302 2024-04-27 00:05:55.000000 granian-1.3.0/src/asgi/mod.rs
--rw-r--r--   0     1001      127     4839 2024-04-27 00:05:55.000000 granian-1.3.0/src/asgi/serve.rs
--rw-r--r--   0     1001      127      259 2024-04-27 00:05:55.000000 granian-1.3.0/src/asgi/types.rs
--rw-r--r--   0     1001      127     4679 2024-04-27 00:05:55.000000 granian-1.3.0/src/asgi/utils.rs
--rw-r--r--   0     1001      127     1030 2024-04-27 00:05:55.000000 granian-1.3.0/src/asyncio.rs
--rw-r--r--   0     1001      127    13845 2024-04-27 00:05:55.000000 granian-1.3.0/src/callbacks.rs
--rw-r--r--   0     1001      127     2900 2024-04-27 00:05:55.000000 granian-1.3.0/src/conversion.rs
--rw-r--r--   0     1001      127     1345 2024-04-27 00:05:55.000000 granian-1.3.0/src/http.rs
--rw-r--r--   0     1001      127     1298 2024-04-27 00:05:55.000000 granian-1.3.0/src/io.rs
--rw-r--r--   0     1001      127      964 2024-04-27 00:05:55.000000 granian-1.3.0/src/lib.rs
--rw-r--r--   0     1001      127     9737 2024-04-27 00:05:55.000000 granian-1.3.0/src/rsgi/callbacks.rs
--rw-r--r--   0     1001      127      564 2024-04-27 00:05:55.000000 granian-1.3.0/src/rsgi/errors.rs
--rw-r--r--   0     1001      127     5970 2024-04-27 00:05:55.000000 granian-1.3.0/src/rsgi/http.rs
--rw-r--r--   0     1001      127    13340 2024-04-27 00:05:55.000000 granian-1.3.0/src/rsgi/io.rs
--rw-r--r--   0     1001      127      742 2024-04-27 00:05:55.000000 granian-1.3.0/src/rsgi/mod.rs
--rw-r--r--   0     1001      127     4839 2024-04-27 00:05:55.000000 granian-1.3.0/src/rsgi/serve.rs
--rw-r--r--   0     1001      127     8849 2024-04-27 00:05:55.000000 granian-1.3.0/src/rsgi/types.rs
--rw-r--r--   0     1001      127    11181 2024-04-27 00:05:55.000000 granian-1.3.0/src/runtime.rs
--rw-r--r--   0     1001      127     2298 2024-04-27 00:05:55.000000 granian-1.3.0/src/tcp.rs
--rw-r--r--   0     1001      127     1111 2024-04-27 00:05:55.000000 granian-1.3.0/src/tls.rs
--rw-r--r--   0     1001      127     1272 2024-04-27 00:05:55.000000 granian-1.3.0/src/utils.rs
--rw-r--r--   0     1001      127    37312 2024-04-27 00:05:55.000000 granian-1.3.0/src/workers.rs
--rw-r--r--   0     1001      127     4007 2024-04-27 00:05:55.000000 granian-1.3.0/src/ws.rs
--rw-r--r--   0     1001      127     4690 2024-04-27 00:05:55.000000 granian-1.3.0/src/wsgi/callbacks.rs
--rw-r--r--   0     1001      127     1557 2024-04-27 00:05:55.000000 granian-1.3.0/src/wsgi/http.rs
--rw-r--r--   0     1001      127       58 2024-04-27 00:05:55.000000 granian-1.3.0/src/wsgi/mod.rs
--rw-r--r--   0     1001      127     2455 2024-04-27 00:05:55.000000 granian-1.3.0/src/wsgi/serve.rs
--rw-r--r--   0     1001      127     6339 2024-04-27 00:05:55.000000 granian-1.3.0/src/wsgi/types.rs
--rw-r--r--   0     1001      127     4104 2024-04-27 00:05:55.000000 granian-1.3.0/tests/apps/asgi.py
--rw-r--r--   0     1001      127     3140 2024-04-27 00:05:55.000000 granian-1.3.0/tests/apps/rsgi.py
--rw-r--r--   0     1001      127     1123 2024-04-27 00:05:55.000000 granian-1.3.0/tests/apps/wsgi.py
--rw-r--r--   0     1001      127     2434 2024-04-27 00:05:55.000000 granian-1.3.0/tests/conftest.py
--rw-r--r--   0     1001      127       95 2024-04-27 00:05:55.000000 granian-1.3.0/tests/fixtures/media.png
--rw-r--r--   0     1001      127     1139 2024-04-27 00:05:55.000000 granian-1.3.0/tests/fixtures/tls/cert.pem
--rw-r--r--   0     1001      127     1704 2024-04-27 00:05:55.000000 granian-1.3.0/tests/fixtures/tls/key.pem
--rw-r--r--   0     1001      127     2791 2024-04-27 00:05:55.000000 granian-1.3.0/tests/test_asgi.py
--rw-r--r--   0     1001      127     1750 2024-04-27 00:05:55.000000 granian-1.3.0/tests/test_https.py
--rw-r--r--   0     1001      127     2756 2024-04-27 00:05:55.000000 granian-1.3.0/tests/test_rsgi.py
--rw-r--r--   0     1001      127     2611 2024-04-27 00:05:55.000000 granian-1.3.0/tests/test_ws.py
--rw-r--r--   0     1001      127     2300 2024-04-27 00:05:55.000000 granian-1.3.0/tests/test_wsgi.py
--rw-r--r--   0     1001      127    33752 2024-04-27 00:05:55.000000 granian-1.3.0/Cargo.lock
--rw-r--r--   0     1001      127     2911 2024-04-27 00:05:55.000000 granian-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    12565 1970-01-01 00:00:00.000000 granian-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 granian-1.3.1/Cargo.toml
+-rw-r--r--   0     1001      127     1486 2024-05-01 22:25:47.000000 granian-1.3.1/LICENSE
+-rw-r--r--   0     1001      127    10387 2024-05-01 22:25:47.000000 granian-1.3.1/README.md
+-rw-r--r--   0     1001      127       87 2024-05-01 22:25:47.000000 granian-1.3.1/granian/__init__.py
+-rw-r--r--   0     1001      127       50 2024-05-01 22:25:47.000000 granian-1.3.1/granian/__main__.py
+-rw-r--r--   0     1001      127      276 2024-05-01 22:25:47.000000 granian-1.3.1/granian/_futures.py
+-rw-r--r--   0     1001      127     3043 2024-05-01 22:25:47.000000 granian-1.3.1/granian/_granian.pyi
+-rw-r--r--   0     1001      127      143 2024-05-01 22:25:47.000000 granian-1.3.1/granian/_imports.py
+-rw-r--r--   0     1001      127     1677 2024-05-01 22:25:47.000000 granian-1.3.1/granian/_internal.py
+-rw-r--r--   0     1001      127     2935 2024-05-01 22:25:47.000000 granian-1.3.1/granian/_loops.py
+-rw-r--r--   0     1001      127       93 2024-05-01 22:25:47.000000 granian-1.3.1/granian/_types.py
+-rw-r--r--   0     1001      127     3895 2024-05-01 22:25:47.000000 granian-1.3.1/granian/asgi.py
+-rw-r--r--   0     1001      127     9221 2024-05-01 22:25:47.000000 granian-1.3.1/granian/cli.py
+-rw-r--r--   0     1001      127      379 2024-05-01 22:25:47.000000 granian-1.3.1/granian/constants.py
+-rw-r--r--   0     1001      127      615 2024-05-01 22:25:47.000000 granian-1.3.1/granian/http.py
+-rw-r--r--   0     1001      127     1480 2024-05-01 22:25:47.000000 granian-1.3.1/granian/log.py
+-rw-r--r--   0     1001      127      144 2024-05-01 22:25:47.000000 granian-1.3.1/granian/net.py
+-rw-r--r--   0     1001      127        0 2024-05-01 22:25:47.000000 granian-1.3.1/granian/py.typed
+-rw-r--r--   0     1001      127      769 2024-05-01 22:25:47.000000 granian-1.3.1/granian/rsgi.py
+-rw-r--r--   0     1001      127    19087 2024-05-01 22:25:47.000000 granian-1.3.1/granian/server.py
+-rw-r--r--   0     1001      127     1354 2024-05-01 22:25:47.000000 granian-1.3.1/granian/wsgi.py
+-rw-r--r--   0     1001      127    12724 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/callbacks.rs
+-rw-r--r--   0     1001      127     2031 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/errors.rs
+-rw-r--r--   0     1001      127     6352 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/http.rs
+-rw-r--r--   0     1001      127    22320 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/io.rs
+-rw-r--r--   0     1001      127      302 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/mod.rs
+-rw-r--r--   0     1001      127     4839 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/serve.rs
+-rw-r--r--   0     1001      127      259 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/types.rs
+-rw-r--r--   0     1001      127     4679 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/utils.rs
+-rw-r--r--   0     1001      127     1030 2024-05-01 22:25:47.000000 granian-1.3.1/src/asyncio.rs
+-rw-r--r--   0     1001      127    13845 2024-05-01 22:25:47.000000 granian-1.3.1/src/callbacks.rs
+-rw-r--r--   0     1001      127     2900 2024-05-01 22:25:47.000000 granian-1.3.1/src/conversion.rs
+-rw-r--r--   0     1001      127     1345 2024-05-01 22:25:47.000000 granian-1.3.1/src/http.rs
+-rw-r--r--   0     1001      127     1298 2024-05-01 22:25:47.000000 granian-1.3.1/src/io.rs
+-rw-r--r--   0     1001      127      964 2024-05-01 22:25:47.000000 granian-1.3.1/src/lib.rs
+-rw-r--r--   0     1001      127     9737 2024-05-01 22:25:47.000000 granian-1.3.1/src/rsgi/callbacks.rs
+-rw-r--r--   0     1001      127      564 2024-05-01 22:25:47.000000 granian-1.3.1/src/rsgi/errors.rs
+-rw-r--r--   0     1001      127     5970 2024-05-01 22:25:47.000000 granian-1.3.1/src/rsgi/http.rs
+-rw-r--r--   0     1001      127    13340 2024-05-01 22:25:47.000000 granian-1.3.1/src/rsgi/io.rs
+-rw-r--r--   0     1001      127      742 2024-05-01 22:25:47.000000 granian-1.3.1/src/rsgi/mod.rs
+-rw-r--r--   0     1001      127     4839 2024-05-01 22:25:47.000000 granian-1.3.1/src/rsgi/serve.rs
+-rw-r--r--   0     1001      127     8849 2024-05-01 22:25:47.000000 granian-1.3.1/src/rsgi/types.rs
+-rw-r--r--   0     1001      127    11181 2024-05-01 22:25:47.000000 granian-1.3.1/src/runtime.rs
+-rw-r--r--   0     1001      127     2298 2024-05-01 22:25:47.000000 granian-1.3.1/src/tcp.rs
+-rw-r--r--   0     1001      127     1111 2024-05-01 22:25:47.000000 granian-1.3.1/src/tls.rs
+-rw-r--r--   0     1001      127     1272 2024-05-01 22:25:47.000000 granian-1.3.1/src/utils.rs
+-rw-r--r--   0     1001      127    37312 2024-05-01 22:25:47.000000 granian-1.3.1/src/workers.rs
+-rw-r--r--   0     1001      127     4007 2024-05-01 22:25:47.000000 granian-1.3.1/src/ws.rs
+-rw-r--r--   0     1001      127     4690 2024-05-01 22:25:47.000000 granian-1.3.1/src/wsgi/callbacks.rs
+-rw-r--r--   0     1001      127     1557 2024-05-01 22:25:47.000000 granian-1.3.1/src/wsgi/http.rs
+-rw-r--r--   0     1001      127       58 2024-05-01 22:25:47.000000 granian-1.3.1/src/wsgi/mod.rs
+-rw-r--r--   0     1001      127     2455 2024-05-01 22:25:47.000000 granian-1.3.1/src/wsgi/serve.rs
+-rw-r--r--   0     1001      127     6339 2024-05-01 22:25:47.000000 granian-1.3.1/src/wsgi/types.rs
+-rw-r--r--   0     1001      127     4104 2024-05-01 22:25:47.000000 granian-1.3.1/tests/apps/asgi.py
+-rw-r--r--   0     1001      127     3140 2024-05-01 22:25:47.000000 granian-1.3.1/tests/apps/rsgi.py
+-rw-r--r--   0     1001      127     1123 2024-05-01 22:25:47.000000 granian-1.3.1/tests/apps/wsgi.py
+-rw-r--r--   0     1001      127     2434 2024-05-01 22:25:47.000000 granian-1.3.1/tests/conftest.py
+-rw-r--r--   0     1001      127       95 2024-05-01 22:25:47.000000 granian-1.3.1/tests/fixtures/media.png
+-rw-r--r--   0     1001      127     1139 2024-05-01 22:25:47.000000 granian-1.3.1/tests/fixtures/tls/cert.pem
+-rw-r--r--   0     1001      127     1704 2024-05-01 22:25:47.000000 granian-1.3.1/tests/fixtures/tls/key.pem
+-rw-r--r--   0     1001      127     2791 2024-05-01 22:25:47.000000 granian-1.3.1/tests/test_asgi.py
+-rw-r--r--   0     1001      127     1750 2024-05-01 22:25:47.000000 granian-1.3.1/tests/test_https.py
+-rw-r--r--   0     1001      127     2756 2024-05-01 22:25:47.000000 granian-1.3.1/tests/test_rsgi.py
+-rw-r--r--   0     1001      127     2611 2024-05-01 22:25:47.000000 granian-1.3.1/tests/test_ws.py
+-rw-r--r--   0     1001      127     2300 2024-05-01 22:25:47.000000 granian-1.3.1/tests/test_wsgi.py
+-rw-r--r--   0     1001      127    33752 2024-05-01 22:25:47.000000 granian-1.3.1/Cargo.lock
+-rw-r--r--   0     1001      127     2907 2024-05-01 22:25:47.000000 granian-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    12565 1970-01-01 00:00:00.000000 granian-1.3.1/PKG-INFO
```

### Comparing `granian-1.3.0/Cargo.toml` & `granian-1.3.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "granian"
-version = "1.3.0"
+version = "1.3.1"
 description = "A Rust HTTP server for Python applications"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 edition = "2021"
 
 keywords = ["web", "asyncio"]
 
@@ -30,15 +30,15 @@
 name = "_granian"
 crate-type = ["cdylib"]
 
 [dependencies]
 anyhow = "=1.0"
 futures = "0.3"
 http-body-util = { version = "=0.1" }
-hyper = { version = "=1.2", features = ["http1", "http2", "server"] }
+hyper = { version = "=1.3", features = ["http1", "http2", "server"] }
 hyper-util = { version = "=0.1", features = ["server-auto", "tokio"] }
 log = "0.4"
 percent-encoding = "=2.3"
 pin-project = "1.1"
 pyo3 = { version = "=0.21", features = ["anyhow", "extension-module", "generate-import-lib"] }
 pyo3-log = "=0.10"
 rustls-pemfile = "2.1"
```

### Comparing `granian-1.3.0/LICENSE` & `granian-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/README.md` & `granian-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/granian/_granian.pyi` & `granian-1.3.1/granian/_granian.pyi`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/granian/_internal.py` & `granian-1.3.1/granian/_internal.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/granian/_loops.py` & `granian-1.3.1/granian/_loops.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/granian/asgi.py` & `granian-1.3.1/granian/asgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/granian/cli.py` & `granian-1.3.1/granian/cli.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/granian/http.py` & `granian-1.3.1/granian/http.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/granian/log.py` & `granian-1.3.1/granian/log.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/granian/rsgi.py` & `granian-1.3.1/granian/rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/granian/server.py` & `granian-1.3.1/granian/server.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/granian/wsgi.py` & `granian-1.3.1/granian/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/asgi/callbacks.rs` & `granian-1.3.1/src/asgi/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/asgi/errors.rs` & `granian-1.3.1/src/asgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/asgi/http.rs` & `granian-1.3.1/src/asgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/asgi/io.rs` & `granian-1.3.1/src/asgi/io.rs`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 use super::{
     errors::{error_flow, error_message, UnsupportedASGIMessage},
     types::ASGIMessageType,
 };
 use crate::{
     conversion::BytesToPy,
     http::{response_404, HTTPResponse, HTTPResponseBody, HV_SERVER},
-    runtime::{empty_future_into_py, future_into_py_futlike, future_into_py_iter, RuntimeRef},
+    runtime::{empty_future_into_py, future_into_py_futlike, future_into_py_iter, Runtime, RuntimeRef},
     ws::{HyperWebsocket, UpgradeData, WSRxStream, WSTxStream},
 };
 
 const EMPTY_BYTES: Cow<[u8]> = Cow::Borrowed(b"");
 const EMPTY_STRING: String = String::new();
 static WS_SUBPROTO_HNAME: &str = "Sec-WebSocket-Protocol";
 
@@ -222,15 +222,15 @@
             }
             Ok(ASGIMessageType::HTTPFile(file_path)) => match (
                 self.response_started.load(atomic::Ordering::Relaxed),
                 self.tx.lock().unwrap().take(),
             ) {
                 (true, Some(tx)) => {
                     let (status, headers) = self.response_intent.lock().unwrap().take().unwrap();
-                    future_into_py_iter(self.rt.clone(), py, async move {
+                    self.rt.spawn(async move {
                         let res = match File::open(&file_path).await {
                             Ok(file) => {
                                 let stream = ReaderStream::new(file);
                                 let stream_body = http_body_util::StreamBody::new(stream.map_ok(body::Frame::data));
                                 let mut res =
                                     Response::new(BodyExt::map_err(stream_body, std::convert::Into::into).boxed());
                                 *res.status_mut() = StatusCode::from_u16(status as u16).unwrap();
@@ -239,16 +239,16 @@
                             }
                             Err(_) => {
                                 log::info!("Cannot open file {}", &file_path);
                                 response_404()
                             }
                         };
                         let _ = tx.send(res);
-                        Ok(())
-                    })
+                    });
+                    empty_future_into_py(py)
                 }
                 _ => error_flow!(),
             },
             Err(err) => Err(err.into()),
             _ => error_message!(),
         }
     }
```

### Comparing `granian-1.3.0/src/asgi/serve.rs` & `granian-1.3.1/src/asgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/asgi/utils.rs` & `granian-1.3.1/src/asgi/utils.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/asyncio.rs` & `granian-1.3.1/src/asyncio.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/callbacks.rs` & `granian-1.3.1/src/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/conversion.rs` & `granian-1.3.1/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/http.rs` & `granian-1.3.1/src/http.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/io.rs` & `granian-1.3.1/src/io.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/lib.rs` & `granian-1.3.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/rsgi/callbacks.rs` & `granian-1.3.1/src/rsgi/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/rsgi/errors.rs` & `granian-1.3.1/src/rsgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/rsgi/http.rs` & `granian-1.3.1/src/rsgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/rsgi/io.rs` & `granian-1.3.1/src/rsgi/io.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/rsgi/mod.rs` & `granian-1.3.1/src/rsgi/mod.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/rsgi/serve.rs` & `granian-1.3.1/src/rsgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/rsgi/types.rs` & `granian-1.3.1/src/rsgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/runtime.rs` & `granian-1.3.1/src/runtime.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/tcp.rs` & `granian-1.3.1/src/tcp.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/tls.rs` & `granian-1.3.1/src/tls.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/utils.rs` & `granian-1.3.1/src/utils.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/workers.rs` & `granian-1.3.1/src/workers.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/ws.rs` & `granian-1.3.1/src/ws.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/wsgi/callbacks.rs` & `granian-1.3.1/src/wsgi/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/wsgi/http.rs` & `granian-1.3.1/src/wsgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/wsgi/serve.rs` & `granian-1.3.1/src/wsgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/src/wsgi/types.rs` & `granian-1.3.1/src/wsgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/tests/apps/asgi.py` & `granian-1.3.1/tests/apps/asgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/tests/apps/rsgi.py` & `granian-1.3.1/tests/apps/rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/tests/apps/wsgi.py` & `granian-1.3.1/tests/apps/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/tests/conftest.py` & `granian-1.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/tests/fixtures/tls/cert.pem` & `granian-1.3.1/tests/fixtures/tls/cert.pem`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/tests/fixtures/tls/key.pem` & `granian-1.3.1/tests/fixtures/tls/key.pem`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/tests/test_asgi.py` & `granian-1.3.1/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/tests/test_https.py` & `granian-1.3.1/tests/test_https.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/tests/test_rsgi.py` & `granian-1.3.1/tests/test_rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/tests/test_ws.py` & `granian-1.3.1/tests/test_ws.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/tests/test_wsgi.py` & `granian-1.3.1/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.0/Cargo.lock` & `granian-1.3.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "granian"
-version = "1.3.0"
+version = "1.3.1"
 dependencies = [
  "anyhow",
  "futures",
  "http-body-util",
  "hyper",
  "hyper-util",
  "log",
@@ -373,17 +373,17 @@
 name = "httpdate"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "df3b46402a9d5adb4c86a0cf463f42e19994e3ee891101b1841f30a545cb49a9"
 
 [[package]]
 name = "hyper"
-version = "1.2.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "186548d73ac615b32a73aafe38fb4f56c0d340e110e5a200bcadbaf2e199263a"
+checksum = "fe575dd17d0862a9a33781c8c4696a55c320909004a67a00fb286ba8b1bc496d"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
  "h2",
  "http",
  "http-body",
@@ -860,17 +860,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
```

### Comparing `granian-1.3.0/pyproject.toml` & `granian-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 Funding = 'https://github.com/sponsors/gi0baro'
 Source = 'https://github.com/emmett-framework/granian'
 
 [project.scripts]
 granian = 'granian:cli.entrypoint'
 
 [build-system]
-requires = ['maturin>=1.1.0,<1.5.0']
+requires = ['maturin>=1.1.0,<2']
 build-backend = 'maturin'
 
 [tool.maturin]
 module-name = 'granian._granian'
 bindings = 'pyo3'
 
 [tool.ruff]
```

### Comparing `granian-1.3.0/PKG-INFO` & `granian-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: granian
-Version: 1.3.0
+Version: 1.3.1
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

