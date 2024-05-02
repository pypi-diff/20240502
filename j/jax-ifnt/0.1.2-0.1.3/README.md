# Comparing `tmp/jax_ifnt-0.1.2.tar.gz` & `tmp/jax_ifnt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_ifnt-0.1.2.tar", last modified: Thu May  2 15:11:01 2024, max compression
+gzip compressed data, was "jax_ifnt-0.1.3.tar", last modified: Thu May  2 16:11:30 2024, max compression
```

## Comparing `jax_ifnt-0.1.2.tar` & `jax_ifnt-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:11:01.501866 jax_ifnt-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 15:10:36.000000 jax_ifnt-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-02 15:11:01.501866 jax_ifnt-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-02 15:10:36.000000 jax_ifnt-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:11:01.501866 jax_ifnt-0.1.2/ifnt/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-02 15:10:36.000000 jax_ifnt-0.1.2/ifnt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-02 15:10:36.000000 jax_ifnt-0.1.2/ifnt/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-02 15:10:36.000000 jax_ifnt-0.1.2/ifnt/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-02 15:10:36.000000 jax_ifnt-0.1.2/ifnt/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:11:01.501866 jax_ifnt-0.1.2/jax_ifnt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-02 15:11:01.000000 jax_ifnt-0.1.2/jax_ifnt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-02 15:11:01.000000 jax_ifnt-0.1.2/jax_ifnt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:11:01.000000 jax_ifnt-0.1.2/jax_ifnt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 15:11:01.000000 jax_ifnt-0.1.2/jax_ifnt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 15:11:01.000000 jax_ifnt-0.1.2/jax_ifnt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 15:10:36.000000 jax_ifnt-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:11:01.501866 jax_ifnt-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:11:01.501866 jax_ifnt-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-02 15:10:36.000000 jax_ifnt-0.1.2/tests/test_ifnt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:11:30.873512 jax_ifnt-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 16:11:06.000000 jax_ifnt-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-02 16:11:30.873512 jax_ifnt-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-02 16:11:06.000000 jax_ifnt-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:11:30.869512 jax_ifnt-0.1.3/ifnt/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-02 16:11:06.000000 jax_ifnt-0.1.3/ifnt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-02 16:11:06.000000 jax_ifnt-0.1.3/ifnt/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-02 16:11:06.000000 jax_ifnt-0.1.3/ifnt/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-02 16:11:06.000000 jax_ifnt-0.1.3/ifnt/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:11:30.873512 jax_ifnt-0.1.3/jax_ifnt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-02 16:11:30.000000 jax_ifnt-0.1.3/jax_ifnt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-02 16:11:30.000000 jax_ifnt-0.1.3/jax_ifnt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:11:30.000000 jax_ifnt-0.1.3/jax_ifnt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 16:11:30.000000 jax_ifnt-0.1.3/jax_ifnt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 16:11:30.000000 jax_ifnt-0.1.3/jax_ifnt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 16:11:06.000000 jax_ifnt-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:11:30.873512 jax_ifnt-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:11:30.873512 jax_ifnt-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-02 16:11:06.000000 jax_ifnt-0.1.3/tests/test_ifnt.py
```

### Comparing `jax_ifnt-0.1.2/LICENSE` & `jax_ifnt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_ifnt-0.1.2/PKG-INFO` & `jax_ifnt-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-ifnt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Execute runtime assertions, indexing checks, and more if `jax` code is not traced.
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: jax
 Requires-Dist: jaxlib
 
 ifnt
```

### Comparing `jax_ifnt-0.1.2/README.rst` & `jax_ifnt-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `jax_ifnt-0.1.2/ifnt/random.py` & `jax_ifnt-0.1.3/ifnt/random.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,49 @@
 import functools
 import inspect
 from jax import numpy as jnp
 from jax import random
 from typing import Callable, TypeVar
-from .util import is_traced
 
 
 C = TypeVar("C", bound=Callable[..., jnp.ndarray])
 
 
+def keys(seed):
+    """
+    Random key generator.
+
+    Args:
+        seed: Initial seed.
+
+    Example:
+
+        >>> keys = ifnt.random.keys(9)
+        >>> next(keys)
+        Array((), dtype=key<fry>) overlaying: [4109519897 3077142452]
+        >>> next(keys)
+        Array((), dtype=key<fry>) overlaying: [3656642974 2192743943]
+    """
+    key = random.key(seed)
+    while True:
+        key, subkey = random.split(key)
+        yield subkey
+
+
 def _wrap_random(func: C) -> C:
     signature = inspect.signature(func)
     for param in signature.parameters:
         assert (
             param == "key"
         ), f"The first parameter must be `key` but got `{param}` for `{func}`."
         break
 
     @functools.wraps(func)
     def _inner(self: "JaxRandomState", *args, **kwargs):
-        return func(self.get_key(), *args, **kwargs)
+        return func(next(self.keys), *args, **kwargs)
 
     return _inner
 
 
 class JaxRandomState:
     """
     Utility class for sampling random variables using the JAX interface with automatic
@@ -40,33 +60,24 @@
     Example:
 
         >>> rng = ifnt.random.JaxRandomState(7)
         >>> rng.normal()
         Array(-1.4622004, dtype=float32)
         >>> rng.normal()
         Array(2.0224454, dtype=float32)
-        >>> jax.jit(rng.normal)()
-        Traceback (most recent call last):
-        ...
-        RuntimeError: `JaxRandomState.get_key()` does not support jit compilation.
     """
 
     def __init__(self, seed: int) -> None:
-        self._key = random.PRNGKey(seed)
+        self.keys = keys(seed)
 
     def get_key(self) -> jnp.ndarray:
         """
         Get a random key and update the state.
         """
-        self._key, key = random.split(self._key)
-        if is_traced(key):
-            raise RuntimeError(
-                "`JaxRandomState.get_key()` does not support jit compilation."
-            )
-        return key
+        return next(self.keys)
 
     ball = _wrap_random(random.ball)
     bernoulli = _wrap_random(random.bernoulli)
     beta = _wrap_random(random.beta)
     binomial = _wrap_random(random.binomial)
     bits = _wrap_random(random.bits)
     categorical = _wrap_random(random.categorical)
```

### Comparing `jax_ifnt-0.1.2/ifnt/testing.py` & `jax_ifnt-0.1.3/ifnt/testing.py`

 * *Files identical despite different names*

### Comparing `jax_ifnt-0.1.2/ifnt/util.py` & `jax_ifnt-0.1.3/ifnt/util.py`

 * *Files identical despite different names*

### Comparing `jax_ifnt-0.1.2/jax_ifnt.egg-info/PKG-INFO` & `jax_ifnt-0.1.3/jax_ifnt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-ifnt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Execute runtime assertions, indexing checks, and more if `jax` code is not traced.
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: jax
 Requires-Dist: jaxlib
 
 ifnt
```

### Comparing `jax_ifnt-0.1.2/tests/test_ifnt.py` & `jax_ifnt-0.1.3/tests/test_ifnt.py`

 * *Files identical despite different names*

