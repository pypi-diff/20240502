# Comparing `tmp/clii-1.0.1.tar.gz` & `tmp/clii-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clii-1.0.1.tar", last modified: Tue Sep 20 03:24:41 2022, max compression
+gzip compressed data, was "clii-1.0.3.tar", last modified: Thu May  2 11:57:29 2024, max compression
```

## Comparing `clii-1.0.1.tar` & `clii-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwx------   0 james     (1000) james     (1000)        0 2022-09-20 03:24:41.797617 clii-1.0.1/
--rw-------   0 james     (1000) james     (1000)     1058 2020-07-11 13:47:29.000000 clii-1.0.1/LICENSE
--rw-------   0 james     (1000) james     (1000)     6245 2022-09-20 03:24:41.797617 clii-1.0.1/PKG-INFO
--rw-------   0 james     (1000) james     (1000)     5605 2022-09-20 03:23:32.000000 clii-1.0.1/README.md
-drwx------   0 james     (1000) james     (1000)        0 2022-09-20 03:24:41.797617 clii-1.0.1/clii.egg-info/
--rw-------   0 james     (1000) james     (1000)     6245 2022-09-20 03:24:41.000000 clii-1.0.1/clii.egg-info/PKG-INFO
--rw-------   0 james     (1000) james     (1000)      156 2022-09-20 03:24:41.000000 clii-1.0.1/clii.egg-info/SOURCES.txt
--rw-------   0 james     (1000) james     (1000)        1 2022-09-20 03:24:41.000000 clii-1.0.1/clii.egg-info/dependency_links.txt
--rw-------   0 james     (1000) james     (1000)        5 2022-09-20 03:24:41.000000 clii-1.0.1/clii.egg-info/top_level.txt
--rw-------   0 james     (1000) james     (1000)     8940 2022-09-20 03:24:32.000000 clii-1.0.1/clii.py
--rw-------   0 james     (1000) james     (1000)      438 2022-09-20 03:24:41.797617 clii-1.0.1/setup.cfg
--rw-------   0 james     (1000) james     (1000)      873 2022-09-20 03:24:38.000000 clii-1.0.1/setup.py
+drwx------   0 james     (1000) users      (984)        0 2024-05-02 11:57:29.870466 clii-1.0.3/
+-rw-------   0 james     (1000) users      (984)     1058 2022-10-21 14:02:21.000000 clii-1.0.3/LICENSE
+-rw-r--r--   0 james     (1000) users      (984)     6733 2024-05-02 11:57:29.870466 clii-1.0.3/PKG-INFO
+-rw-------   0 james     (1000) users      (984)     6399 2024-05-02 11:37:38.000000 clii-1.0.3/README.md
+-rw-------   0 james     (1000) users      (984)      915 2024-05-02 11:54:38.000000 clii-1.0.3/pyproject.toml
+-rw-------   0 james     (1000) users      (984)       38 2024-05-02 11:57:29.870466 clii-1.0.3/setup.cfg
+drwx------   0 james     (1000) users      (984)        0 2024-05-02 11:57:29.867133 clii-1.0.3/src/
+drwx------   0 james     (1000) users      (984)        0 2024-05-02 11:57:29.870466 clii-1.0.3/src/clii/
+-rw-------   0 james     (1000) users      (984)       27 2024-05-02 11:52:18.000000 clii-1.0.3/src/clii/__init__.py
+-rw-------   0 james     (1000) users      (984)     8862 2024-05-02 11:53:27.000000 clii-1.0.3/src/clii/clii.py
+-rw-------   0 james     (1000) users      (984)        0 2024-05-02 11:37:47.000000 clii-1.0.3/src/clii/py.typed
+drwx------   0 james     (1000) users      (984)        0 2024-05-02 11:57:29.870466 clii-1.0.3/src/clii.egg-info/
+-rw-r--r--   0 james     (1000) users      (984)     6733 2024-05-02 11:57:29.000000 clii-1.0.3/src/clii.egg-info/PKG-INFO
+-rw-------   0 james     (1000) users      (984)      239 2024-05-02 11:57:29.000000 clii-1.0.3/src/clii.egg-info/SOURCES.txt
+-rw-------   0 james     (1000) users      (984)        1 2024-05-02 11:57:29.000000 clii-1.0.3/src/clii.egg-info/dependency_links.txt
+-rw-------   0 james     (1000) users      (984)       11 2024-05-02 11:57:29.000000 clii-1.0.3/src/clii.egg-info/top_level.txt
+drwx------   0 james     (1000) users      (984)        0 2024-05-02 11:57:29.870466 clii-1.0.3/src/tests/
+-rwx------   0 james     (1000) users      (984)      561 2022-10-21 14:02:23.000000 clii-1.0.3/src/tests/test_misc.py
```

### Comparing `clii-1.0.1/LICENSE` & `clii-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clii-1.0.1/PKG-INFO` & `clii-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 Metadata-Version: 2.1
 Name: clii
-Version: 1.0.1
-Summary: function annotations -> cli
-Home-page: https://github.com/jamesob/clii
-Author: James O'Beirne
-Author-email: james.obeirne@pm.me
-License: MIT license
-Keywords: clii
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Version: 1.0.3
+Summary: Python functions -> CLI
+Author-email: James O'Beirne <w.clii@au92.org>
+Project-URL: Homepage, https://github.com/jamesob/clii
+Project-URL: Bug Tracker, https://github.com/jamesob/clii/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # clii
 
 Generate argument parsers from Python 3 function annotations with minimal
@@ -28,22 +19,31 @@
 #!/usr/bin/env python3.8
 from clii import App
 from pathlib import Path
 from subprocess import run
 
 cli = App()
 
+
 @cli.cmd
 def add(a: int, b: int = 3):
     print(a + b)
 
+
 @cli.cmd
+@cli.arg('path', '-p', help='Destroy where?')
 def subtract(path: Path):
     run(f'rm -rf {path}')
 
+
+@cli.main
+def main():
+    print(f"{add(1, 2)} and {subtract('/uhoh')}")
+
+
 if __name__ == '__main__':
     cli.run() 
 ```
 
 - **No dependencies.** This library has no dependencies and is a single file.
   You wanna vendor it? Vendor it.
 
@@ -54,14 +54,19 @@
 - **Nothing to learn.** if you know how to use Python function annotations, you
   already know 98% of this library. 
 
 - **Optimized for the common case.** Check out `test_bad_git.py`. I know what
   you want to do (create a subpar reproduction of git), and I've made it
   concise. 
 
+- **Functions can still be used as plain old functions.** You can still call
+  the clii-decorated functions regularly with no special ceremony. The
+  decorators are only used to construct a parser.
+
+---
 
 Okay, you and I both know the last thing that anyone needs is another way to
 generate command line interfaces. The idea of adding an additional dependency
 to your project just so you can learn yet another
 only-slightly-more-ergonomic-than-stdlib interface for parsing args is right up
 there with rewriting all your Makefiles in whatever flavor-of-the-week
 Javascript-based build system. I get it.
@@ -94,15 +99,15 @@
 # Requires Python >=3.7
 python3 -m pip install --user clii
 ```
 
 ## Substantial usage example
 
 ```python
-#!/usr/bin/env python3.8
+#!/usr/bin/env python3
 """
 A really lame version of git.
 """
 
 from pathlib import Path
 import typing as t
 
@@ -182,14 +187,28 @@
 optional arguments:
   -h, --help       show this help message and exit
   --branch BRANCH  default: None
 ```
 
 ## Usage notes
 
+### Add a main command with `@App.main`
+
+Decorating any function with the `@cli.main` decorator means that function
+is the default subparser chosen if no function argument is given.
+
+
+### Add `add_argument` arguments with `@cli.arg(...)`
+
+You can add arbitrary `ArgumentParser.add_argument(...)` args for a given
+parameter by using the `@cli.arg('paramname', <additional args>...)` 
+decorator.
+
+This decorator must be applied on lines *after* the `@cli.cmd` decorator.
+
 ### Help text from docstrings
 
 clii will pull argument help text from docstrings that are formatted like so:
 ```python
 import clii
 cli = clii.App()
```

### Comparing `clii-1.0.1/README.md` & `clii-1.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,22 +8,31 @@
 #!/usr/bin/env python3.8
 from clii import App
 from pathlib import Path
 from subprocess import run
 
 cli = App()
 
+
 @cli.cmd
 def add(a: int, b: int = 3):
     print(a + b)
 
+
 @cli.cmd
+@cli.arg('path', '-p', help='Destroy where?')
 def subtract(path: Path):
     run(f'rm -rf {path}')
 
+
+@cli.main
+def main():
+    print(f"{add(1, 2)} and {subtract('/uhoh')}")
+
+
 if __name__ == '__main__':
     cli.run() 
 ```
 
 - **No dependencies.** This library has no dependencies and is a single file.
   You wanna vendor it? Vendor it.
 
@@ -34,14 +43,19 @@
 - **Nothing to learn.** if you know how to use Python function annotations, you
   already know 98% of this library. 
 
 - **Optimized for the common case.** Check out `test_bad_git.py`. I know what
   you want to do (create a subpar reproduction of git), and I've made it
   concise. 
 
+- **Functions can still be used as plain old functions.** You can still call
+  the clii-decorated functions regularly with no special ceremony. The
+  decorators are only used to construct a parser.
+
+---
 
 Okay, you and I both know the last thing that anyone needs is another way to
 generate command line interfaces. The idea of adding an additional dependency
 to your project just so you can learn yet another
 only-slightly-more-ergonomic-than-stdlib interface for parsing args is right up
 there with rewriting all your Makefiles in whatever flavor-of-the-week
 Javascript-based build system. I get it.
@@ -74,15 +88,15 @@
 # Requires Python >=3.7
 python3 -m pip install --user clii
 ```
 
 ## Substantial usage example
 
 ```python
-#!/usr/bin/env python3.8
+#!/usr/bin/env python3
 """
 A really lame version of git.
 """
 
 from pathlib import Path
 import typing as t
 
@@ -162,14 +176,28 @@
 optional arguments:
   -h, --help       show this help message and exit
   --branch BRANCH  default: None
 ```
 
 ## Usage notes
 
+### Add a main command with `@App.main`
+
+Decorating any function with the `@cli.main` decorator means that function
+is the default subparser chosen if no function argument is given.
+
+
+### Add `add_argument` arguments with `@cli.arg(...)`
+
+You can add arbitrary `ArgumentParser.add_argument(...)` args for a given
+parameter by using the `@cli.arg('paramname', <additional args>...)` 
+decorator.
+
+This decorator must be applied on lines *after* the `@cli.cmd` decorator.
+
 ### Help text from docstrings
 
 clii will pull argument help text from docstrings that are formatted like so:
 ```python
 import clii
 cli = clii.App()
```

### Comparing `clii-1.0.1/clii.egg-info/PKG-INFO` & `clii-1.0.3/src/clii.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 Metadata-Version: 2.1
 Name: clii
-Version: 1.0.1
-Summary: function annotations -> cli
-Home-page: https://github.com/jamesob/clii
-Author: James O'Beirne
-Author-email: james.obeirne@pm.me
-License: MIT license
-Keywords: clii
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Version: 1.0.3
+Summary: Python functions -> CLI
+Author-email: James O'Beirne <w.clii@au92.org>
+Project-URL: Homepage, https://github.com/jamesob/clii
+Project-URL: Bug Tracker, https://github.com/jamesob/clii/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # clii
 
 Generate argument parsers from Python 3 function annotations with minimal
@@ -28,22 +19,31 @@
 #!/usr/bin/env python3.8
 from clii import App
 from pathlib import Path
 from subprocess import run
 
 cli = App()
 
+
 @cli.cmd
 def add(a: int, b: int = 3):
     print(a + b)
 
+
 @cli.cmd
+@cli.arg('path', '-p', help='Destroy where?')
 def subtract(path: Path):
     run(f'rm -rf {path}')
 
+
+@cli.main
+def main():
+    print(f"{add(1, 2)} and {subtract('/uhoh')}")
+
+
 if __name__ == '__main__':
     cli.run() 
 ```
 
 - **No dependencies.** This library has no dependencies and is a single file.
   You wanna vendor it? Vendor it.
 
@@ -54,14 +54,19 @@
 - **Nothing to learn.** if you know how to use Python function annotations, you
   already know 98% of this library. 
 
 - **Optimized for the common case.** Check out `test_bad_git.py`. I know what
   you want to do (create a subpar reproduction of git), and I've made it
   concise. 
 
+- **Functions can still be used as plain old functions.** You can still call
+  the clii-decorated functions regularly with no special ceremony. The
+  decorators are only used to construct a parser.
+
+---
 
 Okay, you and I both know the last thing that anyone needs is another way to
 generate command line interfaces. The idea of adding an additional dependency
 to your project just so you can learn yet another
 only-slightly-more-ergonomic-than-stdlib interface for parsing args is right up
 there with rewriting all your Makefiles in whatever flavor-of-the-week
 Javascript-based build system. I get it.
@@ -94,15 +99,15 @@
 # Requires Python >=3.7
 python3 -m pip install --user clii
 ```
 
 ## Substantial usage example
 
 ```python
-#!/usr/bin/env python3.8
+#!/usr/bin/env python3
 """
 A really lame version of git.
 """
 
 from pathlib import Path
 import typing as t
 
@@ -182,14 +187,28 @@
 optional arguments:
   -h, --help       show this help message and exit
   --branch BRANCH  default: None
 ```
 
 ## Usage notes
 
+### Add a main command with `@App.main`
+
+Decorating any function with the `@cli.main` decorator means that function
+is the default subparser chosen if no function argument is given.
+
+
+### Add `add_argument` arguments with `@cli.arg(...)`
+
+You can add arbitrary `ArgumentParser.add_argument(...)` args for a given
+parameter by using the `@cli.arg('paramname', <additional args>...)` 
+decorator.
+
+This decorator must be applied on lines *after* the `@cli.cmd` decorator.
+
 ### Help text from docstrings
 
 clii will pull argument help text from docstrings that are formatted like so:
 ```python
 import clii
 cli = clii.App()
```

### Comparing `clii-1.0.1/clii.py` & `clii-1.0.3/src/clii/clii.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,26 +29,26 @@
 import inspect
 import typing as t
 import os
 import logging
 from textwrap import dedent
 
 
-__VERSION__ = '1.0.1'
+__VERSION__ = '1.0.3'
 
 logger = logging.getLogger("clii")
 if os.environ.get("CLII_DEBUG"):
     logger.setLevel(logging.DEBUG)
     logger.addHandler(logging.StreamHandler())
 
 
 # Storage to that maps functions to a map of overrides for arguments. Allows
 # users to manually specify ArgumentParser.add_arguments() arguments using
 # the @cli.arg(...) decorator.
-ARG_OVERRIDES_MAP = {}
+ARG_OVERRIDES_MAP: t.Dict[t.Callable, dict] = {}
 
 
 class Arg:
     def __init__(
         self,
         param_name: str,
         flags: t.Sequence[str],
@@ -210,35 +210,30 @@
         if not self.subparsers:
             self.subparsers = self.parser.add_subparsers()
 
         desc = fnc.__doc__ or ""
         doclines = []
 
         for line in desc.splitlines():
-            if line.strip().lower() in ["args:", "kwargs;"]:
+            if line.strip().lower() in ["args:", "kwargs:"]:
                 break
             doclines.append(line)
 
         sub = self.subparsers.add_parser(
             fnc.__name__.replace("_", "-"),
             description="\n".join(doclines),
         )
         logger.debug("Added subparser: %s", sub)
 
         for arg in Arg.from_func(fnc):
             arg.add_to_parser(sub)
             logger.debug("  Adding argument: %s", arg)
 
         sub.set_defaults(func=fnc)
-
-        @functools.wraps(fnc)
-        def wrapper(*args, **kwargs):
-            return fnc(*args, **kwargs)
-
-        return wrapper
+        return fnc
 
     def arg(self, name: str, *args, **kwargs) -> t.Callable:
         """
         Add additional ArgumentParser.add_argument() args for a certain arg.
         """
         def wrapper(fnc):
             ARG_OVERRIDES_MAP.setdefault(fnc, {})
@@ -272,11 +267,11 @@
             elif p.kind == inspect.Parameter.VAR_POSITIONAL:
                 func_args.extend(args[p.name])
             else:
                 func_args.append(args[p.name])
 
         return (fnc, (func_args, func_kwargs))
 
-    def run(self):
+    def run(self) -> object:
         (fnc, (func_args, func_kwargs)) = self.parse_for_run()
 
         return fnc(*func_args, **func_kwargs)
```

