# Comparing `tmp/makim-1.9.0.tar.gz` & `tmp/makim-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makim-1.9.0.tar", max compression
+gzip compressed data, was "makim-1.9.1.tar", max compression
```

## Comparing `makim-1.9.0.tar` & `makim-1.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1514 2023-12-08 17:47:01.041247 makim-1.9.0/LICENSE
--rw-r--r--   0        0        0     5356 2023-12-08 17:47:01.041247 makim-1.9.0/README.md
--rw-r--r--   0        0        0     2035 2023-12-08 17:50:02.748006 makim-1.9.0/pyproject.toml
--rw-r--r--   0        0        0      194 2023-12-08 17:50:02.748006 makim-1.9.0/src/makim/__init__.py
--rw-r--r--   0        0        0      111 2023-12-08 17:47:01.045247 makim-1.9.0/src/makim/__main__.py
--rw-r--r--   0        0        0     5117 2023-12-08 17:47:01.045247 makim-1.9.0/src/makim/cli.py
--rw-r--r--   0        0        0      418 2023-12-08 17:47:01.045247 makim-1.9.0/src/makim/errors.py
--rw-r--r--   0        0        0    17184 2023-12-08 17:47:01.045247 makim-1.9.0/src/makim/makim.py
--rw-r--r--   0        0        0        0 2023-12-08 17:47:01.045247 makim-1.9.0/src/makim/py.typed
--rw-r--r--   0        0        0     6213 1970-01-01 00:00:00.000000 makim-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1514 2023-12-13 00:28:07.697166 makim-1.9.1/LICENSE
+-rw-r--r--   0        0        0     3257 2023-12-13 00:28:07.697166 makim-1.9.1/README.md
+-rw-r--r--   0        0        0     2035 2023-12-13 00:31:53.228068 makim-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-12-13 00:31:53.228068 makim-1.9.1/src/makim/__init__.py
+-rw-r--r--   0        0        0      111 2023-12-13 00:28:07.701166 makim-1.9.1/src/makim/__main__.py
+-rw-r--r--   0        0        0     5117 2023-12-13 00:28:07.701166 makim-1.9.1/src/makim/cli.py
+-rw-r--r--   0        0        0      418 2023-12-13 00:28:07.701166 makim-1.9.1/src/makim/errors.py
+-rw-r--r--   0        0        0    17184 2023-12-13 00:28:07.701166 makim-1.9.1/src/makim/makim.py
+-rw-r--r--   0        0        0        0 2023-12-13 00:28:07.701166 makim-1.9.1/src/makim/py.typed
+-rw-r--r--   0        0        0     4114 1970-01-01 00:00:00.000000 makim-1.9.1/PKG-INFO
```

### Comparing `makim-1.9.0/LICENSE` & `makim-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `makim-1.9.0/pyproject.toml` & `makim-1.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makim"
-version = "1.9.0"  # semantic-release
+version = "1.9.1"  # semantic-release
 description = "Simplify the usage of containers"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD 3 Clause"
 repository = "https://github.com/osl-incubator/makim"
 homepage = "https://github.com/osl-incubator/makim"
 readme = "README.md"
```

### Comparing `makim-1.9.0/src/makim/cli.py` & `makim-1.9.1/src/makim/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 
     note: when added new flags, update the list of flags to be
           skipped at extract_makim_args function.
     """
     makim_file_default = str(Path(os.getcwd()) / '.makim.yaml')
 
     parser = argparse.ArgumentParser(
-        prog='MakIm',
+        prog='Makim',
         description=(
-            'MakIm is a tool that helps you to organize '
+            'Makim is a tool that helps you to organize '
             'and simplify your helper commands.'
         ),
         epilog=(
             'If you have any problem, open an issue at: '
             'https://github.com/osl-incubator/makim'
         ),
         add_help=False,
@@ -64,15 +64,15 @@
         action='store_true',
         help='Show the help menu',
     )
 
     parser.add_argument(
         '--version',
         action='store_true',
-        help='Show the version of the installed MakIm tool.',
+        help='Show the version of the installed Makim tool.',
     )
 
     parser.add_argument(
         '--verbose',
         action='store_true',
         help='Show the commands to be executed.',
     )
```

### Comparing `makim-1.9.0/src/makim/makim.py` & `makim-1.9.1/src/makim/makim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Makim main class.
 
-`MakIm` or just `makim` is based on `make` and focus on improve
+`Makim` or just `makim` is based on `make` and focus on improve
 the way to define targets and dependencies. Instead of using the
 `Makefile` format, it uses `yaml` format.
 """
 import io
 import os
 import pprint
 import sys
```

