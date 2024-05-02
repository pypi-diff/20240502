# Comparing `tmp/param-2.1.0a2.tar.gz` & `tmp/param-2.1.0rc1.tar.gz`

## Comparing `param-2.1.0a2.tar` & `param-2.1.0rc1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0    27942 2020-02-02 00:00:00.000000 param-2.1.0a2/numbergen/__init__.py
--rw-r--r--   0        0        0     5045 2020-02-02 00:00:00.000000 param-2.1.0a2/param/__init__.py
--rw-r--r--   0        0        0    18545 2020-02-02 00:00:00.000000 param-2.1.0a2/param/_utils.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 param-2.1.0a2/param/_version.py
--rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 param-2.1.0a2/param/depends.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 param-2.1.0a2/param/display.py
--rw-r--r--   0        0        0    15026 2020-02-02 00:00:00.000000 param-2.1.0a2/param/ipython.py
--rw-r--r--   0        0        0   179011 2020-02-02 00:00:00.000000 param-2.1.0a2/param/parameterized.py
--rw-r--r--   0        0        0   105855 2020-02-02 00:00:00.000000 param-2.1.0a2/param/parameters.py
--rw-r--r--   0        0        0    41071 2020-02-02 00:00:00.000000 param-2.1.0a2/param/reactive.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 param-2.1.0a2/param/serializer.py
--rw-r--r--   0        0        0    31105 2020-02-02 00:00:00.000000 param-2.1.0a2/param/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/__init__.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/conftest.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testaddparameter.py
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testbind.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testbooleanparam.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testbytesparam.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testcalendardateparam.py
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testcalendardaterangeparam.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testcallable.py
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testclassselector.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testcolorparameter.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testcomparator.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testcompositeparams.py
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testcustomparam.py
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testdateparam.py
--rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testdaterangeparam.py
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testdefaults.py
--rw-r--r--   0        0        0    12920 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testdeprecations.py
--rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testdynamicparams.py
--rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testfiledeserialization.py
--rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testfileselector.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testipythonmagic.py
--rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testjsonserialization.py
--rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testlist.py
--rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testlistselector.py
--rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testmultifileselector.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testnumbergen.py
--rw-r--r--   0        0        0    21644 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testnumberparameter.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testnumpy.py
--rw-r--r--   0        0        0    19778 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testobjectselector.py
--rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testpandas.py
--rw-r--r--   0        0        0    40700 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testparamdepends.py
--rw-r--r--   0        0        0    45849 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testparameterizedobject.py
--rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testparameterizedrepr.py
--rw-r--r--   0        0        0     6781 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testparamoutput.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testparamunion.py
--rw-r--r--   0        0        0    13748 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testpathparam.py
--rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testpickle.py
--rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testrangeparameter.py
--rw-r--r--   0        0        0    13470 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testreactive.py
--rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testrefs.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testreprhtml.py
--rw-r--r--   0        0        0    14046 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testselector.py
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testsignatures.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/teststringparam.py
--rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testtimedependent.py
--rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testtupleparam.py
--rw-r--r--   0        0        0    11539 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testutils.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testversion.py
--rw-r--r--   0        0        0    32010 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/testwatch.py
--rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 param-2.1.0a2/tests/utils.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 param-2.1.0a2/.gitignore
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 param-2.1.0a2/LICENSE.txt
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 param-2.1.0a2/README.md
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 param-2.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 param-2.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0    27942 2020-02-02 00:00:00.000000 param-2.1.0rc1/numbergen/__init__.py
+-rw-r--r--   0        0        0     5045 2020-02-02 00:00:00.000000 param-2.1.0rc1/param/__init__.py
+-rw-r--r--   0        0        0    18545 2020-02-02 00:00:00.000000 param-2.1.0rc1/param/_utils.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 param-2.1.0rc1/param/_version.py
+-rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 param-2.1.0rc1/param/depends.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 param-2.1.0rc1/param/display.py
+-rw-r--r--   0        0        0    15026 2020-02-02 00:00:00.000000 param-2.1.0rc1/param/ipython.py
+-rw-r--r--   0        0        0   179137 2020-02-02 00:00:00.000000 param-2.1.0rc1/param/parameterized.py
+-rw-r--r--   0        0        0   105855 2020-02-02 00:00:00.000000 param-2.1.0rc1/param/parameters.py
+-rw-r--r--   0        0        0    43643 2020-02-02 00:00:00.000000 param-2.1.0rc1/param/reactive.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 param-2.1.0rc1/param/serializer.py
+-rw-r--r--   0        0        0    31105 2020-02-02 00:00:00.000000 param-2.1.0rc1/param/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testaddparameter.py
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testbind.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testbooleanparam.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testbytesparam.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testcalendardateparam.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testcalendardaterangeparam.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testcallable.py
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testclassselector.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testcolorparameter.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testcomparator.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testcompositeparams.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testcustomparam.py
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testdateparam.py
+-rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testdaterangeparam.py
+-rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testdefaults.py
+-rw-r--r--   0        0        0    12920 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testdeprecations.py
+-rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testdynamicparams.py
+-rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testfiledeserialization.py
+-rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testfileselector.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testipythonmagic.py
+-rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testjsonserialization.py
+-rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testlist.py
+-rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testlistselector.py
+-rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testmultifileselector.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testnumbergen.py
+-rw-r--r--   0        0        0    21644 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testnumberparameter.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testnumpy.py
+-rw-r--r--   0        0        0    19778 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testobjectselector.py
+-rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testpandas.py
+-rw-r--r--   0        0        0    40700 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testparamdepends.py
+-rw-r--r--   0        0        0    45849 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testparameterizedobject.py
+-rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testparameterizedrepr.py
+-rw-r--r--   0        0        0     6781 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testparamoutput.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testparamunion.py
+-rw-r--r--   0        0        0    13748 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testpathparam.py
+-rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testpickle.py
+-rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testrangeparameter.py
+-rw-r--r--   0        0        0    16534 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testreactive.py
+-rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testrefs.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testreprhtml.py
+-rw-r--r--   0        0        0    14046 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testselector.py
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testsignatures.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/teststringparam.py
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testtimedependent.py
+-rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testtupleparam.py
+-rw-r--r--   0        0        0    11539 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testutils.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testversion.py
+-rw-r--r--   0        0        0    32010 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/testwatch.py
+-rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 param-2.1.0rc1/tests/utils.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 param-2.1.0rc1/.gitignore
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 param-2.1.0rc1/LICENSE.txt
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 param-2.1.0rc1/README.md
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 param-2.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 param-2.1.0rc1/PKG-INFO
```

### Comparing `param-2.1.0a2/numbergen/__init__.py` & `param-2.1.0rc1/numbergen/__init__.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/param/__init__.py` & `param-2.1.0rc1/param/__init__.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/param/_utils.py` & `param-2.1.0rc1/param/_utils.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/param/depends.py` & `param-2.1.0rc1/param/depends.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/param/display.py` & `param-2.1.0rc1/param/display.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/param/ipython.py` & `param-2.1.0rc1/param/ipython.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/param/parameterized.py` & `param-2.1.0rc1/param/parameterized.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,19 +160,21 @@
         arg_deps = function._dinfo['dependencies']
         kw_deps = function._dinfo.get('kw', {})
         if kw_deps or any(isinstance(d, Parameter) for d in arg_deps):
             args = (getattr(dep.owner, dep.name) for dep in arg_deps)
             kwargs = {n: getattr(dep.owner, dep.name) for n, dep in kw_deps.items()}
     return function(*args, **kwargs)
 
-def resolve_value(value):
+def resolve_value(value, recursive=True):
     """
     Resolves the current value of a dynamic reference.
     """
-    if isinstance(value, (list, tuple)):
+    if not recursive:
+        pass
+    elif isinstance(value, (list, tuple)):
         return type(value)(resolve_value(v) for v in value)
     elif isinstance(value, dict):
         return type(value)((resolve_value(k), resolve_value(v)) for k, v in value.items())
     elif isinstance(value, slice):
         return slice(
             resolve_value(value.start),
             resolve_value(value.stop),
@@ -2003,22 +2005,23 @@
         self_._setup_refs(deps)
         self_.self._param__private.refs = refs
 
     def _sync_refs(self_, *events):
         updates = {}
         for pname, ref in self_.self._param__private.refs.items():
             # Skip updating value if dependency has not changed
-            deps = resolve_ref(ref, self_[pname].nested_refs)
+            recursive = self_[pname].nested_refs
+            deps = resolve_ref(ref, recursive)
             is_gen = inspect.isgeneratorfunction(ref)
             is_async = iscoroutinefunction(ref) or is_gen
             if not any((dep.owner is e.obj and dep.name == e.name) for dep in deps for e in events) and not is_async:
                 continue
 
             try:
-                new_val = resolve_value(ref)
+                new_val = resolve_value(ref, recursive)
             except Skip:
                 new_val = Undefined
             if new_val is Skip or new_val is Undefined:
                 continue
             elif is_async:
                 async_executor(partial(self_._async_ref, pname, new_val))
                 continue
@@ -2033,15 +2036,15 @@
         is_gen = inspect.isgeneratorfunction(value)
         is_async = iscoroutinefunction(value) or is_gen
         deps = resolve_ref(value, recursive=pobj.nested_refs)
         if not (deps or is_async or is_gen):
             return None, None, value, False
         ref = value
         try:
-            value = resolve_value(value)
+            value = resolve_value(value, recursive=pobj.nested_refs)
         except Skip:
             value = Undefined
         if is_async:
             async_executor(partial(self_._async_ref, pobj.name, value))
             value = None
         return ref, deps, value, is_async
```

### Comparing `param-2.1.0a2/param/parameters.py` & `param-2.1.0rc1/param/parameters.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/param/reactive.py` & `param-2.1.0rc1/param/reactive.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,48 +86,100 @@
 import operator
 
 from collections.abc import Iterable, Iterator
 from functools import partial
 from types import FunctionType, MethodType
 from typing import Any, Callable, Optional
 
-from . import Event
 from .depends import depends
 from .display import _display_accessors, _reactive_display_objs
 from .parameterized import (
     Parameter, Parameterized, Skip, Undefined, eval_function_with_deps, get_method_owner,
     register_reference_transform, resolve_ref, resolve_value, transform_reference
 )
+from .parameters import Boolean, Event
 from ._utils import iscoroutinefunction, full_groupby
 
 
 class Wrapper(Parameterized):
     """
-    Simple wrapper to allow updating literal values easily.
+    Helper class to allow updating literal values easily.
     """
 
     object = Parameter(allow_refs=False)
 
 
 class GenWrapper(Parameterized):
     """
-    Wrapper to allow streaming from generator functions.
+    Helper class to allow streaming from generator functions.
     """
 
     object = Parameter(allow_refs=True)
 
 
 class Trigger(Parameterized):
+    """
+    Helper class to allow triggering an event under some condition.
+    """
 
     value = Event()
 
     def __init__(self, parameters, **params):
         super().__init__(**params)
         self.parameters = parameters
 
+class Resolver(Parameterized):
+    """
+    Helper class to allow (recursively) resolving references.
+    """
+
+    object = Parameter(allow_refs=True)
+
+    recursive = Boolean(default=False)
+
+    value = Parameter()
+
+    def __init__(self, **params):
+        self._watchers = []
+        super().__init__(**params)
+
+    def _resolve_value(self, *events):
+        nested = self.param.object.nested_refs
+        refs = resolve_ref(self.object, nested)
+        value = resolve_value(self.object, nested)
+        if self.recursive:
+            new_refs = [r for r in resolve_ref(value, nested) if r not in refs]
+            while new_refs:
+                refs += new_refs
+                value = resolve_value(value, nested)
+                new_refs = [r for r in resolve_ref(value, nested) if r not in refs]
+            if events:
+                self._update_refs(refs)
+        self.value = value
+        return refs
+
+    @depends('object', watch=True, on_init=True)
+    def _resolve_object(self):
+        refs = self._resolve_value()
+        self._update_refs(refs)
+
+    def _update_refs(self, refs):
+        for w in self._watchers:
+            (w.inst or w.cls).param.unwatch(w)
+        self._watchers = []
+        for _, params in full_groupby(refs, lambda x: id(x.owner)):
+            self._watchers.append(
+                params[0].owner.param.watch(self._resolve_value, [p.name for p in params])
+            )
+
+
+class NestedResolver(Resolver):
+
+    object = Parameter(allow_refs=True, nested_refs=True)
+
 
 class reactive_ops:
     """
     Namespace for reactive operators.
 
     Implements operators that cannot be implemented using regular
     Python syntax.
@@ -231,14 +283,35 @@
         args: iterable, optional
           Positional arguments to pass to `func`.
         kwargs: mapping, optional
           A dictionary of keywords to pass to `func`.
         """
         return self._as_rx()._apply_operator(func, *args, **kwargs)
 
+    def resolve(self, nested=True, recursive=False):
+        """
+        Resolves references held by the expression.
+
+        As an example if the expression returns a list of parameters
+        this operation will return a list of the parameter values.
+
+        Arguments
+        ---------
+        nested: bool
+          Whether to resolve references contained within nested objects,
+          i.e. tuples, lists, sets and dictionaries.
+        recursive: bool
+          Whether to recursively resolve references, i.e. if a reference
+          itself returns a reference we recurse into it until no more
+          references can be resolved.
+        """
+        resolver_type = NestedResolver if nested else Resolver
+        resolver = resolver_type(object=self._reactive, recursive=recursive)
+        return resolver.param.value.rx()
+
     def updating(self):
         """
         Returns a new expression that is True while the expression is updating.
         """
         wrapper = Wrapper(object=False)
         self._watch(lambda e: wrapper.param.update(object=True), precedence=-999)
         self._watch(lambda e: wrapper.param.update(object=False), precedence=999)
@@ -759,15 +832,17 @@
            it has to re-evaluate the pipeline. This is done by marking
            the pipeline as `_dirty`. The next time the `_current` value
            is requested the value is resolved by re-executing the
            pipeline.
         """
         if self._fn is not None:
             for _, params in full_groupby(self._fn_params, lambda x: id(x.owner)):
-                params[0].owner.param._watch(self._invalidate_obj, [p.name for p in params], precedence=-1)
+                fps = [p.name for p in params if p in self._root._fn_params]
+                if fps:
+                    params[0].owner.param._watch(self._invalidate_obj, fps, precedence=-1)
         for _, params in full_groupby(self._internal_params, lambda x: id(x.owner)):
             params[0].owner.param._watch(self._invalidate_current, [p.name for p in params], precedence=-1)
 
     def _invalidate_current(self, *events):
         self._dirty = True
         self._error_state = None
 
@@ -786,14 +861,15 @@
                     raise Skip
                 operation = self._operation
                 if operation:
                     obj = self._eval_operation(obj, operation)
                     if obj is Skip:
                         raise Skip
             except Skip:
+                self._dirty = False
                 return self._current_
             except Exception as e:
                 self._error_state = e
                 raise e
             self._current_ = current = obj
         else:
             current = self._current_
```

### Comparing `param-2.1.0a2/param/serializer.py` & `param-2.1.0rc1/param/serializer.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/param/version.py` & `param-2.1.0rc1/param/version.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testaddparameter.py` & `param-2.1.0rc1/tests/testaddparameter.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testbind.py` & `param-2.1.0rc1/tests/testbind.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testbooleanparam.py` & `param-2.1.0rc1/tests/testbooleanparam.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testbytesparam.py` & `param-2.1.0rc1/tests/testbytesparam.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testcalendardateparam.py` & `param-2.1.0rc1/tests/testcalendardateparam.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testcalendardaterangeparam.py` & `param-2.1.0rc1/tests/testcalendardaterangeparam.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testclassselector.py` & `param-2.1.0rc1/tests/testclassselector.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testcolorparameter.py` & `param-2.1.0rc1/tests/testcolorparameter.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testcomparator.py` & `param-2.1.0rc1/tests/testcomparator.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testcompositeparams.py` & `param-2.1.0rc1/tests/testcompositeparams.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testcustomparam.py` & `param-2.1.0rc1/tests/testcustomparam.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testdateparam.py` & `param-2.1.0rc1/tests/testdateparam.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testdaterangeparam.py` & `param-2.1.0rc1/tests/testdaterangeparam.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testdefaults.py` & `param-2.1.0rc1/tests/testdefaults.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testdeprecations.py` & `param-2.1.0rc1/tests/testdeprecations.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testdynamicparams.py` & `param-2.1.0rc1/tests/testdynamicparams.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testfiledeserialization.py` & `param-2.1.0rc1/tests/testfiledeserialization.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testfileselector.py` & `param-2.1.0rc1/tests/testfileselector.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testipythonmagic.py` & `param-2.1.0rc1/tests/testipythonmagic.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testjsonserialization.py` & `param-2.1.0rc1/tests/testjsonserialization.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testlist.py` & `param-2.1.0rc1/tests/testlist.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testlistselector.py` & `param-2.1.0rc1/tests/testlistselector.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testmultifileselector.py` & `param-2.1.0rc1/tests/testmultifileselector.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testnumbergen.py` & `param-2.1.0rc1/tests/testnumbergen.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testnumberparameter.py` & `param-2.1.0rc1/tests/testnumberparameter.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testnumpy.py` & `param-2.1.0rc1/tests/testnumpy.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testobjectselector.py` & `param-2.1.0rc1/tests/testobjectselector.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testpandas.py` & `param-2.1.0rc1/tests/testpandas.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testparamdepends.py` & `param-2.1.0rc1/tests/testparamdepends.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testparameterizedobject.py` & `param-2.1.0rc1/tests/testparameterizedobject.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testparameterizedrepr.py` & `param-2.1.0rc1/tests/testparameterizedrepr.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testparamoutput.py` & `param-2.1.0rc1/tests/testparamoutput.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testparamunion.py` & `param-2.1.0rc1/tests/testparamunion.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testpathparam.py` & `param-2.1.0rc1/tests/testpathparam.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testpickle.py` & `param-2.1.0rc1/tests/testpickle.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testrangeparameter.py` & `param-2.1.0rc1/tests/testrangeparameter.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testreactive.py` & `param-2.1.0rc1/tests/testreactive.py`

 * *Files 20% similar despite different names*

```diff
@@ -63,14 +63,16 @@
 
     number = param.Number(default=3.14)
 
     function = param.Callable()
 
     boolean = param.Boolean(default=False)
 
+    parameter = param.Parameter(allow_refs=False)
+
     event = param.Event()
 
     @param.depends('integer')
     def multiply_integer(self):
         return self.integer * 2
 
 @pytest.mark.parametrize('op', NUMERIC_BINARY_OPERATORS)
@@ -429,14 +431,104 @@
     integer = p.param.integer.rx().rx.when(p.param.event, initial=None)
     assert integer.rx.value is None
     p.integer = 4
     assert integer.rx.value is None
     p.param.trigger('event')
     assert integer.rx.value == 4
 
+def test_reactive_resolve():
+    p = Parameters(integer=3)
+    p2 = Parameters(parameter=p.param.integer)
+
+    prx = p2.param.parameter.rx()
+    assert prx.rx.value is p.param.integer
+
+    resolved_prx = prx.rx.resolve()
+    assert resolved_prx.rx.value == 3
+
+    changes = []
+    resolved_prx.rx.watch(changes.append)
+
+    # Test changing referenced value
+    p.integer = 4
+    assert resolved_prx.rx.value == 4
+    assert changes == [4]
+
+    # Test changing reference itself
+    p2.parameter = p.param.number
+    assert resolved_prx.rx.value == 3.14
+    assert changes == [4, 3.14]
+
+    # Ensure no updates triggered when old reference is updated
+    p.integer = 5
+    assert resolved_prx.rx.value == 3.14
+    assert changes == [4, 3.14]
+
+def test_reactive_resolve_nested():
+    p = Parameters(integer=3)
+    p2 = Parameters(parameter=[p.param.integer])
+
+    prx = p2.param.parameter.rx()
+    assert prx.rx.value == [p.param.integer]
+
+    resolved_prx = prx.rx.resolve(nested=True)
+    assert resolved_prx.rx.value == [3]
+
+    changes = []
+    resolved_prx.rx.watch(changes.append)
+
+    # Test changing referenced value
+    p.integer = 4
+    assert resolved_prx.rx.value == [4]
+    assert changes == [[4]]
+
+    # Test changing reference itself
+    p2.parameter = [p.param.number]
+    assert resolved_prx.rx.value == [3.14]
+    assert changes == [[4], [3.14]]
+
+    # Ensure no updates triggered when old reference is updated
+    p.integer = 5
+    assert resolved_prx.rx.value == [3.14]
+    assert changes == [[4], [3.14]]
+
+def test_reactive_resolve_recursive():
+    p = Parameters(integer=3)
+    p2 = Parameters(parameter=p.param.integer)
+    p3 = Parameters(parameter=p2.param.parameter)
+
+    prx = p3.param.parameter.rx()
+    assert prx.rx.value is p2.param.parameter
+
+    resolved_prx = prx.rx.resolve(recursive=True)
+    assert resolved_prx.rx.value == 3
+
+    changes = []
+    resolved_prx.rx.watch(changes.append)
+
+    # Test changing referenced value
+    p.integer = 4
+    assert resolved_prx.rx.value == 4
+    assert changes == [4]
+
+    # Test changing recursive reference
+    p2.parameter = p.param.number
+    assert resolved_prx.rx.value == 3.14
+    assert changes == [4, 3.14]
+
+    # Ensure no updates triggered when old reference is updated
+    p.integer = 5
+    assert resolved_prx.rx.value == 3.14
+    assert changes == [4, 3.14]
+
+    # Test changing reference itself
+    p3.parameter = p.param.string
+    assert resolved_prx.rx.value == 'string'
+    assert changes == [4, 3.14, 'string']
+
 async def test_reactive_async_func():
     async def async_func():
         await asyncio.sleep(0.02)
         return 2
 
     async_rx = rx(async_func) + 2
     assert async_rx.rx.value is param.Undefined
@@ -504,7 +596,30 @@
     await asyncio.sleep(0.05)
     assert rxgen.rx.value == 1
     irx.rx.value = 3
     await asyncio.sleep(0.05)
     irx.rx.value = 4
     await asyncio.sleep(0.1)
     assert rxgen.rx.value == 5
+
+def test_root_invalidation():
+    arx = rx('a')
+    brx = rx('b')
+
+    computed = []
+    def debug(value, info):
+        computed.append(info)
+        return value
+
+    expr = arx.title().rx.pipe(debug, '1') + brx.title().rx.pipe(debug, '2')
+
+    assert expr.rx.value == 'AB'
+    assert computed == ['1', '2']
+
+    brx.rx.value = 'c'
+
+    assert expr.rx.value == 'AC'
+    assert computed == ['1', '2', '2']
+
+    arx.rx.value = 'd'
+    assert expr.rx.value == 'DC'
+    assert computed == ['1', '2', '2', '1']
```

### Comparing `param-2.1.0a2/tests/testrefs.py` & `param-2.1.0rc1/tests/testrefs.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testreprhtml.py` & `param-2.1.0rc1/tests/testreprhtml.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testselector.py` & `param-2.1.0rc1/tests/testselector.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testsignatures.py` & `param-2.1.0rc1/tests/testsignatures.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/teststringparam.py` & `param-2.1.0rc1/tests/teststringparam.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testtimedependent.py` & `param-2.1.0rc1/tests/testtimedependent.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testtupleparam.py` & `param-2.1.0rc1/tests/testtupleparam.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testutils.py` & `param-2.1.0rc1/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/testwatch.py` & `param-2.1.0rc1/tests/testwatch.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/tests/utils.py` & `param-2.1.0rc1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/LICENSE.txt` & `param-2.1.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/README.md` & `param-2.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/pyproject.toml` & `param-2.1.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `param-2.1.0a2/PKG-INFO` & `param-2.1.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: param
-Version: 2.1.0a2
+Version: 2.1.0rc1
 Summary: Make your Python code clearer and more reliable by declaring Parameters.
 Project-URL: Homepage, https://param.holoviz.org/
 Project-URL: Tracker, https://github.com/holoviz/param/issues
 Project-URL: Releases, https://github.com/holoviz/param/releases
 Project-URL: Source, https://github.com/holoviz/param
 Project-URL: HoloViz, https://holoviz.org/
 Author-email: HoloViz <developers@holoviz.org>
```

