# Comparing `tmp/tlslib-0.0.2rc0.tar.gz` & `tmp/tlslib-0.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlslib-0.0.2rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tlslib-0.0.2rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tlslib-0.0.2rc0.tar` & `tlslib-0.0.2rc1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10174 2024-05-02 15:54:44.029505 tlslib-0.0.2rc0/LICENSE
--rw-r--r--   0        0        0      593 2024-05-02 15:54:44.029505 tlslib-0.0.2rc0/README.md
--rw-r--r--   0        0        0     1989 2024-05-02 15:54:44.029505 tlslib-0.0.2rc0/pyproject.toml
--rw-r--r--   0        0        0       51 2024-05-02 15:54:44.033505 tlslib-0.0.2rc0/src/tlslib/__init__.py
--rw-r--r--   0        0        0     7176 2024-05-02 15:54:44.033505 tlslib-0.0.2rc0/src/tlslib/insecure/__init__.py
--rw-r--r--   0        0        0     6146 2024-05-02 15:54:44.033505 tlslib-0.0.2rc0/src/tlslib/insecure/stdlib_insecure.py
--rw-r--r--   0        0        0    36106 2024-05-02 15:54:44.033505 tlslib-0.0.2rc0/src/tlslib/stdlib.py
--rw-r--r--   0        0        0    32460 2024-05-02 15:54:44.033505 tlslib-0.0.2rc0/src/tlslib/tlslib.py
--rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 tlslib-0.0.2rc0/PKG-INFO
+-rw-r--r--   0        0        0    10174 2024-05-02 17:29:09.523704 tlslib-0.0.2rc1/LICENSE
+-rw-r--r--   0        0        0      593 2024-05-02 17:29:09.523704 tlslib-0.0.2rc1/README.md
+-rw-r--r--   0        0        0     1989 2024-05-02 17:29:09.523704 tlslib-0.0.2rc1/pyproject.toml
+-rw-r--r--   0        0        0       51 2024-05-02 17:29:09.523704 tlslib-0.0.2rc1/src/tlslib/__init__.py
+-rw-r--r--   0        0        0     7176 2024-05-02 17:29:09.523704 tlslib-0.0.2rc1/src/tlslib/insecure/__init__.py
+-rw-r--r--   0        0        0     6146 2024-05-02 17:29:09.523704 tlslib-0.0.2rc1/src/tlslib/insecure/stdlib_insecure.py
+-rw-r--r--   0        0        0    36201 2024-05-02 17:29:09.523704 tlslib-0.0.2rc1/src/tlslib/stdlib.py
+-rw-r--r--   0        0        0    32460 2024-05-02 17:29:09.523704 tlslib-0.0.2rc1/src/tlslib/tlslib.py
+-rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 tlslib-0.0.2rc1/PKG-INFO
```

### Comparing `tlslib-0.0.2rc0/LICENSE` & `tlslib-0.0.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tlslib-0.0.2rc0/README.md` & `tlslib-0.0.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `tlslib-0.0.2rc0/pyproject.toml` & `tlslib-0.0.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tlslib-0.0.2rc0/src/tlslib/insecure/__init__.py` & `tlslib-0.0.2rc1/src/tlslib/insecure/__init__.py`

 * *Files identical despite different names*

### Comparing `tlslib-0.0.2rc0/src/tlslib/insecure/stdlib_insecure.py` & `tlslib-0.0.2rc1/src/tlslib/insecure/stdlib_insecure.py`

 * *Files identical despite different names*

### Comparing `tlslib-0.0.2rc0/src/tlslib/stdlib.py` & `tlslib-0.0.2rc1/src/tlslib/stdlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,16 +638,19 @@
         ignored or not is up to the specific application.
 
         As at any time a re-negotiation is possible, a call to ``read()``
         can also cause write operations.
         """
 
         with _error_converter():
-            # MyPy insists that buffer must be a bytearray
-            return self._object.read(amt, buffer)  # type: ignore[arg-type]
+            try:
+                # MyPy insists that buffer must be a bytearray
+                return self._object.read(amt, buffer)  # type: ignore[arg-type]
+            except ssl.SSLZeroReturnError:
+                return b""
 
     def write(self, buf: Buffer) -> int:
         """
         Write ``buf`` in encrypted form to the output buffer and return the
         number of bytes written. The ``buf`` argument must be an object
         supporting the buffer interface.
```

### Comparing `tlslib-0.0.2rc0/src/tlslib/tlslib.py` & `tlslib-0.0.2rc1/src/tlslib/tlslib.py`

 * *Files identical despite different names*

### Comparing `tlslib-0.0.2rc0/PKG-INFO` & `tlslib-0.0.2rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlslib
-Version: 0.0.2rc0
+Version: 0.0.2rc1
 Summary: An example MVP for the updated PEP 543 proposal
 Author-email: Trail of Bits <opensource@trailofbits.com>
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: truststore
```

