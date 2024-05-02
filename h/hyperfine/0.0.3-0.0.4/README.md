# Comparing `tmp/hyperfine-0.0.3.tar.gz` & `tmp/hyperfine-0.0.4.tar.gz`

## Comparing `hyperfine-0.0.3.tar` & `hyperfine-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/_version.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/demagnetization.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/distributions.py
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/dpass.py
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/minuit.py
--rw-r--r--   0        0        0    13475 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/srim.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/bnmr/__init__.py
--rw-r--r--   0        0        0    14249 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/bnmr/lineshape.py
--rw-r--r--   0        0        0    18998 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/bnmr/meissner.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/bnmr/nlme.py
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/bnmr/susceptibility.py
--rw-r--r--   0        0        0     8229 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/musr/__init__.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/musr/_meissner.py
--rw-r--r--   0        0        0    26336 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/musr/meissner.py
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/__init__.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/_muhlschlegel.py
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/bcs.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/ccf.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/interpolation.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/intertype.py
--rw-r--r--   0        0        0    18362 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/london.py
--rw-r--r--   0        0        0    15737 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/pippard.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 hyperfine-0.0.3/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 hyperfine-0.0.3/LICENSE
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 hyperfine-0.0.3/README.md
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 hyperfine-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 hyperfine-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/_version.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/demagnetization.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/distributions.py
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/dpass.py
+-rw-r--r--   0        0        0     7534 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/minuit.py
+-rw-r--r--   0        0        0    13475 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/srim.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/bnmr/__init__.py
+-rw-r--r--   0        0        0    14249 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/bnmr/lineshape.py
+-rw-r--r--   0        0        0    18998 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/bnmr/meissner.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/bnmr/nlme.py
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/bnmr/susceptibility.py
+-rw-r--r--   0        0        0     8229 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/musr/__init__.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/musr/_meissner.py
+-rw-r--r--   0        0        0    26336 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/musr/meissner.py
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/superconductivity/__init__.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/superconductivity/_muhlschlegel.py
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/superconductivity/bcs.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/superconductivity/ccf.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/superconductivity/interpolation.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/superconductivity/intertype.py
+-rw-r--r--   0        0        0    18362 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/superconductivity/london.py
+-rw-r--r--   0        0        0    15737 2020-02-02 00:00:00.000000 hyperfine-0.0.4/hyperfine/superconductivity/pippard.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 hyperfine-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 hyperfine-0.0.4/LICENSE
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 hyperfine-0.0.4/README.md
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 hyperfine-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 hyperfine-0.0.4/PKG-INFO
```

### Comparing `hyperfine-0.0.3/hyperfine/demagnetization.py` & `hyperfine-0.0.4/hyperfine/demagnetization.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/distributions.py` & `hyperfine-0.0.4/hyperfine/distributions.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/dpass.py` & `hyperfine-0.0.4/hyperfine/dpass.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/minuit.py` & `hyperfine-0.0.4/hyperfine/minuit.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,38 +41,78 @@
         # add the parameter specific minos dictionary to the minos dictionary
         minos[par] = mdict
 
     # return the filled minos dictionary
     return minos
 
 
+def covariance2dict(minuit: Minuit) -> dict:
+    """Convert the covariance matrix to a serializable dictionary.
+
+    Convert the covariance matrix (i.e., the MIGRAD or HESSE errors) determined
+    by the MINUIT2 minimizer to a *serializable* dictionary (i.e., one that is
+    compatible with JSON).
+
+    Args:
+        minuit: The ``iminuit.Minuit`` object.
+
+    Returns:
+        A serializable dictionary containing the covariance matrix (i.e., errors computed by MIGRAD or HESSE).
+    """
+
+    # empty dictionary to hold the matrix
+    covariance = {}
+
+    # check if the covariance matrix exists
+    if minuit.covariance is not None:
+        # loop over all fit parameters
+        for par1 in minuit.parameters:
+            # for each parameter, create an empty dictionary...
+            covariance[par1] = {}
+            # loop over all fit parameters
+            for par2 in m.parameters:
+                # ...to be filled with the covariance for each
+                # parameter pair combination
+                covariance[par1][par2] = m.covariance[par1, par2]
+
+    # return the covariance matrix
+    return covariance
+
+
 def minuit2json(minuit: Minuit, filename: str) -> None:
-    """Serialize fitting results from an `iminuit.Minuit` object to a JSON file.
+    """Serialize fitting results from an ``iminuit.Minuit`` object to a JSON file.
+
+    Serialization includes data for: ``values``, ``errors``, ``limits``,
+    ``fixed``, ``covariance``, and ``merrors``.
 
     Args:
         minuit: The ``iminuit.Minuit`` object.
         filename: Name of JSON file to save the serialized fit results.
     """
 
     # convert the results to a dictionary
     results = {
         "values": minuit.values.to_dict(),
         "errors": minuit.errors.to_dict(),
         "limits": minuit.limits.to_dict(),
         "fixed": minuit.fixed.to_dict(),
+        "covariance": covariance2dict(minuit),
         "merrors": minos2dict(minuit),
     }
 
     # write the results dictionary to a file
     with open(filename, "w") as fh:
         json.dump(results, fh, indent="\t")
 
 
 def json2minuit(minuit: Minuit, filename: str) -> None:
-    """De-serialize fitting results from a JSON file to an `iminuit.Minuit` object.
+    """De-serialize fitting results from a JSON file to an ``iminuit.Minuit`` object.
+
+    De-serialization includes data for: ``values``, ``errors``, ``limits``,
+    and ``fixed`` (``covariance`` and ``merrors`` are not yet implemented).
 
     Args:
         minuit: The ``iminuit.Minuit`` object.
         filename: Name of JSON file containing the serialized fit results.
     """
 
     # read the results into a dictionary
@@ -81,15 +121,16 @@
 
     # restore the fit quantities
     for quantity in ["values", "errors", "limits", "fixed"]:
         if quantity in results:
             for key, value in results[quantity].items():
                 minuit.__getattribute__(quantity)[key] = value
 
-    # TODO: restore the minos errors
+    # TODO: restore the covariance matrix?
+    # TODO: restore the minos errors?
 
 
 class GenericLeastSquares3D:
     """Generic 3D least-squares cost function with error.
 
     https://iminuit.readthedocs.io/en/stable/tutorial/generic_least_squares.html
     """
```

### Comparing `hyperfine-0.0.3/hyperfine/srim.py` & `hyperfine-0.0.4/hyperfine/srim.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/bnmr/lineshape.py` & `hyperfine-0.0.4/hyperfine/bnmr/lineshape.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/bnmr/meissner.py` & `hyperfine-0.0.4/hyperfine/bnmr/meissner.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/bnmr/nlme.py` & `hyperfine-0.0.4/hyperfine/bnmr/nlme.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/bnmr/susceptibility.py` & `hyperfine-0.0.4/hyperfine/bnmr/susceptibility.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/musr/__init__.py` & `hyperfine-0.0.4/hyperfine/musr/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/musr/_meissner.py` & `hyperfine-0.0.4/hyperfine/musr/_meissner.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/musr/meissner.py` & `hyperfine-0.0.4/hyperfine/musr/meissner.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/superconductivity/__init__.py` & `hyperfine-0.0.4/hyperfine/superconductivity/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/superconductivity/_muhlschlegel.py` & `hyperfine-0.0.4/hyperfine/superconductivity/_muhlschlegel.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/superconductivity/bcs.py` & `hyperfine-0.0.4/hyperfine/superconductivity/bcs.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/superconductivity/ccf.py` & `hyperfine-0.0.4/hyperfine/superconductivity/ccf.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/superconductivity/interpolation.py` & `hyperfine-0.0.4/hyperfine/superconductivity/interpolation.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/superconductivity/intertype.py` & `hyperfine-0.0.4/hyperfine/superconductivity/intertype.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/superconductivity/london.py` & `hyperfine-0.0.4/hyperfine/superconductivity/london.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/hyperfine/superconductivity/pippard.py` & `hyperfine-0.0.4/hyperfine/superconductivity/pippard.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/.gitignore` & `hyperfine-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/LICENSE` & `hyperfine-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/README.md` & `hyperfine-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/pyproject.toml` & `hyperfine-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.3/PKG-INFO` & `hyperfine-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hyperfine
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Homepage, https://github.com/rmlmcfadden/hyperfine
 Project-URL: Documentation, https://hyperfine.readthedocs.io/
 Project-URL: Repository, https://github.com/rmlmcfadden/hyperfine.git
 Project-URL: Issues, https://github.com/rmlmcfadden/hyperfine/issues
 Author-email: "Ryan M. L. McFadden" <rmlm@triumf.ca>
 License-Expression: MIT
 License-File: LICENSE
```

