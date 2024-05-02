# Comparing `tmp/timed_decorator-1.4.0.tar.gz` & `tmp/timed_decorator-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timed_decorator-1.4.0.tar", last modified: Wed May  1 09:05:04 2024, max compression
+gzip compressed data, was "timed_decorator-1.5.0.tar", last modified: Thu May  2 19:41:25 2024, max compression
```

## Comparing `timed_decorator-1.4.0.tar` & `timed_decorator-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:05:04.843890 timed_decorator-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-05-01 09:05:04.843890 timed_decorator-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 09:05:04.843890 timed_decorator-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:05:04.843890 timed_decorator-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/tests/test_usage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:05:04.843890 timed_decorator-1.4.0/timed_decorator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/timed_decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/timed_decorator/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/timed_decorator/nested_timed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/timed_decorator/simple_timed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-01 09:04:57.000000 timed_decorator-1.4.0/timed_decorator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:05:04.843890 timed_decorator-1.4.0/timed_decorator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17096 2024-05-01 09:05:04.000000 timed_decorator-1.4.0/timed_decorator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-01 09:05:04.000000 timed_decorator-1.4.0/timed_decorator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:05:04.000000 timed_decorator-1.4.0/timed_decorator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 09:05:04.000000 timed_decorator-1.4.0/timed_decorator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 09:05:04.000000 timed_decorator-1.4.0/timed_decorator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:41:25.033379 timed_decorator-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-02 19:41:25.033379 timed_decorator-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15808 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:41:25.033379 timed_decorator-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:41:25.029379 timed_decorator-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/tests/test_usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:41:25.029379 timed_decorator-1.5.0/timed_decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/timed_decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/timed_decorator/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/timed_decorator/nested_timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/timed_decorator/simple_timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-02 19:41:06.000000 timed_decorator-1.5.0/timed_decorator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:41:25.033379 timed_decorator-1.5.0/timed_decorator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-02 19:41:25.000000 timed_decorator-1.5.0/timed_decorator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-02 19:41:25.000000 timed_decorator-1.5.0/timed_decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:41:25.000000 timed_decorator-1.5.0/timed_decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 19:41:25.000000 timed_decorator-1.5.0/timed_decorator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 19:41:25.000000 timed_decorator-1.5.0/timed_decorator.egg-info/top_level.txt
```

### Comparing `timed_decorator-1.4.0/LICENSE` & `timed_decorator-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timed_decorator-1.4.0/PKG-INFO` & `timed_decorator-1.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timed-decorator
-Version: 1.4.0
+Version: 1.5.0
 Summary: A timing decorator for python functions.
 Author-email: George Stoica <george.stoica@senticlab.com>
 Maintainer-email: George Stoica <george.stoica@senticlab.com>
 License: Copyright (c) 2024 George Stoica
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
@@ -21,15 +21,16 @@
         EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
         MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
         NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
         LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
         OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
         WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
-Project-URL: repository, https://github.com/ancestor-mithril/timed-decorator
+Project-URL: Repository, https://github.com/ancestor-mithril/timed-decorator
+Project-URL: Issues, https://github.com/ancestor-mithril/timed-decorator/issues
 Keywords: timing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -37,15 +38,15 @@
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 
 # timed-decorator
 
-Simple and configurable timing decorator with little overhead that can be easily attached to python functions to measure their execution time.
+Simple and configurable timing decorator with little overhead that can be attached to python functions to measure their execution time.
 Can easily display parameter types and lengths if available and is compatible with NumPy ndarrays, Pandas DataFrames and PyTorch tensors.
 
 
 ## Installation
 
 ```
 pip install --upgrade timed-decorator
@@ -86,15 +87,15 @@
     * `show_kwargs` (`bool`): If `True`, displays the keyword arguments according to `display_level`. Default: `False`.
     * `display_level` (`int`): The level of verbosity used when printing function arguments ad keyword arguments. If `0`, prints the type of the parameters. If `1`, prints values for all primitive types, shapes for arrays, tensors, dataframes and length for sequences. Otherwise, prints values for all parameters. Default: `1`.
     * `sep` (`str`): The separator used when printing function arguments and keyword arguments. Default: `', '`.
     * `stdout` (`bool`): If `True`, writes the elapsed time to stdout. Default: `True`.
     * `file_path` (`str`): If not `None`, writes the measurement at the end of the given file path. For thread safe file writing configure use `logger_name` instead. Default: `None`.
     * `logger_name` (`str`): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. Default: `None`. See [Using a logger](#using-a-logger).
     * `return_time` (`bool`): If `True`, returns the elapsed time in addition to the wrapped function's return value. Default: `False`.
-    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the fully qualified function name as key.  If the key already exists, adds the time to the existing value. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
+    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the fully qualified function name as key, in the following format: (function call counts, total elapsed time, total "own time"). If the key already exists, updates the existing value. The elapsed time is equal to "own time" for the simple timed decorator. For the nested time decorator, the elapsed time is different from "own time" only when another function decorated with a nested timer is called during the execution of the current function. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
     * `use_qualname` (`bool`): If `True`, If `True`, uses the qualified name of the function when logging the elapsed time. Default: `False`.
 
 2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after subtracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
 
 3. `create_timed_decorator` registers a timed decorator with a given name.
    * `name` (`str`): The name of the timed decorator which will be instantiated using the provided arguments. Use this name for retrieving the timed decorator with `timed_decorator.builder.get_timed_decorator`.
    * `nested` (`bool`): If `True`, uses the `timed_decorator.nested_timed.nested_timed` as decorator, otherwise uses `timed_decorator.simple_timed.timed`. Default: `False`.
@@ -447,16 +448,16 @@
 fn()
 print(ns)
 fn()
 print(ns)
 ```
 Prints
 ```
-{'fn': 1000767300}
-{'fn': 2001006100}
+{'fn': [1, 1000672000, 1000672000]}
+{'fn': [2, 2001306900, 2001306900]}
 ```
 
 ### Compatible with PyTorch tensors
 
 Synchronizes cuda device when cuda tensors are passed as function parameters.
 
 ```py
@@ -523,58 +524,59 @@
     nested_function()
     function_1()
 
 
 if __name__ == '__main__':
     my_measurements = {}
     create_timed_decorator("MyCustomTimer",
+                           nested=False,  # This is true by default
                            collect_gc=False,  # I don't want to explicitly collect garbage
                            disable_gc=True,  # I don't want to wait for garbage collection during measuring
                            stdout=False,  # I don't wat to print stuff to console
                            out=my_measurements  # My measurements dict
                            )
     main()
-    for key, value in my_measurements.items():
-        print(f'Function {key} took {value / 1e+9}s')
-    print()
+    for key, (counts, elapsed, own_time) in my_measurements.items():
+        print(f'Function {key} was called {counts} time(s) and took {elapsed / 1e+9}s')
     print()
 
     # Now I can do stuff with my measurements.
     functions = sorted(my_measurements.keys(), reverse=True)
 
     for i in range(len(functions)):
         fn_1 = functions[i]
         print(f'Function {fn_1}:')
         for j in range(i + 1, len(functions)):
             fn_2 = functions[j]
             if fn_1.startswith(fn_2):
-                ratio = my_measurements[fn_1] / my_measurements[fn_2] * 100
+                _, elapsed_1, _ = my_measurements[fn_1]
+                _, elapsed_2, _ = my_measurements[fn_2]
+                ratio = elapsed_1 / elapsed_2 * 100
                 print(f'* took {ratio:.2f}% from {fn_2}')
         print()
 ```
 
 Prints:
 ```
-Function main.<locals>.nested_function.<locals>.function_2 took 0.8016428s
-Function main.<locals>.nested_function.<locals>.function_3 took 0.6014647s
-Function main.<locals>.nested_function took 1.403586s
-Function main.<locals>.function_1 took 0.2006981s
-Function main took 1.6045189s
-
+Function main.<locals>.nested_function.<locals>.function_2 was called 4 time(s) and took 0.8019482s
+Function main.<locals>.nested_function.<locals>.function_3 was called 2 time(s) and took 0.6010157s
+Function main.<locals>.nested_function was called 2 time(s) and took 1.403365s
+Function main.<locals>.function_1 was called 2 time(s) and took 0.2007625s
+Function main was called 1 time(s) and took 1.6043592s
 
 Function main.<locals>.nested_function.<locals>.function_3:
-* took 42.85% from main.<locals>.nested_function
-* took 37.49% from main
+* took 42.83% from main.<locals>.nested_function
+* took 37.46% from main
 
 Function main.<locals>.nested_function.<locals>.function_2:
-* took 57.11% from main.<locals>.nested_function
-* took 49.96% from main
+* took 57.14% from main.<locals>.nested_function
+* took 49.99% from main
 
 Function main.<locals>.nested_function:
-* took 87.48% from main
+* took 87.47% from main
 
 Function main.<locals>.function_1:
 * took 12.51% from main
 
 Function main:
 
 ```
```

### Comparing `timed_decorator-1.4.0/README.md` & `timed_decorator-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # timed-decorator
 
-Simple and configurable timing decorator with little overhead that can be easily attached to python functions to measure their execution time.
+Simple and configurable timing decorator with little overhead that can be attached to python functions to measure their execution time.
 Can easily display parameter types and lengths if available and is compatible with NumPy ndarrays, Pandas DataFrames and PyTorch tensors.
 
 
 ## Installation
 
 ```
 pip install --upgrade timed-decorator
@@ -45,15 +45,15 @@
     * `show_kwargs` (`bool`): If `True`, displays the keyword arguments according to `display_level`. Default: `False`.
     * `display_level` (`int`): The level of verbosity used when printing function arguments ad keyword arguments. If `0`, prints the type of the parameters. If `1`, prints values for all primitive types, shapes for arrays, tensors, dataframes and length for sequences. Otherwise, prints values for all parameters. Default: `1`.
     * `sep` (`str`): The separator used when printing function arguments and keyword arguments. Default: `', '`.
     * `stdout` (`bool`): If `True`, writes the elapsed time to stdout. Default: `True`.
     * `file_path` (`str`): If not `None`, writes the measurement at the end of the given file path. For thread safe file writing configure use `logger_name` instead. Default: `None`.
     * `logger_name` (`str`): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. Default: `None`. See [Using a logger](#using-a-logger).
     * `return_time` (`bool`): If `True`, returns the elapsed time in addition to the wrapped function's return value. Default: `False`.
-    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the fully qualified function name as key.  If the key already exists, adds the time to the existing value. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
+    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the fully qualified function name as key, in the following format: (function call counts, total elapsed time, total "own time"). If the key already exists, updates the existing value. The elapsed time is equal to "own time" for the simple timed decorator. For the nested time decorator, the elapsed time is different from "own time" only when another function decorated with a nested timer is called during the execution of the current function. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
     * `use_qualname` (`bool`): If `True`, If `True`, uses the qualified name of the function when logging the elapsed time. Default: `False`.
 
 2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after subtracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
 
 3. `create_timed_decorator` registers a timed decorator with a given name.
    * `name` (`str`): The name of the timed decorator which will be instantiated using the provided arguments. Use this name for retrieving the timed decorator with `timed_decorator.builder.get_timed_decorator`.
    * `nested` (`bool`): If `True`, uses the `timed_decorator.nested_timed.nested_timed` as decorator, otherwise uses `timed_decorator.simple_timed.timed`. Default: `False`.
@@ -406,16 +406,16 @@
 fn()
 print(ns)
 fn()
 print(ns)
 ```
 Prints
 ```
-{'fn': 1000767300}
-{'fn': 2001006100}
+{'fn': [1, 1000672000, 1000672000]}
+{'fn': [2, 2001306900, 2001306900]}
 ```
 
 ### Compatible with PyTorch tensors
 
 Synchronizes cuda device when cuda tensors are passed as function parameters.
 
 ```py
@@ -482,58 +482,59 @@
     nested_function()
     function_1()
 
 
 if __name__ == '__main__':
     my_measurements = {}
     create_timed_decorator("MyCustomTimer",
+                           nested=False,  # This is true by default
                            collect_gc=False,  # I don't want to explicitly collect garbage
                            disable_gc=True,  # I don't want to wait for garbage collection during measuring
                            stdout=False,  # I don't wat to print stuff to console
                            out=my_measurements  # My measurements dict
                            )
     main()
-    for key, value in my_measurements.items():
-        print(f'Function {key} took {value / 1e+9}s')
-    print()
+    for key, (counts, elapsed, own_time) in my_measurements.items():
+        print(f'Function {key} was called {counts} time(s) and took {elapsed / 1e+9}s')
     print()
 
     # Now I can do stuff with my measurements.
     functions = sorted(my_measurements.keys(), reverse=True)
 
     for i in range(len(functions)):
         fn_1 = functions[i]
         print(f'Function {fn_1}:')
         for j in range(i + 1, len(functions)):
             fn_2 = functions[j]
             if fn_1.startswith(fn_2):
-                ratio = my_measurements[fn_1] / my_measurements[fn_2] * 100
+                _, elapsed_1, _ = my_measurements[fn_1]
+                _, elapsed_2, _ = my_measurements[fn_2]
+                ratio = elapsed_1 / elapsed_2 * 100
                 print(f'* took {ratio:.2f}% from {fn_2}')
         print()
 ```
 
 Prints:
 ```
-Function main.<locals>.nested_function.<locals>.function_2 took 0.8016428s
-Function main.<locals>.nested_function.<locals>.function_3 took 0.6014647s
-Function main.<locals>.nested_function took 1.403586s
-Function main.<locals>.function_1 took 0.2006981s
-Function main took 1.6045189s
-
+Function main.<locals>.nested_function.<locals>.function_2 was called 4 time(s) and took 0.8019482s
+Function main.<locals>.nested_function.<locals>.function_3 was called 2 time(s) and took 0.6010157s
+Function main.<locals>.nested_function was called 2 time(s) and took 1.403365s
+Function main.<locals>.function_1 was called 2 time(s) and took 0.2007625s
+Function main was called 1 time(s) and took 1.6043592s
 
 Function main.<locals>.nested_function.<locals>.function_3:
-* took 42.85% from main.<locals>.nested_function
-* took 37.49% from main
+* took 42.83% from main.<locals>.nested_function
+* took 37.46% from main
 
 Function main.<locals>.nested_function.<locals>.function_2:
-* took 57.11% from main.<locals>.nested_function
-* took 49.96% from main
+* took 57.14% from main.<locals>.nested_function
+* took 49.99% from main
 
 Function main.<locals>.nested_function:
-* took 87.48% from main
+* took 87.47% from main
 
 Function main.<locals>.function_1:
 * took 12.51% from main
 
 Function main:
 
 ```
```

### Comparing `timed_decorator-1.4.0/pyproject.toml` & `timed_decorator-1.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "timed-decorator"
-version = "1.4.0"
+version = "1.5.0"
 #requires-python = ">=3.10"
 requires-python = ">=3.7"
 description = "A timing decorator for python functions."
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "George Stoica", email = "george.stoica@senticlab.com" },
@@ -21,15 +21,16 @@
 ]
 
 keywords = [
     'timing',
 ]
 
 [project.urls]
-repository = "https://github.com/ancestor-mithril/timed-decorator"
+Repository = "https://github.com/ancestor-mithril/timed-decorator"
+Issues = "https://github.com/ancestor-mithril/timed-decorator/issues"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "flake8"
 ]
```

### Comparing `timed_decorator-1.4.0/tests/test_usage.py` & `timed_decorator-1.5.0/tests/test_usage.py`

 * *Files 20% similar despite different names*

```diff
@@ -102,25 +102,55 @@
         logged = log_stream.getvalue().split('\n')[:-1]
         self.assertEqual(len(logged), 2)
         self.assertIn(fn_1.__name__, logged[0])
         self.assertNotIn(fn_1.__qualname__, logged[0])
         self.assertIn(fn_2.__name__, logged[1])
         self.assertIn(fn_2.__qualname__, logged[1])
 
-    def test_ns_output(self):
+    def test_dict_output(self):
         out = {}
 
         @timed(out=out, stdout=False)
         def fn():
             sleep(0.1)
 
         fn()
 
-        self.assertIsInstance(out[fn.__qualname__], int)
-        self.assertGreater(out[fn.__qualname__], 1e+8)
+        counts, elapsed, own_time = out[fn.__qualname__]
+        self.assertEqual(counts, 1)
+        self.assertIsInstance(elapsed, int)
+        self.assertGreater(elapsed, 1e+8)
+        self.assertEqual(elapsed, own_time)
+
+        fn()
+        counts, elapsed, own_time = out[fn.__qualname__]
+        self.assertEqual(counts, 2)
+        self.assertIsInstance(elapsed, int)
+        self.assertGreater(elapsed, 2e+8)
+        self.assertEqual(elapsed, own_time)
+
+    def test_dict_output_with_nested_timed(self):
+        out = {}
+
+        @nested_timed(out=out, stdout=False)
+        def fn1():
+            @nested_timed(out=out, stdout=False)
+            def fn2():
+                sleep(0.1)
+
+            fn2()
+
+        fn1()
+
+        counts_1, elapsed_1, own_time_1 = out[fn1.__qualname__]
+        counts_2, elapsed_2, own_time_2 = out[fn1.__qualname__ + '.<locals>.fn2']
+
+        self.assertTrue(counts_1 == counts_2 == 1)
+        self.assertEqual(own_time_2, elapsed_2)
+        self.assertGreater(elapsed_1, own_time_1)
 
     def test_qualname(self):
         out = {}
 
         class ClassA:
             @timed(out=out)
             def wait(self, x):
```

### Comparing `timed_decorator-1.4.0/timed_decorator/builder.py` & `timed_decorator-1.5.0/timed_decorator/builder.py`

 * *Files identical despite different names*

### Comparing `timed_decorator-1.4.0/timed_decorator/nested_timed.py` & `timed_decorator-1.5.0/timed_decorator/nested_timed.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import gc
 from functools import wraps
 from gc import collect
 from time import perf_counter_ns
 from typing import Union
 
-from .utils import nop, TimeFormatter, InputFormatter, synchronize_cuda, Logger, write_mutable
+from .utils import nop, TimeFormatter, InputFormatter, synchronize_cuda, Logger, update_timing_dict
 
 nested_level = 0
 nested_times = dict()
 
 
 def nested_timed(collect_gc: bool = True,
                  disable_gc: bool = False,
@@ -31,15 +31,15 @@
     See Also:
         :class:`timed_decorator.simple_timed.timed` for parameter documentation.
     """
     gc_collect = collect if collect_gc else nop
     time_formatter = TimeFormatter(use_seconds, precision)
     input_formatter = InputFormatter(show_args, show_kwargs, display_level, sep)
     logger = Logger(stdout, file_path, logger_name)
-    ns_out = write_mutable if out is not None else nop
+    update_dict = update_timing_dict if out is not None else nop
 
     def decorator(fn):
         @wraps(fn)
         def wrap(*args, **kwargs):
             global nested_level, nested_times
             nested_level += 1
 
@@ -71,15 +71,15 @@
 
             if nested_level != 0:
                 if nested_level not in nested_times:
                     nested_times[nested_level] = []
                 nested_times[nested_level].append(elapsed)
 
             fn_name = fn.__qualname__ if use_qualname else fn.__name__
-            ns_out(out, fn.__qualname__, elapsed)
+            update_dict(out, fn.__qualname__, elapsed, own_time)
             logger('\t' * nested_level + f'{input_formatter(fn_name, *args, **kwargs)} '
                                          f'-> total time: {time_formatter(elapsed)}, '
                                          f'own time: {time_formatter(own_time)}')
             if return_time:
                 return ret, elapsed
             return ret
```

### Comparing `timed_decorator-1.4.0/timed_decorator/simple_timed.py` & `timed_decorator-1.5.0/timed_decorator/simple_timed.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import gc
 from functools import wraps
 from gc import collect
 from time import perf_counter_ns
 from typing import Union
 
-from .utils import nop, TimeFormatter, InputFormatter, synchronize_cuda, Logger, write_mutable
+from .utils import nop, TimeFormatter, InputFormatter, synchronize_cuda, Logger, update_timing_dict
 
 
 def timed(collect_gc: bool = True,
           disable_gc: bool = False,
           use_seconds: bool = False,
           precision: int = 9,
           show_args: bool = False,
@@ -43,23 +43,27 @@
         file_path (str): If not `None`, writes the measurement at the end of the given file path. For thread safe
             file writing configure use `logger_name` instead. Default: `None`.
         logger_name (str): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction
             with `file_path`. Default: `None`.
         return_time (bool): If `True`, returns the elapsed time in addition to the wrapped function's return value.
             Default: `False`.
         out (dict): If not `None`, stores the elapsed time in nanoseconds in the given dict using the fully qualified
-            function name as key. If the key already exists, adds the time to the existing value. Default: `None`.
+            function name as key, in the following format: (function call counts, total elapsed time, total "own time").
+            If the key already exists, updates the existing value. The elapsed time is equal to "own time" for the simple
+            timed decorator. For the nested time decorator, the elapsed time is different from "own time" only when
+            another function decorated with a nested timer is called during the execution of the current function.
+            Default: `None`.
         use_qualname (bool): If `True`, uses the qualified name of the function when logging the elapsed time. Default:
             `False`.
     """
     gc_collect = collect if collect_gc else nop
     time_formatter = TimeFormatter(use_seconds, precision)
     input_formatter = InputFormatter(show_args, show_kwargs, display_level, sep)
     logger = Logger(stdout, file_path, logger_name)
-    ns_out = write_mutable if out is not None else nop
+    update_dict = update_timing_dict if out is not None else nop
 
     def decorator(fn):
         @wraps(fn)
         def wrap(*args, **kwargs):
             gc_collect()
             if disable_gc:
                 gc.disable()
@@ -71,15 +75,15 @@
                 end = perf_counter_ns()
             finally:
                 if disable_gc:
                     gc.enable()
 
             elapsed = end - start
             fn_name = fn.__qualname__ if use_qualname else fn.__name__
-            ns_out(out, fn.__qualname__, elapsed)
+            update_dict(out, fn.__qualname__, elapsed, elapsed)
             logger(f'{input_formatter(fn_name, *args, **kwargs)} -> total time: {time_formatter(elapsed)}')
             if return_time:
                 return ret, elapsed
             return ret
 
         return wrap
```

### Comparing `timed_decorator-1.4.0/timed_decorator/utils.py` & `timed_decorator-1.5.0/timed_decorator/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,9 +135,10 @@
     device = get_tensor_device(args)
     if device == '':
         device = get_tensor_device(kwargs.values())
     if device != '':
         torch.cuda.synchronize(device)
 
 
-def write_mutable(out: dict, key: str, value: int):
-    out[key] = out.get(key, 0) + value
+def update_timing_dict(out: dict, key: str, elapsed: int, own_time: int):
+    counts, elapsed_total, own_time_total = out.get(key, (0, 0, 0))
+    out[key] = [counts + 1, elapsed_total + elapsed, own_time_total + own_time]
```

### Comparing `timed_decorator-1.4.0/timed_decorator.egg-info/PKG-INFO` & `timed_decorator-1.5.0/timed_decorator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timed-decorator
-Version: 1.4.0
+Version: 1.5.0
 Summary: A timing decorator for python functions.
 Author-email: George Stoica <george.stoica@senticlab.com>
 Maintainer-email: George Stoica <george.stoica@senticlab.com>
 License: Copyright (c) 2024 George Stoica
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
@@ -21,15 +21,16 @@
         EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
         MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
         NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
         LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
         OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
         WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
-Project-URL: repository, https://github.com/ancestor-mithril/timed-decorator
+Project-URL: Repository, https://github.com/ancestor-mithril/timed-decorator
+Project-URL: Issues, https://github.com/ancestor-mithril/timed-decorator/issues
 Keywords: timing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -37,15 +38,15 @@
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 
 # timed-decorator
 
-Simple and configurable timing decorator with little overhead that can be easily attached to python functions to measure their execution time.
+Simple and configurable timing decorator with little overhead that can be attached to python functions to measure their execution time.
 Can easily display parameter types and lengths if available and is compatible with NumPy ndarrays, Pandas DataFrames and PyTorch tensors.
 
 
 ## Installation
 
 ```
 pip install --upgrade timed-decorator
@@ -86,15 +87,15 @@
     * `show_kwargs` (`bool`): If `True`, displays the keyword arguments according to `display_level`. Default: `False`.
     * `display_level` (`int`): The level of verbosity used when printing function arguments ad keyword arguments. If `0`, prints the type of the parameters. If `1`, prints values for all primitive types, shapes for arrays, tensors, dataframes and length for sequences. Otherwise, prints values for all parameters. Default: `1`.
     * `sep` (`str`): The separator used when printing function arguments and keyword arguments. Default: `', '`.
     * `stdout` (`bool`): If `True`, writes the elapsed time to stdout. Default: `True`.
     * `file_path` (`str`): If not `None`, writes the measurement at the end of the given file path. For thread safe file writing configure use `logger_name` instead. Default: `None`.
     * `logger_name` (`str`): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. Default: `None`. See [Using a logger](#using-a-logger).
     * `return_time` (`bool`): If `True`, returns the elapsed time in addition to the wrapped function's return value. Default: `False`.
-    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the fully qualified function name as key.  If the key already exists, adds the time to the existing value. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
+    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the fully qualified function name as key, in the following format: (function call counts, total elapsed time, total "own time"). If the key already exists, updates the existing value. The elapsed time is equal to "own time" for the simple timed decorator. For the nested time decorator, the elapsed time is different from "own time" only when another function decorated with a nested timer is called during the execution of the current function. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
     * `use_qualname` (`bool`): If `True`, If `True`, uses the qualified name of the function when logging the elapsed time. Default: `False`.
 
 2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after subtracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
 
 3. `create_timed_decorator` registers a timed decorator with a given name.
    * `name` (`str`): The name of the timed decorator which will be instantiated using the provided arguments. Use this name for retrieving the timed decorator with `timed_decorator.builder.get_timed_decorator`.
    * `nested` (`bool`): If `True`, uses the `timed_decorator.nested_timed.nested_timed` as decorator, otherwise uses `timed_decorator.simple_timed.timed`. Default: `False`.
@@ -447,16 +448,16 @@
 fn()
 print(ns)
 fn()
 print(ns)
 ```
 Prints
 ```
-{'fn': 1000767300}
-{'fn': 2001006100}
+{'fn': [1, 1000672000, 1000672000]}
+{'fn': [2, 2001306900, 2001306900]}
 ```
 
 ### Compatible with PyTorch tensors
 
 Synchronizes cuda device when cuda tensors are passed as function parameters.
 
 ```py
@@ -523,58 +524,59 @@
     nested_function()
     function_1()
 
 
 if __name__ == '__main__':
     my_measurements = {}
     create_timed_decorator("MyCustomTimer",
+                           nested=False,  # This is true by default
                            collect_gc=False,  # I don't want to explicitly collect garbage
                            disable_gc=True,  # I don't want to wait for garbage collection during measuring
                            stdout=False,  # I don't wat to print stuff to console
                            out=my_measurements  # My measurements dict
                            )
     main()
-    for key, value in my_measurements.items():
-        print(f'Function {key} took {value / 1e+9}s')
-    print()
+    for key, (counts, elapsed, own_time) in my_measurements.items():
+        print(f'Function {key} was called {counts} time(s) and took {elapsed / 1e+9}s')
     print()
 
     # Now I can do stuff with my measurements.
     functions = sorted(my_measurements.keys(), reverse=True)
 
     for i in range(len(functions)):
         fn_1 = functions[i]
         print(f'Function {fn_1}:')
         for j in range(i + 1, len(functions)):
             fn_2 = functions[j]
             if fn_1.startswith(fn_2):
-                ratio = my_measurements[fn_1] / my_measurements[fn_2] * 100
+                _, elapsed_1, _ = my_measurements[fn_1]
+                _, elapsed_2, _ = my_measurements[fn_2]
+                ratio = elapsed_1 / elapsed_2 * 100
                 print(f'* took {ratio:.2f}% from {fn_2}')
         print()
 ```
 
 Prints:
 ```
-Function main.<locals>.nested_function.<locals>.function_2 took 0.8016428s
-Function main.<locals>.nested_function.<locals>.function_3 took 0.6014647s
-Function main.<locals>.nested_function took 1.403586s
-Function main.<locals>.function_1 took 0.2006981s
-Function main took 1.6045189s
-
+Function main.<locals>.nested_function.<locals>.function_2 was called 4 time(s) and took 0.8019482s
+Function main.<locals>.nested_function.<locals>.function_3 was called 2 time(s) and took 0.6010157s
+Function main.<locals>.nested_function was called 2 time(s) and took 1.403365s
+Function main.<locals>.function_1 was called 2 time(s) and took 0.2007625s
+Function main was called 1 time(s) and took 1.6043592s
 
 Function main.<locals>.nested_function.<locals>.function_3:
-* took 42.85% from main.<locals>.nested_function
-* took 37.49% from main
+* took 42.83% from main.<locals>.nested_function
+* took 37.46% from main
 
 Function main.<locals>.nested_function.<locals>.function_2:
-* took 57.11% from main.<locals>.nested_function
-* took 49.96% from main
+* took 57.14% from main.<locals>.nested_function
+* took 49.99% from main
 
 Function main.<locals>.nested_function:
-* took 87.48% from main
+* took 87.47% from main
 
 Function main.<locals>.function_1:
 * took 12.51% from main
 
 Function main:
 
 ```
```

