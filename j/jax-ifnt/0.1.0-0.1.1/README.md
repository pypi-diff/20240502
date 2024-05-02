# Comparing `tmp/jax_ifnt-0.1.0.tar.gz` & `tmp/jax_ifnt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_ifnt-0.1.0.tar", last modified: Sun Apr 28 16:29:45 2024, max compression
+gzip compressed data, was "jax_ifnt-0.1.1.tar", last modified: Thu May  2 03:25:34 2024, max compression
```

## Comparing `jax_ifnt-0.1.0.tar` & `jax_ifnt-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:29:45.326460 jax_ifnt-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-28 16:29:21.000000 jax_ifnt-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-28 16:29:45.326460 jax_ifnt-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-28 16:29:21.000000 jax_ifnt-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:29:45.326460 jax_ifnt-0.1.0/ifnt/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-28 16:29:21.000000 jax_ifnt-0.1.0/ifnt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-28 16:29:21.000000 jax_ifnt-0.1.0/ifnt/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-28 16:29:21.000000 jax_ifnt-0.1.0/ifnt/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-28 16:29:21.000000 jax_ifnt-0.1.0/ifnt/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:29:45.326460 jax_ifnt-0.1.0/jax_ifnt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-28 16:29:45.000000 jax_ifnt-0.1.0/jax_ifnt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-28 16:29:45.000000 jax_ifnt-0.1.0/jax_ifnt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:29:45.000000 jax_ifnt-0.1.0/jax_ifnt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 16:29:45.000000 jax_ifnt-0.1.0/jax_ifnt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-28 16:29:45.000000 jax_ifnt-0.1.0/jax_ifnt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-28 16:29:21.000000 jax_ifnt-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 16:29:45.326460 jax_ifnt-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:29:45.326460 jax_ifnt-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-28 16:29:21.000000 jax_ifnt-0.1.0/tests/test_ifnt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:25:34.173441 jax_ifnt-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 03:25:04.000000 jax_ifnt-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-02 03:25:34.173441 jax_ifnt-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-02 03:25:04.000000 jax_ifnt-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:25:34.169441 jax_ifnt-0.1.1/ifnt/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-02 03:25:04.000000 jax_ifnt-0.1.1/ifnt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-02 03:25:04.000000 jax_ifnt-0.1.1/ifnt/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-02 03:25:04.000000 jax_ifnt-0.1.1/ifnt/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-02 03:25:04.000000 jax_ifnt-0.1.1/ifnt/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:25:34.169441 jax_ifnt-0.1.1/jax_ifnt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-02 03:25:34.000000 jax_ifnt-0.1.1/jax_ifnt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-02 03:25:34.000000 jax_ifnt-0.1.1/jax_ifnt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 03:25:34.000000 jax_ifnt-0.1.1/jax_ifnt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 03:25:34.000000 jax_ifnt-0.1.1/jax_ifnt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 03:25:34.000000 jax_ifnt-0.1.1/jax_ifnt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 03:25:04.000000 jax_ifnt-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 03:25:34.173441 jax_ifnt-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:25:34.169441 jax_ifnt-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-02 03:25:04.000000 jax_ifnt-0.1.1/tests/test_ifnt.py
```

### Comparing `jax_ifnt-0.1.0/LICENSE` & `jax_ifnt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_ifnt-0.1.0/PKG-INFO` & `jax_ifnt-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-ifnt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Execute runtime assertions, indexing checks, and more if `jax` code is not traced.
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: jax
 Requires-Dist: jaxlib
 
 ifnt
```

### Comparing `jax_ifnt-0.1.0/README.rst` & `jax_ifnt-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `jax_ifnt-0.1.0/ifnt/random.py` & `jax_ifnt-0.1.1/ifnt/random.py`

 * *Files identical despite different names*

### Comparing `jax_ifnt-0.1.0/ifnt/testing.py` & `jax_ifnt-0.1.1/ifnt/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,30 +63,36 @@
 
 @skip_if_traced
 def assert_samples_close(
     samples: jnp.ndarray,
     expected: jnp.ndarray,
     q: float = 0.001,
     on_weak: str = "raise",
+    rtol: float = 1e-7,
+    atol: float = 0.0,
 ) -> None:
     """
     Assert that i.i.d samples are close to a target using a normal approximation of the
     sample mean. If samples are not scalars, a
     `Bonferroni correction <https://en.wikipedia.org/wiki/Bonferroni_correction>`__ is
     applied to the tail probability :code:`q` to avoid incorrect rejection of the null
     hypothesis (that :code:`expected` is the mean of the distribution that generated
-    :code:`samples`) because of sampling noise.
+    :code:`samples`) because of sampling noise. The assertion also passes without
+    failure if all samples are close to the target as determined by :code:`rtol` and
+    :code:`atol`.
 
     Args:
         samples: Samples with shape :code:`(n_samples, ...)`.
         expected: Target with shape :code:`(...)`.
         q: Tail probability where to reject the null that :code:`expected` is the mean
             of the distribution that generated :code:`samples`.
         on_weak: Action if the sample size is too small to confidently reject the null
             hypothesis.
+        rtol: Relative tolerance.
+        atol: Absolute tolerance.
 
     Example:
 
         >>> samples = jax.random.normal(jax.random.key(7), (1000,))
         >>> ifnt.testing.assert_samples_close(samples, 0.0)
         >>> ifnt.testing.assert_samples_close(samples, 1.0)
         Traceback (most recent call last):
@@ -124,15 +130,16 @@
             warnings.warn(message)
 
     z = (expected - mean) / stderr
     # Compute p-value and apply Bonferroni correction (see
     # https://en.wikipedia.org/wiki/Bonferroni_correction).
     p = stats.norm.cdf(z)
     p = jnp.size(expected) * jnp.minimum(p, 1 - p)
-    if (p < q).any():
+    within_tol = jnp.isclose(samples, expected, rtol=rtol, atol=atol).all(axis=0)
+    if ((p < q) & ~within_tol).any():
         raise AssertionError(
             f"Sample mean {mean} with standard error {stderr} is not consistent with "
             f"the expected value {expected} (z-score = {z})."
         )
 
 
 @broadcast_over_dict
```

### Comparing `jax_ifnt-0.1.0/ifnt/util.py` & `jax_ifnt-0.1.1/ifnt/util.py`

 * *Files identical despite different names*

### Comparing `jax_ifnt-0.1.0/jax_ifnt.egg-info/PKG-INFO` & `jax_ifnt-0.1.1/jax_ifnt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-ifnt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Execute runtime assertions, indexing checks, and more if `jax` code is not traced.
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: jax
 Requires-Dist: jaxlib
 
 ifnt
```

### Comparing `jax_ifnt-0.1.0/tests/test_ifnt.py` & `jax_ifnt-0.1.1/tests/test_ifnt.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,13 +45,21 @@
         assert not ifnt.util.IS_ENABLED
         ifnt.testing.assert_allclose(1, 2)
     assert ifnt.util.IS_ENABLED
     with pytest.raises(AssertionError):
         ifnt.testing.assert_allclose(1, 2)
 
 
-def test_assert_samples_close() -> None:
+def test_assert_samples_close_weak() -> None:
     with pytest.raises(ValueError, match="Consider increasing the sample size"):
         ifnt.testing.assert_samples_close(jnp.arange(3), 0.001)
     with pytest.warns(match="Consider increasing the sample size"):
         ifnt.testing.assert_samples_close(jnp.arange(3), 0.001, on_weak="warn")
     ifnt.testing.assert_samples_close(jnp.arange(3), 0.001, on_weak="ignore")
+
+
+def test_assert_samples_close_tol() -> None:
+    samples = ifnt.random.JaxRandomState(17).normal((1000,)) * 1e-6
+    ifnt.testing.assert_samples_close(samples, 0)
+    with pytest.raises(AssertionError):
+        ifnt.testing.assert_samples_close(samples, 1e-3)
+    ifnt.testing.assert_samples_close(samples, 1e-3, atol=1e-2)
```

